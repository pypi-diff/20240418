# Comparing `tmp/petrinet2vec-1.0.2.tar.gz` & `tmp/petrinet2vec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrinet2vec-1.0.2.tar", last modified: Sun Apr 14 00:05:27 2024, max compression
+gzip compressed data, was "petrinet2vec-1.0.3.tar", last modified: Sun Apr 14 00:38:22 2024, max compression
```

## Comparing `petrinet2vec-1.0.2.tar` & `petrinet2vec-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:05:27.512670 petrinet2vec-1.0.2/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1063 2024-04-05 12:52:41.000000 petrinet2vec-1.0.2/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     1816 2024-04-14 00:05:27.512670 petrinet2vec-1.0.2/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)       74 2024-04-12 18:02:06.000000 petrinet2vec-1.0.2/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)      600 2024-04-14 00:03:47.000000 petrinet2vec-1.0.2/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-14 00:05:27.512670 petrinet2vec-1.0.2/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:05:27.512670 petrinet2vec-1.0.2/src/
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:05:27.512670 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     1816 2024-04-14 00:05:27.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      267 2024-04-14 00:05:27.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-14 00:05:27.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       33 2024-04-14 00:05:27.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       22 2024-04-14 00:05:27.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)    19710 2024-04-12 16:54:24.000000 petrinet2vec-1.0.2/src/PetriNet2Vec.py
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-12 16:37:29.000000 petrinet2vec-1.0.2/src/__init__.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:38:22.561183 petrinet2vec-1.0.3/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1063 2024-04-05 12:52:41.000000 petrinet2vec-1.0.3/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     4644 2024-04-14 00:38:22.561183 petrinet2vec-1.0.3/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2901 2024-04-14 00:36:29.000000 petrinet2vec-1.0.3/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)      601 2024-04-14 00:37:30.000000 petrinet2vec-1.0.3/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-14 00:38:22.561183 petrinet2vec-1.0.3/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:38:22.561183 petrinet2vec-1.0.3/src/
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-14 00:38:22.561183 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4644 2024-04-14 00:38:22.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      267 2024-04-14 00:38:22.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-14 00:38:22.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       33 2024-04-14 00:38:22.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       22 2024-04-14 00:38:22.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19710 2024-04-12 16:54:24.000000 petrinet2vec-1.0.3/src/PetriNet2Vec.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-12 16:37:29.000000 petrinet2vec-1.0.3/src/__init__.py
```

### Comparing `petrinet2vec-1.0.2/LICENSE` & `petrinet2vec-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petrinet2vec-1.0.2/pyproject.toml` & `petrinet2vec-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ['setuptools>=69.3.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "PetriNet2Vec"
-version = "1.0.2"
+version = "1.0.3"
 authors = [{ name="Juan G. Colonna", email="juancolonna@icomp.edu.ufam.br" }]
 license = { file = "LICENSE" }
 description = "Process Mining Embeddings: Learning Representations for Petri Nets"
 readme = "README.md"
 requires-python = ">=3.10.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"]
-dependencies = [ "numpy", "pm4py", "gensim", "scipy==1.11.1"]
+dependencies = [ "numpy", "pm4py", "gensim", "scipy==1.11.1"]
```

### Comparing `petrinet2vec-1.0.2/src/PetriNet2Vec.py` & `petrinet2vec-1.0.3/src/PetriNet2Vec.py`

 * *Files identical despite different names*

