# Comparing `tmp/ntqr-0.2.tar.gz` & `tmp/ntqr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntqr-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ntqr-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ntqr-0.2.tar` & `ntqr-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,45 @@
--rw-r--r--   0        0        0     1148 2024-02-05 20:00:32.987803 ntqr-0.2/ACKNOWLEDGEMENTS.md
--rw-r--r--   0        0        0     1086 2024-01-16 18:36:30.844289 ntqr-0.2/LICENSE.txt
--rw-r--r--   0        0        0      275 2024-01-29 19:41:47.216444 ntqr-0.2/MANIFEST.in
--rw-r--r--   0        0        0      350 2024-01-18 10:30:20.837055 ntqr-0.2/Makefile
--rw-r--r--   0        0        0     3695 2024-02-24 13:26:58.274120 ntqr-0.2/README.md
--rw-r--r--   0        0        0     1051 2024-01-27 15:39:05.468366 ntqr-0.2/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2024-01-19 10:34:30.767245 ntqr-0.2/docs/Makefile
--rw-r--r--   0        0        0        0 2024-02-06 23:12:20.977433 ntqr-0.2/docs/conf.py
--rw-r--r--   0        0        0      804 2024-01-19 10:34:30.768496 ntqr-0.2/docs/make.bat
--rw-r--r--   0        0        0      112 2024-02-27 19:48:50.032819 ntqr-0.2/docs/requirements.txt
--rw-r--r--   0        0        0     1282 2024-02-24 13:26:58.274562 ntqr-0.2/docs/source/conceptual.md
--rw-r--r--   0        0        0     2223 2024-02-27 21:36:32.553021 ntqr-0.2/docs/source/conf.py
--rw-r--r--   0        0        0      554 2024-02-27 21:25:03.756041 ntqr-0.2/docs/source/index.md
--rw-r--r--   0        0        0       49 2024-02-12 15:27:49.840150 ntqr-0.2/docs/source/modules.md
--rw-r--r--   0        0        0   225845 2024-02-27 21:36:07.022399 ntqr-0.2/docs/source/notebooks/ExactAlgebraicSolutionErrorIndependent.ipynb
--rw-r--r--   0        0        0   142688 2024-02-25 16:39:55.863901 ntqr-0.2/docs/source/notebooks/LogicOfUnsupervisedEvaluationTutorial.ipynb
--rw-r--r--   0        0        0    14517 2024-02-27 19:31:23.924145 ntqr-0.2/docs/source/notebooks/Tutorial.ipynb
--rw-r--r--   0        0        0      185 2024-01-25 10:41:46.061314 ntqr-0.2/docs/source/ntqr.md
--rw-r--r--   0        0        0      564 2024-01-25 10:41:46.037353 ntqr-0.2/docs/source/ntqr.r2.md
--rw-r--r--   0        0        0     4074 2024-02-24 13:26:58.276701 ntqr-0.2/docs/source/research/GradingLLMs.md
--rw-r--r--   0        0        0     2869 2024-02-24 13:26:58.277499 ntqr-0.2/docs/source/research/MathematicsOfAlgebraicEvaluation.md
--rw-r--r--   0        0        0     5363 2024-02-24 13:26:58.278216 ntqr-0.2/docs/source/research/TheScienceOfAlgebraicEvaluation.md
--rw-r--r--   0        0        0     4902 2024-01-26 10:23:53.799362 ntqr-0.2/img/NTQRpt24.png
--rw-r--r--   0        0        0    27489 2024-02-27 19:41:21.768885 ntqr-0.2/img/uciAdultEvalPiaGauges.png
--rw-r--r--   0        0        0    19682 2024-02-14 11:07:07.643715 ntqr-0.2/img/uciAdultEvalPrevalenceGauges.png
--rw-r--r--   0        0        0     1294 2024-01-30 14:34:15.184346 ntqr-0.2/pyproject.toml
--rw-r--r--   0        0        0      414 2024-02-27 19:48:30.064573 ntqr-0.2/src/ntqr/__init__.py
--rw-r--r--   0        0        0       40 2024-01-18 10:53:21.631767 ntqr-0.2/src/ntqr/r2/__init__.py
--rw-r--r--   0        0        0    12158 2024-02-12 15:16:46.872814 ntqr-0.2/src/ntqr/r2/datasketches.py
--rw-r--r--   0        0        0    25541 2024-02-27 19:21:14.429894 ntqr-0.2/src/ntqr/r2/evaluators.py
--rw-r--r--   0        0        0      658 2024-01-16 14:20:41.109821 ntqr-0.2/src/ntqr/r2/examples.py
--rw-r--r--   0        0        0     8199 2024-02-27 11:57:56.728242 ntqr-0.2/src/ntqr/r2/postulates.py
--rw-r--r--   0        0        0        0 2024-02-15 13:52:58.865012 ntqr-0.2/src/ntqr/r3/__init__.py
--rw-r--r--   0        0        0     1949 2024-02-17 11:22:35.508926 ntqr-0.2/src/ntqr/r3/postulates.py
--rw-r--r--   0        0        0     1886 2024-01-25 19:00:53.660352 ntqr-0.2/tests/test_datasketches.py
--rw-r--r--   0        0        0     2596 2024-02-26 14:49:25.025914 ntqr-0.2/tests/test_evaluators.py
--rw-r--r--   0        0        0      554 2024-02-27 19:28:11.720071 ntqr-0.2/tests/test_r2_postulates.py
--rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 ntqr-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1148 2024-02-05 20:00:32.987803 ntqr-0.3.1/ACKNOWLEDGEMENTS.md
+-rw-r--r--   0        0        0     1086 2024-01-16 18:36:30.844289 ntqr-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      275 2024-01-29 19:41:47.216444 ntqr-0.3.1/MANIFEST.in
+-rw-r--r--   0        0        0      350 2024-01-18 10:30:20.837055 ntqr-0.3.1/Makefile
+-rw-r--r--   0        0        0     3694 2024-02-28 21:01:28.714321 ntqr-0.3.1/README.md
+-rw-r--r--   0        0        0     1051 2024-01-27 15:39:05.468366 ntqr-0.3.1/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2024-01-19 10:34:30.767245 ntqr-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-02-06 23:12:20.977433 ntqr-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0      804 2024-01-19 10:34:30.768496 ntqr-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0      108 2024-04-17 01:08:35.299258 ntqr-0.3.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1282 2024-02-24 13:26:58.274562 ntqr-0.3.1/docs/source/conceptual.md
+-rw-r--r--   0        0        0     2265 2024-04-17 01:09:17.397423 ntqr-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0      595 2024-04-17 20:12:13.969382 ntqr-0.3.1/docs/source/index.md
+-rw-r--r--   0        0        0       49 2024-02-12 15:27:49.840150 ntqr-0.3.1/docs/source/modules.md
+-rw-r--r--   0        0        0   278251 2024-04-17 21:43:54.521706 ntqr-0.3.1/docs/source/notebooks/ExactAlgebraicSolutionErrorIndependent.ipynb
+-rw-r--r--   0        0        0   143333 2024-04-17 14:15:49.073849 ntqr-0.3.1/docs/source/notebooks/LogicOfUnsupervisedEvaluationTutorial.ipynb
+-rw-r--r--   0        0        0   211160 2024-04-18 01:47:45.364392 ntqr-0.3.1/docs/source/notebooks/Tutorial.ipynb
+-rw-r--r--   0        0        0      185 2024-01-25 10:41:46.061314 ntqr-0.3.1/docs/source/ntqr.md
+-rw-r--r--   0        0        0      564 2024-01-25 10:41:46.037353 ntqr-0.3.1/docs/source/ntqr.r2.md
+-rw-r--r--   0        0        0   440564 2024-04-18 11:34:35.565726 ntqr-0.3.1/docs/source/research/EvaluatingLLMsThatGradeOtherLLMs.ipynb
+-rw-r--r--   0        0        0     4074 2024-02-24 13:26:58.276701 ntqr-0.3.1/docs/source/research/GradingLLMs.md
+-rw-r--r--   0        0        0     2869 2024-02-24 13:26:58.277499 ntqr-0.3.1/docs/source/research/MathematicsOfAlgebraicEvaluation.md
+-rw-r--r--   0        0        0     5363 2024-02-24 13:26:58.278216 ntqr-0.3.1/docs/source/research/TheScienceOfAlgebraicEvaluation.md
+-rw-r--r--   0        0        0     4902 2024-01-26 10:23:53.799362 ntqr-0.3.1/img/NTQRpt24.png
+-rw-r--r--   0        0        0   168641 2024-04-18 11:31:39.123560 ntqr-0.3.1/img/evals-llms-multistep-arithmetic.png
+-rw-r--r--   0        0        0    27489 2024-02-27 19:41:21.768885 ntqr-0.3.1/img/uciAdultEvalPiaGauges.png
+-rw-r--r--   0        0        0    19682 2024-02-14 11:07:07.643715 ntqr-0.3.1/img/uciAdultEvalPrevalenceGauges.png
+-rw-r--r--   0        0        0    40181 2024-04-16 13:20:04.993314 ntqr-0.3.1/img/uciadult-a-prevalence-comparisons.png
+-rw-r--r--   0        0        0     1353 2024-04-18 11:13:22.068773 ntqr-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      416 2024-04-18 11:44:49.906874 ntqr-0.3.1/src/ntqr/__init__.py
+-rw-r--r--   0        0        0       40 2024-01-18 10:53:21.631767 ntqr-0.3.1/src/ntqr/r2/__init__.py
+-rw-r--r--   0        0        0    12206 2024-04-17 00:22:20.189802 ntqr-0.3.1/src/ntqr/r2/datasketches.py
+-rw-r--r--   0        0        0     4180 2024-04-18 01:12:41.807237 ntqr-0.3.1/src/ntqr/r2/evaluations.py
+-rw-r--r--   0        0        0    26509 2024-04-18 01:43:25.551694 ntqr-0.3.1/src/ntqr/r2/evaluators.py
+-rw-r--r--   0        0        0      658 2024-01-16 14:20:41.109821 ntqr-0.3.1/src/ntqr/r2/examples.py
+-rw-r--r--   0        0        0     6258 2024-04-17 14:11:13.098620 ntqr-0.3.1/src/ntqr/r2/paxioms.py
+-rw-r--r--   0        0        0     3683 2024-04-18 11:44:28.674293 ntqr-0.3.1/src/ntqr/r2/plots.py
+-rw-r--r--   0        0        0      975 2024-04-17 13:52:31.177924 ntqr-0.3.1/src/ntqr/r2/raxioms.py
+-rw-r--r--   0        0        0    61532 2024-04-15 10:51:59.016338 ntqr-0.3.1/src/ntqr/r2/uci_adult_20240415.py
+-rw-r--r--   0        0        0        0 2024-02-15 13:52:58.865012 ntqr-0.3.1/src/ntqr/r3/__init__.py
+-rw-r--r--   0        0        0     1949 2024-02-17 11:22:35.508926 ntqr-0.3.1/src/ntqr/r3/postulates.py
+-rw-r--r--   0        0        0     1886 2024-01-25 19:00:53.660352 ntqr-0.3.1/tests/test_datasketches.py
+-rw-r--r--   0        0        0     3640 2024-04-17 00:57:18.073040 ntqr-0.3.1/tests/test_evaluators.py
+-rw-r--r--   0        0        0      554 2024-02-27 19:28:11.720071 ntqr-0.3.1/tests/test_r2_postulates.py
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 ntqr-0.3.1/PKG-INFO
```

### Comparing `ntqr-0.2/ACKNOWLEDGEMENTS.md` & `ntqr-0.3.1/ACKNOWLEDGEMENTS.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/LICENSE.txt` & `ntqr-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/README.md` & `ntqr-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 useful in AI safety applications:
 
 1. It is **universal**. The algorithms here apply to any domain. There is no
    Out of Distribution (OOD) problem when you use algebraic evaluation because
    it does not use any probability theory. By only using summary statistics of
    how a group of classifiers labeled a test set, we can treat all classifiers,
    whether human or robotic, as black boxes. There are no hyperparameters
-   to tune or set in NTQR algorithms. If they where, these algorithms could
+   to tune or set in NTQR algorithms. If they were, these algorithms could
    not claim to be universal.
 
 2. It is **complete**. The finite nature of any test given to a group of
    binary classifiers means we can guarantee the existence of a complete
    set of postulates that must be obeyed during any evaluation. Completeness
    is a logical safety shield. It allows us to create theorem provers that
    can unequivocably detect violations of the logical consistency of **any**
```

### Comparing `ntqr-0.2/docs/.readthedocs.yaml` & `ntqr-0.3.1/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/Makefile` & `ntqr-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/make.bat` & `ntqr-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/source/conceptual.md` & `ntqr-0.3.1/docs/source/conceptual.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/source/conf.py` & `ntqr-0.3.1/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
+import ntqr
+
 sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "NTQR"
 copyright = "2024, Andrés Corrada-Emmanuel, Walker Lee, Adam Sloat"
 authors = ["Andrés Corrada-Emmanuel", "Walker Lee", "Adam Sloat"]
 
 # The full version, including alpha/beta/rc tags
-release = "0.1"
+version = ntqr.__version__
+release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ntqr-0.2/docs/source/index.md` & `ntqr-0.3.1/docs/source/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 :relative-images:
 ```
 
 ```{toctree}
 :caption: 'Contents:'
 :maxdepth: 2
 
-
 conceptual
 notebooks/Tutorial
 notebooks/LogicOfUnsupervisedEvaluationTutorial
 notebooks/ExactAlgebraicSolutionErrorIndependent
 research/GradingLLMs
+research/EvaluatingLLMsThatGradeOtherLLMs
 research/MathematicsOfAlgebraicEvaluation
 research/TheScienceOfAlgebraicEvaluation
 ntqr
 ```
```

