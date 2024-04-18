# Comparing `tmp/bioencoder-0.1.1.tar.gz` & `tmp/bioencoder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioencoder-0.1.1.tar", last modified: Thu Mar 28 22:46:26 2024, max compression
+gzip compressed data, was "bioencoder-0.2.0.tar", last modified: Thu Apr 18 21:46:07 2024, max compression
```

## Comparing `bioencoder-0.1.1.tar` & `bioencoder-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.296517 bioencoder-0.1.1/
--rw-rw-rw-   0        0        0     1126 2024-03-28 22:06:00.000000 bioencoder-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4647 2024-03-28 22:46:26.295517 bioencoder-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3750 2024-03-28 21:39:09.000000 bioencoder-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.254599 bioencoder-0.1.1/bioencoder/
--rw-rw-rw-   0        0        0      532 2024-03-28 22:17:18.000000 bioencoder-0.1.1/bioencoder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.282088 bioencoder-0.1.1/bioencoder/core/
--rw-rw-rw-   0        0        0      205 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/__init__.py
--rw-rw-rw-   0        0        0     2218 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/augmentations.py
--rw-rw-rw-   0        0        0      213 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/backbones.py
--rw-rw-rw-   0        0        0     2072 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/datasets.py
--rw-rw-rw-   0        0        0     6357 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/losses.py
--rw-rw-rw-   0        0        0     4580 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/models.py
--rw-rw-rw-   0        0        0      281 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/optimizers.py
--rw-rw-rw-   0        0        0      368 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/schedulers.py
--rw-rw-rw-   0        0        0    21520 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.289088 bioencoder-0.1.1/bioencoder/scripts/
--rw-rw-rw-   0        0        0      188 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/__init__.py
--rw-rw-rw-   0        0        0     3038 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/archive.py
--rw-rw-rw-   0        0        0     2050 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/configure.py
--rw-rw-rw-   0        0        0     3729 2024-03-28 20:48:34.000000 bioencoder-0.1.1/bioencoder/scripts/interactive_plots.py
--rw-rw-rw-   0        0        0     3323 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/lr_finder.py
--rw-rw-rw-   0        0        0     5086 2024-03-28 20:48:34.000000 bioencoder-0.1.1/bioencoder/scripts/model_explorer.py
--rw-rw-rw-   0        0        0      732 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/model_explorer_wrapper.py
--rw-rw-rw-   0        0        0     8634 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/scripts/split_dataset.py
--rw-rw-rw-   0        0        0     3529 2024-03-28 20:48:34.000000 bioencoder-0.1.1/bioencoder/scripts/swa.py
--rw-rw-rw-   0        0        0    11611 2024-03-28 20:48:34.000000 bioencoder-0.1.1/bioencoder/scripts/train.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.293517 bioencoder-0.1.1/bioencoder/vis/
--rw-rw-rw-   0        0        0       70 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/vis/__init__.py
--rw-rw-rw-   0        0        0    11283 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/vis/classes.py
--rw-rw-rw-   0        0        0     9856 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/vis/helpers.py
--rw-rw-rw-   0        0        0     6720 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/vis/methods.py
--rw-rw-rw-   0        0        0    14028 2024-03-11 21:33:49.000000 bioencoder-0.1.1/bioencoder/vis/methods_backup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:46:26.294517 bioencoder-0.1.1/bioencoder.egg-info/
--rw-rw-rw-   0        0        0     4647 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1008 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      432 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      212 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2024-03-28 22:46:26.000000 bioencoder-0.1.1/bioencoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2024-03-28 22:45:34.000000 bioencoder-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      227 2024-03-11 21:33:49.000000 bioencoder-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 22:46:26.296517 bioencoder-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.549732 bioencoder-0.2.0/
+-rw-rw-rw-   0        0        0     1126 2024-03-28 22:06:00.000000 bioencoder-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6178 2024-04-18 21:46:07.548730 bioencoder-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5283 2024-04-18 21:24:57.000000 bioencoder-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.273192 bioencoder-0.2.0/bioencoder/
+-rw-rw-rw-   0        0        0      532 2024-03-28 22:17:18.000000 bioencoder-0.2.0/bioencoder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.385000 bioencoder-0.2.0/bioencoder/core/
+-rw-rw-rw-   0        0        0      205 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/__init__.py
+-rw-rw-rw-   0        0        0     2218 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/augmentations.py
+-rw-rw-rw-   0        0        0      213 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/backbones.py
+-rw-rw-rw-   0        0        0     2072 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/datasets.py
+-rw-rw-rw-   0        0        0     6357 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/losses.py
+-rw-rw-rw-   0        0        0     4594 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/core/models.py
+-rw-rw-rw-   0        0        0      281 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/optimizers.py
+-rw-rw-rw-   0        0        0      368 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/core/schedulers.py
+-rw-rw-rw-   0        0        0    21555 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.493074 bioencoder-0.2.0/bioencoder/scripts/
+-rw-rw-rw-   0        0        0      188 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4561 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/archive.py
+-rw-rw-rw-   0        0        0     2971 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/configure.py
+-rw-rw-rw-   0        0        0     5195 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/interactive_plots.py
+-rw-rw-rw-   0        0        0     4891 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/lr_finder.py
+-rw-rw-rw-   0        0        0     5941 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/model_explorer.py
+-rw-rw-rw-   0        0        0      732 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/scripts/model_explorer_wrapper.py
+-rw-rw-rw-   0        0        0    11228 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/split_dataset.py
+-rw-rw-rw-   0        0        0     4338 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/swa.py
+-rw-rw-rw-   0        0        0    13758 2024-04-18 21:43:24.000000 bioencoder-0.2.0/bioencoder/scripts/train.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.544704 bioencoder-0.2.0/bioencoder/vis/
+-rw-rw-rw-   0        0        0       70 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/__init__.py
+-rw-rw-rw-   0        0        0    11283 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/classes.py
+-rw-rw-rw-   0        0        0     9856 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/helpers.py
+-rw-rw-rw-   0        0        0     6720 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/methods.py
+-rw-rw-rw-   0        0        0    14028 2024-03-11 21:33:49.000000 bioencoder-0.2.0/bioencoder/vis/methods_backup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 21:46:07.547218 bioencoder-0.2.0/bioencoder.egg-info/
+-rw-rw-rw-   0        0        0     6178 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      432 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      212 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2024-04-18 21:46:07.000000 bioencoder-0.2.0/bioencoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2024-04-18 21:44:09.000000 bioencoder-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      227 2024-03-11 21:33:49.000000 bioencoder-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 21:46:07.549732 bioencoder-0.2.0/setup.cfg
```

### Comparing `bioencoder-0.1.1/LICENSE` & `bioencoder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/PKG-INFO` & `bioencoder-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioencoder
-Version: 0.1.1
+Version: 0.2.0
 Summary: A metric learning toolkit
 Author-email: Arthur Porto <agporto@gmail.com>, Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://github.com/agporto/BioEncoder
 Project-URL: Bug Tracker, https://github.com/agporto/BioEncoder/issues
 Keywords: metric learning,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
