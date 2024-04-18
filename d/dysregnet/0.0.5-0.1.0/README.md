# Comparing `tmp/dysregnet-0.0.5.tar.gz` & `tmp/dysregnet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysregnet-0.0.5.tar", last modified: Wed Nov 15 13:56:54 2023, max compression
+gzip compressed data, was "dysregnet-0.1.0.tar", last modified: Thu Apr 18 07:22:28 2024, max compression
```

## Comparing `dysregnet-0.0.5.tar` & `dysregnet-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:56:54.627888 dysregnet-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-15 13:56:43.000000 dysregnet-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2023-11-15 13:56:54.627888 dysregnet-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2023-11-15 13:56:43.000000 dysregnet-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 13:56:54.627888 dysregnet-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-15 13:56:43.000000 dysregnet-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:56:54.623888 dysregnet-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:56:54.627888 dysregnet-0.0.5/src/dysregnet/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-15 13:56:43.000000 dysregnet-0.0.5/src/dysregnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2023-11-15 13:56:43.000000 dysregnet-0.0.5/src/dysregnet/dysregnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2023-11-15 13:56:43.000000 dysregnet-0.0.5/src/dysregnet/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:56:54.627888 dysregnet-0.0.5/src/dysregnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2023-11-15 13:56:54.000000 dysregnet-0.0.5/src/dysregnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-15 13:56:54.000000 dysregnet-0.0.5/src/dysregnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 13:56:54.000000 dysregnet-0.0.5/src/dysregnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-15 13:56:54.000000 dysregnet-0.0.5/src/dysregnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-15 13:56:54.000000 dysregnet-0.0.5/src/dysregnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:22:28.367302 dysregnet-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 07:22:20.000000 dysregnet-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-18 07:22:28.367302 dysregnet-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-18 07:22:20.000000 dysregnet-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:22:28.367302 dysregnet-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 07:22:20.000000 dysregnet-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:22:28.367302 dysregnet-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:22:28.367302 dysregnet-0.1.0/src/dysregnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 07:22:20.000000 dysregnet-0.1.0/src/dysregnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-18 07:22:20.000000 dysregnet-0.1.0/src/dysregnet/dysregnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-18 07:22:20.000000 dysregnet-0.1.0/src/dysregnet/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:22:28.367302 dysregnet-0.1.0/src/dysregnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-18 07:22:28.000000 dysregnet-0.1.0/src/dysregnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 07:22:28.000000 dysregnet-0.1.0/src/dysregnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:22:28.000000 dysregnet-0.1.0/src/dysregnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 07:22:28.000000 dysregnet-0.1.0/src/dysregnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 07:22:28.000000 dysregnet-0.1.0/src/dysregnet.egg-info/top_level.txt
```

### Comparing `dysregnet-0.0.5/LICENSE` & `dysregnet-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dysregnet-0.0.5/PKG-INFO` & `dysregnet-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysregnet
-Version: 0.0.5
+Version: 0.1.0
 Summary: DysRegNet
 Home-page: https://github.com/biomedbigdata/DysRegNet_package
 Author: Zakaria Louadi, Olga Lazareva, Johannes Kersting
 Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,156 +23,118 @@
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 
 [![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
 
 # DysRegNet package
-
-
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
-
-
 ## Installation
 To install the package from PyPI please run:
-
-`pip install dysregnet`
-
+```bash
+pip install dysregnet
+```
 
 or you can install it from git:
-
-`git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package`
-
-`python setup.py install`
-
-
+```bash
+git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package
+python setup.py install
+```
 
 ## Data input
+The inputs of the  package are the following Pandas DataFrame objects:
 
-The inputs of the  package are the following Pandas DataFrame object:
-
-
-- expression_data  - Gene expression matrix with the format: patients as rows (first column - patients/samples ids), and genes as columns.
+- expression_data  - Gene expression matrix in the format: patients as rows (first column - patients/samples ids), and genes as columns.
 - GRN - Gene Regulatory Network (GRN) with two columns in the following order ['TF', 'target'].
 - meta -  Metadata with the first column containing patients/samples ids and other columns for the condition and the covariates.
 
-
 The patients id or samples ids must be the same in the "expression_data" and  "meta". Additionally, gene names or ids must match the ones in the "GRN" DataFrame. 
 
 In the condition column of the meta DataFrame, the control samples should be encoded as 0 and case samples as 1.
 
 The gene regulatory network should be provided by the user. You can either use an experimental validated GRN or learn it from control samples. We recommend using software like [arboreto](https://github.com/aertslab/arboreto) since you can use its output directly to DysRegNet.
 
-
-
-
-
 ## Parameters 
-
-
 Additionally, you can provide the following parameters:
 
-
-            
 - conCol: Column name for the condition in the meta DataFrame.
 
 - CatCov: List of categorical variable names. They should match the name of their columns in the meta Dataframe.
 
 - ConCov: List of continuous covariates. They should match the name of their columns in the meta Dataframe.
 
-- zscoring: Boolean, default: False. zscoring of expression data (if needed).
+- zscoring: If True, DysRegNet will scale the expression of each gene and all continuous confounders based on their mean and standard deviation in the control samples.
 
 - bonferroni_alpha: P-value threshold for multiple testing correction
 
-- normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
+- normaltest: If True, DysRegNet runs a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
-- normaltest_alpha: p-value threshold for normaltest (if True).
+- normaltest_alpha: P-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down-regulation of an activation or up-regulation of a supressions). Please check the paper for more details.
+- direction_condition:  If True, DysRegNet will only consider case samples with positive residuals (target gene overexpressed) for models with a negative TF coefficient as potentially dysregulated. Similarly, for positive TF coefficients, only case samples with negative residuals are considered. Please check the paper for more details.
 
+The parameters are also annotated with dockstrings for more details.
 
 ## Get Started
-
-
-Please note that the functions are annotated with dockstrings for more details.
-
 Import the package and pandas:
-
-
 ```python
 import dysregnet
 import pandas as pd
 ```
 
-
-
 Define the confounding variables or the design matrix 
-
 ```python
-# The condition column
+# define condition column (0 indicated control, 1 indicates case)
 conCol='condition'
 
-# categorical variable columns in meta dataframe.
-# these columns will be transformed to variables for regression 
+# define categorical confounder columns in meta dataframe 
 CatCov=['race','gender']  
 
-# continuous variable columns in meta dataframe.
+# define continuous confounder columns in meta dataframe.
 ConCov=['birth_days_to']
 ```
 
-
 Run DysRegNet
-
 ```python
 data=dysregnet.run(expression_data=expr,
                    meta=meta, 
                    GRN=grn,
                    conCol=conCol
                    CatCov=CatCov,
                    ConCov=ConCov,
                    direction_condition=True,
                    normaltest=True,
-                   R2_threshold=.2 )
+                   R2_threshold=.2)
 
-# results table
+# get the patient-specific dysregulate networks
 data.get_results()
 
-# or a binary result
-
+# or with binary edges
 data.get_results_binary()
 
 # get R2 values, coefficients, and coefficient p-values for all models/edges
 data.get_model_stats()
-
 ```
 
-The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
-
-
-
 ## The output
-
 The package outputs a data frame that represents patient-specific dysregulated edges. The columns represent edges, and the rows are patient IDs. 
 
-In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported, with a positive in case of activation and a negative sign in case of repression (different than the sign of the residual). 
+In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported. 
 
 The method "get_results_binary()" outputs binarized dysregulations instead of z-scores. 
 
+"get_model_stats()" outputs R2 values, coefficients, and coefficient p-values for all models/edges.
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
-
 You will need to download the demo dataset and extract the files into test dataset/
 
 Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
-
-
 ## Cite
-
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
-Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
+Johannes Kersting*, Olga Lazareva*, Zakaria Louadi*, David B. Blumenthal, Jan Baumbach, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

### Comparing `dysregnet-0.0.5/README.md` & `dysregnet-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,114 @@
 [![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
 
 # DysRegNet package
-
-
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
-
-
 ## Installation
 To install the package from PyPI please run:
-
-`pip install dysregnet`
-
+```bash
+pip install dysregnet
+```
 
 or you can install it from git:
-
-`git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package`
-
-`python setup.py install`
-
-
+```bash
+git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package
+python setup.py install
+```
 
 ## Data input
+The inputs of the  package are the following Pandas DataFrame objects:
 
-The inputs of the  package are the following Pandas DataFrame object:
-
-
-- expression_data  - Gene expression matrix with the format: patients as rows (first column - patients/samples ids), and genes as columns.
+- expression_data  - Gene expression matrix in the format: patients as rows (first column - patients/samples ids), and genes as columns.
 - GRN - Gene Regulatory Network (GRN) with two columns in the following order ['TF', 'target'].
 - meta -  Metadata with the first column containing patients/samples ids and other columns for the condition and the covariates.
 
-
 The patients id or samples ids must be the same in the "expression_data" and  "meta". Additionally, gene names or ids must match the ones in the "GRN" DataFrame. 
 
 In the condition column of the meta DataFrame, the control samples should be encoded as 0 and case samples as 1.
 
 The gene regulatory network should be provided by the user. You can either use an experimental validated GRN or learn it from control samples. We recommend using software like [arboreto](https://github.com/aertslab/arboreto) since you can use its output directly to DysRegNet.
 
-
-
-
-
 ## Parameters 
-
-
 Additionally, you can provide the following parameters:
 
-
-            
 - conCol: Column name for the condition in the meta DataFrame.
 
 - CatCov: List of categorical variable names. They should match the name of their columns in the meta Dataframe.
 
 - ConCov: List of continuous covariates. They should match the name of their columns in the meta Dataframe.
 
-- zscoring: Boolean, default: False. zscoring of expression data (if needed).
+- zscoring: If True, DysRegNet will scale the expression of each gene and all continuous confounders based on their mean and standard deviation in the control samples.
 
 - bonferroni_alpha: P-value threshold for multiple testing correction
 
-- normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
+- normaltest: If True, DysRegNet runs a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
-- normaltest_alpha: p-value threshold for normaltest (if True).
+- normaltest_alpha: P-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down-regulation of an activation or up-regulation of a supressions). Please check the paper for more details.
+- direction_condition:  If True, DysRegNet will only consider case samples with positive residuals (target gene overexpressed) for models with a negative TF coefficient as potentially dysregulated. Similarly, for positive TF coefficients, only case samples with negative residuals are considered. Please check the paper for more details.
 
+The parameters are also annotated with dockstrings for more details.
 
 ## Get Started
-
-
-Please note that the functions are annotated with dockstrings for more details.
-
 Import the package and pandas:
-
-
 ```python
 import dysregnet
 import pandas as pd
 ```
 
-
-
 Define the confounding variables or the design matrix 
-
 ```python
-# The condition column
+# define condition column (0 indicated control, 1 indicates case)
 conCol='condition'
 
-# categorical variable columns in meta dataframe.
-# these columns will be transformed to variables for regression 
+# define categorical confounder columns in meta dataframe 
 CatCov=['race','gender']  
 
-# continuous variable columns in meta dataframe.
+# define continuous confounder columns in meta dataframe.
 ConCov=['birth_days_to']
 ```
 
-
 Run DysRegNet
-
 ```python
 data=dysregnet.run(expression_data=expr,
                    meta=meta, 
                    GRN=grn,
                    conCol=conCol
                    CatCov=CatCov,
                    ConCov=ConCov,
                    direction_condition=True,
                    normaltest=True,
-                   R2_threshold=.2 )
+                   R2_threshold=.2)
 
-# results table
+# get the patient-specific dysregulate networks
 data.get_results()
 
-# or a binary result
-
+# or with binary edges
 data.get_results_binary()
 
 # get R2 values, coefficients, and coefficient p-values for all models/edges
 data.get_model_stats()
-
 ```
 
-The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
-
-
-
 ## The output
-
 The package outputs a data frame that represents patient-specific dysregulated edges. The columns represent edges, and the rows are patient IDs. 
 
-In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported, with a positive in case of activation and a negative sign in case of repression (different than the sign of the residual). 
+In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported. 
 
 The method "get_results_binary()" outputs binarized dysregulations instead of z-scores. 
 
+"get_model_stats()" outputs R2 values, coefficients, and coefficient p-values for all models/edges.
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
-
 You will need to download the demo dataset and extract the files into test dataset/
 
 Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
-
-
 ## Cite
-
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
-Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
+Johannes Kersting*, Olga Lazareva*, Zakaria Louadi*, David B. Blumenthal, Jan Baumbach, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

### Comparing `dysregnet-0.0.5/setup.py` & `dysregnet-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(name='dysregnet',
-      version='0.0.5',
+      version='0.1.0',
       description='DysRegNet',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/biomedbigdata/DysRegNet_package',
       author='Zakaria Louadi, Olga Lazareva, Johannes Kersting',
       author_email='zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de',
       license='GPLv3',
```

### Comparing `dysregnet-0.0.5/src/dysregnet/dysregnet.py` & `dysregnet-0.1.0/src/dysregnet/dysregnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,70 +17,69 @@
                      expression_data,
                      GRN,
                      meta, 
                      conCol='condition', 
                      CatCov=[],  
                      ConCov=[],
                      zscoring=False,
-                     bonferroni_alpha= 1e-2,
+                     bonferroni_alpha=1e-2,
                      R2_threshold=None,
                      normaltest=False,
                      normaltest_alpha=1e-3,
-                     direction_condition=True):
-
+                     direction_condition=False):
                     """
                     Raw data processing for further analysis
 
-                    expression_data: a pandas DataFrame (rows=samples, columns=genes)
-                             Gene expression matrix with the format: patients as rows (first column - patients/samples ids), and genes as columns.
-                             Patients/samples ids must match the ones in meta DataFrame.
-                             Gene names or ids must match the ones in GRN DataFrame
-
-                    GRN: a pandas DataFrame 
-                          Gene Regulatory Network (GRN) with two columns in the following order ['TF', 'target'].
-
-                    meta: a pandas DataFrame  
-                            Meta data: First column should contain patients/samples ids and other column for covariates/condition. 
-                            Please make sure to have condition column in the meta DataFrame with 0 as control and 1 as the condition.
-                            Specify the condition Column name in "conCol". 
-                            Optionally :
-                                Specify categorical variable columns in the parameter CatCov.
-                                Specify continuous variable columns in the parameter ConCov.
-
-                    conCol: str, default=='condition'
-                            Column name for the condition in the meta data. Should be provided in case of desing=="two".
-
-
-                    CatCov: List of strings.
-                            List of categorical variable names. They should match the name of their columns in meta Dataframe.
-
-                    ConCov: List of strings.
-                            List of continuous covariates. They should match the name of their columns in meta Dataframe.
-
-
-                    zscoring: boolean, default: False 
-                         zscoring of expression data (if needed).
-
-                    bonferroni_alpha: Float
-                            P value threshold for multiple testing correction
-
-                    normaltest: Bool
-                            If True. Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
-
-                    normaltest_alpha: Float
-                         normaltest p value threshold.
-
-                    R2_threshold: float from 0 to 1 (optional)
-
-                        Coefficient of determination threshold for every edge in GRN. If the R2 is less that threshold, the edge will not be considered in the analysis. 
-
-                    direction_condition: Bool
-                         If True: only include dysregulation that are relevalant for the interactions: down regulation of an activation or up regulation of a supressions. Please check the paper for more details.
-
-                          """
+                    expression_data: pandas DataFrame (rows=samples, columns=genes)
+                        Gene expression matrix in the format: patients as rows (first column - patients/samples ids), and genes as columns.
+                        Patients/sample IDs must match the ones in the meta DataFrame.
+                        Gene names or IDs must match the ones in the GRN DataFrame.
+
+                    GRN: pandas DataFrame 
+                        Gene Regulatory Network (GRN) with two columns in the following order ['TF', 'target'].
+
+                    meta: pandas DataFrame  
+                        The first column has to contain patients/sample IDs. 
+                        Further columns can be used to define covariates and the sample condition. 
+                        Please make sure to have a condition column in the meta DataFrame with 0 indicating control and 1 indicating case samples.
+                        Specify the condition Column name in 'conCol'.
+                        Optionally :
+                            Specify categorical variable columns in the parameter CatCov.
+                            Specify continuous variable columns in the parameter ConCov.
+
+                    conCol: str, default: 'condition'
+                        Column name for the condition in the metadata.
+
+                    CatCov: List of strings, default: []
+                        List of categorical variable names. They should match the name of their columns in the meta Dataframe.
+
+                    ConCov: List of strings, default: []
+                        List of continuous covariates. They should match the name of their columns in the meta Dataframe.
+
+                    zscoring: bool, default: False 
+                        If True, DysRegNet will scale the expression of each gene and all continuous confounders based on their mean and standard deviation in the control samples.
+                        This can make the obtained model coefficients more interpretable.
+
+                    bonferroni_alpha: float, default: 0.01
+                        P value threshold for multiple testing correction.
+
+                    normaltest: bool, default: False
+                        If True, DysRegNet runs a normality test for the control residuals with "scipy.stats.normaltest". 
+                        If residuals do not follow a normal distribution, the edge will not be considered in the analysis. 
+
+                    normaltest_alpha: float, default: 0.001
+                        P-value threshold for the normal test.
+
+                    R2_threshold: float, default: None
+                        R-squared (R2) threshold from 0 to 1.  If the fit is weaker, the edge will not be considered in the analysis.
+
+                    direction_condition: boolean, default: False
+                         If True, DysRegNet will only consider case samples with positive residuals (target gene overexpressed) for models with a negative TF coefficient
+                         as potentially dysregulated. Similarly, for positive TF coefficients, only case samples with negative residuals are considered. Please check the paper for more details.
+                    """
 
 
 
                     # init method 
                     self.conCol=conCol
                     self.CatCov=CatCov
                     self.ConCov=ConCov
```

### Comparing `dysregnet-0.0.5/src/dysregnet/functions.py` & `dysregnet-0.1.0/src/dysregnet/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 import pandas as pd
 from scipy.stats import zscore
-from sklearn.linear_model import LinearRegression
+from sklearn.preprocessing import StandardScaler
 from tqdm import tqdm
 import numpy as np
 from scipy import stats
 import statsmodels.stats.multitest as mt
 import statsmodels.api as sm
 
 
 def process_data(data):
        
 
         # process covariates and design matrix
         
-        all_covariates= data.CatCov + data.ConCov
+        all_covariates = data.CatCov + data.ConCov
 
         if not all_covariates or len(data.meta)==1:
 
                 # No covariate provided
-                print('You did not input any covariates in CatCov or ConCov parameters, proceed without them.')
+                print('You did not input any covariates in CatCov or ConCov parameters, proceeding without them.')
                 cov_df=None
 
         else:
 
 
                 # check if covariates exist in meta
                 if not set(all_covariates).issubset(data.meta.columns):
                     raise ValueError("Invalid elements in CatCov or ConCov. Please check that all covariates names (continuous or categorials) are in the meta DataFrame. ")
 
-                cov_df=data.meta[all_covariates]
+                cov_df = data.meta[all_covariates]
 
                 # process categorial covariate
                 # drop_first is important to avoid multicollinear
-                cov_df=pd.get_dummies(cov_df, columns=data.CatCov, drop_first=True, dtype=int)
+                cov_df = pd.get_dummies(cov_df, columns=data.CatCov, drop_first=True, dtype=int)
                 
                 
                 
-        # z scoring of expression
-        if data.zscoring: expr=data.expression_data.apply(zscore) 
-        else:  expr=data.expression_data
+        # z scoring
+        if data.zscoring:
+
+            # expression data
+            # fit a scaler base on the control samples
+            scaler = StandardScaler()
+            scaler.fit(data.expression_data[data.meta[data.conCol]==0])
+
+            # scale the expression data
+            expr = pd.DataFrame(
+                scaler.transform(data.expression_data),
+                columns=data.expression_data.columns, 
+                index=data.expression_data.index
+            )
+            
+            # continuous confounders
+            if cov_df is not None and len(data.ConCov)>0:
+
+                # fit a scaler base on the control samples
+                scaler = StandardScaler()
+                scaler.fit(data.meta.loc[data.meta[data.conCol]==0,data.ConCov])
+
+                # scale the continuous confounders data
+                cov_df[data.ConCov] = scaler.transform(data.meta[data.ConCov])
+            
+        else:  
+            expr = data.expression_data
         
         
         #get control and case sample 
-        control= data.meta[ data.meta[data.conCol]==0 ].index.values.tolist()
-        case=data.meta[ data.meta[data.conCol]==1 ].index.values.tolist()
+        control = data.meta[ data.meta[data.conCol]==0 ].index.values.tolist()
+        case = data.meta[ data.meta[data.conCol]==1 ].index.values.tolist()
 
         return cov_df, expr, control, case
     
     
     
 def dyregnet_model(data):
         
@@ -76,48 +100,47 @@
                     edge = (tup[1],tup[2])
                     
                     # skip self loops
                     if edge[0] != edge[1]:
 
                         # prepare control for fitting model
                         x_train = control[  [edge[0]] + covariate_name ]
-                        x_train = sm.add_constant(x_train) # add bias
+                        x_train = sm.add_constant(x_train, has_constant='add') # add bias
                         y_train = control[edge[1]].values
 
                         # fit the model
                         model = sm.OLS(y_train, x_train)
                         results = model.fit()
                         
                         model_stats[edge] = [results.rsquared] + list(results.params.values) + list(results.pvalues.values)
                         
-
                         # get residuals of control
-                        resid_control = results.predict(x_train) -  y_train
+                        resid_control = y_train - results.predict(x_train) 
 
                         # test data (case or condition)
                         x_test = case[  [edge[0]]+ covariate_name    ]
-                        x_test = sm.add_constant(x_test) # add bias
+                        x_test = sm.add_constant(x_test, has_constant='add') # add bias
                         y_test = case[edge[1]].values
 
 
                         # define residue for cases
-                        resid_case =  results.predict(x_test) - y_test
+                        resid_case =  y_test - results.predict(x_test)
 
                         
                         # condition of direction
                         cond = True
                         direction = np.sign(results.params.iloc[1])
                         
                         
                         # two sided p_value as default
                         # if direction_condition is false calculate, two sided p value
                         sides = 2
 
                         if data.direction_condition: 
-                            cond = ( direction * resid_case ) > 0
+                            cond = ( direction * resid_case ) < 0
                             
                             # if direction_condition is true only calculate one sided p value
                             sides = 1
 
                         
                         # calculate zscore
                         zscore= (resid_case - resid_control.mean()) / resid_control.std()
@@ -147,17 +170,14 @@
 
                         # correct for multi. testing
                         pvalues=sm.stats.multipletests(pvalues,method='bonferroni',alpha=data.bonferroni_alpha)[1]
 
                         pvalues= pvalues < data.bonferroni_alpha
 
 
-                        # add direction to z scores
-                        zscore=abs(zscore) * direction
-
 
                         # direction condition and a p_value 
                         valid= cond * pvalues
 
 
 
                         # shrink the z scores that are not signifcant or not in the condition
```

### Comparing `dysregnet-0.0.5/src/dysregnet.egg-info/PKG-INFO` & `dysregnet-0.1.0/src/dysregnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysregnet
-Version: 0.0.5
+Version: 0.1.0
 Summary: DysRegNet
 Home-page: https://github.com/biomedbigdata/DysRegNet_package
 Author: Zakaria Louadi, Olga Lazareva, Johannes Kersting
 Author-email: zakaria.louadi@tum.de, olga.lazareva@tum.de, johannes.kersting@tum.de
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,156 +23,118 @@
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 
 [![PyPI version](https://badge.fury.io/py/dysregnet.svg)](https://badge.fury.io/py/dysregnet)
 
 # DysRegNet package
-
-
 DysRegNet, is a  method for inferring patient-specific regulatory alterations (dysregulations) from gene expression profiles. DysRegNet uses linear models to account for confounders and residual-derived z-scores to assess significance.
-
-
 ## Installation
 To install the package from PyPI please run:
-
-`pip install dysregnet`
-
+```bash
+pip install dysregnet
+```
 
 or you can install it from git:
-
-`git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package`
-
-`python setup.py install`
-
-
+```bash
+git clone https://github.com/biomedbigdata/DysRegNet_package.git  && cd DysRegNet_package
+python setup.py install
+```
 
 ## Data input
+The inputs of the  package are the following Pandas DataFrame objects:
 
-The inputs of the  package are the following Pandas DataFrame object:
-
-
-- expression_data  - Gene expression matrix with the format: patients as rows (first column - patients/samples ids), and genes as columns.
+- expression_data  - Gene expression matrix in the format: patients as rows (first column - patients/samples ids), and genes as columns.
 - GRN - Gene Regulatory Network (GRN) with two columns in the following order ['TF', 'target'].
 - meta -  Metadata with the first column containing patients/samples ids and other columns for the condition and the covariates.
 
-
 The patients id or samples ids must be the same in the "expression_data" and  "meta". Additionally, gene names or ids must match the ones in the "GRN" DataFrame. 
 
 In the condition column of the meta DataFrame, the control samples should be encoded as 0 and case samples as 1.
 
 The gene regulatory network should be provided by the user. You can either use an experimental validated GRN or learn it from control samples. We recommend using software like [arboreto](https://github.com/aertslab/arboreto) since you can use its output directly to DysRegNet.
 
-
-
-
-
 ## Parameters 
-
-
 Additionally, you can provide the following parameters:
 
-
-            
 - conCol: Column name for the condition in the meta DataFrame.
 
 - CatCov: List of categorical variable names. They should match the name of their columns in the meta Dataframe.
 
 - ConCov: List of continuous covariates. They should match the name of their columns in the meta Dataframe.
 
-- zscoring: Boolean, default: False. zscoring of expression data (if needed).
+- zscoring: If True, DysRegNet will scale the expression of each gene and all continuous confounders based on their mean and standard deviation in the control samples.
 
 - bonferroni_alpha: P-value threshold for multiple testing correction
 
-- normaltest: Boolean. If True, Run a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
+- normaltest: If True, DysRegNet runs a normality test for residuals "scipy.stats.normaltest". If residuals are not normal, the edge will not be considered in the analysis. 
 
-- normaltest_alpha: p-value threshold for normaltest (if True).
+- normaltest_alpha: P-value threshold for normaltest (if True).
 
 - R2_threshold: R-squared (R2) threshold from 0 to 1 (optional).  If the fit is weaker, the edge will not be considered in the analysis. 
 
-- direction_condition: Boolean. If True: only include dysregulation that are relevant for the interactions (down-regulation of an activation or up-regulation of a supressions). Please check the paper for more details.
+- direction_condition:  If True, DysRegNet will only consider case samples with positive residuals (target gene overexpressed) for models with a negative TF coefficient as potentially dysregulated. Similarly, for positive TF coefficients, only case samples with negative residuals are considered. Please check the paper for more details.
 
+The parameters are also annotated with dockstrings for more details.
 
 ## Get Started
-
-
-Please note that the functions are annotated with dockstrings for more details.
-
 Import the package and pandas:
-
-
 ```python
 import dysregnet
 import pandas as pd
 ```
 
-
-
 Define the confounding variables or the design matrix 
-
 ```python
-# The condition column
+# define condition column (0 indicated control, 1 indicates case)
 conCol='condition'
 
-# categorical variable columns in meta dataframe.
-# these columns will be transformed to variables for regression 
+# define categorical confounder columns in meta dataframe 
 CatCov=['race','gender']  
 
-# continuous variable columns in meta dataframe.
+# define continuous confounder columns in meta dataframe.
 ConCov=['birth_days_to']
 ```
 
-
 Run DysRegNet
-
 ```python
 data=dysregnet.run(expression_data=expr,
                    meta=meta, 
                    GRN=grn,
                    conCol=conCol
                    CatCov=CatCov,
                    ConCov=ConCov,
                    direction_condition=True,
                    normaltest=True,
-                   R2_threshold=.2 )
+                   R2_threshold=.2)
 
-# results table
+# get the patient-specific dysregulate networks
 data.get_results()
 
-# or a binary result
-
+# or with binary edges
 data.get_results_binary()
 
 # get R2 values, coefficients, and coefficient p-values for all models/edges
 data.get_model_stats()
-
 ```
 
-The expected run time for the installation and running the demo dataset on a "normal" desktop computer is around 3~5 minutes.
-
-
-
 ## The output
-
 The package outputs a data frame that represents patient-specific dysregulated edges. The columns represent edges, and the rows are patient IDs. 
 
-In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported, with a positive in case of activation and a negative sign in case of repression (different than the sign of the residual). 
+In the result table, a value of 0 means that the edge is not significantly dysregulated (different from control samples). Otherwise, the z-score is reported. 
 
 The method "get_results_binary()" outputs binarized dysregulations instead of z-scores. 
 
+"get_model_stats()" outputs R2 values, coefficients, and coefficient p-values for all models/edges.
 
 ## Example
 
 A simple example for running DysRegNet:
 ([Notebook](https://github.com/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)/[Google Colab](https://colab.research.google.com/github/biomedbigdata/DysRegNet_package/blob/main/test.ipynb)).
 
-
 You will need to download the demo dataset and extract the files into test dataset/
 
 Link for the demo dataset: https://figshare.com/ndownloader/files/35142652
 
-
-
 ## Cite
-
 "DysRegNet: Patient-specific and confounder-aware dysregulated network inference"
-Olga Lazareva*, Zakaria Louadi*, Johannes Kersting, Jan Baumbach, David B. Blumenthal, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
+Johannes Kersting*, Olga Lazareva*, Zakaria Louadi*, David B. Blumenthal, Jan Baumbach, Markus List. bioRxiv 2022.04.29.490015; doi: https://doi.org/10.1101/2022.04.29.490015. * equal first-authors
```