### Comparing `ntqr-0.2/docs/source/notebooks/ExactAlgebraicSolutionErrorIndependent.ipynb` & `ntqr-0.3.1/docs/source/notebooks/ExactAlgebraicSolutionErrorIndependent.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9839482442901328%*

 * *Differences: {"'cells'": "{3: {'source': ['The observations of agreement and disagreement vote patterns for "*

 * *            'noisy classification functions are not without structure. This can be seen in the '*

 * *            'polynomial generating set for three binary classifiers that are arbitrarily '*

 * *            'correlated. The idea of a "generating set" is that the data sketch of observations is '*

 * *            'explained by unknown statistics of correctness during a test that we want to '*

 * *            'estimate. In other wo […]*

```diff
@@ -25,20 +25,20 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9ad1fe6c-4abb-49cf-9654-240115bd6bde",
             "metadata": {},
             "source": [
-                "The observations of agreement and disagreement vote patterns for noisy classification functions is not without structure. This can be seen in the polynomial generating set for three binary classifiers that are arbitrarily correlated. The idea of a \"generating set\" is that the data sketch of observations is explained by unknown statistics of correctness during a test that we want to estimate. In other words, the aligned decisions of binary classifiers and their resulting counts are not just random numbers. They follow a pattern that is given by the generating set of polynomials. Let's take a peek at that complicated generating set for arbitrarly correlated classifiers."
+                "The observations of agreement and disagreement vote patterns for noisy classification functions are not without structure. This can be seen in the polynomial generating set for three binary classifiers that are arbitrarily correlated. The idea of a \"generating set\" is that the data sketch of observations is explained by unknown statistics of correctness during a test that we want to estimate. In other words, the aligned decisions of binary classifiers and their resulting counts are not just random numbers. They follow a pattern that is given by the generating set of polynomials. Let's take a peek at that complicated generating set for arbitrarly correlated classifiers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 1,
             "id": "5db87a8b-08c4-42c6-ab3f-d2e3c885e124",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -56,119 +56,119 @@
                     ]
                 }
             ],
             "source": [
                 "import sympy\n",
                 "\n",
                 "import ntqr\n",
-                "from pprint import pprint\n",
+                "import pprint\n",
                 "sympy.init_session()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 2,
             "id": "e2866ed1-0c37-474c-9e23-00563f25c89f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}P_{a} \\left(P_{i, a} P_{j, a} P_{k, a} + P_{i, a} \\Gamma_{j, k, a} + P_{j, a} \\Gamma_{i, k, a} + P_{k, a} \\Gamma_{i, j, a} + \\Gamma_{i, j, k, a}\\right) + P_{b} \\left(\\Gamma_{i, j, b} \\left(1 - P_{k, b}\\right) - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b} \\left(1 - P_{j, b}\\right) + \\Gamma_{j, k, b} \\left(1 - P_{i, b}\\right) + \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right)\\right) - f_{a_i, a_j, a_k}\\\\P_{a} \\left(P_{i, a} P_{j, a} \\left(1 - P_{k, a}\\right) - P_{i, a} \\Gamma_{j, k, a} - P_{j, a} \\Gamma_{i, k, a} + \\Gamma_{i, j, a} \\left(1 - P_{k, a}\\right) - \\Gamma_{i, j, k, a}\\right) + P_{b} \\left(P_{k, b} \\Gamma_{i, j, b} + P_{k, b} \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) + \\Gamma_{i, j, k, b} - \\Gamma_{i, k, b} \\left(1 - P_{j, b}\\right) - \\Gamma_{j, k, b} \\left(1 - P_{i, b}\\right)\\right) - f_{a_i, a_j, b_k}\\\\P_{a} \\left(P_{i, a} P_{k, a} \\left(1 - P_{j, a}\\right) - P_{i, a} \\Gamma_{j, k, a} - P_{k, a} \\Gamma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a} \\left(1 - P_{j, a}\\right)\\right) + P_{b} \\left(P_{j, b} \\Gamma_{i, k, b} + P_{j, b} \\left(1 - P_{i, b}\\right) \\left(1 - P_{k, b}\\right) - \\Gamma_{i, j, b} \\left(1 - P_{k, b}\\right) + \\Gamma_{i, j, k, b} - \\Gamma_{j, k, b} \\left(1 - P_{i, b}\\right)\\right) - f_{a_i, b_j, a_k}\\\\P_{a} \\left(P_{i, a} \\Gamma_{j, k, a} + P_{i, a} \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right) - \\Gamma_{i, j, a} \\left(1 - P_{k, a}\\right) + \\Gamma_{i, j, k, a} - \\Gamma_{i, k, a} \\left(1 - P_{j, a}\\right)\\right) + P_{b} \\left(P_{j, b} P_{k, b} \\left(1 - P_{i, b}\\right) - P_{j, b} \\Gamma_{i, k, b} - P_{k, b} \\Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{j, k, b} \\left(1 - P_{i, b}\\right)\\right) - f_{a_i, b_j, b_k}\\\\P_{a} \\left(P_{j, a} P_{k, a} \\left(1 - P_{i, a}\\right) - P_{j, a} \\Gamma_{i, k, a} - P_{k, a} \\Gamma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{j, k, a} \\left(1 - P_{i, a}\\right)\\right) + P_{b} \\left(P_{i, b} \\Gamma_{j, k, b} + P_{i, b} \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right) - \\Gamma_{i, j, b} \\left(1 - P_{k, b}\\right) + \\Gamma_{i, j, k, b} - \\Gamma_{i, k, b} \\left(1 - P_{j, b}\\right)\\right) - f_{b_i, a_j, a_k}\\\\P_{a} \\left(P_{j, a} \\Gamma_{i, j, a} + P_{j, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{k, a}\\right) - \\Gamma_{i, j, a} \\left(1 - P_{k, a}\\right) + \\Gamma_{i, j, k, a} - \\Gamma_{j, k, a} \\left(1 - P_{i, a}\\right)\\right) + P_{b} \\left(P_{i, b} P_{k, b} \\left(1 - P_{j, b}\\right) - P_{i, b} \\Gamma_{j, k, b} - P_{k, b} \\Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b} \\left(1 - P_{j, b}\\right)\\right) - f_{b_i, a_j, b_k}\\\\P_{a} \\left(P_{k, a} \\Gamma_{i, j, a} + P_{k, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) + \\Gamma_{i, j, k, a} - \\Gamma_{i, k, a} \\left(1 - P_{j, a}\\right) - \\Gamma_{j, k, a} \\left(1 - P_{i, a}\\right)\\right) + P_{b} \\left(P_{i, b} P_{j, b} \\left(1 - P_{k, b}\\right) - P_{i, b} \\Gamma_{j, k, b} - P_{j, b} \\Gamma_{i, k, b} + \\Gamma_{i, j, b} \\left(1 - P_{k, b}\\right) - \\Gamma_{i, j, k, b}\\right) - f_{b_i, b_j, a_k}\\\\P_{a} \\left(\\Gamma_{i, j, a} \\left(1 - P_{k, a}\\right) - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a} \\left(1 - P_{j, a}\\right) + \\Gamma_{j, k, a} \\left(1 - P_{i, a}\\right) + \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right)\\right) + P_{b} \\left(P_{i, b} P_{j, b} P_{k, b} + P_{i, b} \\Gamma_{j, k, b} + P_{j, b} \\Gamma_{i, k, b} + P_{k, b} \\Gamma_{i, j, b} + \\Gamma_{i, j, k, b}\\right) - f_{b_i, b_j, b_k}\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1P\u2090\u22c5(P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} + P_{i, a}\u22c5\\Gamma_{j, k, a} + P_{j, a}\u22c5\\Gamm\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) - P_{i, a}\u22c5\\Gamma_{j, k, a} - P_{j, a}\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) - P_{i, a}\u22c5\\Gamma_{j, k, a} - P_{k, a}\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5\\Gamma_{j, k, a} + P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) - \\G\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) - P_{j, a}\u22c5\\Gamma_{i, k, a} - P_{k, a}\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{j, a}\u22c5\\Gamma_{i, j, a} + P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) - \\G\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5(P_{k, a}\u22c5\\Gamma_{i, j, a} + P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + \\G\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a3P\u2090\u22c5(\\Gamma_{i, j, a}\u22c5(1 - P_{k, a}) - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a\n",
+                            "\u23a1P\u2090\u22c5(P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} + P_{i, a}\u22c5\\Gamma_{j, k, a} + P_{j, a}\u22c5\\Gamma_{i,\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) - P_{i, a}\u22c5\\Gamma_{j, k, a} - P_{j, a}\u22c5\\Gam\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) - P_{i, a}\u22c5\\Gamma_{j, k, a} - P_{k, a}\u22c5\\Gam\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{i, a}\u22c5\\Gamma_{j, k, a} + P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) - \\Gamma_\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) - P_{j, a}\u22c5\\Gamma_{i, k, a} - P_{k, a}\u22c5\\Gam\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{j, a}\u22c5\\Gamma_{i, j, a} + P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) - \\Gamma_\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5(P_{k, a}\u22c5\\Gamma_{i, j, a} + P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + \\Gamma_\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a3P\u2090\u22c5(\\Gamma_{i, j, a}\u22c5(1 - P_{k, a}) - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a}\u22c5(1 \n",
                             "\n",
-                            "a_{i, k, a} + P_{k, a}\u22c5\\Gamma_{i, j, a} + \\Gamma_{i, j, k, a}) + P_b\u22c5(\\Gamma\n",
-                            "                                                                            \n",
-                            "\u22c5\\Gamma_{i, k, a} + \\Gamma_{i, j, a}\u22c5(1 - P_{k, a}) - \\Gamma_{i, j, k, a}) +\n",
-                            "                                                                            \n",
-                            "\u22c5\\Gamma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a}\u22c5(1 - P_{j, a})) +\n",
-                            "                                                                            \n",
-                            "amma_{i, j, a}\u22c5(1 - P_{k, a}) + \\Gamma_{i, j, k, a} - \\Gamma_{i, k, a}\u22c5(1 - \n",
-                            "                                                                            \n",
-                            "\u22c5\\Gamma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{j, k, a}\u22c5(1 - P_{i, a})) +\n",
-                            "                                                                            \n",
-                            "amma_{i, j, a}\u22c5(1 - P_{k, a}) + \\Gamma_{i, j, k, a} - \\Gamma_{j, k, a}\u22c5(1 - \n",
-                            "                                                                            \n",
-                            "amma_{i, j, k, a} - \\Gamma_{i, k, a}\u22c5(1 - P_{j, a}) - \\Gamma_{j, k, a}\u22c5(1 - \n",
-                            "                                                                            \n",
-                            "}\u22c5(1 - P_{j, a}) + \\Gamma_{j, k, a}\u22c5(1 - P_{i, a}) + (1 - P_{i, a})\u22c5(1 - P_{\n",
+                            " k, a} + P_{k, a}\u22c5\\Gamma_{i, j, a} + \\Gamma_{i, j, k, a}) + P_b\u22c5(\\Gamma_{i, j, b}\n",
+                            "                                                                                 \n",
+                            "ma_{i, k, a} + \\Gamma_{i, j, a}\u22c5(1 - P_{k, a}) - \\Gamma_{i, j, k, a}) + P_b\u22c5(P_{k\n",
+                            "                                                                                 \n",
+                            "ma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{i, k, a}\u22c5(1 - P_{j, a})) + P_b\u22c5(P_{j\n",
+                            "                                                                                 \n",
+                            "{i, j, a}\u22c5(1 - P_{k, a}) + \\Gamma_{i, j, k, a} - \\Gamma_{i, k, a}\u22c5(1 - P_{j, a}))\n",
+                            "                                                                                 \n",
+                            "ma_{i, j, a} - \\Gamma_{i, j, k, a} + \\Gamma_{j, k, a}\u22c5(1 - P_{i, a})) + P_b\u22c5(P_{i\n",
+                            "                                                                                 \n",
+                            "{i, j, a}\u22c5(1 - P_{k, a}) + \\Gamma_{i, j, k, a} - \\Gamma_{j, k, a}\u22c5(1 - P_{i, a}))\n",
+                            "                                                                                 \n",
+                            "{i, j, k, a} - \\Gamma_{i, k, a}\u22c5(1 - P_{j, a}) - \\Gamma_{j, k, a}\u22c5(1 - P_{i, a}))\n",
+                            "                                                                                 \n",
+                            "- P_{j, a}) + \\Gamma_{j, k, a}\u22c5(1 - P_{i, a}) + (1 - P_{i, a})\u22c5(1 - P_{j, a})\u22c5(1 \n",
                             "\n",
-                            "_{i, j, b}\u22c5(1 - P_{k, b}) - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b}\u22c5(1 - P_{j\n",
-                            "                                                                            \n",
-                            " P_b\u22c5(P_{k, b}\u22c5\\Gamma_{i, j, b} + P_{k, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{j, b}) + \\\n",
-                            "                                                                            \n",
-                            " P_b\u22c5(P_{j, b}\u22c5\\Gamma_{i, k, b} + P_{j, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{k, b}) - \\\n",
-                            "                                                                            \n",
-                            "P_{j, a})) + P_b\u22c5(P_{j, b}\u22c5P_{k, b}\u22c5(1 - P_{i, b}) - P_{j, b}\u22c5\\Gamma_{i, k, \n",
-                            "                                                                            \n",
-                            " P_b\u22c5(P_{i, b}\u22c5\\Gamma_{j, k, b} + P_{i, b}\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b}) - \\\n",
-                            "                                                                            \n",
-                            "P_{i, a})) + P_b\u22c5(P_{i, b}\u22c5P_{k, b}\u22c5(1 - P_{j, b}) - P_{i, b}\u22c5\\Gamma_{j, k, \n",
-                            "                                                                            \n",
-                            "P_{i, a})) + P_b\u22c5(P_{i, b}\u22c5P_{j, b}\u22c5(1 - P_{k, b}) - P_{i, b}\u22c5\\Gamma_{j, k, \n",
-                            "                                                                            \n",
-                            "j, a})\u22c5(1 - P_{k, a})) + P_b\u22c5(P_{i, b}\u22c5P_{j, b}\u22c5P_{k, b} + P_{i, b}\u22c5\\Gamma_{\n",
+                            "\u22c5(1 - P_{k, b}) - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b}\u22c5(1 - P_{j, b}) + \\Gamma_\n",
+                            "                                                                                 \n",
+                            ", b}\u22c5\\Gamma_{i, j, b} + P_{k, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{j, b}) + \\Gamma_{i, j, k,\n",
+                            "                                                                                 \n",
+                            ", b}\u22c5\\Gamma_{i, k, b} + P_{j, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{k, b}) - \\Gamma_{i, j, b}\n",
+                            "                                                                                 \n",
+                            " + P_b\u22c5(P_{j, b}\u22c5P_{k, b}\u22c5(1 - P_{i, b}) - P_{j, b}\u22c5\\Gamma_{i, k, b} - P_{k, b}\u22c5\\\n",
+                            "                                                                                 \n",
+                            ", b}\u22c5\\Gamma_{j, k, b} + P_{i, b}\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b}) - \\Gamma_{i, j, b}\n",
+                            "                                                                                 \n",
+                            " + P_b\u22c5(P_{i, b}\u22c5P_{k, b}\u22c5(1 - P_{j, b}) - P_{i, b}\u22c5\\Gamma_{j, k, b} - P_{k, b}\u22c5\\\n",
+                            "                                                                                 \n",
+                            " + P_b\u22c5(P_{i, b}\u22c5P_{j, b}\u22c5(1 - P_{k, b}) - P_{i, b}\u22c5\\Gamma_{j, k, b} - P_{j, b}\u22c5\\\n",
+                            "                                                                                 \n",
+                            "- P_{k, a})) + P_b\u22c5(P_{i, b}\u22c5P_{j, b}\u22c5P_{k, b} + P_{i, b}\u22c5\\Gamma_{j, k, b} + P_{j\n",
                             "\n",
-                            ", b}) + \\Gamma_{j, k, b}\u22c5(1 - P_{i, b}) + (1 - P_{i, b})\u22c5(1 - P_{j, b})\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "Gamma_{i, j, k, b} - \\Gamma_{i, k, b}\u22c5(1 - P_{j, b}) - \\Gamma_{j, k, b}\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "Gamma_{i, j, b}\u22c5(1 - P_{k, b}) + \\Gamma_{i, j, k, b} - \\Gamma_{j, k, b}\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "b} - P_{k, b}\u22c5\\Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{j, k, b}\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "Gamma_{i, j, b}\u22c5(1 - P_{k, b}) + \\Gamma_{i, j, k, b} - \\Gamma_{i, k, b}\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "b} - P_{k, b}\u22c5\\Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b}\u22c5(1 -\n",
-                            "                                                                            \n",
-                            "b} - P_{j, b}\u22c5\\Gamma_{i, k, b} + \\Gamma_{i, j, b}\u22c5(1 - P_{k, b}) - \\Gamma_{i\n",
-                            "                                                                            \n",
-                            "j, k, b} + P_{j, b}\u22c5\\Gamma_{i, k, b} + P_{k, b}\u22c5\\Gamma_{i, j, b} + \\Gamma_{i\n",
+                            "{j, k, b}\u22c5(1 - P_{i, b}) + (1 - P_{i, b})\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b})) - f_{a_i\n",
+                            "                                                                                 \n",
+                            " b} - \\Gamma_{i, k, b}\u22c5(1 - P_{j, b}) - \\Gamma_{j, k, b}\u22c5(1 - P_{i, b})) - f_{a_i\n",
+                            "                                                                                 \n",
+                            "\u22c5(1 - P_{k, b}) + \\Gamma_{i, j, k, b} - \\Gamma_{j, k, b}\u22c5(1 - P_{i, b})) - f_{a_i\n",
+                            "                                                                                 \n",
+                            "Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{j, k, b}\u22c5(1 - P_{i, b})) - f_{a_i\n",
+                            "                                                                                 \n",
+                            "\u22c5(1 - P_{k, b}) + \\Gamma_{i, j, k, b} - \\Gamma_{i, k, b}\u22c5(1 - P_{j, b})) - f_{b_i\n",
+                            "                                                                                 \n",
+                            "Gamma_{i, j, b} - \\Gamma_{i, j, k, b} + \\Gamma_{i, k, b}\u22c5(1 - P_{j, b})) - f_{b_i\n",
+                            "                                                                                 \n",
+                            "Gamma_{i, k, b} + \\Gamma_{i, j, b}\u22c5(1 - P_{k, b}) - \\Gamma_{i, j, k, b}) - f_{b_i\n",
+                            "                                                                                 \n",
+                            ", b}\u22c5\\Gamma_{i, k, b} + P_{k, b}\u22c5\\Gamma_{i, j, b} + \\Gamma_{i, j, k, b}) - f_{b_i\n",
                             "\n",
-                            " P_{k, b})) - f_{a_i, a_j, a_k}\u23a4\n",
-                            "                               \u23a5\n",
-                            " P_{i, b})) - f_{a_i, a_j, b_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            " P_{i, b})) - f_{a_i, b_j, a_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            " P_{i, b})) - f_{a_i, b_j, b_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            " P_{j, b})) - f_{b_i, a_j, a_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            " P_{j, b})) - f_{b_i, a_j, b_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            ", j, k, b}) - f_{b_i, b_j, a_k}\u23a5\n",
-                            "                               \u23a5\n",
-                            ", j, k, b}) - f_{b_i, b_j, b_k}\u23a6"
+                            ", a_j, a_k}\u23a4\n",
+                            "           \u23a5\n",
+                            ", a_j, b_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", b_j, a_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", b_j, b_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", a_j, a_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", a_j, b_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", b_j, a_k}\u23a5\n",
+                            "           \u23a5\n",
+                            ", b_j, b_k}\u23a6"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ntqr.r2.postulates import (\n",
+                "from ntqr.r2.paxioms import (\n",
                 "    trio_binary_classifiers_generating_set,\n",
                 "    pa, pb,\n",
                 "    pia, pib, pja, pjb, pka, pkb,\n",
                 "    gija, gijb, gika, gikb, gjka, gjkb,\n",
                 "    gijka, gijkb,\n",
                 "    trio_frequencies)\n",
                 "from ntqr.r2.datasketches import trio_vote_patterns\n",
@@ -181,59 +181,59 @@
             "metadata": {},
             "source": [
                 "The set above is the one used to derive the axioms of evaluation for binary classification up to N=3. We want to test the error-independent solution so we want the generating set for error-independent binary classifiers. That is given by setting all the error correlations identically to zero."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 3,
             "id": "5b95e190-25b2-4059-996e-1a131ff29592",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}P_{a} P_{i, a} P_{j, a} P_{k, a} + P_{b} \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right) - f_{a_i, a_j, a_k}\\\\P_{a} P_{i, a} P_{j, a} \\left(1 - P_{k, a}\\right) + P_{b} P_{k, b} \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) - f_{a_i, a_j, b_k}\\\\P_{a} P_{i, a} P_{k, a} \\left(1 - P_{j, a}\\right) + P_{b} P_{j, b} \\left(1 - P_{i, b}\\right) \\left(1 - P_{k, b}\\right) - f_{a_i, b_j, a_k}\\\\P_{a} P_{i, a} \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right) + P_{b} P_{j, b} P_{k, b} \\left(1 - P_{i, b}\\right) - f_{a_i, b_j, b_k}\\\\P_{a} P_{j, a} P_{k, a} \\left(1 - P_{i, a}\\right) + P_{b} P_{i, b} \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right) - f_{b_i, a_j, a_k}\\\\P_{a} P_{j, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{k, a}\\right) + P_{b} P_{i, b} P_{k, b} \\left(1 - P_{j, b}\\right) - f_{b_i, a_j, b_k}\\\\P_{a} P_{k, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) + P_{b} P_{i, b} P_{j, b} \\left(1 - P_{k, b}\\right) - f_{b_i, b_j, a_k}\\\\P_{a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right) + P_{b} P_{i, b} P_{j, b} P_{k, b} - f_{b_i, b_j, b_k}\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} + P_b\u22c5(1 - P_{i, b})\u22c5(1 - P_{j, b})\u22c5(1 - P_{k\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) + P_b\u22c5P_{k, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{j\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) + P_b\u22c5P_{j, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{k\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{j, b}\u22c5P_{k, b}\u22c5(1 - P_{i\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) + P_b\u22c5P_{i, b}\u22c5(1 - P_{j, b})\u22c5(1 - P_{k\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{i, b}\u22c5P_{k, b}\u22c5(1 - P_{j\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + P_b\u22c5P_{i, b}\u22c5P_{j, b}\u22c5(1 - P_{k\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a3P\u2090\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{i, b}\u22c5P_{j, b}\u22c5P_{\n",
+                            "\u23a1P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} + P_b\u22c5(1 - P_{i, b})\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) + P_b\u22c5P_{k, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{j, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) + P_b\u22c5P_{j, b}\u22c5(1 - P_{i, b})\u22c5(1 - P_{k, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{j, b}\u22c5P_{k, b}\u22c5(1 - P_{i, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) + P_b\u22c5P_{i, b}\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{i, b}\u22c5P_{k, b}\u22c5(1 - P_{j, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + P_b\u22c5P_{i, b}\u22c5P_{j, b}\u22c5(1 - P_{k, b})\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a3P\u2090\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_b\u22c5P_{i, b}\u22c5P_{j, b}\u22c5P_{k, b}\n",
                             "\n",
-                            ", b}) - f_{a_i, a_j, a_k}\u23a4\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{a_i, a_j, b_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{a_i, b_j, a_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{a_i, b_j, b_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{b_i, a_j, a_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{b_i, a_j, b_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            ", b}) - f_{b_i, b_j, a_k}\u23a5\n",
-                            "                         \u23a5\n",
-                            "k, b} - f_{b_i, b_j, b_k}\u23a6"
+                            " - f_{a_i, a_j, a_k}\u23a4\n",
+                            "                    \u23a5\n",
+                            " - f_{a_i, a_j, b_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{a_i, b_j, a_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{a_i, b_j, b_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{b_i, a_j, a_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{b_i, a_j, b_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{b_i, b_j, a_k}\u23a5\n",
+                            "                    \u23a5\n",
+                            " - f_{b_i, b_j, b_k}\u23a6"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "zero_error_correlations = {gija: 0, gijb: 0,\n",
                 "                           gika: 0, gikb: 0,\n",
@@ -249,15 +249,15 @@
             "metadata": {},
             "source": [
                 "The structure of this generating set is the reason we can obtain information about the evaluation using only the observed frequencies that appear at the right. This can be stated precisely by saying that the data sketches of binary classifiers are not generated by eight random integers in an unstructured way as follows."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 4,
             "id": "eeeb006b-bec3-473b-9a92-f283215adc1c",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
@@ -277,15 +277,15 @@
                             "\u23a2-f_{b_i, a_j, b_k} + x\u2086\u23a5\n",
                             "\u23a2                       \u23a5\n",
                             "\u23a2-f_{b_i, b_j, a_k} + x\u2087\u23a5\n",
                             "\u23a2                       \u23a5\n",
                             "\u23a3-f_{b_i, b_j, b_k} + x\u2088\u23a6"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "incorrect_generating_set = [(sympy.Symbol(\"x_{}\".format(i)) - trio_frequencies[i-1]) for i in range(1,9)]\n",
                 "sympy.Matrix(incorrect_generating_set)"
@@ -313,147 +313,147 @@
             "metadata": {},
             "source": [
                 "We can now demonstrate the exact solution for the case of error independent classifiers by using the generating set. We randomly pick values for all the statistics in the generating set, substitute them in the generating set to get the data sketch that would be observed in that case. We then use the data sketch to recover the stastics we used to generate the set."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 5,
             "id": "96bda2ed-4b2b-49c0-8aa7-e974c4a4a120",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}P_{a} P_{i, a} P_{j, a} P_{k, a} - f_{a_i, a_j, a_k} + \\left(1 - P_{a}\\right) \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right)\\\\P_{a} P_{i, a} P_{j, a} \\left(1 - P_{k, a}\\right) + P_{k, b} \\left(1 - P_{a}\\right) \\left(1 - P_{i, b}\\right) \\left(1 - P_{j, b}\\right) - f_{a_i, a_j, b_k}\\\\P_{a} P_{i, a} P_{k, a} \\left(1 - P_{j, a}\\right) + P_{j, b} \\left(1 - P_{a}\\right) \\left(1 - P_{i, b}\\right) \\left(1 - P_{k, b}\\right) - f_{a_i, b_j, a_k}\\\\P_{a} P_{i, a} \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right) + P_{j, b} P_{k, b} \\left(1 - P_{a}\\right) \\left(1 - P_{i, b}\\right) - f_{a_i, b_j, b_k}\\\\P_{a} P_{j, a} P_{k, a} \\left(1 - P_{i, a}\\right) + P_{i, b} \\left(1 - P_{a}\\right) \\left(1 - P_{j, b}\\right) \\left(1 - P_{k, b}\\right) - f_{b_i, a_j, a_k}\\\\P_{a} P_{j, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{k, a}\\right) + P_{i, b} P_{k, b} \\left(1 - P_{a}\\right) \\left(1 - P_{j, b}\\right) - f_{b_i, a_j, b_k}\\\\P_{a} P_{k, a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) + P_{i, b} P_{j, b} \\left(1 - P_{a}\\right) \\left(1 - P_{k, b}\\right) - f_{b_i, b_j, a_k}\\\\P_{a} \\left(1 - P_{i, a}\\right) \\left(1 - P_{j, a}\\right) \\left(1 - P_{k, a}\\right) + P_{i, b} P_{j, b} P_{k, b} \\left(1 - P_{a}\\right) - f_{b_i, b_j, b_k}\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} - f_{a_i, a_j, a_k} + (1 - P\u2090)\u22c5(1 - P_{i, b})\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) + P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{i, b})\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) + P_{j, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{i, b})\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_{j, b}\u22c5P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) + P_{i, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{j, b})\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) + P_{i, b}\u22c5P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a2P\u2090\u22c5P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + P_{i, b}\u22c5P_{j, b}\u22c5(1 - P\u2090)\u22c5(1 -\n",
-                            "\u23a2                                                                           \n",
-                            "\u23a3P\u2090\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_{i, b}\u22c5P_{j, b}\u22c5P_{k, b\n",
+                            "\u23a1P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5P_{k, a} - f_{a_i, a_j, a_k} + (1 - P\u2090)\u22c5(1 - P_{i, b})\u22c5(1 -\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{j, a}\u22c5(1 - P_{k, a}) + P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{i, b})\u22c5(1 - P_{j\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5P_{k, a}\u22c5(1 - P_{j, a}) + P_{j, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{i, b})\u22c5(1 - P_{k\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{i, a}\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_{j, b}\u22c5P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{i\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5P_{k, a}\u22c5(1 - P_{i, a}) + P_{i, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{j, b})\u22c5(1 - P_{k\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{j, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{k, a}) + P_{i, b}\u22c5P_{k, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{j\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2P\u2090\u22c5P_{k, a}\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a}) + P_{i, b}\u22c5P_{j, b}\u22c5(1 - P\u2090)\u22c5(1 - P_{k\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a3P\u2090\u22c5(1 - P_{i, a})\u22c5(1 - P_{j, a})\u22c5(1 - P_{k, a}) + P_{i, b}\u22c5P_{j, b}\u22c5P_{k, b}\u22c5(1 \n",
                             "\n",
-                            "\u22c5(1 - P_{j, b})\u22c5(1 - P_{k, b})\u23a4\n",
-                            "                              \u23a5\n",
-                            " P_{j, b}) - f_{a_i, a_j, b_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            " P_{k, b}) - f_{a_i, b_j, a_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            " P_{i, b}) - f_{a_i, b_j, b_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            " P_{k, b}) - f_{b_i, a_j, a_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            " P_{j, b}) - f_{b_i, a_j, b_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            " P_{k, b}) - f_{b_i, b_j, a_k}\u23a5\n",
-                            "                              \u23a5\n",
-                            "}\u22c5(1 - P\u2090) - f_{b_i, b_j, b_k}\u23a6"
+                            " P_{j, b})\u22c5(1 - P_{k, b})\u23a4\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{a_i, a_j, b_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{a_i, b_j, a_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{a_i, b_j, b_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{b_i, a_j, a_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{b_i, a_j, b_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            ", b}) - f_{b_i, b_j, a_k}\u23a5\n",
+                            "                         \u23a5\n",
+                            "- P\u2090) - f_{b_i, b_j, b_k}\u23a6"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Let's simplify the substitution by using the relation between pa and pb\n",
                 "simplified_generating_set = [poly.subs({pb:(1-pa)}) for poly in error_independent_generating_set]\n",
                 "sympy.Matrix(simplified_generating_set)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 6,
             "id": "6a215346-2783-4eb0-9e81-a5ac61d23baa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/latex": [
-                            "$\\displaystyle \\left[\\begin{matrix}\\frac{1881}{80000} - f_{a_i, a_j, a_k}\\\\\\frac{10089}{80000} - f_{a_i, a_j, b_k}\\\\\\frac{6859}{80000} - f_{a_i, b_j, a_k}\\\\\\frac{53371}{80000} - f_{a_i, b_j, b_k}\\\\\\frac{159}{80000} - f_{b_i, a_j, a_k}\\\\\\frac{1071}{80000} - f_{b_i, a_j, b_k}\\\\\\frac{701}{80000} - f_{b_i, b_j, a_k}\\\\\\frac{5869}{80000} - f_{b_i, b_j, b_k}\\end{matrix}\\right]$"
+                            "$\\displaystyle \\left[\\begin{matrix}\\frac{67239}{160000} - f_{a_i, a_j, a_k}\\\\\\frac{10881}{160000} - f_{a_i, a_j, b_k}\\\\\\frac{31681}{160000} - f_{a_i, b_j, a_k}\\\\\\frac{3799}{160000} - f_{a_i, b_j, b_k}\\\\\\frac{22901}{160000} - f_{b_i, a_j, a_k}\\\\\\frac{10179}{160000} - f_{b_i, a_j, b_k}\\\\\\frac{10179}{160000} - f_{b_i, b_j, a_k}\\\\\\frac{3141}{160000} - f_{b_i, b_j, b_k}\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1 1881                    \u23a4\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{a_i, a_j, a_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a210089                    \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{a_i, a_j, b_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a2 6859                    \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{a_i, b_j, a_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a253371                    \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{a_i, b_j, b_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a2 159                     \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{b_i, a_j, a_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a2 1071                    \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{b_i, a_j, b_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a2 701                     \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{b_i, b_j, a_k}\u23a5\n",
-                            "\u23a280000                    \u23a5\n",
-                            "\u23a2                         \u23a5\n",
-                            "\u23a2 5869                    \u23a5\n",
-                            "\u23a2\u2500\u2500\u2500\u2500\u2500 - f_{b_i, b_j, b_k}\u23a5\n",
-                            "\u23a380000                    \u23a6"
+                            "\u23a167239                     \u23a4\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{a_i, a_j, a_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a210881                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{a_i, a_j, b_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a231681                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{a_i, b_j, a_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a2 3799                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{a_i, b_j, b_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a222901                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{b_i, a_j, a_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a210179                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{b_i, a_j, b_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a210179                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{b_i, b_j, a_k}\u23a5\n",
+                            "\u23a2160000                    \u23a5\n",
+                            "\u23a2                          \u23a5\n",
+                            "\u23a2 3141                     \u23a5\n",
+                            "\u23a2\u2500\u2500\u2500\u2500\u2500\u2500 - f_{b_i, b_j, b_k}\u23a5\n",
+                            "\u23a3160000                    \u23a6"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from random import randint\n",
                 "from fractions import Fraction\n",
-                "random_performance_statistics = {var:Fraction(randint(1,19),20) for var in [pa, pia, pib, pja, pjb, pka, pkb]}\n",
+                "random_performance_statistics = {var:Fraction(randint(1,39),40) for var in [pa, pia, pib, pja, pjb, pka, pkb]}\n",
                 "generated_data_sketch = [poly.subs(random_performance_statistics) for poly in simplified_generating_set]\n",
                 "sympy.Matrix(generated_data_sketch)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 7,
             "id": "f1350785-2818-4aa6-9baa-b02c9230ea84",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAk4AAAAyCAYAAACqJlRmAAAACXBIWXMAAA7EAAAOxAGVKw4bAAASrklEQVR4Ae2d7bUTtxaGDYsCTkgFFzrgo4JAB5BbAdBBsvIr+cciHRAqSKADSAUhdAC3gpDTwbnvI4/myGONtX2OP8b2q7XGo9Hskbae2ZK2NRr7xsXFxawVfvnll/eS+VH7Ty1ZnzcBEzABEzABEzCBQyIg/+ZM+r7V9lTx81W631x1knPKgIzeam+nqQXL5ydNQDZ8b6ig0s603RmmT/F4H/rDRttzbXQqJxf2wfzQIZ+KzZxKPdexx0NuL9IdZ+lHbX8rvrK/u7UKii7Gafqi/W+r5MbO6ToGKvK4r/iSB6c0lPupuJ5jnLQPRdosKpevkfzKcrPcrvcRvSTzqtPrH+3vanultC9DXSNykgnxJW/Jvi7KuK34M6Ut3bNCZmdR6ZGZ5DJ/V1rvyCsereefnWy+lusI9+e7y0/JTZFHSH/pjiP4oqsNdeQYOxq2q4gcbQkWr3W9dkvhXOnflKk6nmT7K3XM8YCuIebkp7ymaDO5qqF9gAf1zO1xrI86apspQK5VzwC3PuvIfeiFpxUJtRfVL9pnp9oV7HJtF8YAEiVz7fanPD5pS86TsmT8rYZRx0kXP9cVfNt8Wr1yJFHyAHmj7au2B9pWfZunM88dvETnM1zkoe1dSph/NOXWLLfIervRdfSS7N/S5mWue3ct3u9jbb3zpHhITnlFuZEfA+Ov0NCeDuF/2uPw9uVybpdBZWM7ON48Jk6DvvZpBlRppVE369npjU0SqB/1wsbgfa59Copjv5PkIb2i+sOrb1eKP9G177VnCjq1K+2pZ1NOMg+1wb5mB4/IQ9usyy/a7rlkb2FNXaPMp2ozTc7r8JBspO85OpsZgRiqJ9dGuK1zH0b0mUJys710Sob6bDFpjgEdt421P+X3TttDbUziVP2fquMkYZTlW8XSN/HWndG1DEKpMMV/UJxBainoHI4ZlR2GZ0r4U1vu4KNyoXKHhW37eE0eCw4j12qDA570Y3TVMTyick2+yovB7rbyTU6T4pSB1/1R0b5c0vcQcJJ+ly7lTAkDfj+I61zIPjrdqVe1IRR1mzKPiP7w4NEajlJqQzrO/H5SPKdF5WbKJ9lewYi09IVI+5Sf9pNsf6XOOb6mrhHmU7aZXO3RfZSH5EJ9DwVJ9qhsZgxesJ4hbsrrYNrQGA+lN9uL6gmPyNhEMc0xQDIbb3/SkS+Vn9FV29ITt5toVgnvlcY38X6AqshcN4kZg6XGVck0Kle59KCSGNA/VTT+S2mPdC9wGAhRuSg3ZiNq9xldynIpe2dB9UUvnO4Fo1U6s2+l3UTrGdV9kjyiykuO+0YHzJaCePXxnKZ9VA77q4Wlb4w1oRNJO3Sbid6maN9zKjYTrWeUW/Q+HLpcqM9eYwzYVvtjNp1+Lo+9Pfclx0lCeIMLMxC99GYjGN0Tlcc341IxZrrKZ5VRuc1qt/vceOzxtVJsdmo4T4jKNbkV3Gvl/jMvLj1u7aI73fGoiRm32qBfKtKsZym8Kj5xHqtU78+pDh+0fcM+JypOx0Lo29UacnmGap6DPnUtbfRln3DCEbHIfdcU29Cm70yo7xGTk7CZNeoZ4rbpmzXh/KJ9dnMM2Gb76+4v429e09cjvdXHLiMILXzLvzy1uRhKdYrRqf+rON4dnmj5iGEWlducZrvPSXXMne+qwnFmQ3JkEuEmGRwTxG/zMQjfdsd3Bum7OnyggngxgVmn/2rDkcM+Fl4eiNRT1/RB8mnaXAnUj7oxs8rsy0z7KfNARXQc1T8JDD4kT6dNm36h+Gi7XkMOZvckn9Y2DYo7ykPVdZS5zk3eZjZxU1TPcN8zLE/XnoTN1Op5HW5DjodyrDqPthfqoPOhsV+izTFAeW27/dHP4ZMw85QnMWY3qUgOOsGaJBrITr5NqjymMHNnTudOJ58GMe37EJXrLzi8SHZczleozn2JyqVsgtz4dkjHNgw4LIRIhzmX3OxnLveB6sHz5l+18Q0ExynPoKQSdRyyIwmT5x9dXjQINhbfY3c5TJUH+kX0T/VQnXBuaM8wo019TCcGH1G54jLaKduphAjzKdvMpu7TWn3PoNBTsZlaPa/DbYDxIA4j7WWmfifSZ5MXoTUGbK39SU9m7uk/F/q8BcdJJ+lk8QbPtd96UDkMgJTFTAIKMoCzIGs4MIbkdO0xhzwD1KpjLxfk+4wMJds7D4rjNGUb6L3sVsGbOq/yc4Nh8M+Odc7+D0XeFDIzxUP2ITnWR+V6cR11w+76R1iKT46HdEohqH+WZZEmziYd1O/acBAX2hWCSgvJdbK0z0e6pn8MSPoxB9X1oG1mx/em73tyueJ3EjZzzXouccv8Dm0fbC8zya3ss3V+nTFg2302E0ksK8o6Xc44KZHBEiNHaOtB5TGdR6fEbAKPZFjwSydP6AfGqNz8soP9/LpC8/yNhUdVUblZlJvkcCT+o41X1X/QhmeNHfAcmrBzx2le7GjZvI2BAT9AQvqG7AjZkUD9+NkN6kx+U+ZRq8KC/jUB1YlvZNSL2TrYVUNAji9W+7SHqt57SFxgfoA2cxVk4b5nkPmp2MxYPa/KbYDxoA+H7WWdPrvW3wzHgG332fmLInqncCtHtOdVZZ4XfirSthllgGbA7gMdtzZmnz5rYwaEDj8qJ9HDDHS82lC+NqjlNJzLkFxHIcyNfHUNDb8PSuN6Qs1w52e29FnUE73GQnJ0dDJUT+XJm6KsE7s/kmHmPKN8yUyGB/pKp5D+kuMLEPLDdvxRybSp1K6icuRVBL4l7tweivJ3GhWjEHOUkuzkbGaTsKifNrLs20mRf06r2cap2Ey1ntfgVuA9jKjqGm0vzT5beeELUHHa1VjIY8BMsltrf+StDeeJMSH9bM/NQiM61OxZFcmbj0oJGtpZV9mFApRG48NhYpALyS1kcLgHsO8NoahGnnHK96YptyFuDMC8obXKcAs1Nx6lntz/sYAjuY59MENVyy/xVV5DR2NY7r55RPXn21jzLwOQCcolDh1r7HNf9pD02PFHlPmYWvu2mTG9rpre7HvKjE/FZgL1XItbyfDA4s320rFqjv1dvZtjQIPPJtvfW5XVP5lIjpMqQwEMKniMWw8qj84XL67mKFA+uuRBuynHBUcQuDEY3jAwQ8I6lDxgNeWifClIsjy75a1GmKfQxXGk9/nmFOuOavYBD2xiXfv4TdcwmzkMC18YJDNVHiH9VTnspLZOMdsWnREhKjeXvrTNVY8esuyx7EPMJ2wzm74Pzb5nUGC2uWO3mVY91+U2wHgwh832orZCvxMd05tjAGR21P5YW0tgvOjXOKUDHedOlXObCHnR2+1KZqxnWlpzIQg8R+T1vzztG5Uri1hVbim36/ioXqovi6C/YgRZKcVxZr7Xlha/kR6Vk2iUG87JsGOjofP6emsWRmLbCSqbWUeco/zIcKb4Eg/JROvJX8qUi8DJj7fOCOSRwyR5SLmo/un12VwZ9qonNgU77ikdFyEqN5e+nK3L1+f02n7UzmvCe05bpWuU+VRt5ipoR3nIdkJ9VFEoNkc4NpuZ1+ryc2U9r8CNnEfvw2Wxk4tF20uozxa36Biw9fbX9ZvYMWuxZzcuLi5mSmSmiVf+Fv6sE4GrBOXDwEvAIcOoGIBxhHCI+rekFGemi7VV5cC98Ds9OjdbQy5ULnnuMkj/kF6SgxWOAjfoH20PtfW/M6R4CmvIRflm54TyCUv3YJ68+0/VFd2yXjjgNR7RetLA8iwaeWF3vJwA7z50ZXKcy50ED+kV1Z92N3QG+R2ShS9GOg7JAaIrm8d7zxSnQ1sKSg/Z+dKFe0iI6trV+2BtJop2DR60iWYfRbkdu6OxmTGWwXqGuEXvw5gu+07vWETaS6jPpj7KMzIGbH0Mkx74STyuu5sdp3+V8FEJyZtCWQcTMAETMAETMAETMIHegePN8xs39YEnzJYfjZmRCZiACZiACZiACZjAJQHe9p/JZ3p0U3um/wkpcR71pwmYgAmYgAmYgAmYQEfgY7e/VzpOnnGyfZiACZiACZiACZjAMoHsI93FcWKRLCEnzo/8aQImYAImYAImYAImwCO68w7DbRwn1jcRcuL8yJ8mYAImYAImYAImYAIlgTMcp/x7EeVPApRCjpuACZiACZiACZjAqRNggmlhxunUgbj+JmACJmACJmACJjBGgAmms1v6SGuciud3YxcspEv+YiHhwA9UnxubroIZtYmakRm1CbQlbEdm1CbQlrAdmVGbwOz2jZ9//plf++X/uTbuOAQUsIgJmIAJmIAJmIAJTJ6A/CR+tik9qktrm5SQF4lPXnkraAImYAImYAImYAJ7IPCVxeH5bbr8swR70GN6RdqRbN8TMzKjNoG2hO3IjNoE2hK2IzNqE7i2BH7SOY4TfyZL8IzTnMOsa4D/as8fVDpUCJhRBcogyYwGQCqHZlSBMkgyowGQyqEZVaAMksxoAOTqh1/KGaerZ3NkV8rAmIXjB0HPOmM7shpevzpm1GZoRmbUJtCWsB2ZUZtAW8J21GYUkGCC6Stv1eXfb7rSozrdDDL6qSiQ47dK/1CkpajSXnVpzHLd1fZKaUu/WL4vuU63tJMOd7U9KdOuGlc+ZtSAZ0YNQDptRmbUJtCWsB2ZUZtAW+JY7Wis5l19OX0+01t197RdaHt+cXExW3fTda+H1yjtrbYnZbqO/y7TFD/T9lnbnSnIlTrkuHR7lePX2SsfM2rYlhm1254ZmdF1+qF8re3IdpRt4Tr7Y7ajGhfVN/tKP9yUF/Wp87Duj3laY+m69rnO1dYBPVN6PwvVyfHY613OS/FzxTl+XaSR387lcvnlXvoxS5TXf5Wn1op3dTejFdTMaAWc7pQZmZEIuD9aYQbusxfH0xoqM2ozqnHr0u50+7TGiTiPyx50ievseNz2OHDBU8lkB60U/0sHj7qbSfq+5Eqdcvy59Po1H1xjb0ZteGZkRm5rq38Sxv3R4lhRazFmZEZMeBCivsRcOvaZHadPLA4n4NTkxJQQ/MDx4ccz3xfOD5eylqmfSVL8kba8lkrRPuT1TZwn7EtuXnrxuSGniRzNqOA6EjWjETBFshkVMEaiZjQCpkg2owLGSNSMRsAUyUfLqKjjMPqQBPkGX1gcTnivDQeIx2Q8QgsFyb5jkzCLqHl9/0ftmT3AkUqP5bTPHqCSR8PtfcmNarShE3DoWJjRCFMzGgFTJJtRAWMkakYjYIpkMypgjETNaARMkXyijJjYSS+95Rmnjx2TPPNTIFodFUCmxH7rpJhpIo/ysVx+W2+VQ4ZztS+5TvXt7cyozdaMzKhNoC1hOzKjNoG2hO3IjEoCsgeeyOGnMMk0S46TEnF0cGz+S+I6Qdcyk8K1zDThjVHA5y5d0VD4NiQ1m+1LLqheXcyM6lzKVDMqadTjZlTnUqaaUUmjHjejOpcy1YxKGvX4iTHKk0rpSdqtAskfin9fHDejAsdbcPe1f9EJP+5gvtXxG8VxpGprmzrxfpaJt0X2JZd12crejNpYzciM2gTaErYjM2oTaEvYjsyoQoCX4L7INtK67PyoDjmcHdY4Zc+KtFbg0Rzrmvqg6/HImH1iWos35piNInA8DDkNhfYiN1RoC8dm1IZqRmbUJtCWsB2ZUZtAW8J2ZEZDAjxZ61946x0nOS7MDuFNsWapGSSP01NdTK5z5IMDldct5Ud4w3zL85zbl9xQr40cm1EboxmZUZtAW8J2ZEZtAm0J25EZDQnIJniyRshruedrnOZp6RNP+3lnPEXyclQyzBCda8+aplrAscIRIjCb9SDFFj/40c1PXV6c2ZfcolYbOjKjNkgzMqM2gbaE7ciM2gTaErYjM6oQ4Kkab8fnp2KLjpNO4FFxsv/V70omZRKzU/wvHU5SH3SMh8ZPEqTngV2+X7VnuisFxbmGNVX8yngK+5LL5W9pb0ZtsGZkRm0CbQnbkRm1CbQlbEdmlAjIJ2HpEpNDC0uSbvCfLGWQIE4Pz/K+Ubz3sEqZMi6ZezrG0SoXdy/9ya/kcJSY0SJPFoM/1PZS6bzR14d9yfUKbCFiRm2oZmRGbQJtCduRGbUJtCVsR2YEAdkBPz/AkzWc6T4sOU6ckRD/rfZB+wUvq7/KERMwARMwARMwARM4UgLyf5htwnFamkTqF4cP6s7jM9Y6ja1fGoj70ARMwARMwARMwASOhgBP3p7KD1p68lZ1nCTI47OX2rjQwQRMwARMwARMwAROgoB8IJYV8eJa+sHLYaWrjhNCuoB/K+fZHhk4mIAJmIAJmIAJmMBRE5DPwyM6foNyYV1TWelRxwmh7kIy6N+GKy923ARMwARMwARMwASOgYB8HV52Y7Lou1X1Wek4caEy4reWXnQZrsrL50zABEzABEzABEzg4AjIx+HN/zfavlN8aV1TWaH/A99EryktPQVGAAAAAElFTkSuQmCC",
+                        "image/png": "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",
                         "text/latex": [
-                            "$\\displaystyle \\left( \\frac{1881}{80000}, \\  \\frac{10089}{80000}, \\  \\frac{6859}{80000}, \\  \\frac{53371}{80000}, \\  \\frac{159}{80000}, \\  \\frac{1071}{80000}, \\  \\frac{701}{80000}, \\  \\frac{5869}{80000}\\right)$"
+                            "$\\displaystyle \\left( \\frac{67239}{160000}, \\  \\frac{10881}{160000}, \\  \\frac{31681}{160000}, \\  \\frac{3799}{160000}, \\  \\frac{22901}{160000}, \\  \\frac{10179}{160000}, \\  \\frac{10179}{160000}, \\  \\frac{3141}{160000}\\right)$"
                         ],
                         "text/plain": [
-                            "\u239b 1881  10089   6859  53371   159    1071   701    5869\u239e\n",
-                            "\u239c\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u239f\n",
-                            "\u239d80000  80000  80000  80000  80000  80000  80000  80000\u23a0"
+                            "\u239b67239   10881   31681    3799   22901   10179   10179    3141 \u239e\n",
+                            "\u239c\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u239f\n",
+                            "\u239d160000  160000  160000  160000  160000  160000  160000  160000\u23a0"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Let's turn the voting frequencies back into integer counts\n",
                 "# First, we get the rational fractions.\n",
@@ -461,86 +461,90 @@
                 "# to access the members\n",
                 "data_sketch_frequencies = list(sympy.linsolve(generated_data_sketch, trio_frequencies))[0]\n",
                 "data_sketch_frequencies"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 8,
             "id": "e516dd2b-3878-4f87-89a5-7bb520444390",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/latex": [
-                            "$\\displaystyle \\left[ 1881, \\  10089, \\  6859, \\  53371, \\  159, \\  1071, \\  701, \\  5869\\right]$"
+                            "$\\displaystyle \\left[ 67239, \\  10881, \\  31681, \\  3799, \\  22901, \\  10179, \\  10179, \\  3141\\right]$"
                         ],
                         "text/plain": [
-                            "[1881, 10089, 6859, 53371, 159, 1071, 701, 5869]"
+                            "[67239, 10881, 31681, 3799, 22901, 10179, 10179, 3141]"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import math\n",
                 "maxDenominator = math.lcm(*[val.denominator for val in data_sketch_frequencies])\n",
                 "data_sketch_integers = [val*maxDenominator for val in data_sketch_frequencies]\n",
                 "data_sketch_integers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 9,
             "id": "0d25b068-0137-477f-bb27-62287f061cbe",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{('a', 'a', 'a'): 1881,\n",
-                            " ('a', 'a', 'b'): 10089,\n",
-                            " ('a', 'b', 'a'): 6859,\n",
-                            " ('a', 'b', 'b'): 53371,\n",
-                            " ('b', 'a', 'a'): 159,\n",
-                            " ('b', 'a', 'b'): 1071,\n",
-                            " ('b', 'b', 'a'): 701,\n",
-                            " ('b', 'b', 'b'): 5869}"
+                            "{('a', 'a', 'a'): 67239,\n",
+                            " ('a', 'a', 'b'): 10881,\n",
+                            " ('a', 'b', 'a'): 31681,\n",
+                            " ('a', 'b', 'b'): 3799,\n",
+                            " ('b', 'a', 'a'): 22901,\n",
+                            " ('b', 'a', 'b'): 10179,\n",
+                            " ('b', 'b', 'a'): 10179,\n",
+                            " ('b', 'b', 'b'): 3141}"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# And now we turn them into a data_sketch with their vote patterns\n",
                 "vote_pattern_counts = {trio_vote_patterns[i]: data_sketch_integers[i] for i in range(8)}\n",
                 "vote_pattern_counts"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 10,
             "id": "8682bab4-478c-403f-9d38-2691a10f8871",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{\"'a' prevalence solutions\": [19/20, 1/20],\n",
-                            " 'accuracies': [{'a': [9/10, 19/20], 'b': [1/20, 1/10]},\n",
-                            "  {'a': [3/20, 9/20], 'b': [11/20, 17/20]},\n",
-                            "  {'a': [1/10, 1/2], 'b': [1/2, 9/10]}]}"
+                            "[{'prevalence': {'a': 1/5, 'b': 4/5},\n",
+                            "  'accuracy': [{'a': 9/20, 'b': 9/40},\n",
+                            "   {'a': 31/40, 'b': 13/40},\n",
+                            "   {'a': 13/40, 'b': 1/20}]},\n",
+                            " {'prevalence': {'a': 4/5, 'b': 1/5},\n",
+                            "  'accuracy': [{'a': 31/40, 'b': 11/20},\n",
+                            "   {'a': 27/40, 'b': 9/40},\n",
+                            "   {'a': 19/20, 'b': 27/40}]}]"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from ntqr.r2.evaluators import ErrorIndependentEvaluation\n",
                 "from ntqr.r2.datasketches import TrioVoteCounts\n",
@@ -556,31 +560,31 @@
             "metadata": {},
             "source": [
                 "Note how the error independent solution is the best you could possibly do in an unlabeled setting - it returns just two points. In the language of algebraic geometry we would say that the variety (the set of possible solutions) of the error indepedent ideal (the generating set of polynomials) is zero dimensional and consists of two points. One of these two solutions should be an exact match with the random values you got when running this notebook."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 11,
             "id": "18315ee1-4e4b-4736-9efc-658967aa08ca",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{P_a: Fraction(19, 20),\n",
-                            " P_{i, a}: Fraction(9, 10),\n",
-                            " P_{i, b}: Fraction(1, 20),\n",
-                            " P_{j, a}: Fraction(3, 20),\n",
-                            " P_{j, b}: Fraction(11, 20),\n",
-                            " P_{k, a}: Fraction(1, 10),\n",
-                            " P_{k, b}: Fraction(1, 2)}"
+                            "{P_a: Fraction(4, 5),\n",
+                            " P_{i, a}: Fraction(31, 40),\n",
+                            " P_{i, b}: Fraction(11, 20),\n",
+                            " P_{j, a}: Fraction(27, 40),\n",
+                            " P_{j, b}: Fraction(9, 40),\n",
+                            " P_{k, a}: Fraction(19, 20),\n",
+                            " P_{k, b}: Fraction(27, 40)}"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "random_performance_statistics"
             ]
@@ -601,147 +605,149 @@
                 "Majority voting (MV) is usually discussed in the ML/AI literature as a **decision** algorithm. But it can also be used to carry out algebraic evaluation by using those decisions to impute an answer key for the test. Note that this means that the MV algorithm is saying exactly what each item's true label should be. This is to be contrasted with the solution presented here which is **fully** inferential since it never decides what the label of any item on the test should be.\n",
                 "\n",
                 "The main problem with MV as an evaluator is that it cannot deal with the **minority report** situation. The crowd is not always right and there are cases where one classifier or two may be badly tuned. We are going to demonstrate that problem by doing a simulation of error independent classifiers that has a 'flipped' classifier."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 12,
             "id": "f8c7b9b3-9af4-4165-8d92-6155877eec4c",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "{P_{i, a}: Fraction(3, 5),\n",
-                            " P_{i, b}: Fraction(13, 20),\n",
-                            " P_{j, a}: Fraction(7, 10),\n",
-                            " P_{j, b}: Fraction(4, 5),\n",
-                            " P_{k, a}: Fraction(1, 10),\n",
-                            " P_{k, b}: Fraction(11, 20),\n",
-                            " P_a: Fraction(1, 5)}"
-                        ]
-                    },
-                    "execution_count": 37,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "P_i_a + P_i_b: -1/100\n",
+                        "P_j_a + P_j_b: 3/50\n",
+                        "P_k_a + P_k_b: -7/25\n"
+                    ]
                 }
             ],
             "source": [
                 "# Let's pick all the classifiers above 50% performance to start with.\n",
-                "simulated_error_independent_performance = {var:Fraction(randint(11,20),20) for var in [pia, pib, pja, pjb, pka, pkb]}\n",
-                "# Then let's flip, say, classifier k on the 'a' label below 50% accuracy\n",
-                "simulated_error_independent_performance[pka] = Fraction(randint(0,9),20)\n",
+                "size_test=100\n",
+                "simulated_error_independent_performance = {var:Fraction(randint(0,size_test),size_test) for var in [pia, pib, pja, pjb, pka, pkb]}\n",
+                "# Then let's flip, say, classifiers j,k on the 'a' label below 50% accuracy\n",
+                "simulated_error_independent_performance[pja] = Fraction(randint(0,int(size_test/2)-1),size_test)\n",
+                "simulated_error_independent_performance[pka] = Fraction(randint(0,int(size_test/2)-1),size_test)\n",
                 "# And let's set the 'a' label prevalence to some number below 50%\n",
-                "simulated_error_independent_performance[pa] = Fraction(randint(3,7),20)\n",
-                "simulated_error_independent_performance"
+                "simulated_error_independent_performance[pa] = Fraction(randint(1,int(size_test/2)-1),size_test)\n",
+                "smeip = simulated_error_independent_performance\n",
+                "print(\"P_i_a + P_i_b: {}\".format(smeip[pia] + smeip[pib]-1))\n",
+                "print(\"P_j_a + P_j_b: {}\".format(smeip[pja] + smeip[pjb]-1))\n",
+                "print(\"P_k_a + P_k_b: {}\".format(smeip[pka] + smeip[pkb]-1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 13,
             "id": "6c132101-87a5-4118-bb71-f328482f7624",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/latex": [
-                            "$\\displaystyle \\left( \\frac{21}{625}, \\  \\frac{133}{1250}, \\  \\frac{261}{2500}, \\  \\frac{389}{2500}, \\  \\frac{131}{2500}, \\  \\frac{269}{2500}, \\  \\frac{237}{1250}, \\  \\frac{313}{1250}\\right)$"
+                            "$\\displaystyle \\left( \\frac{314001}{5000000}, \\  \\frac{139557}{2500000}, \\  \\frac{843219}{5000000}, \\  \\frac{344583}{2500000}, \\  \\frac{423299}{5000000}, \\  \\frac{190293}{2500000}, \\  \\frac{1133481}{5000000}, \\  \\frac{468567}{2500000}\\right)$"
                         ],
                         "text/plain": [
-                            "\u239b 21  133   261   389   131   269   237   313 \u239e\n",
-                            "\u239c\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u239f\n",
-                            "\u239d625  1250  2500  2500  2500  2500  1250  1250\u23a0"
+                            "\u239b 314001   139557   843219   344583   423299   190293  1133481   468567\u239e\n",
+                            "\u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500, \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u239f\n",
+                            "\u239d5000000  2500000  5000000  2500000  5000000  2500000  5000000  2500000\u23a0"
                         ]
                     },
-                    "execution_count": 41,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "generated_data_sketch = [poly.subs(simulated_error_independent_performance) for poly in simplified_generating_set]\n",
                 "sympy.Matrix(generated_data_sketch)\n",
                 "data_sketch_frequencies = list(sympy.linsolve(generated_data_sketch, trio_frequencies))[0]\n",
                 "data_sketch_frequencies"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 14,
             "id": "9c7ea207-22fc-47a9-a57d-63b5480f1769",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/latex": [
-                            "$\\displaystyle \\left[ 84, \\  266, \\  261, \\  389, \\  131, \\  269, \\  474, \\  626\\right]$"
+                            "$\\displaystyle \\left[ 314001, \\  279114, \\  843219, \\  689166, \\  423299, \\  380586, \\  1133481, \\  937134\\right]$"
                         ],
                         "text/plain": [
-                            "[84, 266, 261, 389, 131, 269, 474, 626]"
+                            "[314001, 279114, 843219, 689166, 423299, 380586, 1133481, 937134]"
                         ]
                     },
-                    "execution_count": 43,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "maxDenominator = math.lcm(*[val.denominator for val in data_sketch_frequencies])\n",
                 "data_sketch_integers = [val*maxDenominator for val in data_sketch_frequencies]\n",
                 "data_sketch_integers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 15,
             "id": "324e2e9c-02f0-4a54-8943-0e1342d04d34",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{('a', 'a', 'a'): 84,\n",
-                            " ('a', 'a', 'b'): 266,\n",
-                            " ('a', 'b', 'a'): 261,\n",
-                            " ('a', 'b', 'b'): 389,\n",
-                            " ('b', 'a', 'a'): 131,\n",
-                            " ('b', 'a', 'b'): 269,\n",
-                            " ('b', 'b', 'a'): 474,\n",
-                            " ('b', 'b', 'b'): 626}"
+                            "{('a', 'a', 'a'): 314001,\n",
+                            " ('a', 'a', 'b'): 279114,\n",
+                            " ('a', 'b', 'a'): 843219,\n",
+                            " ('a', 'b', 'b'): 689166,\n",
+                            " ('b', 'a', 'a'): 423299,\n",
+                            " ('b', 'a', 'b'): 380586,\n",
+                            " ('b', 'b', 'a'): 1133481,\n",
+                            " ('b', 'b', 'b'): 937134}"
                         ]
                     },
-                    "execution_count": 44,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "vote_pattern_counts = {trio_vote_patterns[i]: data_sketch_integers[i] for i in range(8)}\n",
                 "vote_pattern_counts"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 16,
             "id": "2bcf4758-2623-4dff-98ea-729f6d67ad39",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{\"'a' prevalence solutions\": [4/5, 1/5],\n",
-                            " 'accuracies': [{'a': [7/20, 3/5], 'b': [2/5, 13/20]},\n",
-                            "  {'a': [1/5, 7/10], 'b': [3/10, 4/5]},\n",
-                            "  {'a': [9/20, 1/10], 'b': [9/10, 11/20]}]}"
+                            "[{'prevalence': {'a': 49/100, 'b': 51/100},\n",
+                            "  'accuracy': [{'a': 21/50, 'b': 57/100},\n",
+                            "   {'a': 31/100, 'b': 3/4},\n",
+                            "   {'a': 2/5, 'b': 8/25}]},\n",
+                            " {'prevalence': {'a': 51/100, 'b': 49/100},\n",
+                            "  'accuracy': [{'a': 43/100, 'b': 29/50},\n",
+                            "   {'a': 1/4, 'b': 69/100},\n",
+                            "   {'a': 17/25, 'b': 3/5}]}]"
                         ]
                     },
-                    "execution_count": 45,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "tvc = TrioVoteCounts(vote_pattern_counts)\n",
                 "evaluator = ErrorIndependentEvaluation(tvc)\n",
@@ -755,44 +761,68 @@
             "metadata": {},
             "source": [
                 "Note that the error independent algebraic solution correctly picked up that classifier k (3) is actually below 50%. What does majority voting say?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 17,
             "id": "3e04fe9a-d480-456d-85dc-ccc037fe0d9c",
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ntqr.r2.evaluators import MajorityVotingEvaluation\n",
+                "mv_estimate = MajorityVotingEvaluation(tvc)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "c790a182-22a5-47d7-a0ff-219865f409f9",
+            "metadata": {},
+            "source": [
+                "How does the MV evaluation do?"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 18,
+            "id": "9facc3bd-14c7-4fbc-a528-cbecfaf16578",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "image/png": "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/vz5Yvv27SIhIUHExsaK1q1biyZNmoiioiKp3/vvvy8ACD8/PzF9+nQRHx8vvvvuO61lGunp6cLBwUGEhISI7777Tuzfv1+sW7dOjBw5Utp2QUGBaNWqlXBychKffPKJiIuLE++9956wsbER/fr103ptAQh/f3/x5JNPik2bNomdO3eK4OBgYWNjI/74448K35esrCzh4+Mj6tatK5YtWyZ27dolXn/9dQFATJw4UQghRE5Ojjh8+LBQqVSia9eu4vDhw+Lw4cPi3r175a731VdfFba2tuKtt94Su3btEuvXrxdPPPGE8PT0FJmZmVK/CRMmCDs7O5GYmCiEEGLv3r3CyspKvPvuu1rrGzNmjFi5cqWIj48X8fHx4qOPPhJKpVJ88MEHWv0e9TlLTU0VXbt2FSqVShrH4cOHK3yNPvroI/Hf//5X7NixQ+zfv18sW7ZMBAQEiJ49e2r1e/h9FkKI4cOHCysrKzFjxgwRFxcnFi9eLOrXry/c3NzE6NGjpX4ZGRmifv36ws/PT/zf//2f2LNnj/joo4+Evb29GDNmjNQvPT1d+ux269ZNbNmyRXz77beiY8eOwtbWVhw6dEinnrI+k99++62YPXu22LZtm0hISBAbN24UPXr0EHXr1hV//vmntI59+/YJAGLfvn1S265du4Stra1o1aqVWLNmjfj555/FqlWrxIsvvljh65ifny/atGkj6tSpI6KiosSePXvEkiVLhJubm3jmmWeEWq0WQgixZMkSAUDrZ14IIXbu3CkAiO3bt0ttlf1c9OjRQ/To0aPCcT34+q5evVpqq8xrlZWVJf3+iomJkT5XWVlZQojS31l+fn7SOtVqtejTp4+wsbER7733noiLixOffPKJcHJyEm3bttX62fLz8xO+vr6iWbNmYu3atWL37t1i6NChAoBISEio8DWfMWOGcHZ2ln5XZWZmCgBCqVSKefPmSf0mTpwoPD09pcea35Hp6elCiIp/bjSvmb+/v3j22WfFd999J7777jvRsmVLUbt2bXH79u0Ka9S8F99++6147733hLe3tyguLhZCCPHTTz8JhUIhLly4IPr376/1GgohxEsvvSRsbW2l11lj6NChwsHBQet3Of2DIc0MrV27VgAQy5YtE0IIkZeXJ5ydncXTTz/9yOdevHhRWFtbixEjRpTbJzs7WyiVSp0AcuXKFWFv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",
                         "text/plain": [
-                            "{'prevalence': {'a': Fraction(371, 1250), 'b': Fraction(879, 1250)},\n",
-                            " 'accuracies': [{'a': Fraction(611, 2500), 'b': Fraction(1369, 2500)},\n",
-                            "  {'a': Fraction(481, 2500), 'b': Fraction(1489, 2500)},\n",
-                            "  {'a': Fraction(119, 625), 'b': Fraction(321, 625)}]}"
+                            "<Figure size 700x600 with 1 Axes>"
                         ]
                     },
-                    "execution_count": 46,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "from ntqr.r2.evaluators import MajorityVotingEvaluation\n",
-                "mv_estimate = MajorityVotingEvaluation(tvc)\n",
-                "mv_estimate.evaluation_exact"
+                "%matplotlib inline\n",
+                "from ntqr.r2.plots import plot_evaluations\n",
+                "mv_exact = mv_estimate.evaluation_exact\n",
+                "size=40\n",
+                "plot_evaluations([\n",
+                "    [\"algebraic evaluation\",[d['a']*100 for d in eval_exact[0][\"accuracy\"]],\n",
+                "    [d['b']*100 for d in eval_exact[0][\"accuracy\"]],\n",
+                "    \"^\", \"k\",size],\n",
+                "    [\"majority voting\",[d['a']*100 for d in mv_exact[0][\"accuracy\"]],\n",
+                "    [d['b']*100 for d in mv_exact[0][\"accuracy\"]],\n",
+                "    \"o\", \"g\",size]],\"A comparison of exact algebraic evaluation with MV\",figsize=(7,6),legend_loc=\"best\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c790a182-22a5-47d7-a0ff-219865f409f9",
+            "id": "c716262e-31d7-4ed0-8c9e-88144dfbe5c2",
             "metadata": {},
             "source": [
-                "This is a terrible evaluation. Yes, it identified that the third classifier was below 50% but note that it also said that all the classifiers are less than 50% in their 'a' label accuracy. It would thus say that no classifier is doing a good job classifying 'a' items, a false statement."
+                "This figure encapsulates the huge advantage of algebraic evaluation over majority voting when it comes to the problem of AI safety. When things are going well, monitoring is useful but not critical. The most important reason for monitoring is the detection of misaligned or malfunctioning algorithms. We see in the figure above that MV thinks that all is well with classifier 2."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `ntqr-0.2/docs/source/notebooks/LogicOfUnsupervisedEvaluationTutorial.ipynb` & `ntqr-0.3.1/docs/source/notebooks/LogicOfUnsupervisedEvaluationTutorial.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9474774017349353%*

 * *Differences: {"'cells'": "{4: {'execution_count': 1, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['IPython console for SymPy 1.12 (Python "*

 * *            "3.11.5-64-bit) (ground types: gmpy)\\n', '\\n', 'These commands were executed:\\n', "*

 * *            '\'>>> from sympy import *\\n\', ">>> x, y, z, t = symbols(\'x y z t\')\\n", ">>> k, '*

 * *            'm, n = symbols(\'k m n\', integer=True)\\n", ">>> f, g, h = symbols(\'f g h\', '*

 * *            'cls=Function)\\n", \'>>> ini […]*

```diff
@@ -38,30 +38,17 @@
             "metadata": {},
             "source": [
                 "We say the expressions in `ntqr.r2.postulates` are postulates because they are always identically zero for sample statistics that come from summarizing the decisions of binary classifiers. This section will demonstrate this with the example data sketch from an UCI Adult dataset evaluation contained in `ntqr.r2.examples`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 1,
             "id": "75ca2ffd-bbfc-4935-baff-84675becc508",
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "import sympy\n",
-                "\n",
-                "import ntqr\n",
-                "from pprint import pprint"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
-            "id": "4360d38b-fcf0-4258-a4a1-a16b7a3c04e5",
-            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "IPython console for SymPy 1.12 (Python 3.11.5-64-bit) (ground types: gmpy)\n",
                         "\n",
@@ -74,14 +61,17 @@
                         "\n",
                         "Documentation can be found at https://docs.sympy.org/1.12/\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
+                "import sympy\n",
+                "import ntqr\n",
+                "from pprint import pp\n",
                 "sympy.init_session()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "85be1465-a5e6-4cc3-ad22-c0d0ef853864",
             "metadata": {},
@@ -93,15 +83,15 @@
                 "The count of three thus makes this example easy to use throughout the documentation. The postulates released so far are applicable to any number of classifiers. For example, the pair postulates apply to any pair you pick out from an ensemble. But as of v0.1.5 only the N <= 2 postulates have been released for the case R=2. The next release will contain the N = 3 postulates.\n",
                 "\n",
                 "In the examples shown here, we check the postulates up to N = 2."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 2,
             "id": "3b484555-bd93-4d05-8c73-f54a151c4262",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'a': {('a', 'a', 'a'): 715,\n",
@@ -118,15 +108,15 @@
                             "  ('a', 'b', 'b'): 7517,\n",
                             "  ('b', 'a', 'a'): 272,\n",
                             "  ('b', 'a', 'b'): 399,\n",
                             "  ('b', 'b', 'a'): 6377,\n",
                             "  ('b', 'b', 'b'): 12455}}"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from ntqr.r2.examples import uciadult_label_counts as data_sketch\n",
                 "data_sketch"
@@ -138,15 +128,15 @@
             "metadata": {},
             "source": [
                 "Let us use these by-label voting events counts to calculate the exact evaluation for the classifiers on this test."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 3,
             "id": "fa46f8d6-a683-4651-bb44-128a60c8e8f7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create a class that gives us convenience functions for\n",
                 "# making marginalized counts or percentages of counts.\n",
                 "trio_label_counts = ntqr.TrioLabelVoteCounts(data_sketch)\n",
@@ -164,77 +154,73 @@
             "metadata": {},
             "source": [
                 "We are so accustomed to turning numbers into floats in our computers that we forget that for any finite test the sample statistics of correctness can only be rational numbers. In the case of grading a test, we either have integers or ratios of integers - the rationals."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 4,
             "id": "1e0e94b5-7025-42ae-b58e-0d9e48ae64ba",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'accuracies': {'a': [Fraction(3737, 5687),\n",
-                        "                      Fraction(1260, 5687),\n",
-                        "                      Fraction(4746, 5687)],\n",
-                        "                'b': [Fraction(6501, 10385),\n",
-                        "                      Fraction(29744, 31155),\n",
-                        "                      Fraction(4168, 6231)]},\n",
-                        " 'pair_correlations': {'a': {(0, 1): Fraction(273192, 32341969),\n",
-                        "                             (0, 2): Fraction(13325, 32341969),\n",
-                        "                             (1, 2): Fraction(-264525, 32341969)},\n",
-                        "                       'b': {(0, 1): Fraction(2204576, 323544675),\n",
-                        "                             (0, 2): Fraction(-79682, 12941787),\n",
-                        "                             (1, 2): Fraction(94508, 38825361)}},\n",
-                        " 'prevalence': {'a': Fraction(5687, 36842), 'b': Fraction(31155, 36842)}}\n"
+                        "{'prevalence': {'a': 5687/36842, 'b': 31155/36842},\n",
+                        " 'accuracy': [{'a': 3737/5687, 'b': 6501/10385},\n",
+                        "              {'a': 1260/5687, 'b': 29744/31155},\n",
+                        "              {'a': 4746/5687, 'b': 4168/6231}],\n",
+                        " 'pair_correlation': {(0, 1): {'a': 273192/32341969, 'b': 2204576/323544675},\n",
+                        "                      (0, 2): {'a': 13325/32341969, 'b': -79682/12941787},\n",
+                        "                      (1, 2): {'a': -264525/32341969, 'b': 94508/38825361}},\n",
+                        " '3_way_correlation': {(0, 1, 2): {'a': 452568508/183928777703,\n",
+                        "                                   'b': -27265589/134400457995}}}\n"
                     ]
                 }
             ],
             "source": [
                 "# The current version does not implement the last correlations needed\n",
                 "# for three binary classifiers - the 3-way correlations.\n",
-                "pprint(supervised_eval_exact, depth=4)"
+                "pp(supervised_eval_exact, sort_dicts=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "11aebe5e-3305-48f4-bffb-cf221a67e5ea",
             "metadata": {},
             "source": [
                 "Although exact, these numbers are hard for humans to interpret since we prefer decimal numbers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 5,
             "id": "ced779b0-19d3-47f4-8bde-c00acc0fb0bd",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'accuracies': [{'a': 0.6571127132055565, 'b': 0.625999037072701},\n",
-                        "                {'a': 0.22155793915948654, 'b': 0.9547103193708875},\n",
-                        "                {'a': 0.8345349041673993, 'b': 0.6689134970309741}],\n",
-                        " 'pair_correlations': {'a': {(0, 1): 0.008446981072797392,\n",
-                        "                             (0, 2): 0.00041200336318422665,\n",
-                        "                             (1, 2): -0.008179001099160041},\n",
-                        "                       'b': {(0, 1): 0.0068138225424356005,\n",
-                        "                             (0, 2): -0.006156954986200901,\n",
-                        "                             (1, 2): 0.0024341821316226785}},\n",
-                        " 'prevalence': {'a': 0.15436186960534173, 'b': 0.8456381303946583}}\n"
+                        "{'prevalence': {'a': 0.15436186960534173, 'b': 0.8456381303946583},\n",
+                        " 'accuracy': [{'a': 0.6571127132055565, 'b': 0.625999037072701},\n",
+                        "              {'a': 0.22155793915948654, 'b': 0.9547103193708875},\n",
+                        "              {'a': 0.8345349041673993, 'b': 0.6689134970309741}],\n",
+                        " 'pair_correlation': {(0, 1): {'a': 0.008446981072797392,\n",
+                        "                               'b': 0.0068138225424356005},\n",
+                        "                      (0, 2): {'a': 0.00041200336318422665,\n",
+                        "                               'b': -0.006156954986200901},\n",
+                        "                      (1, 2): {'a': -0.008179001099160041,\n",
+                        "                               'b': 0.0024341821316226785}}}\n"
                     ]
                 }
             ],
             "source": [
-                "pprint(supervised_eval_float,depth=4)"
+                "pp(supervised_eval_float, sort_dicts=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "86912545-74b6-4aef-84f1-5bf7158b4505",
             "metadata": {},
             "source": [
@@ -249,20 +235,20 @@
             "metadata": {},
             "source": [
                 "## The NTQR postulates for N=2, R=2 binary classifiers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "id": "00c23857-4a81-4c41-9832-6f556422923d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ntqr.r2.postulates import single_binary_classifier_postulate"
+                "from ntqr.r2.paxioms import single_binary_classifier_axiom"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "77d52049-b841-4e9f-8761-6ce53aae494d",
             "metadata": {},
             "source": [
@@ -275,48 +261,48 @@
             "metadata": {},
             "source": [
                 "### The single binary classifier postulate check"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "id": "b75837fe-c3c1-4efd-b835-0d970bde661a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAARUAAAAWCAYAAADuDQj4AAAACXBIWXMAAA7EAAAOxAGVKw4bAAAHQklEQVR4Ae2cb3LVNhTFX5m3gDRdAekOaFkBdAeBroB0BzD9lHxj6A6gK2BgB8AKoOyg7ACaHaTnp0gP+/nalmTJfpNYM45sWbo6997jqz923ubq6mqz9HF+fn6yNIab3v9tt/Ft178Wvy273tksnC4uLp4Kwr2FYdyG7k+8rW+Dri0dV461zFH6osOrH4hgzeQd8JvKHvry98ov/fmR8mMdn3Q8U91Q7m+nZWp/qhb3lT+zWs6Jxep/yTLp/lL9B/s+13U4z4bl7Xmp/FW2kIINPZ6qXFMfK8cMn8kuxfjl/bjjVSeohP5VkWjzWfkvoSzkKnun81913NV5FtnV7kjtP1jyQz8hV52qWEI/h5JL3xfCcqLjuY4POp6o7K3yyUly/pGQB8qz/DYZgCFAWKr4V3JXjtn2Ls6vJq/M5Y8qhOXIawMTRUQ5HHbGRWZCMeQMppmwDGJY4CZ2xfZhVshssVTC5tj+IFJl/64cs71cg187Xm3tPltLH6sKoyjpp+ss6+9jEeqPiJbNZZhVvQQWS+4iZbIJ+hKw3+uc2UTJgLKRzFc6/tMxeflayEA1/btybM9J8nsVfjV5Zc5UhIN17kYVP+9hCpfuvi4YTZOT5LLO/RLZsCqWSAxzVkPfL7IRAaVWwvaPawlPlFvFvyvHer1Qk1+OV9uerolm5ggpZ7E04j4jXV/Q6RG7K0YxU/6uxveT2li+97TgmWzJlBS7oO83Xb/xecxsTlWTEranr0PYsK3l35VjDUrMxC/Hq22jX3eqzsN+Cpuxu6RylhkQnFnGI11P2ThkkzdlPyUKizCxbDhWHjsLUvXDSMLMA87ShE1L3vb8VRHZv5LNw7xoko41ubZyrOHdmfjleNUJKsIRyMar3uaGHg3eqcx8/dvAH3PKw/8tomIqlj8l86uOmg9kBOy8KrJt2B+KncXldXRt+9BXrowS7aL8K7sQfP7WwQyOGUhMWoxjmXhjdJpUp49fBfHyTJ9YQcU5TR09mqTBcONj3Y7ZM0jCIswlAl4vcsmHqLziJY9NzOpil4lu5E6oH4thvx4zuVEdZtA3yr/YQweYU2agi3EsB+8MtoYDJr9y8CLMSI5XVlBh9Ih9CAy5RYsOCctGxicQdr7bKajxfclKeXByu4564GbQN8W/1H2Qq/BAuxQMA2I6t5LwzmBrAA7xKwlvR9vrAserbfOmFHORTGVR02/VZ7RjycHSiHNeMb9U+diDwTRpcKRMwaK6GATsLNlGZ1iqk4tbXVRN6GAG9MKY0R8fLJakTzTXfF0wP9Q5vubh4IPAywEFFuNYJt4BVYrdMvlVEK/j1Z09uDiM1NoYvS5q/xUQBPB1JkGETUYCEf/HE5MIOmNr+igsHsc95eyjnPrrXgz+fi7uXrmFbrC5+HFfVgXMx+pjLPDvwyh9HeVf3yl1wctGNn7GRs39Pl120mIcE5IcvB0FKhSY/CqI1/FqP6j8jiJyXMxMBafygVaTnHz/37xGnJUYjRlthlIsFhSBbKfKY77vmIJ7CO+ke8JPkCVQWzOVaMySMzogqA+WcFY/Kp4txfoXQOy9vJBuYWZCzgMylJbkWA7eIV0m3xvh1yjeFF5tQasGvN6F1EyPuIaYvOkZeovCx1PNpQbROSYYqZr7aI7vMDopFYvquyCmnNfdo6+pVWcK7g7eggXB9pYNozHLDm7zcwQXvqrx/ctIt9lcI4A0N+EJimOD12vVWYpjOXhHbTexwhC/RvGm8CoElSSCqQNGVI6mYyHzG39vozyMKh1b6B67+dRh2dIaMXWdhAXhagMWHhTetHRkUofk62XjvpZS7S/263z7E4tZ9U7VntnfV533Dga655adyq3gVU25IFj9JvtXbY/UrskTguyTINPKqa9jo6PDB5UlY1CbKI55LMl4LR0Kl5n8GsMrvZN5tb/8idJDHREwOFzSNVGQh5ogg8NjElP6ZOf2CKZvSASmnUxd41z6ccnfn4o7iJucCw97QGE0ZbRgdG2lRMzsNfzcEtC9YMTf2aR7+yBLWNYegUw5Xx5/Ut4JwAby2TnmMeTiNVTIL5KNRvkViTeJV1lBxQNh6cOn+jiZ0Q+yEg03Kts9uFxbSXXY3OUHXtzIadVJKGPUxZFPlTcfGGSfqZxoG9Ik3EFIoRysBL7wwPQ9KKOYJYO2BNTeJaDqYA9sfgif5wtKdEJ/9lTwL/ZyPBtr7fVcimPJeMf0ybifwi8Tr2yYzKttBlDXRJ3xIE+dQkMWRuookriOjT/CQhBDViupnCnzj8p3QaUQ7lY/Ey6c09WevIM/yI3BrDoEJh4gZmyMUFaAIuDsZnJB/qHn6DQB9xIcm4K3pDti+dWLV7ZP5lXvjzSV1GxIlkAzevIQ9O4DDLUfuye5LI2YLhN4bnSSjm6DXUryNqylr64Z5d8qb+6D3Wh7BOWk88qxYIyMXPZL41WtH8Q9FLn6Yd6zQ8Gy4lj+R9Zr+GDlWNuv/wMzN3/G8Pvc6gAAAABJRU5ErkJggg==",
                         "text/latex": [
                             "$\\displaystyle P_{a} \\left(P_{i, a} - f_{a_i}\\right) - P_{b} \\left(P_{i, b} - f_{b_i}\\right)$"
                         ],
                         "text/plain": [
                             "P\u2090\u22c5(P_{i, a} - f_{a_i}) - P_b\u22c5(P_{i, b} - f_{b_i})"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "single_binary_classifier_postulate"
+                "single_binary_classifier_axiom"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a30e0440-0c0b-45c0-af9f-bd51714abbc0",
             "metadata": {},
             "source": [
                 "Let's redefine some names to make the checks easier to write out."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "id": "5f587743-42fa-44a6-b537-f2da585be671",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -336,34 +322,34 @@
             "metadata": {},
             "source": [
                 "We also need to know the label accuracy for each of the three classifiers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 9,
             "id": "b37413ed-4ba7-47ba-82d8-add94387a04f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[{'a': Fraction(3737, 5687), 'b': Fraction(6501, 10385)},\n",
-                            " {'a': Fraction(1260, 5687), 'b': Fraction(29744, 31155)},\n",
-                            " {'a': Fraction(4746, 5687), 'b': Fraction(4168, 6231)}]"
+                            "[{'a': 3737/5687, 'b': 6501/10385},\n",
+                            " {'a': 1260/5687, 'b': 29744/31155},\n",
+                            " {'a': 4746/5687, 'b': 4168/6231}]"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "classifier_accuracies = [\n",
-                "    {label: supervised_eval_exact['accuracies'][label][classifier]\n",
+                "    {label: supervised_eval_exact['accuracy'][classifier][label]\n",
                 "     for label in ('a', 'b')\n",
                 "    } for classifier in range(3)]\n",
                 "cla = classifier_accuracies\n",
                 "cla\n",
                 "    "
             ]
         },
@@ -379,30 +365,25 @@
                 "This still leaves a lot of choices. You could keep track of the sequence by which they decided if time was an important variable in your task, for example. Here we will focus on the simplest statistic - their aligned votes on a single item. \"Aligned\" means two things. The event ('a', 'b', 'a') refers to votes cast by the classifiers on the same item. Classifiers 1 and 3 think the item is 'a', but 2 votes 'b'. The order of the vote patterns always refers to the same classifiers - the 2nd meaning of \"aligned\". So in event ('a', 'b', 'a') classifier 1 voted 'a' and in event ('b', 'a', 'a') it voted 'b'.\n",
                 "\n",
                 "The package has a class that turns by-label data sketches to unlabeled data sketches - `TrioVoteCounts`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 10,
             "id": "0678ba47-ece2-41e7-b35f-db0701cd5b19",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "TrioVoteCounts(vote_counts={('a', 'a', 'a'): 986,\n",
-                        "                            ('a', 'a', 'b'): 630,\n",
-                        "                            ('a', 'b', 'a'): 5801,\n",
-                        "                            ('a', 'b', 'b'): 7972,\n",
-                        "                            ('b', 'a', 'a'): 562,\n",
-                        "                            ('b', 'a', 'b'): 493,\n",
-                        "                            ('b', 'b', 'a'): 7712,\n",
-                        "                            ('b', 'b', 'b'): 12686})\n"
+                        "TrioVoteCounts(vote_counts={('a', 'a', 'a'): 986, ('a', 'a', 'b'): 630, ('a', 'b'\n",
+                        ", 'a'): 5801, ('a', 'b', 'b'): 7972, ('b', 'a', 'a'): 562, ('b', 'a', 'b'): 493, \n",
+                        "('b', 'b', 'a'): 7712, ('b', 'b', 'b'): 12686})\n"
                     ]
                 }
             ],
             "source": [
                 "trio_vote_counts = trio_label_counts.to_TrioVoteCounts()\n",
                 "pprint(trio_vote_counts)\n",
                 "tvc = trio_vote_counts"
@@ -414,27 +395,27 @@
             "metadata": {},
             "source": [
                 "This highlights that in the unlabeled case we are seeing the sum of the by-label counts. So the by-label data sketch of the evaluation had 715 cases where the classifiers voted ('a', 'a', 'a') and the items where 'a'. But there where 271 cases where the items where 'b' and the classifiers also voted ('a', 'a', 'a'). 271 + 715 = 986 as we observe above."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 11,
             "id": "fbbd76c6-3f73-4b59-904c-87eae055be9b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[{'a': Fraction(15389, 36842), 'b': Fraction(21453, 36842)},\n",
-                            " {'a': Fraction(2671, 36842), 'b': Fraction(34171, 36842)},\n",
-                            " {'a': Fraction(15061, 36842), 'b': Fraction(21781, 36842)}]"
+                            "[{'a': 15389/36842, 'b': 21453/36842},\n",
+                            " {'a': 2671/36842, 'b': 34171/36842},\n",
+                            " {'a': 15061/36842, 'b': 21781/36842}]"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# We can turn the count integers into percentages or frequencies\n",
                 "classifiers_voting_frequencies = [\n",
@@ -443,47 +424,55 @@
                 "    } for classifier in range(3)]\n",
                 "cvf = classifiers_voting_frequencies\n",
                 "cvf"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 12,
             "id": "8998cbf5-23a4-4967-8d01-b20774342f5b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAEcAAAAVCAYAAAAU9vPjAAAACXBIWXMAAA7EAAAOxAGVKw4bAAABZklEQVRYCe1YwXHCMBC0GQpgQgfQAYQOUgJugXSQr/2FEpISUgJpIXRAOgikhOzaMhaMdXFs+R5Ymjl05iTt3loynOM0TV+iKHqGsSVZlh0Kd3ifyP1KixjibCHDHoGP4clRnzG0yDUZ14erbzFwgat32BL+TxXx62nhkHVTrFpxMHmCNd5gJ9gjbAbz3rRwSLwNlksc7pDELMpzyN3jvYGwCg6Jt8Eaec/4jhYM4gg3M4gTxBEUEEJh5wRxBAWEUNg5QRxBASHUeeeYf54ChJ+QFo7Ntok4UzPhwZ5I3xA+o/+8jbW41sIhNSeWzdtZlSNhFptsTzDWWnyV8QVjBf+KPm/wj8ZtVZhq4ZDjP7DkqhwL5bWVSdzZYdwctnYO+COghUMaTbFKyk2OVTlW6lcAZhHZd9PCyfPoLA5E4ZH77lsVLRw7j87iYLENiO/sRXvytXAu9MsHcvnMCO+Qi/fp/GVOfgFII47tDvTbbgAAAABJRU5ErkJggg==",
+                        "text/latex": [
+                            "$\\displaystyle \\left[ 1, \\  1, \\  1\\right]$"
+                        ],
                         "text/plain": [
-                            "[Fraction(1, 1), Fraction(1, 1), Fraction(1, 1)]"
+                            "[1, 1, 1]"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# By construction, these observed label voting frequencies must add to one.\n",
                 "[sum(cvf[classifier].values()) for classifier in range(3)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "id": "58382871-c493-4e94-82d5-1d897531a78a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAEcAAAAVCAYAAAAU9vPjAAAACXBIWXMAAA7EAAAOxAGVKw4bAAACBklEQVRYCe1Y0VECMRA9HApgtAMoQalASvDsQOxAPuEXO9AWtAPtgPFKsAOREnwPskzgNpLkjv2BzOR2s8nl7b5Ldi7pTKfTp6IoHlFZytlsVm3U03si9h0uOiBnDho+0PF5enToEYOLNSddvXtjdYPY+EEdoM5h+6ahzWKFQ59TsC5CQWKSL/QtICeoz9AnqFxh/dA7OXYrHPqWiqWSg0nGmKsH+S4BQ19BZ/tFbE2lFQ79zMFSycFcJaqWmBewjwDUg2yjWOHQ12SsEDkjTLZUopd8w/42ihUOfU3GqpETuSoumzJjhUM/c7Fq5GAuCZw5JlTa2FZWOIwhC0sjJ0SIb7/yG0fUrXAYQg1LI0fLNRK/fAH+9zQtVjj0MwurRg72p2wnbeuITRJzNkFWOHQwF6tGjouWR4m+030hK6eto4YVDmNIxgqR84bJbnxWnH4NWXlfgl9FVpMy/KDJCoeORGOJ1yo5CPgVA5aQdzLQkXCP9sOe7Rd9PGokFyscOhaL5QfR9Rt7OlcJD5pDSCZgylu0K8h1gb5CZf7hUYNV8pUbESWscOjMQSzf4yA5LlC55/Hf2dExboC6XWE7nRENKxy6EoslbqvbSjoT5NABJ7ySNdQKZ+1cY3JAChNyG/89/7JlheM70ZgcTDaG47zvOXaxwtnGIdekkjPOd8ib+3T+z5V/Al8AQkh7bxYAAAAASUVORK5CYII=",
+                        "text/latex": [
+                            "$\\displaystyle \\left[ 0, \\  0, \\  0\\right]$"
+                        ],
                         "text/plain": [
-                            "[Fraction(0, 1), Fraction(0, 1), Fraction(0, 1)]"
+                            "[0, 0, 0]"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Checking the single binary classifier postulate on all three classifiers\n",
                 "[ (pa * (cla[classifier]['a'] - cvf[classifier]['a']) - \n",
@@ -505,29 +494,29 @@
             "metadata": {},
             "source": [
                 "How well are the postulates obeyed when we use inexact float computations?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "id": "e995ef5e-9303-444b-858d-88069895594d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[ 3.46944695195361 \\cdot 10^{-17}, \\  5.55111512312578 \\cdot 10^{-17}, \\  -4.16333634234434 \\cdot 10^{-17}\\right]$"
                         ],
                         "text/plain": [
                             "[3.469446951953614e-17, 5.551115123125783e-17, -4.163336342344337e-17]"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Checking the single binary classifier postulate on all three classifiers\n",
                 "# but now we use floats\n",
@@ -535,29 +524,29 @@
                 "[ (float(pa) * (float(cla[classifier]['a']) - float(cvf[classifier]['a'])) - \n",
                 "   float(pb) * (float(cla[classifier]['b']) - float(cvf[classifier]['b'])))\n",
                 " for classifier in range(3)]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 15,
             "id": "7a5adf93-18b7-461a-9712-397b1c8e4c09",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[ 0.0302099194792449, \\  0.0188090034826021, \\  0.053721315513076\\right]$"
                         ],
                         "text/plain": [
                             "[0.03020991947924493, 0.01880900348260213, 0.053721315513076]"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# It gets worse when we use the fact that P_b = 1 - P_a\n",
                 "\n",
@@ -572,126 +561,126 @@
             "metadata": {},
             "source": [
                 "### The postulates for pairs of binary classifers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 16,
             "id": "969d11f0-2a5d-45b9-b9ec-62057f1aac63",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}\\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) - \\left(P_{i, b} - f_{b_i}\\right) \\left(P_{j, a} - f_{a_j}\\right)\\\\\\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) \\left(P_{i, a} + P_{i, b} - f_{a_i} - f_{b_i}\\right) + \\left(P_{i, a} - f_{a_i}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, b}\\right) + \\left(P_{i, b} - f_{b_i}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, a}\\right)\\\\\\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) \\left(P_{j, a} + P_{j, b} - f_{a_j} - f_{b_j}\\right) + \\left(P_{j, a} - f_{a_j}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, b}\\right) + \\left(P_{j, b} - f_{b_j}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, a}\\right)\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1                                                         (P_{i, a} - f_{a_i})\u22c5\n",
-                            "\u23a2                                                                              \n",
-                            "\u23a2(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{i, a} + P_{i, b} - f_{a_i} - f_{\n",
-                            "\u23a2                                                                              \n",
-                            "\u23a3(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{j, a} + P_{j, b} - f_{a_j} - f_{\n",
+                            "\u23a1                                                         (P_{i, a} - f_{a_i})\u22c5(P\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{i, a} + P_{i, b} - f_{a_i} - f_{b_\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a3(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{j, a} + P_{j, b} - f_{a_j} - f_{b_\n",
                             "\n",
-                            "(P_{j, b} - f_{b_j}) - (P_{i, b} - f_{b_i})\u22c5(P_{j, a} - f_{a_j})               \n",
-                            "                                                                               \n",
-                            "b_i}) + (P_{i, a} - f_{a_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{i, b} - f\n",
-                            "                                                                               \n",
-                            "b_j}) + (P_{j, a} - f_{a_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{j, b} - f\n",
+                            "_{j, b} - f_{b_j}) - (P_{i, b} - f_{b_i})\u22c5(P_{j, a} - f_{a_j})                   \n",
+                            "                                                                                 \n",
+                            "i}) + (P_{i, a} - f_{a_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{i, b} - f_{b_\n",
+                            "                                                                                 \n",
+                            "j}) + (P_{j, a} - f_{a_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{j, b} - f_{b_\n",
                             "\n",
-                            "                                          \u23a4\n",
-                            "                                          \u23a5\n",
-                            "_{b_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a5\n",
-                            "                                          \u23a5\n",
-                            "_{b_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a6"
+                            "                                      \u23a4\n",
+                            "                                      \u23a5\n",
+                            "i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a5\n",
+                            "                                      \u23a5\n",
+                            "j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a6"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from ntqr.r2.postulates import pair_binary_classifiers_postulates\n",
-                "sympy.Matrix(pair_binary_classifiers_postulates)"
+                "from ntqr.r2.paxioms import pair_binary_classifiers_axioms\n",
+                "sympy.Matrix(pair_binary_classifiers_axioms)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9910965d-17b3-43b9-8ec1-4ee956901d0d",
             "metadata": {},
             "source": [
                 "Starting with pairs of classifiers, one must worry about their error correlation on the test. This requires we introduce new sample statistics to capture this \"moment\" of the unknown sample statistics. We are treating evaluation on unlabeled data as an inverse problem so we are basically doing a moment expansion on the unknown ways a single classifier can be correct, pairs can correlate, trios can correlate, etc."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 17,
             "id": "1374c9af-bdbc-47ea-9510-af0898783d0c",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) - \\left(P_{i, b} - f_{b_i}\\right) \\left(P_{j, a} - f_{a_j}\\right)$"
                         ],
                         "text/plain": [
-                            "(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j}) - (P_{i, b} - f_{b_i})\u22c5(P_{j, a} - f_\n",
-                            "{a_j})"
+                            "(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j}) - (P_{i, b} - f_{b_i})\u22c5(P_{j, a} - f_{a\n",
+                            "_j})"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# The first postulate is interesting because it does not\n",
                 "# involve the unknown pair error correlations.\n",
                 "\n",
-                "pair_binary_classifiers_postulates[0].as_expr()"
+                "pair_binary_classifiers_axioms[0].as_expr()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 18,
             "id": "6d0a6afa-0382-4a13-a7d0-6791f23c3524",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}\\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) \\left(P_{i, a} + P_{i, b} - f_{a_i} - f_{b_i}\\right) + \\left(P_{i, a} - f_{a_i}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, b}\\right) + \\left(P_{i, b} - f_{b_i}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, a}\\right)\\\\\\left(P_{i, a} - f_{a_i}\\right) \\left(P_{j, b} - f_{b_j}\\right) \\left(P_{j, a} + P_{j, b} - f_{a_j} - f_{b_j}\\right) + \\left(P_{j, a} - f_{a_j}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, b}\\right) + \\left(P_{j, b} - f_{b_j}\\right) \\left(- \\Delta_{i,j} + \\Gamma_{i, j, a}\\right)\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{i, a} + P_{i, b} - f_{a_i} - f_{\n",
-                            "\u23a2                                                                              \n",
-                            "\u23a3(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{j, a} + P_{j, b} - f_{a_j} - f_{\n",
+                            "\u23a1(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{i, a} + P_{i, b} - f_{a_i} - f_{b_\n",
+                            "\u23a2                                                                                \n",
+                            "\u23a3(P_{i, a} - f_{a_i})\u22c5(P_{j, b} - f_{b_j})\u22c5(P_{j, a} + P_{j, b} - f_{a_j} - f_{b_\n",
                             "\n",
-                            "b_i}) + (P_{i, a} - f_{a_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{i, b} - f\n",
-                            "                                                                               \n",
-                            "b_j}) + (P_{j, a} - f_{a_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{j, b} - f\n",
+                            "i}) + (P_{i, a} - f_{a_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{i, b} - f_{b_\n",
+                            "                                                                                 \n",
+                            "j}) + (P_{j, a} - f_{a_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, b}) + (P_{j, b} - f_{b_\n",
                             "\n",
-                            "_{b_i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a4\n",
-                            "                                          \u23a5\n",
-                            "_{b_j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a6"
+                            "i})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a4\n",
+                            "                                      \u23a5\n",
+                            "j})\u22c5(-\\Delta_{i,j} + \\Gamma_{i, j, a})\u23a6"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# But the other two do.\n",
                 "# Note that they are symmetric in label and indices i,j.\n",
-                "sympy.Matrix(pair_binary_classifiers_postulates[1:3])"
+                "sympy.Matrix(pair_binary_classifiers_axioms[1:3])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d9e2457b-2b67-4975-8937-ff110390100e",
             "metadata": {},
             "source": [
@@ -704,30 +693,30 @@
             "metadata": {},
             "source": [
                 "Let's use SymPy to carry out the translation from the polynomial expressions above to a numerical value given the true values for all these test sample statistics."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 19,
             "id": "72cea099-1ab9-43c5-972a-5a5d5e55126e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# The decision frequencies we can calculate from the test data sketch\n",
-                "from ntqr.r2.postulates import fai, fbi, faj, fbj, deltaij\n",
-                "# The label accuracies for an arbitrary pair of classifiers\n",
-                "from ntqr.r2.postulates import pia, pib, pja, pjb\n",
+                "from ntqr.r2.paxioms import fai, fbi, faj, fbj, deltaij\n",
+                "# The label paxioms for an arbitrary pair of classifiers\n",
+                "from ntqr.r2.paxioms import pia, pib, pja, pjb\n",
                 "# The pair error correlation variables\n",
-                "from ntqr.r2.postulates import gija, gijb"
+                "from ntqr.r2.paxioms import gija, gijb"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 20,
             "id": "08743488-45e0-4c5e-a4b8-2928a159bef0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
@@ -755,121 +744,109 @@
                             "\u23a2                  32341969 \u23a5\n",
                             "\u23a2                           \u23a5\n",
                             "\u23a2                   2204576 \u23a5\n",
                             "\u23a2\\Gamma_{i, j, b}  \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u23a5\n",
                             "\u23a3                  323544675\u23a6"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "i, j = (0, 1)\n",
                 "values = {pia: cla[i]['a'], pib: cla[i]['b'], \n",
                 "          pja: cla[j]['a'], pjb: cla[j]['b'],\n",
-                "          gija: supervised_eval_exact['pair_correlations']['a'][(i,j)],\n",
-                "          gijb: supervised_eval_exact['pair_correlations']['b'][(i,j)]}\n",
+                "          gija: supervised_eval_exact['pair_correlation'][(i,j)]['a'],\n",
+                "          gijb: supervised_eval_exact['pair_correlation'][(i,j)]['b']}\n",
                 "sympy.Matrix([(key, val) for key, val in values.items()])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 21,
             "id": "35cc47c4-4846-471e-992a-23660acb3ca7",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAABCsAAABOCAYAAAAJvZyrAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAgAElEQVR4Ae2d27Edt5X3N1l8/oqmIphRBjIVgagMLCkCyhlwik+cN9ZMBrYioKwMbEcg2RloHAHpk4G+/w8Hqw+6G9e+7csBqnoDDSwsrBsWLo3u/eS333479dAl0CXQJdAl0CXQJdAl8Ngk8N///d//qev/lvK9tv7Sdnu9Ogl0/dTJqUN1CXQJdAlcqgSe9M2KS1VNp6tLoEtgSwlo0vpc+L7V9Uelfx/i9mVvfd5/+vi18u8mcP+j+48+707lf7ZypSkjUP6Z7v/L3fWf3SXgZT/Ti/LR5R91/dUTwf0n5f/k70++LrdRvak8aTeGo8eXKwHpD52/0vVJF+kvdb1X/j8VnxT/SRH5xKNNC2B0raovnD2skIDkT//L+mbBvBHMZ7pmfVhlWf1OSRP8P3SNxoclMNM6/b5LoEugS6BLYJkEnskpf6Gq/0hU/0nl3yTKenaXQJdAl8BFSUD+6nsR9H+K/xYS5v0cCxYCk99p+B/BsKh1QWkmuPjFz+9z3KKGezYwWMCY33SbFbqn3Y+K/xd4xa90/VXX19w/hiBe/6RrkOEanoUnqscYTsEm9SJ4FprgYjHDQpQxLdxgyupNsOg5Zzcqvv0gOWym272kJRpTNsMmIj7B+iq28Hddv/O02GaE6dlnn4DHntfWN3w3F29pFzn9qWzwK7QpQQ6+Wfd/0T36dZvDiv9Ani6bu5b0O+hFdbAN+nwy1MAkK19hgfi9+L5/hWLtJHcJdAkEEpCf+VW3+OpZUNmTp0Euk2wGhPBiUOihS6BLoEvg4iUgh/YHEfl7xaONCghXHhsM+LjRk1PKfPhe5eFihQUKx8PdxFUx978otqexxOFGBOVDu4IjzYZF1Pmq7BYDGz52gmExf8KR1OMUqWBLeqHKV4J7outzXdPTLlm9Cb5kN1OSbvV+E93uJRzpKWcz79Xuh6BtnsBzysICC13sY7hU8Gfd2wJ5bX1r5xbjTeyioL+sb5ZQ0X2oX3wvGxa2KV3Sr9OL4PH/qfGhGsYB3tbPJjq+LZF0broEugQ2lgBzsXD/gfRwAvZZ0Bi7p1lHHcD2ZJdAl0CXwMVIwE9M3yrOHt/NEIxj/CVTzlPbb4SfzQc2MP6mtNuc8HlMjKf+887DTvOVfXtBcmBRwBPNN7rcCZNWLlUPObboMamXsG3hZSECbvSGXk6K0SV5U/1Qjo6n+cp6nEGyWq3bvSQn2tBh0mZU7jYYg/ZZ3DIxshCmT4LnftjUWlvfGrnFWLJZbRfCkdWf5Jb0zaprm8H0WReUx+t5pF/qwkdn9Qug4KGBPj+cuiI/DDUwIfytpMX3ah3fiiw6H10CXQL7SEB+ZuZ7lUdjjNenp/z00CXQJdAlcOUS4Cjw4pNgOEpdw4RXuJggM0njyToTWS5OUhC7CbDyWSgTyIsFnt6+iBXcap5k4o7Oe5ktYbNajxV6sfbfKsHGA3r7QfXc4Kd015uEUBs20G1tU61wVTYj+tlE4/UBHswMEyOlh00ppbENXt+6mxKhvFX1p/hu5V5y2bXPg3+ij9A3ozt0ZZsWJ8Gy6UBwebqv0S+nN0obrDUw9y3f2K9ks1bHNyaRzk6XQJfAkRIIT1Yc2W5vq0ugS6BLYBMJaCLFpPSl4vC1jMW4hYfJLosWO6VhGw6/qsw9pVXMk9d/K3anKxKNUS+1IE5UOSZbdLOxYwsyPjZo6S0IAPcPuuyd8SqcoqFVj1m9CB+bTehn0JHu3+ueBeuTDFEXq7cMzdEi8bu1nhfpNkrcBpnir9pmBPu/ulh0cfrnxH1Igu7pq3x8N+pHgNe1uH7Y1jnT4mFrm4CdRXYhWqr1RyOC/0JR6JvJxs/8l8rsZNxLMhXCV32oG9Wv8sE3HDd2NSc/NTCTKme9Fb0Xo+OzCqI33iXQJXATEnh6E1x0JroEugQeswTYOGARsTpoksfkmWPDfPvCLeAV25M5mwyfrExwr3SlFvpMjq2ukpcRRDv8sSD/oIvTIfCwZUAX4Tvjtbib9FihF/TEQiQMTh/Kvzq9hUzUpMXjHnpeqtsakpfAtNoMfZU6vIfPwjcM3+pm+spIWH5SnVX1R8jOcLOTTcDJUruo1p9on/lmGlY+m5FsWNCn+c6QjQVTXc7063G+UJz00zUwavdigujdo9/D31IdX4xsOiFdAl0C1ymBvllxnXrrVHcJdAk8SIAF9xYfdmQyzBO6r3Xx3jMTX/IITGZZ4E8DT+8pYxFjsCHMdMIclp0rjbzYqIAfNmCGkwdKrw7ITkjgm8VBS1iix6RefMM8RQ8XpabDa9RbiyyB3VzPK3Q7ol14XumCvrUhazNq47kuTkCFNoB9EuwJ/P3d/atffJF8CGvrD4guJ7G5TcCa5LRrnxf+pG9WmdOtYv7ph9f22LSw/h1KntdHRvrV/XNdfHiXzSsW+Vwnf28bnTUwVLuUcGk6vhS5dDq6BLoErlQCz66U7k52l0CXQJcAk0pbhAynHpaIRXiYDHN0ls0Kw8nklid/BCaxPL1zC3sPY68ZUM7rBUyS3eaEykkzeU4+sVP54cHTxeTbPjS56UZFwBD6QF72lDMomie9PClo1WNJL7Qf6sAd+Q70chV6m0ssn7Oznpt0m6AUG+RaHGpsRjBsOn5SI6EN0DfvdP04adz6/ZC9tv6A6AIS4gW+9+z7TXYhekze2T4vuBrfzHdLzNeYT5hK3dob8oUbf+18Npm+LRb7w6txNTDUvYQgWi9Kx5cgk05Dl0CXwPVL4Nn1s9A56BLoEnjEEmByxqYBi49k8JNQNh+A58QEE9qPiu29db5jwESeeAgqp85JMR954wN7rp6yPtdl37SgnPfZ7encR1/+WvGlBd7HL8prA6J5gtlysqJKj1O6JPOsXgTPZhP/FIFO+MvKk9JsorigdFZvKmehlLMbj+nioj313KrbvYRTazPo22wAWr7UNbzmRYYPbGjEFs5r6xv+c8d72gS8tdpFrf6yvlnt4pPx6Wwy4JdfKz1sQOjeQkq/rtzXR0YE93edyvvp/vb+twYmhD9D+tJ0fAYR9Ca7BLoEbk0CT969e8duM4MBR+HCpw+3xmvnp0ugS+DGJCCfxRM1JqrDxsGNsbgJO8EkmwUCT5qZzH9SvtuM2aSRAInw0g6v5vxO6exGEtUE0/WIIFYGyZEFGwuW3fSsNpp0G2NJODjhQr+1zcIYWDZPdbvNZCV0Xyg57W4TtKR2muyi669CeZUgl6rjSvI7WJdAl0CXwEwC3q/x711Pns1Ke0aXQJdAl8D1SIDTECy+e8hIQM6eI9KcQvhNMUecFy8SM82ERaYTTiawMVIKXY8lCVWUH6TnVt1WUL4IpNtMhdgOsgkoabWLrr8K/dWAXLCOa8jvMF0CXQJdAlkJ9M2KrHh6YZdAl8CFS+CF6OsnwiqUpAktGweEvb5TcY/9/vfO36CfmtD1WCOlCpiUnpXPKUr+UpYTNXbcvQLjDKRVtzMEG2V0m6kUZMomKqvXgrXaRddfrWQr4FI63rDfQ0Wrjiso7yBdAl0CXQJ5CfTNirx8emmXQJfABhLQhOm50PxdF3Ft+Eb1Sk/lwWdP9KJ4hYPTBGcPouNJiogd5RM2yWL1pLZKMg3rLE1ndRJBejV6jNA+yrpUPaN3XWzsrd3cq9at2uOjtbweMA0sVE8qj72GBJ3Dd0WmFYP7q7EZ8fMY+n61XXgdXo3+ApuLJnP6pYLK4XWP8S+kJ+rf1fZW/Z62WnUc0tfTXQJdAl0CiyTQNysWia1X6hLoEmiRgCZMd4Lf47sS4HULnxQ9aju5UEjVOTp/R/mErPBhwbUL1RBfLm06qZ3c3oQecwKh7AL0zMbBVyU6C+XVuhW/sc0I5LD6mxWi8SZs5gJsoqDu6uJqu/AYb0J/NdK5AB1v0e9htVXHNeLpMF0CXQJdAlkJ9M2KrHh6YZdAl0CXQFkCmozyscCjNgLKBMUhvlD2P2NFov258t/q4ov+pPnnDD5stJQncBBYkPRwrASiepYuyUcvr5Rm8cLmFf+c0KqjrlsJzoLk1/v+vTC6XZhRnCfeu9/DVdfxeXTbW+0SeNQS6JsVj1r9nfkugauXAItpm0AlmWFBoUKe8vIPFQTueXd/+td09tekwNypnA9TuqA0X9WnLRbyxPy9nS3m/0tpcHLs3fKUdE/ToxsErvDYn5dq7v20SdENL/wj1Nfwo4tJL/fwsjS88BVrT1ZU6RGcnl7+FvWPSs9O6ygPHRI+6vpM9/x9qQtKoyMW6tBFmgU7HxwddKR0Us++ftGOhPOcIapnEQTfyJkPrWLbb5RGVtHTD8pPhVbdpvCsza+ymVqdCa73/XV9v9UuWvRX6rP4sJxPSJbX2EcNzFpj3qD+3v0eElt1vAFbHUWXQJfAY5fA08cugM5/l0CXwFVL4GdRzyStFFiYsghls4JFOH/VPN2oYIH+Qfn8UwYfoRwW68pjYfc3ynSx+OUaypW2RTB/pwgeu1oXgqq6fRDN0MeEfViUB62wSIM3Fg8WWMyG95Z/Uj4nLsCVC7QHjrscUFBWpUfh+0J1bDNhRoPKKfuomM0j9PhXxbZBRXPw6nTvy2mXd8ldUF6NnrN2ZLjOEYv+nJ75qCYbbKYT4lHfUVkoqxQLrbpN4VmbX2UzagR6szoT373vP2gj2vcrbKPVLmr1V+qzJZ+QLa+xj0qYBwkenJJuVvV7yBWOPfz6wZLozXUJdAncogT6yYpb1GrnqUvg8UiAxfdzTbS4bBGW4v4rwcQW6yflMyH+xcqJdYX/mECaum4BrzIm9PaUifY4kTD6NobumfxdxGaF6GPCfhI9sX8C4Ylk+EFDnmLG4EABjhqeOPGQxOEQjX+q9Ki2gUM3fxhXH+7Q4/BNBsGxCcOGhR3Vfz9A3ic4JfMpyCvpGdCkHQV4zpXM6ZmNieGUidLoaLQhJTmFNp/ioVW3KTxr86tsxjeS1Jl47n3/QRPJvl9hG612Uau/bJ8VXVmfUCov2ceDaG6338Oj5LSHXw/E15NdAl0CXQLLJNA3K5bJrdfqEugSuAAJaILFYtSeEBcXx4JlMv5cl9UzLnjyyr+P8ISKBR/lIT6eOLPodScrFAMfnqxgwTMElXMfLgyHsjMlWISOTpJAh+hEFlzhohXYv/gyYJAvMTwTfq90aWLLwjiUj6uY+hE+0wf1QrmnqszyhcOeLoa8AAf96JQNJRY2YWDTI9RdSc+urvCk7CjEfY50VM+eEDb0Qv7ZpHpNmfKRA6/EcCqFEym50KTbHKI1ZaKzyWYEn9JZ7/sPipj1/QbbaLKLWv0JLrRZKJ322QfqV6Qy9jFgrYEZgI9NLOr3kCiedvPrx4qgt9Yl0CVwqxJ4equMdb66BLoEHo0EfhSnTNZK4a0AWMiyGP5BkzQmvUzWbMEODtKUc1zeJnHAsIBj8+GN0vwVKq8ShN+zGBbIygcvGxtuka/0WQJ06PqLb5yFxIcpIZ7GgU7ds6hnUQc/LGZdUD4bAcgFWYMrGQSLDMEDbEuo1WMKJ+3GwidlvggLRCN65Og/p19CPWb17HFE7SjEf2Ra9Bf17Olhs8bJSDG2zUmicAOLY/mf52j39ZfodooWm+NaG2ptJqozzw8y6X0/0fe9grK2scIuavV3UhvRPrvWgHz9qH1McNfATKrsdyt5rO73wnGEX99PCB1zl0CXwKOQwLNHwWVnskugS+CWJfAnMcd3B5InGTQpY6HN5YLuOVrMYpVXN2wh+6vy3VM8xeD6N/V02UcnefLMUWcmrUyceVI9OmFAnsr48GPN5olAdw2cGAgXqOHCNGyYV0D4xgPyYGEP79CPPNyCUrHbjFHMIneQo9KxwCbHT1Y3BpDIK+oxUa+UjX7RyxBEGydk2KTgBMmJewoVsxBP6lnlOTsCxTlCi57ZhOMfX+B1sFGl0RenSpJ9yDO2VLe++n2ktko2NILP3BRtxrc1tKf73vcfBFrT92tsY6ldFPVnpEpv0T5r5Uvjgn04tDUwS9tfUW+Lfn+EX1/BYq/aJdAl0CVwOvWTFd0KugS6BK5aAppIssHApoI7KRFjJlJmk7RXKnNp1fvF6irPLdJ1zykDAicxeE2E7yUwwWeh963SLG7DwKTdbXiEmWdKM5llAUoMzdEgHpAdGyz8SwQLE3vVZThxEFSEb3DmAgve0qJ3Vl/tFvU4qzTOMJ2Nc+evubhytQc8dLKANz1m9Sy4qY0NdjRt9MD7Wj1ju+gZ/brNGaNR92zm8F2P3PdAAF+kW2tn6xh6hbP3/blga22i2PcrbWORXdToL2RN8LE+G4I0p4Wz2KdrYJobXl+hVsfJfh+QsJtfD9royS6BLoEugUUS6CcrFomtV+oS6BK4MAm8Fj2crkidHuAJOt9asI0EnrYTbKOC2PJcgf/hZAJHZT+Fmcpjks9injLDCQgnLXhaePbg6duaji/gPYVUZZy84NUKk2sKNJVf0mOq3ok2dbGYmeqEOkzYWZD/S1f4sUXgCS993ZKeS3Z0j+3AX9Ed21RqogDedSG/N6oYxaeytbptoqkBuGQzJZ31vp8Rdsk2NrCLpP6EO9tnRXboezNcZItK9kHlGphsI1sXSjbRfrqwnb39+kKyerUugS6BLoF+sqLbQJdAl8ANSIAJtdh4r5inTbHAxC5cQPM0jVMElke94fSB8nnSzuKNTQm3mFHMxDkMLIqnC3d7Qh/CXXVafPPKC+9HI7MpvwNvKkcenD4ZPbUfACoSqlvSYwkLR/ztNMxJ+Eg7PXvcbEaYzsFFOW3+qPIaPZfsCJxXGcT/17o4dYE8RkF5q3U7Qrjhjae39/0NZTpFJRlHbWMLu8jpz5cl++yUzoX3NX26BmZh8+epJtke5tfPw2FvtUugS+BWJNBPVjRqksFZVzjZbcTQwa9FAmt1vbb+tcjpUuiUvFmUvtDFqx3TRTXHlN8q/6Piz6BZ6XBzglcgmLyxaQEMHxrk+xQWgB3e91caHHznYbqwwzf8ovxb8hPw9J2uT+Jr9I0O5YUBGQ8yDQta0mojqUfkKlzQwCYDMnb6UmzfnGCxjZ5CPfLk1gL0mR2Q96UuTtyYHkt6ztoRCG80bKLbvWQj/SVtRm1mdaa6m/b9vXhsxSu+Vvmgyvqb2EVBf9k+C52STc4nZMtL9uHlnrWhVt1sBV+po1Rzh/r1FBE9v0vgGiWwsu+dSvVL5dcoszU0P3n37h1PAvmwGl+332QRLjwcF3VPJVuJU93nqvPW12OQIbxWvptMlsoBFgwTVYJbmOiegSYaVPYPXcOiRGkb2Oy9bO6ZpLvj5Yo54k0e8UheKhuOJCptk2WBnThiy858D5USQM66cgujSkzOHqL2KPzokUUPT25Is3DhCZ3TIzT4/Kiu19YX7psOyE/XJjrcS1CiL2obpfZUr+SnVtkO7fs2+AYG3xkYfJTRpjyO7LNpEvVzvv5bD499EwZfen/bf0sSkBw3s2PharI3wUfHEeWjT/pWdJyCJ1+XZM4+kvZFxVsPktFmut1LVqIxajPK7+PXXkIX3i1tI6PD7DgCe6qb9PPQKBDsIDpHoX4YBD+a74ZlpEvlU/hrvkd2ujaZnwhPtI9es3w67XkJYD+CSPY9lWfH6Ir6WfxQJxxJ31BZXhpDiv6JdizAk65N+hQ4hYt+Bc4nT62RrWIh5agwT6qmTzZrm+CpGE8sudhRZyHJZoqFbLnqwBz/FU99nrbxF4I2oTMcLlY+ip4e20Z54KAOxsImTvgevCmXvwSELrsGBQmevA+KaR85gKeHNgmg56jeWtAIR84eWQg4/Xpd8fdsfPfAQknXa+tbO7cab6LDvYRTsI1Ss1k/pMqrbEe04ZfwQwwWXKOgcvzPZ4rNz/3s80K4Eo0hbE+nJbCJHUs/OV80a13wuXEkO06pbnYcVHnWvmbE3G7GJrrdSzwFm1k7/qytvxfbl4J3E9so6VDlyfmuykp+vjTODLIUrth8t7p8ALydxBH6vR1pdU6mEij1vewYLWQ19XmYGl1rlnxDqdwzUxoD6CNJ/zQViO436VMRvNv+G4iYcrswioeFe6zRQt73qo+CLCBMjjPapkKpHPhho0T1SL9SjGEMwbcxOhkxFN5/gO2JYFjITk9lcGKEsuFSPY6ROp4V0z7HwO3pPPHXAe6erJCA5Idu+KgVA+yioLole3wvxB8C5DylZnPMQlbXAlpb39q5yXgLHe4lmArbKDVd8kOrbEf08UFINjtTPoqFb2i7+Dm+KxFubJRoLPHYyyUByfQIXzSStdqsGUe+ElxqnKJ+chxUvZJ9jei51ZstdLuXbERbH7/2Em4F3i1so0KHJR9d8vOlccZxKjqYU6fGklOpvEJcVwcing/361cnpE5wTgI1fS83Rpfql8pLvqFUDm+lNUzJP43ks0WfGiEMbp4G6S2S7ACtPUXAon/4C8EIUclyCYoNCQb4qVO+U55tdpwEBwz3w2RO6VEQDBsc08k/MEwChyAY7sMNDZ5oschmg8XVV5xsZ0B0wQnR/6uuQX5Hkao2eXWGI/Doa0nI2qPwMmF3m0oeOZ071G+YPgl2pOu19ZcwdG11JKO1OtyL5axtVDSa9EO+7lrbSZIgmdrGK37NBeVZ+qXlKS7RGIBeflI8nsUPIRm1vdaOW+2tahwRXbNxSnlV4+Dla/wYCjfQ7V6EZm1GdPfxay/Je7wb2EZWh2om6aN9P4YS8+0n5Vna/Hx2nKGy6jxXlJzvlsrBcatBvB/t129VlI+Rr2LfQyiysdkY7YVVqp8sF87sHLBUbsoSXGkMSfonwzGNhXNtn5qidPfPorkLMr1wXipedYrAMxpSgLDYYbKTCggiDEO5YFILap6WvwgqsVvEh9hw4rHwVplsQFDvB8F90GXfrBg2QpTH4pbXTNwAohh8XMjggy42KTgWw3uCU7pVdPlBdHOygY5Bx1ml24Xcsvn1gy5eCaoOohuaq+zR8/id4Hk3atCT0kldh4SsrR/iOmdafCBrZ8uK+XaHpdeStUiHaxtN1Rdf1baRwTHYiYcZ/BD3amOV7aTaNdxeN/Dh2tG9+T7yXFBelkaDu4ZYvJzbDyGmRXYs2pvsTfC148hb0RQbp6gfC9NxMAZzFXmS0da+apFu9xJWi80Ilr7Rx6/tbcLUu8g2anQomKyPVjljcNLPq7xmnCnNd0vlJoezx+J3634PT7vpdw+B7SSDPUitwnmt/FT2vbcSQmyMPpXq58op05X0DSrjX+yS5VPFCDY1hmT90xRPcL+oTwX1Z8mns5zlGShkythybKopATIBZ0Ng9nE5EJfKgfGBjQo3gVMd8IXfoDAYF6scJfP3e2YM71XA7vgoqBx8PPUPT03YhghPANmxwliQC4vgYRExQnT5N3x0kgGR3UFbEB1JNTYVO+FSoqHaHsUXx+2/0sXfs9FpR0F5MV0PMGvrD4jOmBAPbEZhv2yy8VQ3fBVLt6vCUh2uajRTudo2MjiGIsmOfhH1U2ttZ2hknmDzjncJn/s2XnoQFqSzkKNxBnyZGef2Q0hlqR232ltxHJE+q8apiSrB68bBSf5V3Yr3PXzVUt3uJbtqm5E8+vi1j02YbpfaRrUOaUh6jI0jVX5edaNzFOWX5rvZchPAJcTiZY9+D2uH6HcLGe4ogy3Ia8ZxC/yIh1TfqxqjU/VNmJnykm8olVsTJ7WRHUMAFEzMPw04JomlfWqC5uF2y80KFjirP4hopEkwLO5xTuHfylkxgouV3w0A4wTGxOYDdfhrw2E3egzmFILzDoM9uZwu3r4V0D9DwADv8BqL8oymaf2w6kWmRTsLd3bIGHQJ6OPQ4OWHnJF3S2iyR98OfHIShk4Zhpmuw0LSa+tP8Z3hHnl90MWCBvsNN+F0uzx42SzR4ahR4XmlCzrXhibbyDUmemJ+KKyy1nZCXENa7aIfBiP8Cq+cMTgQRj6JjAoaAbvYIPrP7ocQjujAly+x4yZ7Uzs2PiXHEcHkxikbc6Y6dePgNPMK7zf3VSt0OxKf8JzFR3n6+/h1WeNXdb+X/qLjiPJr/fxsnPE4k/PdUvnIsC/jZvN+D1uSwyF+fSMR7iKDjWhbguYs/EjnW/lpeJ71PTLVRm6MBsRCtL4VKo6WC3/WN5TKA/wuKXj6QXQMUVnUP01x2L3HtWSuZChm8bNZzoIMEWaLu2FytQDNUMULhqeG7rUDf39SbBsHCC5aLhgETvl00s49kzU+mmmLbu7Byz1f0/9JMd+bYIPE6rN4I9gE8v7u/l1DFvLTAJzVCcum9cOyS01/KTmw43ZSDP108C90mWyOohu7YmFmC7Jsu9DoAZL2KBh0/y9dfADH+MF2CC91WR73HPEf6XptfZBeShAvLHiRhx0d22yjIuCxSYdBvTAJjVyLg3gt2kYtcuFK+qEAx1rbCVA9JD0fbMDis06K0SH3Iz+j+xoaHxBfZupS/BDSabJjyX+pvZXGkeQ4hQ3owpelxsHL1HIFVeJrT1/VpNsEuYf4KMmBdvr4JSHsbBOm5ibbEE3V/V6wSR/t8RT9vIicjTPKw0aS812V4WOS5WrbjS2COXsQLXv2e/jbTb9bCe8AGWxFahWeM/Oz2k8HTMb6HsXJMTqoSzJV38Ci5ZIfPibpGyrKq8YQ4Un6JyMwETf1qQSOIfvZkFqXsIny3To0buBBMO5pvhc2KFGWe7rvBZcsF9x7XdDjFpuCJ/2TYpvED4tQj4udvfD9fBbEBqukO94d1iePYIPR/d3DLxsfLKzdgk9tmEHtsQB8aHXjlOh+I5ThAh2+uH+rC/6ODL+qMXYXa0PRHsXfna5PQhjqmnrY8I+Thma6Xlt/gv/ct2wK2gJnL1padbgXHUXbqGlY+s/6qQDHWtsJUI2S9EdeT7MNPPM7A1ADjUOdS0uIh0vyQ4in1Y6X2pvpMzWOlMap0jh4aaqupWdPX9Wq21qaW+GKNrN2/Flbv5WhneH3tAkjvdU2iu0U/fUAACAASURBVDoEsfRQGkeKft4TGBtnmOuW5rulco/+7NHeOt5FvxtLbW8ZbExuEd2t8DPre57z0hhtAkrVL5WXfEO2vGYMqPBPRmMsbu1TMRxD3rMhtS7xpaqv3qjwJPDf8uz4EA9BQmPDgpAtFxwfzuQoP4r6qOtzXa91jYLK2aSgsxCA50OZ7CSzKfJWaeryV5YnpWOLcxa57ByNgmD5G9M3usL2o9/cGFW8vJvhaSakeb6QDd+P4Nh5uMjfm3oGVPduvtqtsbNae0Svpmt4oF7staOorgW7tj5tni1IltYHmFh90j2LX2Lra1vS1qrDLdsOcdXaRlgnls76oaDCItuRDpjEogd0Q39z/kSxO+mkPO7JR4fOxyk9TDyVR6il8R76Mn8vyQ8hoVY7XmRv0mVpHMmOU9iJruQ4qLKSfV2UNYjeI3xVq273klGtzawdf9bW34v/KrwH2YTR0mobtTos+egaPw+NqXHG0R/IivtwvltV7oDO8BPQvfccZS/9rpbagTJYTWsNglvjRzyn+l52jA5klapvIKnykm8olYO/NAaU/JPRGItb+1QMx5D35N27d+zqQBDHwRBKc1A9960Kxbb4b8bRK1yOBLwz4Un76DSIz+d0BSdNMPJoUBmbTcl3JWOVVCf5egllqoONhq/nxNC4PMF3e0xKZ14gef2mXF6rsoXwHGhlTqsOY80JB+8AskBfTKfqdtuICfcC86QrFqgX44cQkWjqvuiMtiL57+arWnUbE4NwdB8VE8yOeXvahJHdahuC7+OMCW+DeG8dX4N+95bBBmpqQnFOftT2aj/dxOwjBG7tUzERCQdzQP6g4snTGMCCvBeqU/PEewHqXuUMEvhGxjHaqIAG5XGsCT270xXkJQKviuAMWgLvd7EQiAWzLeysJnR7rJGSYCRznrASZvq+z97st1WHmzU8QdRtYyKQC769ND+EqFrtuNvbRgaW8lWMG7r4e3C3QFzRXKtuVzSVrdptJiueh8KUTTxAbJZqtY2uw41En9Kx8rfq91B60fpNyWAjER+OJsXPxjo9nK/e4EgCrX1qVHl6w2sgnKbguPGnaWHD/fNSfRkhT0R6qJCAZPUkB6Zy5P13XcS1gYk/x3KyQTDsZHF8KBU42sTpCmCipyuEA5imoDocZU+FVtu8GnsU32fTtRf2F8Sio2gbKeVU5lfrULRgXxz7nAYmgNAae02FvwqO2uMEydXYxoTus9xKpkn7VNlj80PooNqOvcJuxt7OZQuB4Ud9leii7zOPWXQyNMBfrVu1132UBCc5nMU/BDqL2kRQvlWy2jZ8g73fpyVfNRcNqkd1LNvbqt/T1Kb6FW1bj41RGQQy2iy5A+0x2qL8bKzTk/Dt4qeFt69nvVYli9QY0NqnYnbCQ1Q332ezgierKJTMO11LAvVe5CpmGMpV62URCUiWyHuv72AwkCRf51EZ71KzUXHktyvMtmqN/2bscWddY11f6lo7yQdPKVTrUDzHNiNOyt/i6N7N2EZJ4HuX72ybl+iHEGm1HXv5Pwp729kWzJRzvorNza8McGFcrVvx231UQcgXYBMFCpuKq23DY+39vkm8WeC9+z2Nb6rfHWw/J4Os8FoLd6A9RkKOny18uWtzLz8tvKkFeozXx5rX2qdicsIW2J/4M5sVPWwoARnx0R+f3Ix60e7eD6pAGD1dofoY1he6vlT6mxIewTwXDG1yqsI+cBqrBhyBCcDVBPF3DbaAvv4ZE6rXz1uV8VVfdMAHZ3l/bMnmxlXqUPz2cLAEZF+X6oeQRLfjg+0haC7qq2Qv5KOXV0ozBjERfq30neKW0HUbSEvy6+PXgzy6bTzI4ujU3v0efi5dv1EZQLj6KbRvNU8D5REhyo942cqXH8FDbyMvgU371FabFSxejLAk+Qx+KmQywRNy0kwq+NtQt1gKOp2yXTnxMOmoqA9OnnjYu6vc8+8G/MvHLCif91yzJxRSMMrndMFHj5S/wbS/EORDhbTLbtBoUad847OJTt/GEVH2aaYRAK+6RqcrdI/+eYeQr9D/xr2uO6uTiPkq9R918cQcZxvVk/Jf+PrYTU1osceivYi+lK5PKmNhBe8s5InhyfRetAXBnzu8FAHvp0SIB3jho6Zfw48uBhHusesloVWHS9qoqdNiG7v5qimhku/MF3kd8Je99JGZn1Ief+uJ3eGHPtN99PUr5efstwqH8B8ZLtUPIYNWO66yNxBLT/S5nL7RI2Gmb9VlTEnaK5UEk/RVvn7RF4LnjCHqq0QPfCNnxiXGYmwaWcFPS2jVbQvuFtgqm6nVmeBy/T9pEyK4j18PWmu1jRYdlvptyS8ky0s2Uip/YP+sqb37Pcztot8NpRaVgfS39TxtQ5KzqKL8qMZWvjzb+BaFNX1HMNn5lcpLY3p2TC7hD/kU7GyOSXkOh8rWrFVb+1RI7iz9bJazLONnVWOxWQoohoWPW9h7IfHthd/5im7xakhUzsKIBZJ9z6BUH8Ey+GIgDBb8a4VtIuj2Ifi2v3jImadSMMqHJjZReGcOHNxbOzZppNOFgXKbPFXTGSLYMy0+kNsLxdZ5Ss2xcYCjBJ5TFBgmk8U/KEbHd4qTQeXUtcUVm1azv4ENKiMvJqFZnAF8rT0W9aA2k7pWGXaGjWFrJ8XwxN9/2ms0NbZA1bME0Qt90Ow20SZEoNe/GW++DB04XkNY5XEqxngOi8J0qw7Duluma22j5GvW+qqBJ8kOOxr5IuVxbz4EHY2CyrEz+pnrQ4p5LYuP1NIXh6D7nP1W4RiQHZAQvZfsh5BAqx1X2Zv4LukbuXwUnPsnHMWvdIX9Lmuvgq3xVVVj5wFmMGtC9Od8Fb6H/mjjAzGT4SFMZDXkTxKtup1U3+y2ymbUGvRmdSa+c/2/xibwQeaHjMFwLmN5h8cFmzj3+FWrw1K/LfmFbLmUUrKRUvnheg0bLOi42O/BJRysI9h4M/8QNmHp1r5fq1/DvzguyGBrO19MZ23FAj9Fnap+OO7VNrsHXLbviM6/qNHkHE3lpTF9Ff6QYbU1m2NSXqJRIFkawjYi6dY+FUHxkPXsIbkqxWKHJ+lcOYfwftIKTwXDp+XfIzxd9s8EdETyeGJPG6X6oP/Kw5KOBpUz+M4WXSFwCkb50PSLtUGsK1yoYZyj95l0z9F526iwZop0GuBBMYsejIvBryWwSELvtmCHz+LTd8GHdoI+cnV4qmw2UUNbrT2CK6kH0VjSNXqnLeOdxfwLkPpQawsGf3TsdC2aY7L9VsSEC190FIM7qX5o/ykeWnWYwrM2v9Y2Sr5mC1+F7KK+SPnQiW9h8y8WyEemFtANvnPwwUqX7LeIw5AfGF+yH0IMrXZcZW8V+kaXwzcZBM9GIpM2O6pfsteSr4K3pC+k8Mwh56vYmLCNb8hER6PxXXK6RR8Fr0mdiedS/y/ZRB+/kPB92KXfC3W230qH2XGgVO5pT9pIZbkHO0u0qt9DsWTEnLQU9tJvqd2a8pwMtp6n1dCzFibHz1a+fC2NtfVzfas0vyqN6dCwBr/jQfYfnWN6Bks0lmjwaKJRa5+KIrHMZ5ZYE0sYTJzsaUZ0QQN+weB4w4CgUJgFnEryCXtFfYdHcCjnuS6jy+XzozLy6Sx2EoLsUSjAsBvGMWVb2NNGyHPIz0ll3IcTqaEtlSXpHIAOSogWO72yuEXhQLbwhHxsg6kGH/oIZTitgwPLbWaM4NW26Z16ObyunuBTeijpmteNWDDw6gs798CHdFbbgiPk+B8mq7NXb8QHeuQKJ/zAusWw4pNg2Jih/3IqZnjiS1kiNOkwgWN1tmiusg3B7e6r1EbRF8UYVj18D+HuPhr0wW1o80n7bcBhTRwSi65L9kMm37CPZ+UifqrsLYfE62raH6mC/vGdLCpL9lryVeA7CU/KF7ryM/5EfZWnhw26kH8m8K8pU/7N+ijPOzymdJbs/75uySb6+GVCvverm/d76S60W1rDXkdyfyBheSpjIw5pqXx5y6trLur3tCqesH/C75UubVg0zU+Eb7Vfvyet6jcqA9HAmDAdF4BdM0+rImglUJQfj3MrX76SxPrq0sPM/yovO0dTOXPrqe5odBjTjYIl+FXXrXtUlzai690SjYYDOmI0kF8ITX2qgOv0tATQUP6jYDHCYhDjb3RxPJETB8OmAWldKMsCDmY2ERNMtL6v9JY6ulDWD4LF+Yfhe+W5o7Rh5iQdhVE9FM8Fn8S0wfFTc4onpYcFntK0zWI25ElZLpToNLhrium0PA2G32Fw0D0OKDoAK5+OxMJ3kFvIMHV1Dwz21RJq7TGqB98ubed0jR2xEYU98ldGnysO7XngSfk5W1DVYwJ06OJ4GgFn8sGlgh+Voz8uF3SP/NEt/LAQCAPHIbMLTNVfqsOwHdIjuqaFDfe1tnES7VFfo/wtfFXUz5T4UNvoAVnYgAid6Ijg8nSPzLmi9luDA2RXGjb3Q8jBy3RPX5QSN3qMhU/KfBEWiMaUvWZ9lccR9YUh/iPT4qXoqzw9zBGcjBQzFnPyMdyEvWUfFdWZl0ey/yM3wWRtQuV9/LqXE3Lctd9L1tF+i542CFEbCfCWygPQ/ZOSxep+LxyMg8zPGeuZ5ySDYHfXb7LxREGNDARzp+pcLugeG108T/Nodolq+PENr/bllQyMZFdZJwYW7TvitzRHw+ZiYTqmL8VvuJNzzAoaDUeUBiuMxcINf0t8Zgydy3uWLGkv+JOq8P2J6CmCEJ0Y4Uk0izp2AE/ch+WklQejLPA4SjIKwOua1VcezonLBd2/V4JNEfdahu7BF05iHFz4U4B54WF/FZzbEVcMv/9WzE5rOLijLD6MN9vAAVZlSTp9G9cYwdN34u+N4nBzgoGDTvOzrqn8ca6DLJSeBhbHfBcC59ISivYonDk9FHWt+tgoJwuwUTo0Ew42ZoaNGuWdyFMUtQXKDw7oJRwQpvowcngFhNMi9B8cKHaOLWP7TheK0QtP50p9fqkOhfohqK2cnTwAllNF2zAUajPqa6ycWDBLfFXRF4VtRNKmn198mU3I0BWhaL+CKeFwiK7wZw8/hBiW2nG1vTXKGh3jW4aQsldvo0lfpfKcLxzwH5xo8VU8NOBfi06KhzFX6Zv1UeItp7Ni/1d9/FbSJkzXguvj105zkEDGxXHGYFvigo2cSuUtbW0Iu0W/d3Nx8cfmZWnecGl+HVG2yGCredqGKpyhauFnrS+fNT7N8HY/zW66r+g7S+ZXw5i+Fr/q18wxszRW0JCS2dI+lcK33ckKMcXinQU7AioGwbHgYZGDYTJoDkH3LG4xbo5vuYXRUOgTsfrKm7ZtDuuVx8kHJIcNhQhO2k3CBHVtgXBSntHHojsMKMttaISZpFUnSecU9prukYUuXgFh4B3krDSnLewjqlOWvlMGC95UwEZKi+FZXdpUZtYeBZPUg8qM/pyuObkDv/BHp2eS/K3SI3smT1fUFpR/dKBfIW9iaI4G8YDs2GDhBAETfnTKoBieHGESyzvzuW8rgH+RDqOEbZAJvUKTtY2wGcFv6quEL+tnwrZTaeFgAob+8DvowPTi7Ez3Rfst4Ui1fen54msPPwTbi+xY9DTZW0S+NsZMi+h/puehDP51A63h2Jr1VaqT9IUD4uMTtb4K/4OvwkeNHnzoHhndpI8Sb0mdqczsoo9fZxq/pIOmfi/4WL9d1etyNgLiUvmqxpdXXt3vg6aZk+Xml4Cey68HZM6StTLYcp42I2LDjFp+tvDlG5KdRlXqOyrPzdHo67HAeOV89xr8qls1xyzQeCrREGPA5y3qUxl8p2e5wgVlr1WH0xU/TeuKaZTwL13hB0NMYS+Vb5NshMyiyD0dUcw94ZOuUn1OarDB4XAJnl0qAsqnfY7p02kI3J/8vT3xr4EBl+EFhQWbHNg9T9d5ohYLOTpj8FefJzkPJyiU5mk9xoxOw4XWiE/BsSvOq0JT2Y7gMjdJe/R1SnpI6lo0YZfQPwTlMXCwaKTMbJDynC1Qfljw9G3SnnC513cUvxFCWyyPcKtsrQ5H+Da8SdqGaMYPlHzNSXBLfRULiJIvyrKqttkQ44SM87WK6V/ch30lab8gF2wNDkBvJng5uSdtSlf5IZgX7Fo7TtpbSbhqG73eCW7qV6jK5C5rr75uyVeVfGGJzM3LRXfUp7Q0BO+6kN9N+Sgvg5LOkv1f8ujj1zG2kez30kG230rH4RyixexD2JKNlMpDXIekJZfV/T4glG+nJU9WqOxsfj2gcZbcUgbCVfSBMwI2ztiCn0vgYyKWbN8Rvdn5FfwIX3RM9+0sxu/bLs4xSzSKjiwNE3m4W+Fc26diaLfdrED4ut7r4okOi9Eh+DImTOFkmgk2CuO9spNgUBwLfDYrUDSBhR734M7WFxxOLsTPkweeClve4PyVR1sIFXqh4aSY8iyMytns4ImmTXjNIKcO0egX6CyU6JxVuIEMNiVMRizWkA/fOviPGG+CRT+cWvg6Vl6Tp7pJe/T1S3rI6lr4OYXznHYCeqD7fXBPMmcLE9DruhXvSf2obLUO95IGOtN1Fl9F2+Kr5GdKrGObfHvEJnZmq2E9y0v5qhocIb5bSDf5IRiWvlbbMTrXFbW3SqHiUxgvnd0IF+lhbNP9J93bOKekg3Vjq2+75KtKvhCcVxnE/835KK+Iks6y/V9yKdmE6buPXyaJxtj3vWi/92XJftvYVAq8ZCOl8hTei82XXNmYNF9oc84ZvYK7BL8+o2uPDPGa9IF7tLcXzgvjo9R3SvOr7JguGS7GLzkxT3BzBXShe2x9tN4lX6FEY4mGeyz+17ezat02QhjcPHn37h0DEU+Y2IWxDh6AtCeFB6HwNGPkKHRPW9/p+uixfqmYjQjXruJ/6/65Lxsi5ds3J0r1qftWF/g/A4HqjjZNfB700XnZzEAZfARzOA2iNIplMhiFUTnOEPy0w4LbbaYoHoJgeH/WvSIwZPqEyqronNZ7TPeSkW1aMeFeFYQrZY9FPahuUtcqw06wL/eutGJsYnYSRHBJWxD8zQbxvZkO9xKSaEzZRsnXrPJVxo9vf+ZnlI9tsVGLH4IWjrcP/7qicvKBIeCDPihvGJxcrn6Ul7PfKhyG67HGkuFmdixcKXvL6hvZqy4TC8JTXf9P1zDuqKxkr+BP+irVL/pC1b+5IL430+1ewhGNKZuZ6oyNc3zGEHSf6/9Tm8CP8KBpNA/UfR+/BokuS0iGKR3W9NtwHGC+ynej3OtOirN+Q+VTGzkpb5gTl8qXcXveWuKJef13uj4pPeoPIWUq26zvC1dUv2F7PX1bEpDOS32rOL8SDhvTZ2vJLfAjceHBNmdzTF+WpbFEAzjCIPjN+hR4Pe2sqZ6s2qzwiGabEiHxsbTqmZIpxtkSXiv/jkSp3MOESv5MdQYHTHkYVPYPXXwE0QWlzcHbu2zc49jsSDUCJ494OnCPFgSqAx22+cLTMwaTHiolIHlhiMkBpRKNAxOe5IChMmzuW11/VHqwBSr6srekFWb2eJ/t4JK6Fo5qezR8txSL/830uJdcRGPSPnJtluwD3lU/6S9UThmDwicPxyYtT9sGX+LbiNqnYE8qDxcdI3/n6xbtFzw95CUgWW5mx8IVtbcafQkmp++svU05FK7R+NdaPoW/5nvJYjP97iUH0Ziym6wfgTfRtNgPlervxe+l4N3SNjI6zM59kYXq9r6/g1Ecod8dyO4oL0wCsqOaPpxdDwgHPh48POAknm0SK88Fwc7Gb+Vl8VNRMEk/co/54Xfahu5reGzhYdG4Kzpog7pPnj6Q25ZSZXYv+T7E6PREJRb3mojq8mSIVyqYxP8jqJstVx0Y4Ckj9dlh5mSEbTwEaAaFsXsdBgZ0cFCHAZ5TJcPJCt3bpIBj1tBl12hRrTrkf/A0IAdw9dAmAXQd1V0LGuFI2qPK0L91LDrhNGTtDWDhSOpaZdX2OG34hu430eNe8pCOkvZR0WbJPkr+goHF+RjRgb/irxT/bu0qL2ufKscPuQ0Kq+/zDEWJPoPrcVkCm9ix9JOzt6y+KvRdsreBS+FiwjId/6rLB8DbSWyi373EUbIbtZv0Iyor2UXWD1XU34vtS8G7iW2UdKhy5q3Rua/yS76+pONBlsLV+/4gDZc4Qr/jFvvdLUqgNH5n1wO+X/J9O/fRegmIB+3RtWOsDysvix+BC6bkRwBzIdaGCko84luqeLhvxeFbtc576hE1RWLO7booHi3eG5B8r7o8abTAIMq7xDapKpUDP2ySqB7pV4px5EPwbYxORgyF9x/6fCIYBv/pqQxOi1A2XKrHvyIM/CoNDb8odk9HfcxRmx4aJCC5oR8+4oLxLwqqm7VHdKOLRWLKFrL2prolXVfZ4yLmrqSSZLRaj3uxKtqy9lHRbtY+VL/kL94L5kPQDrvpbNC6IPpK9snCN6yPv+O/6G3jrUTffUP9tyiBLey4wt5K+irpu2Rvjk/RwRib8nmnUnlRWFcIIJ6v2U9l/Qi6Fn/DnIW08sJ5y9r6V6jxepK3sA3hKI01ve/Xq2RTyIP0uynNHdlFSqDUh0vrAdaJw1pVdnmn+xdTTpWfGr9L+EFVmkO45jJtlHis4sF42qLvLdqsEAHs2kR3goy4Qsyin48spkKyXEyjZAaE6SQMhdtmx0lwwHA/bGooPQqCYYMjnPRbOcYwBMFwP93QYHeLRTabLA6H4mRbA7ILTYh23oMc5HckmWqXV2d4PQOdLQl722NS16K5yh6XMHVtdTbQ414s720fWX8hubAZMbzyISYZSEZ1Uox7+6IY/+aC8iz90mcl/aUvv7pIPN6yP0rqq1LfI9tRndn4pLzs+FcqvzqDaSBYvK8dbxpaawLN+inRXfIjWbtYW7+JkysF3sA2sjqUWHrfP6NtHKDfM3LXmz5IAqU+zNibW59ywoC3AZy/Vsz6YrSeVl50/FZ+cb3hYRCFzRNPyrO0zRnJi7ZBRYUkj/fF7q2ELA8ebojU3qpx99mAqTKhBhHWS8WLTxF4osMWEQxPBeyUwvS7D0O5YFILap5UvgiQsjPEMRsUEgtvlckGBPV+ENwHXfbNisHQlMfCAqWYsk9Kg5MLGXzQxSYFx2Z4t2hKu4ouO4hmTjWgVzrPYr2u5JLO+oMuXguqDqJ9V3sU/pKuKY+FqT3GYM6SJ56Q9Z1vnG8nWHoLehbpcYuGYzj2tg/aVBtZf2F0CY5+9p0u3sGr8hPg1oV+sHPXju7NB5J30v0U1+AvKb+2IH5u2h+V9KXykr5r7K00/pXKL8ZsJI89/NXV+infP2Z+RPk1dnFaW/9SDEN87GEXsLfINkRPcS4imKyvVnnv+4GB7aTj3fQbkL5ZcicZbEbfEkTXzJNoT/ZhldncbCqWYT0gGNallLNmZK5jr4OQZyE1Pj83gEkc4i/OGX3dVBsn0ZXkkboqr+FhQqK7XdT3qPk0hq2QxwJ/ykihSrpYTKNcNgRGHz20GqVyg1PMRoVTpOqAL/wGRQDmBM27NvxThyn1vQDYER8FlYOPJ/7TExO0ReDpH087GGCQC4sQt4Cg8IoCH/xjovNK9Kc6297sYFOxUy6ldve2x6W6HuyxxMCR5dIvG1LQxiYbO7ocNdsyLNXjljSEuPa2j6EtyTblLxyMynkV6StdXyvNIFUb2MDjHWe+9k8btjvOADUKKqf/Jv3pCPhybx6NP0roq0rf3hZm45PyS+NftvySzEK87OWvrtZPSSZZP5KyC9Pr2vqG55zxjnYBW0tto2msEQ8xX937vjesHXV8iH636B87ymAL8hbhuCWeEn04JpdhPeDrMMdhzcs69Y3yWMS7oPSS8XnA79Fk/UhLG57e0ZzS5yV58DTEoqV9b9FmBQucVR/KMA7EMAt7JiN8qJMF/ygkymdwvhKTeDYfwMn/hw9PGUZIdaMyBB8GB6v86cLtWwH9MwQkLTjDPbzKojyja4pjWv2i7kU3iyY6CgMtAX0cHrz8kDUybwm72mOFrk3vU5qdPU4zL+AeebFRgXPDfqcbccpaHlbocdSo8LBxBq1rw672MSEu6i9CGC8f+hq76kxWi0Fw6IjBB9/Ca2c4fMLINyk/60/vq1z2r3h4NP4opS/lV+lbmpzZm8eZHP9K5RdoHbv4K8kBv71kvBmJSHjO4qc8/Sk/MrOLEdG6WVt/iu8M97vYBXx42SyxjeqxRm1EfbXye99/MKZddHyEfh9YWJ3aRQarqVqH4Gw8Sfdb+euTcMX6cM16gJP8PCznQTfzOk6zf6v0F7rAmRy/VVaD/yQ8ST9S0YaauQ8eNrZGT/JgdWOx8C0ed5/FEKby1JBNrodFegq2lO+FwNNC99qBvz8pto0DlBYtFwwMUz6arPv754r5aKYturkHL/c/K2Yni29NsEFi9Vm4EWwT4v7u/r2dYcfLMn0MrNULi6Y4wrJLTH8pOfCk5qQY2unMdBqTzZE0Y1d0XluMZduGTg+wtz0mdY3MdOXsMcvDkYWik8Uu/YGTRdCMQ9sjNOkxQQB0ci0O4vEo+zAaef1i5C9EAzz8S9dXSlufQvaEl7osz2XEfjwf2Bm+66QYPXI/+Bqlk/4yhvOC8x6FP8rpS2XYbVbfXn8ze1M+9pYc/8CbK1fbzsYEc/YgWvb2V1fjpySLFj8ys4u19c9uDAEBB9gFrTXZhmiqHmsEm/TVHk/v+xfW91v0G5jqqqTa3Nv/raJvSeUL4Ak/yrUqiI9cH74Tcsqnczs2J8j/FDauPObjrHkoK47Pgk3iN7yCSc4hfFlyjqBym2dGefRt5HiY8m1kWdzkW63SM0tUxjZJRliLg4SBENzTfC84cDHAuqf7pXLBvdcFLU4ogif9k2KbvA/C8rjYyQvfzccwDFZJd2w6rE8ewQag+7vxL5sfLKzdgk/tmHHstQAct77BnWi2p5iGDZ7Qy1td8HZ0+FUN8lSoNhxijyKmpOuSPdbyszccG4NMhFb13woiW/VYLVvTQQAAFIBJREFUgXIRyFH2YcTN/AWy1oVjD/0NdKGDH61iIcb+eE3NNvHMHl014c/60wLuiykWH4/CH1XoK6vvQGExe2PsK41/pfKgibMm9/ZXV+OnZDMtfiRmF6vqn9UK5o3vbRe02GobVWNN7/tzZSZy9tbxLvpN8LI0e28ZLKVrTb2r56miD2fXA6rPyQle6Q3n4czhbI1aGp+z+L1yknMItVucIwgmOaeEbl1JHiqMo7XvOZTPKhCHIF/qJhRwWNaS/oeAn+siHoIE8Ed/ky0XHB/34Bg1Cvmo63Ndr33dIVI5mxR0DgLwfCiTXSM2Rd4qTV3+RvCkdGxxzgKDXaBZEDx/Cca7RiEN0e9uzCpfTsbwFBOSPE/Ihm9HcNw8XGAdQTWdiE487ciptqvsEV6EANtiQgFfTmeK3YkS5ZXsLatr8IDT8Apf1B6Vf5YguqwfwP8n3bPwJbb+tjVdrXrcun3DV2UfBpyJs/YR1Ev5C3yL+RvAoWt49U16KNkn9ordokdnW0oPA5ryaukT6EWHR+GPpIGSvkr6NiWm7M2Ve3uJjX9V5dbI0XFA997+6tr8VNaPBHpK2cXa+kETxycPtAuYa7UNfHrN3Lj3/YzpHKjjvfSb4a6u6EAZ1BG0AdSN8ZTtw+K1tB7AD7NeYNFOYA3KWwQj/xHIDJhh/VqB38HrJzdnBOaUakNFWR5VXsUDbURCa99zKJ68e/eOXXgI41hIdnGqcvetCsU2AYrQ0bOuQQLeSHnKPjoJ4vM5XcFJEwwyGlTGZlPu3apZPdXJvl5CuSphi+ErOjM8liH4bo8mjIpY8vpNYDhF26SpqNUO0qrHWAvCwXdlcLaLaVXdbh8x4V5gnnTFRkz3Rxeom3ORJJvY1V8Jf9N4E5ODcHQ/FRPMjnl72wWkt9qG4PtYs6HO99bxNeh3bxlsqK5qVOfmSe2v9tfVzHbAqARa+p5gmRfyxxVPnkaxpTNfqGi0+5MG7SUXLoFvZACjjQroVR5HzdGxO11BXiLwqggdvyXwrRAmiKlgtoWd1YRujzVSEozkztN7wkzn99mb/rbqcdPGA2TdPgJhXHiy+6MLV9CR5KX8FeOHLv4i3C0OV9LU/dRKAR5dPWUXO9DRaht9rNlICSkdK/+cff9Q/aZksJGIz4ImxdPGej0Lb73RJgm0+laHvPU1kOeq9SlHlgyPpyE9VEhAsnqSAlMZsv67LuLawISfIzbZIBh2qzhqnAq8CsLpCmCipyuEw31fJIUglq86HGHPhaxtRSpejT2K97PoOpDZF6RFR9E+gjpLk9V6FD3YGce9p4HJAfTGXlWxryhP60zvr8Y+poSf416yPouNqt3uj86h8Eyb57KFgKSovxJd9H1OgGZPgQZ4csnup3LSiZRdql1ESF2bVW0bvqGbGWsuVcfn6vs1+hVt6H/L+XrU/6016lT9HeiPNRXlaWO9unaFc5d5pfD29W1Ms5E8ySo1n2z1rQ5762bFnWq5RUSENpeVITBVpedHJCA5Iuu9voHBpkbyVR6V8Y0GNiqO/naF2VatMd+EPe6sa7OuL5XYYoJv+HJxtR7Fe2wz4qT8LY7r3YR95AR9VNnONtr90VGK3KCdnW3BKMz5KzY3vzLAFXH3UyuEN616AXYxJWnNfbVt+EYexVhzATo+vO/X6HcHueT83xq7jtbdgf5YOzmettKra1f87DKvFN7UAjzGb8+LS6DVtzosrZsV8aYfYa6Mlvfpj1r8bSZh0ezeAapAGD1dofo4lS90fan0NyU8gnkuGNrkVIV94DRVDVgCA//VBPF4DbaAzv4ZE6rXEa/18MEfdMAHf3hPbKl9X6UexXMPB0tANtb90cEyv5Lmov5K9kI+/uWV0oxFTIBfK71kzOh+SsKzIBn2ccyE8XCidYldPWDpqSUS6H3/fo591HxtiY6W1DlCr0vo2rROyY+WykvErK1fwn9A+aJxt3WzgsWLNZTkCWGqkIkET8hJM6Hgb1lc51MMDhZHBHuXfphwVNSnDjtn9t4q9/y7gft/WKVHQfm845o8pZAqVz6nCz56ZPxdi/11IFl8qJB2OW40WtQpn6OqTTSC8KCQfYppNMCrrtHpCt2jN94b5Gu3v3Gv687qJGK+YvtHXTwpR+dRHfm6L3yM3dSEFnss2otoTOpbZSyq4J+FPDF8md6ztiDYSwgvRcT7KSHiAV74qOnX8KOLAYV77HppaNXj0nZK9VrsYzd/NSVSMp75I68H/raXvjLzVcrjbz2xPfzRZ7qfvYalvKT9qs6pBgdwB4fH6o+S9ob8pSv6Zc4ekuWqmx17SuUH6z/VXNRfCRi50a8ZnxiT6RfYffRJmvJz4Rr9VB/HjhnHWm1jk7EGY5VNJ/t2qVx1e9/P9fiHsl30+4B+dSrq/7xtbD1fW01sJYIoT6q7pU+vJGUdWKGPltYDpfLTSvyOOeHIrVlGAhBsbE6arC/4rJ8ZIZ/ftPY9h+HZHE8252eV2iZDDpDJAwsft7hXzISC97l+5yu5BaxPn1TOwogOaN80KNVHUAgSvAwS/HNFuJGgrPvg2/7C7qdxqlz50MMGChsP1Oc+bAMa6GRcYQCGCUU1jWHlPdPiA5m9UIx8awKbBgycwHOKAiNjkvgHxej3TnEyqJy6tqhiwyr6N7ABAmTGBDSLN4CvtceiLtRmUt8qw86wMWztpBi++PtPe5WmZAtUO1sQvdAHzW6zcEIIuv2b8ebL0IHjdQJ7Uj59FWeb01GrHqfNbHVfax8lf7PWXw38SG7Y0sgfKY978yPoaRRUjq3R31xfUszrWXyslj7pgtJJ+wUAeEVZHA7RgT+i6bH6o6y9SS4le8iWS4Ulf1cqP9AK5k2J/5y/wufSH83/EDMJHgWV36KfKupNfCf9gMr6OCYrkRw44Wlj98hughtkvcdcpPf9QMjTpPRyqX2/di4xZan5viCDPeZrzTS2VijwtKVPbyWtGV681Iy/pbVhsnwD/CfhKPn6gW8PC09DqKhfHIsGZPNEq291GJ7N8WRzWOw8FyNcNlmIVZg+weWJYPi0/HvVZ7Jt/0xABySPp/a0UapPm195WNLRoHIMIrrookKqXPnQ84tit7gj1jUd3Jj4j95f0j1H59mosFCk0QAPilnsYCgjw6xom8UROrfFOjwyGcwGwYc2gi5KdXiibDaRxe0La+0R8KQuRGdJ3+ietox/JjEvQOpDjS0Y7Dlip2/RHJPttyJoWPQqjZ5icI5u4Qjt2+VFflr1GEGxSVatfZT8zRb+6iTZRf2R8qETH8MmYCyQj0wtoB/8p/PDikv2S70sDkN8cPxY/VHW3kr2UCr3Okz6u8ryg01h1FzOX7ExYRvgVKJfzMZ4yegW/RT8JvVa4Qf6OCYBSk7TuRxynYbWMWyTsUa0ZceCUrlnImkjleVTWRx5f6l9v1a/W8gqJ4M95mtb0FzCkeNpS59eomN1eUUfLK0HsuUb4IfHkq93clBb0TlpZf2Sn3FtRH5afatD8SyCKJklxngCa08ycgsaOnYYmCgzobbARCL5lN0ry2CJp/VdmRf0c90YXS6fH5WRTwcJT0NQ5EKhnCd+HE+2hT34p/yG/JxUzn04ibJ2MIYojQ7gwB/RaCdXFrcqHPACT8jHNpdq8KGLqQyn9XBapQ2NoY7aN71Tr4T7JPiULkr65nUjnsbw+gunCoAP6ayyhYHw4xM4rtnrN+IDXXKFk31g3UJY8Ukwdz6GZ8LvlVdaCDTp8R7t9r+is8o+BLe7v1IbyDnpj1Lcqx4+iOD0QEJ5bJaRNLvP2m8lDvAdGkTXo/RH4rtkb5voQe2k/J3DXyrfhIhlSKL+yqNigy6UH5P319aMym7WTwU8pvSa9QOq/6jHMdnGHyQDTnh+VPp/TZ6JuGkME76txpoEOW3ZoidlIw5RqbyttU2hL7Lv1+p3I0lEZSAamENwbT1f24jsLJooT77Glj49S8RBhaX1QKm8RGZN/ZKvP3l7Ss1Ji/UhUjiyfibBSJNvNRxPLdEQ/yhYDK8YxMgbXRxL5MTBsGlAWtcw+VY5ix92m8JJyEn30fq+4bfU0cUi9QfBMhCF4Xvl5QakaLnqmEOAR9Lg59ipTYJcG7ofHIbStM1iNuQJuBKNDteV/WCcPAWG12HRqnsczqgTGV/Kp0OwwBpkZmUWU19p4LCvllBrj1Fd+HZpO6lvwWBHbERhj/x10eeKQ3se+FJ+yhZU7bgAHbo4+k/AOXxwqeBH5eiQywXdI3/0Cz8sAlxQPgtm+gGyBlcyCHapHqc4R7RNCxvua+3jJNqj/kb5W/irqL8p8aG20QWysE0L6ERPBD6Ih7y5cvabxQGiKw7X6o/QY9TeNtJF1N8FuEvlAej+Scmi6K88FcwTsHfkx5jMCUi3Eav4MfipqN7Ee40feNTjmLcfjvNnN0m9LPeci5zURu/7XiGSxbX0/eq5hGetOqqRgWDuhJDLBd2vnq8Zrj3iGp58u5v49EoeRjKsrNMEJr6z64FSeamxmvqCyfp630ZyTlpZPzoW5egXXsapJb719CyHOFH2J+Xz/YnZKYIpPAzrYlHHk9oT9xEYCGeBFx5zdmDA65rVVx4LJy4XdP9eCTZF3GsZugff7EmyA9ZPofyFh/tVcG7zRDG8/lsxu+eDIQKne4TPR/FGGzi6z9JI3SsN8PWd+HujONycYKKI8f+sayp7FhSDvpSOBRbHfBdicMYxoEhe0R6FM6eLor5VHxvliQw2SgdlosHmzLBZo7wTeYpmtkDZGQK6CQeBqU6MJF4B4bQI/ecTaV3YMvbvdKHY2bxiFgd76VGoH4LaKrXzAJxPFe3DqqvNqL+xcmLBLPFXWX8U4k+kTUe/+HLbMEJfRfv1dXI4Es1eRTZ2clX+yKRaY28G2xILb87fYcPZ8pa2NoRt8Vc8POCfi+BlGHeVvmk/Jf5yeiv6AdV/7OMY8wueGJbmrrvNRay/iI7iWGOwLXHBRk6l8pa2NoS9lr5fPZdYIJsWGWw5X1tAanWVFp628OlFwrz9F+G2AFBb2fVAqbxEQ66+yrK+XuXZOWlF/dxYlCN9qW89Pc1hjZWJCRbwLNphthgEx4KHwQFjRIBD0D0LXAyao+VuYTQU+kSsvvKmbdsk5ZXHyUckR5sKhrei3OrZwuCkOkYbi+5pQPhuUyMsUJ0kjSHctaWRhS5eAWGwNVmdlOa0hX1AdcrWd8pgkpAL2EhpEjGrT7vKzNqjYJK6UJnxkNM3J3fgGR5Z9DFB/lbpkT2Tp2tmC8o7R6BfIXNiaI4G8YDs2GDh9ACTOfTKYDicHAkqwvcuegza2DQpPor2ETYo+E39lfDh45L+KGw7lRYOBgZ0iP/hNIXpBnussd9TDkeq3WvIF19X549CuUK/7qPjYwjXkhbOpL8DT6m8pa0NYWv9FTaPv8JPzR5+eHpu0k/l9KayGj/wqMcxyei57AP/iQ1N+0hoyrvNRcJGREPv+/cCuYq+j92I3OxcM9RvY7pWBlvP1xrJbAKv5Wkrn95E3AHApfVAqbxEYq5+0tfLjmvmpMn6ECUcU//pxh/lx9bIIR+LfCsInoVYGtKvBcvpitnTWhHLgPAvXeHHN3DKhJe63GJOcAiMRRETi5O/J/lJV6k+JzXY4HC4BP+CigoIjPY5pk9HIXB/8vccAQQmWS44eALGcCo5BKeQ4e4+wdN1dlynIUfjFPYm7iU7DJWFFfLmST2GiT7DBZZux0GwPLHnVaGYfMfA8bukPXrwki6S+hZN2Ck8DEF5DBgsGCkzG6Q8ZQuUHRo8fVu3yTdKnH5jiFW2Vo8xtFvkJe1DNO/tr9gEK/mbLI+ikU0xTsk4f6uYfsa99Zek/RriChwGejOxl9NF+SPRVGVvK5VQ8nel8pXNt1eXXGwDrr3yvMbN+SnPYklvST8g+T76cUwycK+iKn4jeUbtTWVrx7DVY83cnJtySjZSKm9qbAtgyTyqi4W49+77Sf0upNdV21gGRkpWFga0V7wxT2flZaGMSuuBUnmp2Wh9yb3k6xknknNSlbGmKa15mv2I6FrlWxdtVqhRnP57XZyWYEE6BF8GozaRpozJ9Z0u3vk6CQZhssBns8KeTiN47sGdrS84nFuIn10engpbHsJ2QXm0hZCgFxoIpXI2OniSaRNdWyzEFmpGP3jDUKIxhL2VNJsSJiMWaciG90P/I8Wg1w+nFr5OwZTy0auuqD36uiVdZPUt3C90PaedgBbs6n1wTzJlCxOw67kVz0zsrF+ZbmcMCA55rNLjDOlGGehNV9Q+fFnW33jeFvkr8IuNkr8pcYp98v0Rm9SZvVo9u8/5qxIOw3VL8cX5oxp720ABJX9XKt+AhGNRSK437ae8NEt6y/oByejRjmNmjZJBcp6hstVjmHCsGmuMzhVxyUZK5SuaPk9Vyfywvp/T73m4H7daK4txrcu8uwFeSuuBUnlJMdH6khsPspK+XmXFOWmuvieqyY8I32rf+uTdu3cwzFPwWGADIHeEnE0ABDNaxOgenN/p+uiRfqmYjQi36FH8b90/92VDpHz75kSpPnXf6gL/ZyBQ3dGmic+DPgYnNjMQ7l8F555OKk2dZLnKcIDgpg0W3G4jRfEoCI53Z90rAmGB8qtoDOs8xrTkZItAOtCqIFwpeyzqQnWT+lYZHQ37cu9JK8YuZidBBBe1BcFebRBP9B368iel2VCMBpVtpsdoAxtkisaUfZT8zSp/ZaT79mf+SPnYF7JlUxdaON4+fLFe5eQDQ8AXfVDesAFCpu6T9uvLiziAe+xBctzMjoVrqb2V7KFUnvV3oitbfo02IJ4eg58q6k1ySPoBlWE3j3Icq7Fpyaf3/RpBXRjMOfq+2oz69nOLplYW56azpv1L5UV0Zcdf401w2fVAqnwL/B5Hja/HjlNz0mR94S+ORSYHYsEXfatgkBeynQWVPWGzgka/nZXeZ8w2IhJwPbtLoEugS6BLoEugS6BLoEugS6BLoEugS6BLoEugS6BKAtqQYOMkGlT25/8PxykEyCoCg/oAAAAASUVORK5CYII=",
                         "text/latex": [
                             "$\\displaystyle \\left[\\begin{matrix}- \\left(\\frac{1260}{5687} - f_{a_j}\\right) \\left(\\frac{6501}{10385} - f_{b_i}\\right) + \\left(\\frac{3737}{5687} - f_{a_i}\\right) \\left(\\frac{29744}{31155} - f_{b_j}\\right)\\\\\\left(\\frac{2204576}{323544675} - \\Delta_{i,j}\\right) \\left(\\frac{3737}{5687} - f_{a_i}\\right) + \\left(\\frac{273192}{32341969} - \\Delta_{i,j}\\right) \\left(\\frac{6501}{10385} - f_{b_i}\\right) + \\left(\\frac{3737}{5687} - f_{a_i}\\right) \\left(\\frac{29744}{31155} - f_{b_j}\\right) \\left(- f_{a_i} - f_{b_i} + \\frac{75779932}{59059495}\\right)\\\\\\left(\\frac{2204576}{323544675} - \\Delta_{i,j}\\right) \\left(\\frac{1260}{5687} - f_{a_j}\\right) + \\left(\\frac{273192}{32341969} - \\Delta_{i,j}\\right) \\left(\\frac{29744}{31155} - f_{b_j}\\right) + \\left(\\frac{3737}{5687} - f_{a_i}\\right) \\left(\\frac{29744}{31155} - f_{b_j}\\right) \\left(- f_{a_j} - f_{b_j} + \\frac{208409428}{177178485}\\right)\\end{matrix}\\right]$"
                         ],
                         "text/plain": [
-                            "\u23a1                                             \u239b1260          \u239e \u239b 6501          \n",
-                            "\u23a2                                           - \u239c\u2500\u2500\u2500\u2500 - f_{a_j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_i}\n",
-                            "\u23a2                                             \u239d5687          \u23a0 \u239d10385          \n",
-                            "\u23a2                                                                              \n",
-                            "\u23a2\u239b 2204576                \u239e \u239b3737          \u239e   \u239b 273192                \u239e \u239b 6501\n",
-                            "\u23a2\u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f + \u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500\n",
-                            "\u23a2\u239d323544675               \u23a0 \u239d5687          \u23a0   \u239d32341969               \u23a0 \u239d10385\n",
-                            "\u23a2                                                                              \n",
-                            "\u23a2\u239b 2204576                \u239e \u239b1260          \u239e   \u239b 273192                \u239e \u239b29744\n",
-                            "\u23a2\u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500 - f_{a_j}\u239f + \u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500\n",
-                            "\u23a3\u239d323544675               \u23a0 \u239d5687          \u23a0   \u239d32341969               \u23a0 \u239d31155\n",
-                            "\n",
-                            "\u239e   \u239b3737          \u239e \u239b29744          \u239e                                         \n",
-                            "\u239f + \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f                                         \n",
-                            "\u23a0   \u239d5687          \u23a0 \u239d31155          \u23a0                                         \n",
-                            "                                                                               \n",
-                            "          \u239e   \u239b3737          \u239e \u239b29744          \u239e \u239b                     75779932\n",
-                            " - f_{b_i}\u239f + \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f\u22c5\u239c-f_{a_i} - f_{b_i} + \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\n",
-                            "          \u23a0   \u239d5687          \u23a0 \u239d31155          \u23a0 \u239d                     59059495\n",
-                            "                                                                               \n",
-                            "          \u239e   \u239b3737          \u239e \u239b29744          \u239e \u239b                     20840942\n",
-                            " - f_{b_j}\u239f + \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f\u22c5\u239c-f_{a_j} - f_{b_j} + \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\n",
-                            "          \u23a0   \u239d5687          \u23a0 \u239d31155          \u23a0 \u239d                     17717848\n",
+                            "\u23a1                                             \u239b1260          \u239e \u239b 6501          \u239e \n",
+                            "\u23a2                                           - \u239c\u2500\u2500\u2500\u2500 - f_{a_j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_i}\u239f \n",
+                            "\u23a2                                             \u239d5687          \u23a0 \u239d10385          \u23a0 \n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2\u239b 2204576                \u239e \u239b3737          \u239e   \u239b 273192                \u239e \u239b 6501  \n",
+                            "\u23a2\u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f + \u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 -\n",
+                            "\u23a2\u239d323544675               \u23a0 \u239d5687          \u23a0   \u239d32341969               \u23a0 \u239d10385  \n",
+                            "\u23a2                                                                                \n",
+                            "\u23a2\u239b 2204576                \u239e \u239b1260          \u239e   \u239b 273192                \u239e \u239b29744  \n",
+                            "\u23a2\u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500 - f_{a_j}\u239f + \u239c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 - \\Delta_{i,j}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 -\n",
+                            "\u23a3\u239d323544675               \u23a0 \u239d5687          \u23a0   \u239d32341969               \u23a0 \u239d31155  \n",
                             "\n",
-                            "  \u23a4\n",
-                            "  \u23a5\n",
-                            "  \u23a5\n",
-                            "  \u23a5\n",
-                            "\u239e \u23a5\n",
-                            "\u239f \u23a5\n",
-                            "\u23a0 \u23a5\n",
-                            "  \u23a5\n",
-                            "8\u239e\u23a5\n",
-                            "\u2500\u239f\u23a5\n",
-                            "5\u23a0\u23a6"
+                            "  \u239b3737          \u239e \u239b29744          \u239e                                           \u23a4\n",
+                            "+ \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f                                           \u23a5\n",
+                            "  \u239d5687          \u23a0 \u239d31155          \u23a0                                           \u23a5\n",
+                            "                                                                               \u23a5\n",
+                            "        \u239e   \u239b3737          \u239e \u239b29744          \u239e \u239b                     75779932\u239e \u23a5\n",
+                            " f_{b_i}\u239f + \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f\u22c5\u239c-f_{a_i} - f_{b_i} + \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u239f \u23a5\n",
+                            "        \u23a0   \u239d5687          \u23a0 \u239d31155          \u23a0 \u239d                     59059495\u23a0 \u23a5\n",
+                            "                                                                               \u23a5\n",
+                            "        \u239e   \u239b3737          \u239e \u239b29744          \u239e \u239b                     208409428\u239e\u23a5\n",
+                            " f_{b_j}\u239f + \u239c\u2500\u2500\u2500\u2500 - f_{a_i}\u239f\u22c5\u239c\u2500\u2500\u2500\u2500\u2500 - f_{b_j}\u239f\u22c5\u239c-f_{a_j} - f_{b_j} + \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u239f\u23a5\n",
+                            "        \u23a0   \u239d5687          \u23a0 \u239d31155          \u23a0 \u239d                     177178485\u23a0\u23a6"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Let's take a look at the postulates now that we have specified \n",
                 "# the unknown sample statistics of correctness.\n",
                 "# We should only have variables left that are moments of the test data sketch\n",
                 "\n",
-                "sympy.Matrix([postulate.subs(values) \n",
-                "              for postulate in pair_binary_classifiers_postulates])"
+                "sympy.Matrix([axiom.subs(values) \n",
+                "              for axiom in pair_binary_classifiers_axioms])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 22,
             "id": "c5d4adc9-b2a4-476b-8659-09053b9af562",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Let's create a dict for the quantities we can calculate from the data sketch\n",
                 "# The pair frequency moment is label independent even though it is calculated \n",
                 "# using only a single label!\n",
                 "pair_moment_a = tvc.pair_frequency_moment((i, j), 'a')\n",
                 "pair_moment_b = tvc.pair_frequency_moment((i, j), 'b')\n",
-                "pair_moment_a == pair_moment_b;;;;;;;;"
+                "pair_moment_a == pair_moment_b"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 23,
             "id": "a62da7ab-ff84-436f-9e81-e7546bdcc2dd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/latex": [
@@ -893,30 +870,30 @@
                             "\u23a2                36842   \u23a5\n",
                             "\u23a2                        \u23a5\n",
                             "\u23a2                34171   \u23a5\n",
                             "\u23a2  f_{b_j}       \u2500\u2500\u2500\u2500\u2500   \u23a5\n",
                             "\u23a3                36842   \u23a6"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "obsv_values = {deltaij: pair_moment_b,\n",
                 "              fai: cvf[i]['a'], fbi: cvf[i]['b'],\n",
                 "              faj: cvf[j]['a'], fbj: cvf[j]['b']}\n",
                 "sympy.Matrix([(key, val) \n",
                 "              for key, val in obsv_values.items()])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 24,
             "id": "ad2f2d93-d4fb-408d-8dfd-adb9d60564ed",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "iVBORw0KGgoAAAANSUhEUgAAABoAAABLCAYAAABumJecAAAACXBIWXMAAA7EAAAOxAGVKw4bAAACTklEQVRYCe1Z7U0CQRAF429DNLEA7MCPCsQO1A7UEvgJf7EDbEE60A6IdIAFmEiIFfge7LvsHbu3c0iMMTvJZWbnc+/t3jjB9mAwOG21Wm94QjQZDoc3IUNVB785dN2qnmvY2vue4REynX169xcJeRSwX0F3Tb1faIzKTRKX8iL2qaTAAjqqNgpRWUsI1K4/4XiCZwSdaXN7tZk9IxLyHKfgfTyEuY/nBXLwXLzQlWgqhGT38O6AT5QA8hIy12Pp6ripEBLw5s0CiabQ9VC0E7CVVNZCPUQtSpHrhc6H9lpKFrLsFhUOa6vAmCzkJeGZxGhn0MUKSH8kIcYtbxQ6G+UTZPyuailZyF1jJgnBI50uRbRYspCLfAXvBrLojWivJWuhZ2Q5D2Q6g27mvXXAZa0yFUIiNswF+KpBMhQyYbvFc8d1ivzunfLl7tlEL8B5+OSXWIc6BkxlMhdCwiVCH8rh9pUJOnu6uGcuFMcmYcnQJQCKmzN0cWwSFnMLYh60oTxAFoBab10eIAvIJFig0wDCP3wx0jQUs5sm1WiwZ/hbA+SB25m4t9HVRyrIQvBIFxsgj5WMZ/TlFuKy+XzbAfJDSSyXgb55gBRiBTd37zxAFpg5wXrrqnGN17lQY8gUkKETEo35r0FnbkF8hTxA+gdpPaM8QPqorWQLdHmA3ICNiiR0blagr4ZFyiLpYgOk/NKFnOe2A2TjQnmALCCTYO7eeYAUZOLJ70iOP+X/r5B/6+a4WVWEdvIPXyZlIfap2A/nyR7GJI70y5fWJf4NG3PVUHf+2SkAAAAASUVORK5CYII=",
                         "text/latex": [
@@ -926,24 +903,24 @@
                             "\u23a10\u23a4\n",
                             "\u23a2 \u23a5\n",
                             "\u23a20\u23a5\n",
                             "\u23a2 \u23a5\n",
                             "\u23a30\u23a6"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# The final check, all entries should be identically zero\n",
                 "\n",
-                "sympy.Matrix([postulate.subs({**values, **obsv_values}) \n",
-                "              for postulate in pair_binary_classifiers_postulates])"
+                "sympy.Matrix([axiom.subs({**values, **obsv_values}) \n",
+                "              for axiom in pair_binary_classifiers_axioms])"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -956,12 +933,19 @@
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.11.5"
+        },
+        "widgets": {
+            "application/vnd.jupyter.widget-state+json": {
+                "state": {},
+                "version_major": 2,
+                "version_minor": 0
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ntqr-0.2/docs/source/ntqr.r2.md` & `ntqr-0.3.1/docs/source/ntqr.r2.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/source/research/GradingLLMs.md` & `ntqr-0.3.1/docs/source/research/GradingLLMs.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/source/research/MathematicsOfAlgebraicEvaluation.md` & `ntqr-0.3.1/docs/source/research/MathematicsOfAlgebraicEvaluation.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/docs/source/research/TheScienceOfAlgebraicEvaluation.md` & `ntqr-0.3.1/docs/source/research/TheScienceOfAlgebraicEvaluation.md`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/img/NTQRpt24.png` & `ntqr-0.3.1/img/NTQRpt24.png`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/img/uciAdultEvalPiaGauges.png` & `ntqr-0.3.1/img/uciAdultEvalPiaGauges.png`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/img/uciAdultEvalPrevalenceGauges.png` & `ntqr-0.3.1/img/uciAdultEvalPrevalenceGauges.png`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/pyproject.toml` & `ntqr-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     {name = "Adam Sloat", email = "adam.sloat@dataengines.com"}]
 
 dynamic = ["version"]
 description = "Tools for the logic of evaluation using unlabeled data"
 readme = "README.md"
 
 dependencies = ["sympy>=1.12",
-                "typing_extensions>=4.9.0"]
+                "typing_extensions>=4.9.0",
+                "matplotlib>=3.8.0"]
 
 license = {file = "LICENSE.txt"}
 keywords = ["evaluation", "algebra", "machine learning", "logic", "ai safety"]
 classifiers = [
  "Development Status :: 3 - Alpha",
  "Framework :: Jupyter",
  "Intended Audience :: Information Technology",
@@ -31,12 +32,13 @@
 
 
 [project.urls]
 Home = "https://github.com/andrescorrada/IntroductionToAlgebraicEvaluation/tree/main/python"
 Documentation="https://ntqr.readthedocs.org/en/latest"
 
 [project.optional-dependencies]
-doc = [
+sphinx = [
     "sphinx>=5.0.2",
     "myst-parser",
-    "nbsphinx"
+    "nbsphinx",
+    "matplotlib",
 ]
```

### Comparing `ntqr-0.2/src/ntqr/r2/datasketches.py` & `ntqr-0.3.1/src/ntqr/r2/datasketches.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """@author: Andrés Corrada-Emmanuel."""
 import math
 
 # The mathematics of evaluating finite samples is, by construction, one
 # of estimating integer fractions. We import this module so we can create
 # two versions of every computation - the exact one using integer ratios,
 # and the one using the default floating point numbers
-from fractions import Fraction
+import sympy
 from typing_extensions import Union, Literal, Mapping, Iterable
 from dataclasses import dataclass
 
 # Types
 Label = Union[Literal["a"], Literal["b"]]
 
 
@@ -19,15 +19,15 @@
 # Vote counts are what we see when we have unlabeled data.
 VoteCounts = Mapping[Votes, int]
 
 # Label vote counts, vote counts by true label, are only available
 # when we are carrying out experiments on labeled data.
 LabelVoteCounts = Mapping[Label, VoteCounts]
 
-VoteFrequencies = Mapping[Votes, Fraction]
+VoteFrequencies = Mapping[Votes, sympy.Rational]
 
 
 # Some definitions and utilities to help various classes
 
 # Three binary classifiers have eight possible voting patterns
 trio_vote_patterns: tuple[tuple[Label, ...], ...] = (
     ("a", "a", "a"),
@@ -194,15 +194,15 @@
         Returns
         -------
         Mapping[Votes, Fraction]
         """
         by_voting_counts = self.to_vote_counts()
         size_of_test = sum(by_voting_counts.values())
         return {
-            vp: Fraction(by_voting_counts[vp], size_of_test)
+            vp: sympy.Rational(by_voting_counts[vp], size_of_test)
             for vp in by_voting_counts.keys()
         }
 
     def to_voting_frequencies_float(self) -> Mapping[Votes, float]:
         """
         Compute observed voting frequencies inexactly, as floats.
 
@@ -281,15 +281,15 @@
 
         Returns
         -------
         VoteFrequencies:
             Maps a trio vote pattern to its Fraction occurence in the test.
         """
         return {
-            vp: Fraction(self.vote_counts[vp], self.test_size)
+            vp: sympy.Rational(self.vote_counts[vp], self.test_size)
             for vp in self.vote_counts.keys()
         }
 
     def to_frequencies_float(self) -> Mapping[Votes, float]:
         """
         Compute observerd voting pattern frequencies, inexactly, as floats.
 
@@ -303,71 +303,71 @@
         return {
             vp: self.vote_counts[vp] / self.test_size
             for vp in self.vote_counts.keys()
         }
 
     def classifier_label_frequency(
         self, classifier: int, label: Label
-    ) -> Fraction:
+    ) -> sympy.Rational:
         """
         Calculate classifier label voting frequency.
 
         Parameters
         ----------
         classifier : int
             The index of the classifier.
         label : Label
             The label.
 
         Returns
         -------
-        Fraction(label_vote_counts, test_size):
-            The Fraction of times the classifier voted the label when
+        sympy.Rational(label_vote_counts, test_size):
+            The fraction of times the classifier voted the label when
             classifying items in the test.
 
         """
         vote_frequencies = self.to_frequencies_exact()
         return sum(
             [
                 vote_frequencies[votes]
                 for votes in classifier_label_votes(classifier, label)
             ]
         )
 
     def pair_label_frequency(
         self, pair: Iterable[int], label: Label
-    ) -> Fraction:
+    ) -> sympy.Rational:
         """
         Compute frequency of times a pair voted with the same label.
 
         Parameters
         ----------
         pair : Iterable[int, int]
             Classifier indicies.
         label : Label
             The label.
 
         Returns
         -------
-        Fraction:
-            The Fraction of times a pair of classifiers voted with the
+        sympy.Rational:
+            The fraction of times a pair of classifiers voted with the
             same label when classifying items in the test.
 
         """
         vote_frequencies = self.to_frequencies_exact()
         return sum(
             [
                 vote_frequencies[votes]
                 for votes in classifiers_labels_votes(pair, (label, label))
             ]
         )
 
     def pair_frequency_moment(
         self, pair: Iterable[int], label: Label
-    ) -> Fraction:
+    ) -> sympy.Rational:
         """
         Calculate the label classifier pair frequency moment.
 
         If (i, j) = pair, then this is -
 
             f_{label_i, label_j} - f_{label_i} * f_{label_j}
 
@@ -379,35 +379,35 @@
         pair : Iterable(int, int)
             The pair of classifiers.
         label : Label
             One of the binary labels.
 
         Returns
         -------
-        Fraction:
+        sympy.Rational:
             The pair frequency moment as a Fraction object
         """
         label_frequencies = [
             self.classifier_label_frequency(classifier, label)
             for classifier in pair
         ]
         return self.pair_label_frequency(pair, label) - math.prod(
             label_frequencies
         )
 
     def label_pairs_frequency_moments(
         self, label: Label
-    ) -> Mapping[tuple[int, int], Fraction]:
+    ) -> Mapping[tuple[int, int], sympy.Rational]:
         """All the label pair frequency moments."""
         return {
             pair: self.pair_frequency_moment(pair, label)
             for pair in trio_pairs
         }
 