@@ -35,15 +35,15 @@
 
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
-- Easy customization of hyperparameters, including augmentations, through `YAML` configs
+- Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
 - Custom augmentations techniques via [albumentations](https://github.com/albumentations-team/albumentations)
 - TensorBoard logs and checkpoints (soon to come: WandB integration)
 - Streamlit app with rich model visualizations (e.g., [Grad-CAM](https://arxiv.org/abs/1610.02391))
 - Interactive [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html) and [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) plots using [Bokeh](https://bokeh.org/)
 
 <div align="center">
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder-interactive-plot.gif" width="500"></p>
@@ -54,19 +54,22 @@
 (for more detailed information consult [the help files](help))
 
 1\. Install BioEncoder (into a virtual environment with pytorch/CUDA): 
 ````
 pip install bioencoder
 ````
 
-2\. Download example dataset (includes images and configs): https://osf.io/download/gsd5z/
+2\. Download example dataset from the data repo: [https://zenodo.org/records/10909614/files/BioEncoder-data.zip](https://zenodo.org/records/10909614/files/BioEncoder-data.zip?download=1&preview=1). 
+This archive contains the images and configuration files needed for step 3/4, as well as the final model checkpoints and a script to reproduce the results and figures presented in the paper. To play around with theinteractive figures and the model explorer you can also skip the training / SWA steps. 
 
-3\. Start interactive session (e.g., in Spyder or VS code) and run:
+3\. Start interactive session (e.g., in Spyder or VS code) and run the following commands one by one:
 
 ```python
+## use "overwrite=True to redo a step
+
 import bioencoder
 
 ## global setup
 bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
@@ -79,29 +82,51 @@
 bioencoder.interactive_plots(config_path=r"bioencoder_configs/plot_stage1.yml")
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage1.yml")
 
 ## (optional) learning rate finder for stage 2
 bioencoder.lr_finder(config_path=r"bioencoder_configs/lr_finder.yml")
 
 ## train stage 2
-bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml", overwrite=True)
+bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage2.yml")
 
 ## explore model from stage 2
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage2.yml")
 
 ```
+4\. Alternatively, you can directly use the command line interface: 
+
+```python
+## use the flag "--overwrite" to redo a step
+
+bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
+bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
+bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
+bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
+bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage2.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage2.yml"
+
+```
 
 ## Citation
 
 Please cite BioEncoder as follows:
 
 ```bibtex
-@UNPUBLISHED{
-    Lurig2024-pb,
-    title     = "BioEncoder: a metric learning toolkit for comparative organismal biology",
-    author    = "L{\"u}rig, Moritz D and Di Martino, Emanuela and Porto, Arthur", 
-    journal  = "bioRxiv",
-    language  = "en",
-    doi       = "xxxx"
+
+@UNPUBLISHED{Luerig2024-ov,
+  title    = "{BioEncoder}: a metric learning toolkit for comparative
+              organismal biology",
+  author   = "Luerig, Moritz D and Di Martino, Emanuela and Porto, Arthur",
+  journal  = "bioRxiv",
+  pages    = "2024.04.03.587987",
+  month    =  apr,
+  year     =  2024,
+  language = "en",
+  doi      = "10.1101/2024.04.03.587987"
 }
+
 ```
```

### Comparing `bioencoder-0.1.1/README.md` & `bioencoder-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
-- Easy customization of hyperparameters, including augmentations, through `YAML` configs
+- Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
 - Custom augmentations techniques via [albumentations](https://github.com/albumentations-team/albumentations)
 - TensorBoard logs and checkpoints (soon to come: WandB integration)
 - Streamlit app with rich model visualizations (e.g., [Grad-CAM](https://arxiv.org/abs/1610.02391))
 - Interactive [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html) and [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) plots using [Bokeh](https://bokeh.org/)
 
 <div align="center">
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder-interactive-plot.gif" width="500"></p>
@@ -27,19 +27,22 @@
 (for more detailed information consult [the help files](help))
 
 1\. Install BioEncoder (into a virtual environment with pytorch/CUDA): 
 ````
 pip install bioencoder
 ````
 
-2\. Download example dataset (includes images and configs): https://osf.io/download/gsd5z/
+2\. Download example dataset from the data repo: [https://zenodo.org/records/10909614/files/BioEncoder-data.zip](https://zenodo.org/records/10909614/files/BioEncoder-data.zip?download=1&preview=1). 
+This archive contains the images and configuration files needed for step 3/4, as well as the final model checkpoints and a script to reproduce the results and figures presented in the paper. To play around with theinteractive figures and the model explorer you can also skip the training / SWA steps. 
 
-3\. Start interactive session (e.g., in Spyder or VS code) and run:
+3\. Start interactive session (e.g., in Spyder or VS code) and run the following commands one by one:
 
 ```python
+## use "overwrite=True to redo a step
+
 import bioencoder
 
 ## global setup
 bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
@@ -52,29 +55,51 @@
 bioencoder.interactive_plots(config_path=r"bioencoder_configs/plot_stage1.yml")
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage1.yml")
 
 ## (optional) learning rate finder for stage 2
 bioencoder.lr_finder(config_path=r"bioencoder_configs/lr_finder.yml")
 
 ## train stage 2
-bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml", overwrite=True)
+bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage2.yml")
 
 ## explore model from stage 2
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage2.yml")
 
 ```
+4\. Alternatively, you can directly use the command line interface: 
+
+```python
+## use the flag "--overwrite" to redo a step
+
+bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
+bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
+bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
+bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
+bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage2.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage2.yml"
+
+```
 
 ## Citation
 
 Please cite BioEncoder as follows:
 
 ```bibtex
-@UNPUBLISHED{
-    Lurig2024-pb,
-    title     = "BioEncoder: a metric learning toolkit for comparative organismal biology",
-    author    = "L{\"u}rig, Moritz D and Di Martino, Emanuela and Porto, Arthur", 
-    journal  = "bioRxiv",
-    language  = "en",
-    doi       = "xxxx"
+
+@UNPUBLISHED{Luerig2024-ov,
+  title    = "{BioEncoder}: a metric learning toolkit for comparative
+              organismal biology",
+  author   = "Luerig, Moritz D and Di Martino, Emanuela and Porto, Arthur",
+  journal  = "bioRxiv",
+  pages    = "2024.04.03.587987",
+  month    =  apr,
+  year     =  2024,
+  language = "en",
+  doi      = "10.1101/2024.04.03.587987"
 }
-```
+
+```
```

### Comparing `bioencoder-0.1.1/bioencoder/__init__.py` & `bioencoder-0.2.0/bioencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/core/augmentations.py` & `bioencoder-0.2.0/bioencoder/core/augmentations.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/core/datasets.py` & `bioencoder-0.2.0/bioencoder/core/datasets.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/core/losses.py` & `bioencoder-0.2.0/bioencoder/core/losses.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/core/models.py` & `bioencoder-0.2.0/bioencoder/core/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     - RuntimeError: If the specified backbone is not found in the `BACKBONES` dictionary or the timm library.
     - TypeError: If the linear layer of the model can't be found.
     
     """
     try:
         if 'timm_' in backbone:
             backbone = backbone[5:]
-            print(f"Using backbone: {backbone}")
             model = timm.create_model(model_name=backbone, pretrained=True)
         else:
             model = BACKBONES[backbone](pretrained=True)
     except RuntimeError or KeyError:
         raise RuntimeError('Specify the correct backbone name. Either one of torchvision backbones, or a timm backbone.'
                            'For timm - add prefix \'timm_\'. For instance, timm_resnet18')
 
@@ -46,30 +45,32 @@
 
     features_dim = potential_last_layer.in_features
     model = torch.nn.Sequential(*list(model.children())[:-1])
 
     return model, features_dim
 
 
-class SupConModel(nn.Module):
+class BioEncoderModel(nn.Module):
     """
-    This class implements the supervised contrastive learning model.
+    This class implements the BioEncoder model based on supervised contrastive learning.
     The model consists of a feature encoder and either a classifier head for the second stage of 
     training or a projection head for the first stage of training.
 
-    Parameters:
-    backbone (str): Name of the backbone network to use for the feature encoder.
-    projection_dim (int): Number of dimensions for the output of the projection head.
-    second_stage (bool): Whether to use the classifier head for second stage of training.
-    num_classes (int): Number of classes for the classification task, required if `second_stage` is True.
+    Parameters
+    ----------
+    backbone : str 
+        Name of the backbone network to use for the feature encoder.
+        projection_dim (int): Number of dimensions for the output of the projection head.
+        second_stage (bool): Whether to use the classifier head for second stage of training.
+        num_classes (int): Number of classes for the classification task, required if `second_stage` is True.
 
 
     """
     def __init__(self, backbone='resnet50', projection_dim=128, second_stage=False, num_classes=None):
-        super(SupConModel, self).__init__()
+        super(BioEncoderModel, self).__init__()
         self.encoder, self.features_dim = create_encoder(backbone)
         self.second_stage = second_stage
         self.projection_head = True
         self.projection_dim = projection_dim
         self.embed_dim = projection_dim
 
         if self.second_stage:
```

### Comparing `bioencoder-0.1.1/bioencoder/core/utils.py` & `bioencoder-0.2.0/bioencoder/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import torch
 from pytorch_metric_learning.utils.accuracy_calculator import AccuracyCalculator
 from sklearn.metrics import f1_score #, accuracy_score
 
 from .losses import LOSSES
 from .optimizers import OPTIMIZERS
 from .schedulers import SCHEDULERS
-from .models import SupConModel
+from .models import BioEncoderModel
 from .datasets import create_dataset
 from .augmentations import get_transforms
 
 
 def load_yaml(yaml_path):
     
     with open(yaml_path, "r") as file:
@@ -80,15 +80,15 @@
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     torch.backends.cudnn.deterministic = True
 
 
 def pprint_fill_hbar(message, symbol="-", ret=True):
-    terminal_width = os.get_terminal_size()[0]
+    terminal_width = os.get_terminal_size()[0] - len("%Y-%m-%d %H:%M:%S")
     message_length = len(message)
 
     if message_length >= terminal_width:
         formatted_message = message
     else:
         bar_length = (terminal_width - message_length - 2) // 2
         horizontal_bar = symbol * bar_length
@@ -251,15 +251,15 @@
     - num_classes (int, optional): The number of classes to predict. Defaults to None.
     - ckpt_pretrained (str, optional): The path to a checkpoint to load as pre-trained weights. Defaults to None.
 
     Returns:
     - model (torch.nn.Module): The SupCon model.
     """
 
-    model = SupConModel(backbone=backbone, second_stage=second_stage, num_classes=num_classes)
+    model = BioEncoderModel(backbone=backbone, second_stage=second_stage, num_classes=num_classes)
 
     if ckpt_pretrained:
         model.load_state_dict(torch.load(ckpt_pretrained, map_location=torch.device(cuda_device))['model_state_dict'], strict=False)
 
     return model
```

### Comparing `bioencoder-0.1.1/bioencoder/scripts/interactive_plots.py` & `bioencoder-0.2.0/bioencoder/scripts/interactive_plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,46 @@
 
 def interactive_plots(    
         config_path, 
         overwrite=False,
         **kwargs,
 ):
 
+    """
+    Generates interactive plots for visualizing high-dimensional embeddings of validation set.
+    This function computes embeddings using a trained model, reduces their dimensionality,
+    and plots them in an interactive plot saved as an HTML file. Optionally, it can also return
+    embeddings data as a DataFrame (ret_embeddings=True).
+    
+    Parameters
+    ----------
+    config_path : str
+        Path to the YAML file that contains settings for the model and training configurations.
+        This configuration includes details on model architecture, data loaders, and other
+        hyperparameters required for embedding computation.
+    overwrite : bool, optional
+        If True, allows the generated HTML plot file to overwrite existing files with the same name.
+        If False, the function will check if the file exists and assert failure if it does. Default is False.
+    
+    
+    Raises
+    ------
+    AssertionError
+        If 'overwrite' is False and a plot file already exists at the specified location.
+    FileNotFoundError
+        If the configuration file does not exist.
+    
+    Examples
+    --------
+    To generate interactive plots for model embeddings:
+        bioencoder.interactive_plots("/path/to/config.yaml")
+    
+
+    """
+        
     ## load bioencoer config
     config = utils.load_config(kwargs.get("bioencoder_config_path"))
     root_dir = config.root_dir
     run_name = config.run_name
     
     ## load config
     hyperparams = utils.load_yaml(config_path)
@@ -107,21 +139,18 @@
     
     helpers.bokeh_plot(df, out_path=plot_path, color_classes=color_classes)
     
     
 def cli():
 
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--config-path",
-        type=str,
-        default=None,
-    )
+    parser.add_argument( "--config-path",type=str, help="Path to the YAML configuration file to create interactive plots.")
+    parser.add_argument("--overwrite", action='store_true', help="Overwrite existing files without asking.")
     args = parser.parse_args()
-    
-    interactive_plots(args.config_path)
+
+    interactive_plots(args.config_path, overwrite=args.overwrite)
     
     
 
 if __name__ == "__main__":
     
     cli()
```

### Comparing `bioencoder-0.1.1/bioencoder/scripts/model_explorer.py` & `bioencoder-0.2.0/bioencoder/scripts/model_explorer.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,30 +32,39 @@
 
 
 def model_explorer(
         config_path,
         **kwargs,
         ):
     """
-    
+    Launches a Streamlit-based web application to interactively explore different visualization
+    techniques of the BioEncoder model, such as filter visualizations, activation maps, 
+    saliency maps, Grad-CAM, and Contrastive-CAM. It provides a user interface to upload an 
+    image, select the visualization type, and dynamically adjust parameters related to each 
+    visualization technique.
 
     Parameters
     ----------
-    config_path : TYPE
-        DESCRIPTION.
-    **kwargs : TYPE
-        DESCRIPTION.
-     : TYPE
-        DESCRIPTION.
-
-    Returns
-    -------
-    None.
+    config_path : str
+        Path to the YAML configuration file that contains model specifications and settings, 
+        including backbone, number of classes, and stage-specific settings (e.g., 'first' or 
+        'second' stage of model training).
+
+    Raises
+    ------
+    FileNotFoundError
+        If the specified configuration file is not found or required model weights are unavailable.
+
+    Examples
+    --------
+    To start the model explorer from the command line using a specific configuration:
+        bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage2.yml")
 
     """
+    
     ## load bioencoer config
     config = utils.load_config(kwargs.get("bioencoder_config_path"))
     root_dir = config.root_dir
     run_name = config.run_name
     
     class_names = os.listdir(os.path.join(root_dir, "data", run_name, "train"))
```

### Comparing `bioencoder-0.1.1/bioencoder/scripts/model_explorer_wrapper.py` & `bioencoder-0.2.0/bioencoder/scripts/model_explorer_wrapper.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/scripts/swa.py` & `bioencoder-0.2.0/bioencoder/scripts/swa.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,28 +12,36 @@
 #%%
 
 def swa(
     config_path, 
     **kwargs,
 ):
     """
-    
+    Applies Stochastic Weight Averaging (SWA) to improve model generalization by averaging multiple model checkpoints.
 
     Parameters
     ----------
-    config_path : TYPE
-        DESCRIPTION.
-    **kwargs : TYPE
-        DESCRIPTION.
-
-    Returns
-    -------
-    None.
+    config_path : str
+        Path to the YAML file containing training configurations including model, training parameters, 
+        and data loader settings. This file dictates how the model and training processes should be structured.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the specified configuration file or model checkpoints are not found.
+    ValueError
+        If required configurations for stages or model details are missing or invalid.
+
+    Examples
+    --------
+    To perform SWA on a model using a configuration file located at '/path/to/config.yaml':
+        bioencoder.swa("/path/to/config.yaml")
 
     """
+    
     ## load bioencoer config
     config = utils.load_config(kwargs.get("bioencoder_config_path"))
     root_dir = config.root_dir
     run_name = config.run_name
     
     ## load config 
     hyperparams = utils.load_yaml(config_path)
@@ -113,21 +121,18 @@
     print("swa stage {} validation metrics: {}".format(stage, valid_metrics))
     
     
     
 def cli():
     
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--config-path",
-        type=str,
-        default=None,
-    )
+    parser.add_argument( "--config-path",type=str, help="Path to the YAML configuration file that specifies hyperparameters for SWA.")
+    parser.add_argument("--overwrite", action='store_true', help="Overwrite existing files without asking.")
     args = parser.parse_args()
 
-    swa(args.config_path)
+    swa(args.config_path, overwrite=args.overwrite)
     
     
     
 if __name__ == "__main__":
     
     cli()
```

### Comparing `bioencoder-0.1.1/bioencoder/scripts/train.py` & `bioencoder-0.2.0/bioencoder/scripts/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,33 +20,46 @@
 
 def train(
     config_path,
     overwrite=False,
     **kwargs,
 ):
     """
-    
+    Trains the BioEncoder model based on the provided configuration settings in the yaml files.
 
     Parameters
     ----------
-    config_path : TYPE
-        DESCRIPTION.
-    overwrite : TYPE
-        DESCRIPTION.
-    **kwargs : TYPE
-        DESCRIPTION.
+    config_path : str
+        Path to the YAML configuration file that specifies detailed training and optimizer parameters.
+        This file controls various aspects of the training process including but not limited to model architecture,
+        optimizer settings, scheduler details, and data augmentation strategies.
+    overwrite : bool, optional
+        If True, existing directories for logs, runs, and weights will be removed and recreated, allowing for a clean training start.
+        If False, the training process will append to existing directories and files, which could lead to mixed results if not managed properly.
+        Default is False.
 
     Raises
     ------
+    FileNotFoundError
+        If the configuration file specified by `config_path` does not exist.
+    AssertionError
+        If certain conditions in the configuration (like minimum image count per class) are not met.
     ValueError
-        DESCRIPTION.
+        If incompatible or inconsistent parameters are detected during the setup or training processes.
+
+    Notes
+    -----
+    There are two separate files for the first and second stage - make sure you set them up appropriately. E.g., for stage two,
+    specify the number of classes, and a different learning rate.
+
+    Examples
+    --------
+    To start a new training session with overwriting previous outputs:
+        bioencoder.train("/path/to/config.yaml", overwrite=True)
 
-    Returns
-    -------
-    None.
 
     """
     
     ## load bioencoer config
     config = utils.load_config(kwargs.get("bioencoder_config_path"))
     root_dir = config.root_dir
     run_name = config.run_name
@@ -141,18 +154,14 @@
         ckpt_pretrained = None   
         num_classes = None
 
     ## add hyperparams to log
     logger.info(utils.pprint_fill_hbar(f"Training {stage} stage ", symbol="#"))
     logger.info(f"Dataset:\n{pretty_repr(data_stats)}")
     logger.info(f"Hyperparameters:\n{pretty_repr(hyperparams)}")
-
-    # ## set cuda device
-    # torch.cuda.set_device(cuda_device)
-    # print(f"Using CUDA device {cuda_device}")
     
     ## scaler
     scaler = torch.cuda.amp.GradScaler()
     if not amp:
         scaler = None
     utils.set_seed()
 
@@ -169,18 +178,28 @@
     model = utils.build_model(
         backbone,
         second_stage=(stage == "second"),
         num_classes=num_classes,
         ckpt_pretrained=ckpt_pretrained,
     ).cuda()
     
-    ## configure multi-GPU system
-    #if torch.cuda.device_count() > 1:
-    #    print("Let's use", torch.cuda.device_count(), "GPUs!")
-    #    model = torch.nn.DataParallel(model)   feedback
+    logger.info(f"Using backbone: {backbone}")
+    
+    ## configure GPU 
+    assert torch.cuda.device_count() > 0, "No GPUs detected on this System (check your CUDA setup) - aborting."
+    if torch.cuda.device_count() == 1:
+        logger.info(f"Found one GPU: {torch.cuda.get_device_name(0)} (device {torch.cuda.current_device()})")
+    else:
+        logger.info(f"Found {torch.cuda.device_count()} GPUs, but unfortunately multi-GPU use isn't implemented yet.")
+        logger.info(f"Using GPU {torch.cuda.get_device_name(0)} (device {torch.cuda.current_device()})")
+        
+        # ## set cuda device
+        # torch.cuda.set_device(cuda_device)
+        # print(f"Using CUDA device {cuda_device}")
+        # model = torch.nn.DataParallel(model)   
 
     ## configure optimizer
     optim = utils.build_optim(
         model, optimizer_params, scheduler_params, criterion_params
     )
     criterion, optimizer, scheduler, loss_optimizer = (
         optim["criterion"],
@@ -240,38 +259,38 @@
             model.use_projection_head(False)
             valid_metrics_encoder = utils.validation_constructive(
                 loaders["valid_loader"], loaders["train_features_loader"], model, scaler
             )
             model.use_projection_head(True)
             #model_copy.use_projection_head(True)
             
-            logger.info(
-                "Summary epoch {}:\ntrain time {:.2f}\nvalid time {:.2f}\ntrain loss {:.2f}\nvalid acc projection head {}\nvalid acc encoder {}".format(
-                    epoch,
-                    end_training_time - start_training_time,
-                    time.time() - start_validation_time,
-                    train_metrics["loss"],
-                    pretty_repr(valid_metrics_projection_head),
-                    pretty_repr(valid_metrics_encoder),
-                )
+            ## epoch summary
+            message = "Summary epoch {}:\ntrain time {:.2f}\nvalid time {:.2f}\ntrain loss {:.2f}\nvalid acc projection head {}\nvalid acc encoder {}".format(
+                epoch,
+                end_training_time - start_training_time,
+                time.time() - start_validation_time,
+                train_metrics["loss"],
+                pretty_repr(valid_metrics_projection_head),
+                pretty_repr(valid_metrics_encoder),
             )
+            logger.info("\n".join(line if i == 0 else "    " + line for i, line in enumerate(message.split("\n"))))
             valid_metrics = valid_metrics_projection_head
         else:
             valid_metrics = utils.validation_ce(
                 model, criterion, loaders["valid_loader"], scaler
             )
-            logger.info(
-                "Summary epoch {}:\ntrain time {:.2f}\nvalid time {:.2f}\ntrain loss {:.2f}\nvalid acc dict {}".format(
+            ## epoch summary
+            message =  "Summary epoch {}:\ntrain time {:.2f}\nvalid time {:.2f}\ntrain loss {:.2f}\nvalid acc dict {}".format(
                     epoch,
                     end_training_time - start_training_time,
                     time.time() - start_validation_time,
                     train_metrics["loss"],
                     pretty_repr(valid_metrics),
-                )
             )
+            logger.info("\n".join(line if i == 0 else "    " + line for i, line in enumerate(message.split("\n"))))
 
         # write train and valid metrics to the logs
         utils.add_to_tensorboard_logs(
             writer, train_metrics["loss"], "Loss/train", epoch
         )
         for valid_metric in valid_metrics:
             try:
@@ -315,20 +334,18 @@
     writer.close()
     logging.shutdown()
 
 
 def cli():
     
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--config-path",
-        type=str,
-    )
+    parser.add_argument( "--config-path",type=str, help="Path to the YAML configuration file that specifies detailed training and optimizer parameters.")
+    parser.add_argument("--overwrite", action='store_true', help="Overwrite existing files without asking.")
     args = parser.parse_args()
     
-    train(args.config_path)
-
+    train(args.config_path,
+          overwrite=args.overwrite)
 
 
 if __name__ == "__main__":
     
     cli()
```

### Comparing `bioencoder-0.1.1/bioencoder/vis/classes.py` & `bioencoder-0.2.0/bioencoder/vis/classes.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/vis/helpers.py` & `bioencoder-0.2.0/bioencoder/vis/helpers.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/vis/methods.py` & `bioencoder-0.2.0/bioencoder/vis/methods.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder/vis/methods_backup.py` & `bioencoder-0.2.0/bioencoder/vis/methods_backup.py`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/bioencoder.egg-info/PKG-INFO` & `bioencoder-0.2.0/bioencoder.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioencoder
-Version: 0.1.1
+Version: 0.2.0
 Summary: A metric learning toolkit
 Author-email: Arthur Porto <agporto@gmail.com>, Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://github.com/agporto/BioEncoder
 Project-URL: Bug Tracker, https://github.com/agporto/BioEncoder/issues
 Keywords: metric learning,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
@@ -35,15 +35,15 @@
 
 ## Features
 - Taxon-agnostic dataloaders (making it applicable to any dataset - not just biological ones)
 - Support of [timm models](https://github.com/rwightman/pytorch-image-models), and [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)
 - Access to state-of-the-art metric losses, such as [Supcon](https://arxiv.org/abs/2004.11362) and  [Sub-center ArcFace](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123560715.pdf).
 - [Exponential Moving Average](https://github.com/fadel/pytorch_ema) for stable training, and Stochastic Moving Average for better generalization and performance.
 - [LRFinder](https://github.com/davidtvs/pytorch-lr-finder) for the second stage of the training.
-- Easy customization of hyperparameters, including augmentations, through `YAML` configs
+- Easy customization of hyperparameters, including augmentations, through `YAML` configs (check the [config-templates](config-templates) folder for examples)
 - Custom augmentations techniques via [albumentations](https://github.com/albumentations-team/albumentations)
 - TensorBoard logs and checkpoints (soon to come: WandB integration)
 - Streamlit app with rich model visualizations (e.g., [Grad-CAM](https://arxiv.org/abs/1610.02391))
 - Interactive [t-SNE](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html) and [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html) plots using [Bokeh](https://bokeh.org/)
 
 <div align="center">
     <p><img src="https://github.com/agporto/BioEncoder/raw/main/assets/bioencoder-interactive-plot.gif" width="500"></p>
@@ -54,19 +54,22 @@
 (for more detailed information consult [the help files](help))
 
 1\. Install BioEncoder (into a virtual environment with pytorch/CUDA): 
 ````
 pip install bioencoder
 ````
 
-2\. Download example dataset (includes images and configs): https://osf.io/download/gsd5z/
+2\. Download example dataset from the data repo: [https://zenodo.org/records/10909614/files/BioEncoder-data.zip](https://zenodo.org/records/10909614/files/BioEncoder-data.zip?download=1&preview=1). 
+This archive contains the images and configuration files needed for step 3/4, as well as the final model checkpoints and a script to reproduce the results and figures presented in the paper. To play around with theinteractive figures and the model explorer you can also skip the training / SWA steps. 
 
-3\. Start interactive session (e.g., in Spyder or VS code) and run:
+3\. Start interactive session (e.g., in Spyder or VS code) and run the following commands one by one:
 
 ```python
+## use "overwrite=True to redo a step
+
 import bioencoder
 
 ## global setup
 bioencoder.configure(root_dir=r"bioencoder_wd", run_name="v1")
 
 ## split dataset
 bioencoder.split_dataset(image_dir=r"~/Downloads/damselflies-aligned-trai_val", max_ratio=6, random_seed=42)
@@ -79,29 +82,51 @@
 bioencoder.interactive_plots(config_path=r"bioencoder_configs/plot_stage1.yml")
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage1.yml")
 
 ## (optional) learning rate finder for stage 2
 bioencoder.lr_finder(config_path=r"bioencoder_configs/lr_finder.yml")
 
 ## train stage 2
-bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml", overwrite=True)
+bioencoder.train(config_path=r"bioencoder_configs/train_stage2.yml")
 bioencoder.swa(config_path=r"bioencoder_configs/swa_stage2.yml")
 
 ## explore model from stage 2
 bioencoder.model_explorer(config_path=r"bioencoder_configs/explore_stage2.yml")
 
 ```
+4\. Alternatively, you can directly use the command line interface: 
+
+```python
+## use the flag "--overwrite" to redo a step
+
+bioencoder_configure --root-dir bioencoder_wd --run-name v1
+bioencoder_split_dataset --image-dir "~/Downloads/damselflies-aligned-trai_val" --max-ratio 6 --random-seed 42
+bioencoder_train --config-path "bioencoder_configs/train_stage1.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage1.yml"
+bioencoder_interactive_plots --config-path "bioencoder_configs/plot_stage1.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage1.yml"
+bioencoder_lr_finder --config-path "bioencoder_configs/lr_finder.yml"
+bioencoder_train --config-path "bioencoder_configs/train_stage2.yml"
+bioencoder_swa --config-path "bioencoder_configs/swa_stage2.yml"
+bioencoder_model_explorer --config-path "bioencoder_configs/explore_stage2.yml"
+
+```
 
 ## Citation
 
 Please cite BioEncoder as follows:
 
 ```bibtex
-@UNPUBLISHED{
-    Lurig2024-pb,
-    title     = "BioEncoder: a metric learning toolkit for comparative organismal biology",
-    author    = "L{\"u}rig, Moritz D and Di Martino, Emanuela and Porto, Arthur", 
-    journal  = "bioRxiv",
-    language  = "en",
-    doi       = "xxxx"
+
+@UNPUBLISHED{Luerig2024-ov,
+  title    = "{BioEncoder}: a metric learning toolkit for comparative
+              organismal biology",
+  author   = "Luerig, Moritz D and Di Martino, Emanuela and Porto, Arthur",
+  journal  = "bioRxiv",
+  pages    = "2024.04.03.587987",
+  month    =  apr,
+  year     =  2024,
+  language = "en",
+  doi      = "10.1101/2024.04.03.587987"
 }
+
 ```
```

### Comparing `bioencoder-0.1.1/bioencoder.egg-info/SOURCES.txt` & `bioencoder-0.2.0/bioencoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioencoder-0.1.1/pyproject.toml` & `bioencoder-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	{name = "Moritz Lürig", email = "moritz.luerig@gmail.com"},
 	]
 description = "A metric learning toolkit"
 readme = "README.md"
 requires-python = "==3.9.*"
 keywords = ["metric learning", "biology"]
 dynamic = ["dependencies"]
-version = "0.1.1"
+version = "0.2.0"
 
 [project.urls]
 "Homepage" = "https://github.com/agporto/BioEncoder"
 "Bug Tracker" = "https://github.com/agporto/BioEncoder/issues"
 
 [project.scripts]
 bioencoder_configure = "bioencoder.scripts.configure:cli"
```