-    def trio_frequency_moment(self) -> Fraction:
+    def trio_frequency_moment(self) -> sympy.Rational:
         """
         Calculate the 3rd frequency moment of a trio of binary classifiers.
 
         Don't ask.
         """
         classifier_label_frequencies = [
             self.classifier_label_frequency(classifier, "b")
```

### Comparing `ntqr-0.2/src/ntqr/r2/evaluators.py` & `ntqr-0.3.1/src/ntqr/r2/evaluators.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,65 +110,51 @@
     """Evaluation for experiments where the true labels are known."""
 
     def __init__(self, label_counts: TrioLabelVoteCounts):
         self.label_counts = label_counts
 
         self.evaluation_exact = {
             "prevalence": self.prevalences(),
-            "accuracies": {
-                label: [
-                    self.classifier_label_accuracy(classifier, label)
-                    for classifier in range(3)
-                ]
-                for label in ("a", "b")
-            },
-            "pair_correlations": {
-                label: {
-                    pair: self.pair_label_error_correlation(pair, label)
-                    for pair in trio_pairs
+            "accuracy": [
+                {
+                    label: self.classifier_label_accuracy(classifier, label)
+                    for label in ("a", "b")
                 }
-                for label in ("a", "b")
+                for classifier in range(3)
+            ],
+            "pair_correlation": {
+                pair: {
+                    label: self.pair_label_error_correlation(pair, label)
+                    for label in ("a", "b")
+                }
+                for pair in trio_pairs
             },
-            "3_way_correlations": {
-                label: {
-                    (0, 1, 2): self.three_way_label_error_correlation(
-                        (0, 1, 2), label
-                    )
+            "3_way_correlation": {
+                trio: {
+                    label: self.three_way_label_error_correlation(trio, label)
+                    for label in ("a", "b")
                 }
-                for label in ("a", "b")
+                for trio in ((0, 1, 2),)
             },
         }
 
         self.evaluation_float = {
             "prevalence": {
-                label: float(val) for label, val in self.prevalences().items()
+                label: float(val)
+                for label, val in self.evaluation_exact["prevalence"].items()
             },
-            "accuracies": {
-                label: [
-                    float(self.classifier_label_accuracy(classifier, label))
-                    for classifier in range(3)
-                ]
-                for label in ("a", "b")
-            },
-            "pair_correlations": {
-                label: {
-                    pair: float(self.pair_label_error_correlation(pair, label))
-                    for pair in trio_pairs
-                }
-                for label in ("a", "b")
-            },
-            "3_way_correlations": {
-                label: {
-                    (0, 1, 2): float(
-                        self.three_way_label_error_correlation(
-                            (0, 1, 2), label
-                        )
-                    )
-                }
-                for label in ("a", "b")
+            "accuracy": [
+                {label: float(val) for label, val in cdict.items()}
+                for cdict in self.evaluation_exact["accuracy"]
+            ],
+            "pair_correlation": {
+                pair: {label: float(val) for label, val in corrs.items()}
+                for pair, corrs in self.evaluation_exact[
+                    "pair_correlation"
+                ].items()
             },
         }
 
     def prevalences(self):
         """
         Calculate the prevalences of the two labels.
 
@@ -177,25 +163,25 @@
         Mapping[Label, Fraction]
             Mapping from labels to percentage of appearance in the test.
 
         """
         test_sizes = self.label_counts.test_sizes
         total = sum(test_sizes.values())
         return {
-            "a": Fraction(test_sizes["a"], total),
-            "b": Fraction(test_sizes["b"], total),
+            "a": sympy.Rational(test_sizes["a"], total),
+            "b": sympy.Rational(test_sizes["b"], total),
         }
 
     def classifier_label_accuracy(self, classifier: int, label: Label):
         """Compute classifier label accuracy."""
         test_size = self.label_counts.test_sizes[label]
         classifier_votes = classifier_label_votes(classifier, label)
         label_counts = self.label_counts[label]
         correct_counts = [label_counts[votes] for votes in classifier_votes]
-        return Fraction(sum(correct_counts), test_size)
+        return sympy.Rational(sum(correct_counts), test_size)
 
     def other_label(self, label: Label):
         """Return the other binary classification label given label."""
         if label == "a":
             o_label = "b"
         else:
             o_label = "a"
@@ -437,91 +423,106 @@
     between the two comes down to the same computation of error correlation.
     """
 
     def __init__(self, vote_counts: TrioVoteCounts):
         self.vote_counts = vote_counts
         self.vote_frequencies = self.vote_counts.to_frequencies_exact()
 
-        self.evaluation_exact = {
-            "'a' prevalence solutions": self.alpha_prevalence_estimates(),
-            "accuracies": [
-                {
-                    "a": self.classifier_a_label_accuracy(classifier),
-                    "b": self.classifier_b_label_accuracy(classifier),
-                }
-                for classifier in range(3)
-            ],
-        }
-        self.evaluation_float = {
-            "'a' prevalence solutions": [
-                float(val) for val in self.alpha_prevalence_estimates()
-            ],
-            "accuracies": [
-                {
-                    "a": [
-                        float(val)
-                        for val in self.classifier_a_label_accuracy(classifier)
-                    ],
-                    "b": [
-                        float(val)
-                        for val in self.classifier_b_label_accuracy(classifier)
-                    ],
-                }
-                for classifier in range(3)
-            ],
-        }
+        # Two solutions are possible
+        self.evaluation_exact = [
+            {
+                "prevalence": {"a": a_prevalence, "b": 1 - a_prevalence},
+                "accuracy": [
+                    {
+                        "a": self.classifier_a_label_accuracy(
+                            classifier, a_prevalence
+                        ),
+                        "b": self.classifier_b_label_accuracy(
+                            classifier, a_prevalence
+                        ),
+                    }
+                    for classifier in range(3)
+                ],
+            }
+            for a_prevalence in self.alpha_prevalence_estimates()
+        ]
+
+        self.evaluation_float = [
+            {
+                "prevalence": {
+                    label: float(val)
+                    for label, val in sol_dict["prevalence"].items()
+                },
+                "accuracy": [
+                    {
+                        label: float(val)
+                        for label, val in classifier_dict.items()
+                    }
+                    for classifier_dict in sol_dict["accuracy"]
+                ],
+            }
+            for sol_dict in self.evaluation_exact
+        ]
 
     def alpha_prevalence_quadratic_terms(self):
         """
         Calculate the coefficients of the 'a' label prevalence quadratic.
 
         If the quadratic is represented as:
             a * (P_a)**2 + b * P_a + c
         then,
             a = terms[2], b = terms[1], c = terms[0].
         The quadratic is written in the 'standard' way seen in algebra
         textbooks. Be careful to not mistake the 'a' or 'b' coefficients
         described here with the two labels being used for classification -
         currently implemented as ('a', 'b').
         """
-        # The coefficient of the square term
+
         pfmds = self.vote_counts.label_pairs_frequency_moments("b")
         vote_frequencies = self.vote_frequencies
         fbbb = vote_frequencies[("b", "b", "b")]
         diff1 = fbbb - self.vote_counts.trio_frequency_moment()
         prodFDs = math.prod(pfmds.values())
         term_coefficients = {
             2: diff1**2 + 4 * prodFDs,
             1: -(diff1**2 + 4 * prodFDs),
-            0: -prodFDs,
+            0: prodFDs,
         }
 
         return term_coefficients
 
     def alpha_prevalence_estimates(self):
-        """Calculate the prevalence of the alpha label."""
+        """Calculate the prevalence of the alpha label.
+
+        Since the quadratic equation has ordered solutions by
+        the plus/minus operations, we arbitrarily return the 'a' label
+        less than 50% solution first."""
         coeffs = self.alpha_prevalence_quadratic_terms()
-        b = coeffs[1]
+        a = coeffs[2]
         c = coeffs[0]
-        sqrTerm = sympy.sqrt(1 - 4 * c / b) / 2
-        return [Fraction(1, 2) + sqrTerm, Fraction(1, 2) - sqrTerm]
+        sqrTerm = sympy.sqrt(1 - 4 * c / a) / 2
+        prev_expr = [
+            sympy.Rational(1, 2) - sqrTerm,
+            sympy.Rational(1, 2) + sqrTerm,
+        ]
+        return [sympy.simplify(expr) for expr in prev_expr]
 
-    def classifier_a_label_accuracy(self, classifier: int):
+    def classifier_a_label_accuracy(self, classifier: int, a_prevalence):
         """
         Calculate classifier 'a' label accuracies.
 
         Parameters
         ----------
         classifier : int
             One of (0, 1, 2).
+        a_prevalence: Sympy expression
 
         Returns
         -------
-        Two possible logically consistent estimates for P_{i,a} given the
-        test error independence assumption.
+        The a label accuracy given the a_prevalence value
         """
         # Assuming the linear equation form a + b * P_a + c * P_{i, a}
 
         classifier_freqs = [
             self.vote_counts.classifier_label_frequency(classifier, "b")
             for classifier in range(3)
         ]
@@ -545,21 +546,17 @@
             - other_moment * (1 - classifier_freqs[classifier]) * freqDiff
             + 2 * prodFDs
         )
 
         b_coeff = -4 * prodFDs - freqDiff**2
         c_coeff = other_moment * freqDiff
 
-        prevalences = self.alpha_prevalence_estimates()
-        return [
-            (-a_coeff - b_coeff * prevalence) / c_coeff
-            for prevalence in prevalences
-        ]
+        return sympy.simplify((-a_coeff - b_coeff * a_prevalence) / c_coeff)
 
-    def classifier_b_label_accuracy(self, classifier: int):
+    def classifier_b_label_accuracy(self, classifier: int, a_prevalence):
         """
         Calculate classifier 'b' label accuracies.
 
         Parameters
         ----------
         classifier : int
             One of (0, 1, 2).
@@ -594,31 +591,29 @@
             classifier_freqs[classifier] * other_moment * freqDiff
             - 2 * prodFDs
         )
 
         b_coeff = 4 * prodFDs + freqDiff**2
         c_coeff = -other_moment * freqDiff
 
-        prevalences = self.alpha_prevalence_estimates()
-        return [
-            (-a_coeff - b_coeff * prevalence) / c_coeff
-            for prevalence in prevalences
-        ]
+        return sympy.simplify((-a_coeff - b_coeff * a_prevalence) / c_coeff)
 
 
 class MajorityVotingEvaluation:
     """
     Evaluate three binary classifiers using majority voting.
 
     Majority voting can be used to carry out evaluation algebraically.
-    Its major drawback is that it assumes that the crowd is always right,
-    as a consequence it cannot minimize its errors when the classifiers
-    are error independent in the test.
+    Typically, majority voting is used with the assumption that the
+    crowd is always right. In the context of safety, however, that the
+    crowd is always wrong is an equally valid a-priori assumption. Hence,
+    this class returns TWO evaluations. The first assuming the crowd is
+    always right and the second assuming they are always wrong.
     Its main virtue is that it is simple and rock solid - always returns
-    a seemingly sensible result.
+    logically consistent evaluations.
     """
 
     def __init__(self, vote_counts: TrioVoteCounts):
         """
         Initialize data structures.
 
         TODO: Implement detection that the TrioVoteCounts are not generated
@@ -634,68 +629,96 @@
         None.
 
         """
         self.vote_counts = vote_counts
         self.vote_frequencies = self.vote_counts.to_frequencies_exact()
         self.labels = ("a", "b")
 
-        self.majority_vote_patterns = {
+        self.majority_right_vote_patterns = {
             label: [
-                votes for votes in trio_vote_patterns if votes.count(label) > 1
+                votes
+                for votes in trio_vote_patterns
+                if votes.count(label) >= 2
             ]
             for label in self.labels
         }
 
-        self.evaluation_exact = {
-            "prevalence": self.prevalences(),
-            "accuracies": [
-                {
-                    label: self.classifier_label_accuracy(classifier, label)
-                    for label in self.labels
-                }
-                for classifier in range(3)
-            ],
+        self.majority_wrong_vote_patterns = {
+            label: [
+                votes
+                for votes in trio_vote_patterns
+                if votes.count(label) <= 1
+            ]
+            for label in self.labels
         }
 
-        self.evaluation_float = {
-            "prevalence": {
-                label: float(val) for label, val in self.prevalences().items()
-            },
-            "accuracies": [
+        self.evaluation_exact = [
+            self.compute_vote_pattern_evaluation(vps, flip)
+            for vps, flip in [
+                (self.majority_right_vote_patterns, False),
+                (self.majority_wrong_vote_patterns, False),
+            ]
+        ]
+
+        self.evaluation_float = [
+            self.to_float(sol) for sol in self.evaluation_exact
+        ]
+
+    def compute_vote_pattern_evaluation(self, vote_patterns, flip):
+        return {
+            "prevalence": self.prevalences(vote_patterns),
+            "accuracy": [
                 {
-                    label: float(
-                        self.classifier_label_accuracy(classifier, label)
+                    label: self.classifier_label_accuracy(
+                        classifier, vote_patterns, label, flip
                     )
                     for label in self.labels
                 }
                 for classifier in range(3)
             ],
         }
 
-    def prevalences(self):
+    def prevalences(self, vote_patterns):
         """Compute label prevalences in the test."""
         return {
             label: sum(
-                [
-                    self.vote_frequencies[vp]
-                    for vp in self.majority_vote_patterns[label]
-                ]
+                [self.vote_frequencies[vp] for vp in vote_patterns[label]]
             )
             for label in self.labels
         }
 
-    def classifier_label_accuracy(self, classifier, label):
+    def classifier_label_accuracy(
+        self, classifier, vote_patterns, label, flip
+    ):
         """Compute the label accuracy for classifier."""
+        if flip:
+            if label == "a":
+                correct_label = "b"
+            elif label == "b":
+                correct_label = "a"
+        else:
+            correct_label = label
         return sum(
             [
                 self.vote_frequencies[vp]
-                for vp in self.majority_vote_patterns[label]
-                if vp[classifier] == label
+                for vp in vote_patterns[label]
+                if vp[classifier] == correct_label
             ]
-        )
+        ) / sum([self.vote_frequencies[vp] for vp in vote_patterns[label]])
+
+    def to_float(self, sol):
+        as_floats = {}
+        as_floats["prevalence"] = {
+            label: float(val) for label, val in sol["prevalence"].items()
+        }
+        as_floats["accuracy"] = [
+            ({label: float(val) for label, val in classifier_dict.items()})
+            for classifier_dict in sol["accuracy"]
+        ]
+        return as_floats
 
 
 if __name__ == "__main__":
     from pprint import pprint
 
     sympy.init_printing(use_unicode=True)
```

### Comparing `ntqr-0.2/src/ntqr/r2/examples.py` & `ntqr-0.3.1/src/ntqr/r2/examples.py`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/src/ntqr/r3/postulates.py` & `ntqr-0.3.1/src/ntqr/r3/postulates.py`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/tests/test_datasketches.py` & `ntqr-0.3.1/tests/test_datasketches.py`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/tests/test_r2_postulates.py` & `ntqr-0.3.1/tests/test_r2_postulates.py`

 * *Files identical despite different names*

### Comparing `ntqr-0.2/PKG-INFO` & `ntqr-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntqr
-Version: 0.2
+Version: 0.3.1
 Summary: Tools for the logic of evaluation using unlabeled data
 Keywords: evaluation,algebra,machine learning,logic,ai safety
 Author-email: Andres Corrada-Emmanuel <andres.corrada@dataengines.com>, Walker Lee <walker.lee@dataengines.com>, Adam Sloat <adam.sloat@dataengines.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Information Technology
@@ -12,20 +12,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Dist: sympy>=1.12
 Requires-Dist: typing_extensions>=4.9.0
-Requires-Dist: sphinx>=5.0.2 ; extra == "doc"
-Requires-Dist: myst-parser ; extra == "doc"
-Requires-Dist: nbsphinx ; extra == "doc"
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: sphinx>=5.0.2 ; extra == "sphinx"
+Requires-Dist: myst-parser ; extra == "sphinx"
+Requires-Dist: nbsphinx ; extra == "sphinx"
+Requires-Dist: matplotlib ; extra == "sphinx"
 Project-URL: Documentation, https://ntqr.readthedocs.org/en/latest
 Project-URL: Home, https://github.com/andrescorrada/IntroductionToAlgebraicEvaluation/tree/main/python
-Provides-Extra: doc
+Provides-Extra: sphinx
 
 # Logic tools to make your AI safer
 
 ![NTQR](./img/NTQRpt24.png)
 
 ```console
 ~$: pip install ntqr
@@ -64,15 +66,15 @@
 useful in AI safety applications:
 
 1. It is **universal**. The algorithms here apply to any domain. There is no
    Out of Distribution (OOD) problem when you use algebraic evaluation because
    it does not use any probability theory. By only using summary statistics of
    how a group of classifiers labeled a test set, we can treat all classifiers,
    whether human or robotic, as black boxes. There are no hyperparameters
-   to tune or set in NTQR algorithms. If they where, these algorithms could
+   to tune or set in NTQR algorithms. If they were, these algorithms could
    not claim to be universal.
 
 2. It is **complete**. The finite nature of any test given to a group of
    binary classifiers means we can guarantee the existence of a complete
    set of postulates that must be obeyed during any evaluation. Completeness
    is a logical safety shield. It allows us to create theorem provers that
    can unequivocably detect violations of the logical consistency of **any**
```
