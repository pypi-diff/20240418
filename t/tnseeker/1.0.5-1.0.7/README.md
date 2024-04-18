# Comparing `tmp/tnseeker-1.0.5.tar.gz` & `tmp/tnseeker-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnseeker-1.0.5.tar", last modified: Sun Mar 24 23:30:56 2024, max compression
+gzip compressed data, was "tnseeker-1.0.7.tar", last modified: Thu Apr 18 20:23:27 2024, max compression
```

## Comparing `tnseeker-1.0.5.tar` & `tnseeker-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-03-24 23:30:56.307170 tnseeker-1.0.5/
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     5986 2024-03-24 23:30:56.290534 tnseeker-1.0.5/PKG-INFO
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      275 2024-03-18 23:20:12.000000 tnseeker-1.0.5/README.txt
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)       38 2024-03-24 23:30:56.307170 tnseeker-1.0.5/setup.cfg
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     1928 2024-03-18 23:17:38.000000 tnseeker-1.0.5/setup.py
-drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-03-24 23:30:56.132649 tnseeker-1.0.5/tnseeker/
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    67649 2024-03-24 22:35:40.000000 tnseeker-1.0.5/tnseeker/Essential_Finder.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    63162 2024-03-21 21:45:02.000000 tnseeker-1.0.5/tnseeker/Essential_Finder_old.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2021-05-14 10:49:48.000000 tnseeker-1.0.5/tnseeker/__init__.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    19991 2024-03-24 20:37:59.000000 tnseeker-1.0.5/tnseeker/__main__.py
-drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-03-24 23:30:56.235532 tnseeker-1.0.5/tnseeker/data/
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    37334 2020-10-11 09:07:31.000000 tnseeker-1.0.5/tnseeker/data/Truenegativs.csv
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      421 2020-04-19 20:08:09.000000 tnseeker-1.0.5/tnseeker/data/Truepositivs.csv
-drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-03-24 23:30:56.274737 tnseeker-1.0.5/tnseeker/extras/
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2021-05-14 10:49:55.000000 tnseeker-1.0.5/tnseeker/extras/__init__.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    10547 2017-07-14 08:02:00.000000 tnseeker-1.0.5/tnseeker/extras/possion_binom.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     8594 2023-08-03 11:59:34.000000 tnseeker-1.0.5/tnseeker/insertions_over_genome_plotter.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    13055 2024-03-21 21:37:55.000000 tnseeker-1.0.5/tnseeker/reads_trimer.py
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    27324 2024-03-24 20:35:55.000000 tnseeker-1.0.5/tnseeker/sam_to_insertions.py
-drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-03-24 23:30:56.196018 tnseeker-1.0.5/tnseeker.egg-info/
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     5986 2024-03-24 23:30:55.000000 tnseeker-1.0.5/tnseeker.egg-info/PKG-INFO
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      503 2024-03-24 23:30:55.000000 tnseeker-1.0.5/tnseeker.egg-info/SOURCES.txt
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        1 2024-03-24 23:30:55.000000 tnseeker-1.0.5/tnseeker.egg-info/dependency_links.txt
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      156 2024-03-24 23:30:55.000000 tnseeker-1.0.5/tnseeker.egg-info/requires.txt
--rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        9 2024-03-24 23:30:55.000000 tnseeker-1.0.5/tnseeker.egg-info/top_level.txt
+drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-04-18 20:23:27.963302 tnseeker-1.0.7/
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     6056 2024-04-18 20:23:27.963302 tnseeker-1.0.7/PKG-INFO
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      468 2024-03-25 00:00:47.000000 tnseeker-1.0.7/README.txt
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)       38 2024-04-18 20:23:27.963302 tnseeker-1.0.7/setup.cfg
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     2024 2024-04-18 20:15:12.000000 tnseeker-1.0.7/setup.py
+drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-04-18 20:23:27.807052 tnseeker-1.0.7/tnseeker/
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    71540 2024-04-18 19:49:36.000000 tnseeker-1.0.7/tnseeker/Essential_Finder.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2021-05-14 10:49:48.000000 tnseeker-1.0.7/tnseeker/__init__.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    20263 2024-04-18 20:15:12.000000 tnseeker-1.0.7/tnseeker/__main__.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     1366 2024-04-15 21:40:14.000000 tnseeker-1.0.7/tnseeker/blaster.py
+drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-04-18 20:23:27.916427 tnseeker-1.0.7/tnseeker/data/
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     2160 2024-04-10 21:55:16.000000 tnseeker-1.0.7/tnseeker/data/barcode2sam.sh
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)  1644188 2024-04-10 22:26:45.000000 tnseeker-1.0.7/tnseeker/data/true_negatives.fasta
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    64979 2024-04-10 22:26:38.000000 tnseeker-1.0.7/tnseeker/data/true_positives.fasta
+drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-04-18 20:23:27.947677 tnseeker-1.0.7/tnseeker/extras/
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2021-05-14 10:49:55.000000 tnseeker-1.0.7/tnseeker/extras/__init__.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    10547 2017-07-14 08:02:00.000000 tnseeker-1.0.7/tnseeker/extras/possion_binom.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     8626 2024-04-16 22:55:08.000000 tnseeker-1.0.7/tnseeker/insertions_over_genome_plotter.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    13108 2024-04-10 13:31:04.000000 tnseeker-1.0.7/tnseeker/reads_trimer.py
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)    27092 2024-04-10 20:48:53.000000 tnseeker-1.0.7/tnseeker/sam_to_insertions.py
+drwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        0 2024-04-18 20:23:27.869553 tnseeker-1.0.7/tnseeker.egg-info/
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)     6056 2024-04-18 20:23:27.000000 tnseeker-1.0.7/tnseeker.egg-info/PKG-INFO
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      527 2024-04-18 20:23:27.000000 tnseeker-1.0.7/tnseeker.egg-info/SOURCES.txt
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        1 2024-04-18 20:23:27.000000 tnseeker-1.0.7/tnseeker.egg-info/dependency_links.txt
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)      211 2024-04-18 20:23:27.000000 tnseeker-1.0.7/tnseeker.egg-info/requires.txt
+-rwxrwxrwx   0 afombravo  (1000) afombravo  (1000)        9 2024-04-18 20:23:27.000000 tnseeker-1.0.7/tnseeker.egg-info/top_level.txt
```

### Comparing `tnseeker-1.0.5/PKG-INFO` & `tnseeker-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: tnseeker
-Version: 1.0.5
+Version: 1.0.7
 Summary: TnSeeker
 Home-page: https://github.com/afombravo/tnseeker
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 Keywords: tn-seq,essentiality,rb-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.19.2
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numba>=0.53.1
-Requires-Dist: biopython>=1.81
-Requires-Dist: datetime
-Requires-Dist: argparse
-Requires-Dist: regex
-Requires-Dist: multiprocess
-Requires-Dist: pathlib
-Requires-Dist: scipy>=1.6.2
-Requires-Dist: seaborn>=0.12.1
-Requires-Dist: statsmodels>=0.12.2
+Requires-Dist: numpy==1.26.4
+Requires-Dist: matplotlib==3.8.2
+Requires-Dist: pandas==2.2.0
+Requires-Dist: numba==0.59.0
+Requires-Dist: biopython==1.83
+Requires-Dist: datetime==5.4
+Requires-Dist: argparse==1.4.0
+Requires-Dist: regex==2023.12.25
+Requires-Dist: multiprocess==0.70.16
+Requires-Dist: pathlib==1.0.1
+Requires-Dist: scipy==1.12.0
+Requires-Dist: seaborn==0.13.2
+Requires-Dist: statsmodels==0.14.1
 
 # Tnseeker
 Tnseeker is an advanced pipeline tailored for transposon insertion sequencing (Tn-Seq) analysis. It performs an array of tasks: from read trimming and alignment to associating genomic locations with transposon insertions, and inferring essential genes based on transposon insertion densities. Additionally, Tnseeker is adept at extracting barcodes from raw fastq files and linking them to corresponding transposon genomic locations for subsequent analysis. What truly distinguishes Tnseeker from other tools is its unique capability to automatically infer and adjust threshold/cutoff parameters. This negates the need for intricate user input, allowing for a more precise determination of gene essentiality based on the data. Compatible with any transposon disruption experiment, Tnseeker efficiently mitigates transposon-specific biases, including those seen with HIMAR. Hence, Tnseeker is versatile enough to handle all Tn-Seq datasets.
 
 Tnseeker is under active developement and is available as is. Contact me if you are interested in using the program or have any questions. Bugs can be expected. Please report any weird or unintented behaviour. 
 
 ## Requirements
```

### Comparing `tnseeker-1.0.5/setup.py` & `tnseeker-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '1.0.5' 
+VERSION = '1.0.7' 
 DESCRIPTION = 'TnSeeker'
 LONG_DESCRIPTION = 'Versatile Python3 module for processing and analyzing anything related with Tn-Seq. Requires bowtie2 to be callable from terminal. File wise, only fastq and genbank annotation files are required.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="tnseeker", 
@@ -17,30 +17,31 @@
         author="Afonso M Bravo",
         author_email="<afonsombravo@hotmail.com>",
         url='https://github.com/afombravo/tnseeker',
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(),
-        install_requires=["numpy >= 1.19.2",
-                           "matplotlib >= 3.3.4",
-                           "numba >= 0.53.1",
-                           "biopython >= 1.81",
-                           "datetime",
-                           "argparse",
-                           "regex",
-                           "multiprocess",
-                           "pathlib",
-                           "scipy >= 1.6.2",
-                           "seaborn >= 0.12.1",
-                           "statsmodels >= 0.12.2"],
+        install_requires=["numpy == 1.26.4",
+                           "matplotlib == 3.8.2",
+                           "pandas ==  2.2.0", 
+                           "numba == 0.59.0",
+                           "biopython == 1.83",
+                           "datetime == 5.4",
+                           "argparse == 1.4.0",
+                           "regex == 2023.12.25",
+                           "multiprocess == 0.70.16",
+                           "pathlib == 1.0.1",
+                           "scipy == 1.12.0",
+                           "seaborn == 0.13.2",
+                           "statsmodels == 0.14.1"],
         
         keywords=['tn-seq', 'essentiality','rb-seq'],
         classifiers= [
             "Development Status :: 3 - Alpha", #change here for when the product is more finished
             "Intended Audience :: Science/Research",
             "Programming Language :: Python :: 3",
             "Operating System :: OS Independent",
         ],
         include_package_data=True,
-        package_data={'': ['data/*.csv']},
+        package_data={'': ['data/*']},
 )
```

### Comparing `tnseeker-1.0.5/tnseeker/Essential_Finder.py` & `tnseeker-1.0.7/tnseeker/Essential_Finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import csv
 import statsmodels.stats.multitest
 from Bio import SeqIO
 import os
 import glob
 import numpy as np
 import scipy
 import re
 from tnseeker.extras.possion_binom import PoiBin
 from scipy.stats import binomtest
 import multiprocessing
 import matplotlib.pyplot as plt
 import sys
-import datetime
 from numba import njit
 import pkg_resources
 import pandas as pd
+import csv
+import subprocess
+from pathlib import Path
 
 """
 Disclaimer: 
     I am aware this script is messy and complex. 
     It was 5y in the making and changed a lot over time to accommodate endless 
     features, exceptions, and use cases.
     It´s more of a pathwork than anything else at the moment.
     Please don´t judge me too harshly.
 """
 
-
 def inputs(argv):
     ''' The inputs function initializes a global Variables instance with various attributes 
     from a given list of command-line arguments. It sets up parameters for directory, 
     strain, annotation, subdomain length, p-value, and output, as well as true positives 
     and true negatives file paths. '''
 
     global variables
     variables = Variables()
     variables.directory = argv[0]  # folder with the unique insertions file
     variables.strain = argv[1]  # strain name, and annotation file name
     variables.annotation_type = argv[2]
     variables.annotation_folder = argv[3]
-    variables.subdomain_length = [float(argv[4]), float(argv[5])]
+    variables.subdomain_length = [float(argv[4]), float(argv[5])] #upstream, downstream
     variables.pvalue = float(argv[6])
     variables.ir_size_cutoff = int(argv[7])
     variables.output_name = variables.strain + "_alldomains"
     variables.domain_uncertain_threshold = float(argv[8])  # 0.75
+    variables.biggest_gene = 0
 
     variables.true_positives = pkg_resources.resource_filename(
-        __name__, 'data/Truepositivs.csv')
+        __name__, 'data/true_positives.fasta')
     variables.true_negatives = pkg_resources.resource_filename(
-        __name__, 'data/Truenegativs.csv')
-
+        __name__, 'data/true_negatives.fasta')
 
 def path_finder():
     ''' The path_finder function searches for and sets file paths for both insertions file and the 
     correct annotation (gb/gff) based on the global variables instance. It uses the nested sub_path_finder 
     function to search for specific file types and names within specified folders. '''
 
     def sub_path_finder(folder, extenction, search):
@@ -230,14 +230,100 @@
         self.GC_content = GC_content
         self.domain_notes = domain_notes
         self.motif_seq = motif_seq
         self.subdomain_insert_orient_plus = subdomain_insert_orient_plus or dict()
         self.subdomain_insert_orient_neg = subdomain_insert_orient_neg or dict()
         self.significant = significant or dict()
 
+def subprocess_cmd(command):
+    try:
+        return subprocess.check_output(command)
+    except subprocess.CalledProcessError as e:
+        return e.output.decode()
+
+def blast_maker():
+    
+    def tblastn(file):
+        
+        out = f"{blast_db}/{Path(variables.strain).stem}_{Path(file).stem}.txt"
+
+        send = ["tblastn",
+                "-query",
+                file,
+                "-db",
+                fasta,
+                "-evalue",
+                "0.00001",
+                "-out",
+                out,
+                "-outfmt",
+                "6"]
+        
+        subprocess_cmd(send)
+
+        found_true = {}
+        with open(out) as current:
+            for line in current:
+                line = line.split("\t")
+                first = int(line[8])
+                last = int(line[9])
+                if first > last:
+                    orientation = "-"
+                    start = last
+                    end = first
+                else:
+                    orientation = "+"
+                    start = first
+                    end = last
+                found_true[line[0]] = Gene(gene=line[0],
+                                           contig=line[1],
+                                           start=start,
+                                           end=end,
+                                           orientation=orientation)
+
+        return found_true
+    
+    blast_db = f"{variables.directory}/blast_db"
+    if not os.path.isdir(blast_db):
+        os.mkdir(blast_db)
+    
+    if variables.annotation_type == "gb":
+        fasta = f"{blast_db}/{Path(variables.strain).stem}.fasta"
+        with open(variables.annotation_file_paths[0], "r") as input_handle:
+            with open(fasta, "w") as output_handle:
+                sequences = SeqIO.parse(input_handle, "genbank")
+                SeqIO.write(sequences, output_handle, "fasta")
+    else:
+        fasta_in = variables.annotation_file_paths[1]
+        fasta = f"{blast_db}/{Path(variables.strain).stem}.fasta"
+        send = ["cp",
+                fasta_in,
+                fasta]
+        subprocess_cmd(send)
+
+    send = ["makeblastdb",
+            "-in",
+            fasta,
+            "-dbtype",
+            "nucl"]
+    
+    subprocess_cmd(send)
+
+    variables.true_positives = tblastn(variables.true_positives)
+    variables.true_negatives = tblastn(variables.true_negatives)
+    
+    print(f"\nFound {len(variables.true_positives)} benchmark essential genes.\n")
+    
+    compiled_benchmark = {**variables.true_positives, **variables.true_negatives}
+    for gene in compiled_benchmark:
+        lenght = compiled_benchmark[gene].end-compiled_benchmark[gene].start
+        if lenght > variables.biggest_gene:
+            variables.biggest_gene = lenght
+    
+    return compiled_benchmark
 
 def domain_resizer(domain_size_multiplier, basket):
     ''' The domain_resizer function takes a domain size multiplier and a dictionary 
     of genes (basket) as input, and resizes gene domains by calculating the new 
     domain size based on genome length, total insertions, and domain size multiplier. 
     It then updates the domain boundaries for each gene in the basket.'''
 
@@ -620,15 +706,19 @@
     genes = []
     for rec in SeqIO.parse(file, "gb"):
         for feature in rec.features:
             # if feature.type == 'gene':
             start = feature.location.start
             end = feature.location.end
             orientation = feature.location.strand
-
+            
+            current = end-start
+            if current > variables.biggest_gene:
+                variables.biggest_gene = current
+            
             try:
                 identity = feature.qualifiers['locus_tag'][0]
 
             except KeyError:
                 identity = None
 
             try:
@@ -735,52 +825,60 @@
     with open(file) as current:
         for line in current:
             GB = line.split('\t')  # len(GB)
             if "#" not in GB[0][:3]:  # ignores headers
                 if GB[2] == "gene":
                     start = int(GB[3])
                     end = int(GB[4])
-    
+                    
+                    lenght = end-start
+                    if lenght > variables.biggest_gene:
+                        variables.biggest_gene = lenght
+                    
                     features = GB[8].split(";")  # gene annotation file
                     feature = {}
                     for entry in features:
                         entry = entry.split("=")
-                        feature[entry[0]] = entry[1].replace("\n", "")
+                        if len(entry) == 2:
+                            feature[entry[0]] = entry[1].replace("\n","")
                     if "gene" in feature:
                         gene = feature["gene"]
                     if "Name" in feature:
                         gene = feature["Name"]
                     else:
                         gene = feature["ID"]
     
                     contig = GB[0]
                     orientation = GB[6]  # orientation of the gene
     
                     basket[feature["ID"]] = Gene(gene=gene, start=start, end=end, orientation=orientation,
                                                  identity=feature["ID"], product=feature["product"], contig=contig)
-    
+
                     genes.append((start, feature["ID"], contig))
 
             if "##FASTA" in GB[0]:
                 break
-
+    
+    if len(basket) == 0:
+        print("Watch out, no genomic features were loaded. The gff file is not being parsed correctly.")
+        
     basket = inter_gene_annotater(basket, genes)
 
     for gene in basket:
 
         domain_size = basket[gene].end - basket[gene].start
         basket[gene].start = int(
             basket[gene].start+(domain_size*variables.subdomain_length[0]))
         basket[gene].end = int(
             basket[gene].start+(domain_size*variables.subdomain_length[1]))
 
     return basket
 
 
-def insertions_parser():
+def insertions_parser(startup=True):
     ''' This function, insertions_parser, performs the following tasks:
 
         1. Parses an insertion file to identify unique insertions and their orientation, 
         updating related data structures.
 
         2. Calculates the total number of insertions and the positive strand transposon 
         insertion ratio.
@@ -790,15 +888,17 @@
         4. Prints the transposon insertion frequency for each leading strand motif.'''
 
     # new code
     insertions_df = pd.read_csv(variables.insertion_file_path)
     insertions_df["unique"] = insertions_df["#Contig"] + \
         insertions_df["position"].astype(str)+insertions_df["Orientation"]
     insertions_df.drop_duplicates(subset=['unique'], inplace=True)
-    print(f"Total Insertions in library: {len(insertions_df)}")
+    if startup:
+        print(f"Total Insertions in library: {len(insertions_df)}")
+        
     insertions_df.drop(
         ['Read Counts', 'Average mapQ across reads', "unique"], axis=1, inplace=True)
 
     insertions_df = insertions_df[insertions_df["Relative Position in Gene (0-1)"].astype(
         float) <= variables.subdomain_length[1]]
     insertions_df = insertions_df[insertions_df["Relative Position in Gene (0-1)"].astype(
         float) >= variables.subdomain_length[0]]
@@ -833,22 +933,23 @@
     for i, element in enumerate(variables.transposon_motiv_count):
         if element != 0:
             variables.transposon_motiv_freq[i] = round(
                 element / total * 100, 1)
 
     # calculating the insertion frequency
     variables.chance_motif_tn = variables.normalizer()
-
-    print("Transposon insertion frequency (on leading strand):")
-    for tn, mtv in zip(variables.transposon_motiv_freq, variables.di_motivs):
-        print("{}: {}%".format(mtv, tn))
+    
+    if startup:
+        print("Transposon insertion frequency (on leading strand):")
+        for tn, mtv in zip(variables.transposon_motiv_freq, variables.di_motivs):
+            print("{}: {}%".format(mtv, tn))
 
 
 def cpu():
-    ''' The cpu function determines the available number of CPUs that cna be used.
+    ''' The cpu function determines the available number of CPUs that can be used.
     If more than one is available, one of them is left to avoid clogging the computer,
     while the others are used by the program. '''
 
     c = multiprocessing.cpu_count()
     if c >= 2:
         c -= 1
     pool = multiprocessing.Pool(processes=c)
@@ -962,25 +1063,27 @@
         for key in basket:
             if key in subresult:
                 basket[key] = subresult[key]
 
     return basket
 
 
-def pvalue_iteration(names, pvalues_list, pvaluing_array, pvalue, pvalue_listing, euclidean_points, variables, baseline_essentials_master, baseline_non_essentials_master):
+def pvalue_iteration(names, pvalues_list, pvaluing_array, pvalue, pvalue_listing, euclidean_points, variables):
     ''' This function performs a p-value iteration analysis to determine the 
     true positive rate (TPR) and specificity of a given test at different 
     p-value thresholds. It calls the function 'pvaluing' to calculate the 
     number of true positives, false negatives, true negatives and false 
     positives at a given p-value threshold. It then calculates the TPR and 
     specificity from these values and appends them, along with the p-value 
     threshold, to two lists. Finally, it returns these two lists. '''
 
-    baseline_essentials, baseline_non_essentials, pvaluing_array_copy = baseline_essentials_master.copy(
-    ), baseline_non_essentials_master.copy(), pvaluing_array.copy()
+    pvaluing_array_copy = pvaluing_array.copy()
+    baseline_essentials = set(variables.true_positives.keys())
+    baseline_non_essentials = set(variables.true_negatives.keys())
+    
     pvaluing_array_discard, strain_existent_essentials, fdr, rejected_baseline_essentials, \
         rejected_baseline_nonessentials, strain_existent_nonessentials = pvaluing(
             names, pvalues_list, pvaluing_array_copy, pvalue, variables, baseline_essentials, baseline_non_essentials)
 
     if len(pvaluing_array_discard) == 1:  # if there is only the header
         rejected_baseline_essentials = strain_existent_essentials
 
@@ -1003,30 +1106,14 @@
 
     pvalue_listing.append(pvalue)
     euclidean_points.append([specificity] + [TPR_sensitivity])
 
     return pvalue_listing, euclidean_points
 
 
-def reference_essentials_loader():
-    ''' This function loads two sets of gene names from two separate files, 
-    representing the known essential and non-essential genes in the reference genome.  '''
-
-    baseline_essentials_master = set()
-    with open(variables.true_positives) as current:
-        for line in current:
-            baseline_essentials_master.add(line[:-1])
-
-    baseline_non_essentials_master = set()
-    with open(variables.true_negatives) as current:
-        for line in current:
-            baseline_non_essentials_master.add(line[:-1])
-    return baseline_essentials_master, baseline_non_essentials_master
-
-
 def class_to_numba(basket):
     ''' The class_to_numba function takes a dictionary basket containing gene 
     information and extracts significant gene domains to convert them into 
     arrays that can be used with the numba library. It first loops through the 
     dictionary to extract gene names, p-values, and domain-related information. 
     Then, it creates a pvaluing_array containing this information in a numerical 
     format. Finally, it calls the reference_essentials_loader function to load 
@@ -1046,36 +1133,35 @@
                                            basket[gene].significant[domain].dom_len,
                                            1,  # non essential
                                            basket[gene].significant[domain].pvalue,
                                            basket[gene].significant[domain].dom_insert),
                                            dtype=np.float64))
 
     pvaluing_array = np.array(pvaluing_array)
-    baseline_essentials_master, baseline_non_essentials_master = reference_essentials_loader()
-    return baseline_essentials_master, baseline_non_essentials_master, pvaluing_array, names, pvalues_list
+    return pvaluing_array, names, pvalues_list
 
 
 def multi_pvalue_iter(basket):
     ''' This function performs multiple iterations of p-value thresholding to 
     determine true positive and false positive rates for a set of genes, 
     using parallel processing for efficiency. It takes a dictionary of genes 
     and their properties, converts them to Numpy arrays, and returns the 
     resulting lists of p-value thresholds and corresponding true/false positive rates.  '''
 
     # change here to increase resolution of iteration
     pvalue = [variables.pvalue * 0.5 ** i for i in range(200)]
     pool, cpus = cpu()
     result_objs, pvalue_listing, euclidean_points = [], [], []
 
-    baseline_essentials_master, baseline_non_essentials_master, pvaluing_array, names, pvalues_list = class_to_numba(
-        basket)
+    pvaluing_array, names, pvalues_list = class_to_numba(basket)
 
     for p in pvalue:
-        result = pool.apply_async(pvalue_iteration, args=((names, pvalues_list, pvaluing_array, p, pvalue_listing,
-                                  euclidean_points, variables, baseline_essentials_master, baseline_non_essentials_master)))
+        result = pool.apply_async(pvalue_iteration, args=((names, pvalues_list, 
+                                                           pvaluing_array, p, pvalue_listing,
+                                                           euclidean_points, variables)))
         result_objs.append(result)
 
     pool.close()
     pool.join()
 
     result = [result.get() for result in result_objs]
 
@@ -1091,24 +1177,28 @@
     using p-value thresholding. The function converts the gene dictionary into 
     Numpy arrays and applies the pvaluing function to determine essentiality. 
     The function then compiles a table of gene properties and essentiality 
     information, and generates an ROC (Receiver Operating Characteristic) 
     curve plot for the data. Finally, the function saves the table and plot 
     to files in a specified directory. '''
 
-    baseline_essentials_master, baseline_non_essentials_master, pvaluing_array, names, pvalues_list = class_to_numba(
-        optimal_basket)
-    result = pvaluing(names, pvalues_list, pvaluing_array, pvalue, variables,
-                      baseline_essentials_master, baseline_non_essentials_master)
-    essentiality_list = result[0]
-    fdr = result[2]
+    pvaluing_array, names, pvalues_list = class_to_numba(optimal_basket)
+
+    fdr = statsmodels.stats.multitest.multipletests(
+        pvalues_list, pvalue, "fdr_bh")  # multitest correction, fdr_bh
+
+    for i, (name, entry) in enumerate(zip(names, pvaluing_array)):
+        remove_signal, pvaluing_array = pvaluing_jit(
+            pvaluing_array, fdr[0], fdr[-1], i)
+    
+    fdr = fdr[3]
     legenda = f"Threshold p-value: {pvalue}"
     essentiality = []
 
-    for i, entry in enumerate(essentiality_list):
+    for i, entry in enumerate(pvaluing_array):
         if entry[3] == 0:
             essentiality.append("too small for assaying")
         if entry[3] == 1:
             essentiality.append("Non-Essential")
         if entry[3] == 2:
             essentiality.append("Probably Essential")
         if entry[3] == 3:
@@ -1121,15 +1211,15 @@
                   ["Insertion Orientation ratio (+/total)"] + ["Insertion Orientation p-value"] +
                   ["Domain part"] + ["Gene Orientation"] + ["Gene name"] + ["Essentiality"]]
 
     i = 0
     for gene in optimal_basket:
         for domain in optimal_basket[gene].significant:
             genes_list.append([optimal_basket[gene].significant[domain].dom_insert] +
-                              [optimal_basket[gene].significant[domain].pvalue] +
+                              [str(optimal_basket[gene].significant[domain].pvalue).replace("'","")] +
                               [optimal_basket[gene].contig] +
                               [optimal_basket[gene].identity] +
                               [optimal_basket[gene].product] +
                               [optimal_basket[gene].significant[domain].dom_len] +
                               [optimal_basket[gene].significant[domain].ratio_orient] +
                               [optimal_basket[gene].significant[domain].orient_pvalue] +
                               [optimal_basket[gene].significant[domain].domain_part] +
@@ -1206,19 +1296,19 @@
     ax1.tick_params(axis='y')
     ax1.set_title("Reciver Operator Curve (ROC)\nused to auto-determine the essentiality calling threshold for %s" %
                   variables.strain, size=9, pad=13)
     ax1.legend([legenda], loc="lower right")
     fig.tight_layout()
     plt.savefig(
         f"{variables.directory}/ROC_curves{variables.strain}.png", dpi=300)
+    plt.close()
+    gene_essentiality_compressor(optimal_basket,genes_list)
 
-    gene_essentiality_compressor()
 
-
-def genome_loader():
+def genome_loader(startup=True):
     ''' This function loads the genome sequence and stores it in a dictionary 
     named `genome_seq` under their respective contigs. It also initializes 
     empty dictionaries named `borders_contig`, `orientation_contig`, and 
     `insertions_contig` for each contig. The function works differently 
     depending on the format of the annotation file: if it is in GFF format, 
     it reads the sequence from a FASTA file referenced in `annotation_file_paths[1]`,
     while if it is in GenBank format, it reads the sequence from the GenBank 
@@ -1234,25 +1324,27 @@
                     variables.borders_contig[contig] = {}
                     variables.orientation_contig[contig] = {}
                     variables.insertions_contig[contig] = {}
                 else:
                     variables.genome_seq[contig] += line[:-1]
 
         for contig in variables.genome_seq:
-            print(f"Loaded: {contig}")
+            if startup:
+                print(f"Loaded: {contig}")
             variables.genome_length += len(variables.genome_seq[contig])
 
     elif variables.annotation_type == "gb":
         for rec in SeqIO.parse(variables.annotation_file_paths[0], "gb"):
             variables.genome_length = len(rec.seq)
             variables.annotation_contig = rec.id
             variables.borders_contig[variables.annotation_contig] = {}
             variables.orientation_contig[variables.annotation_contig] = {}
             variables.insertions_contig[variables.annotation_contig] = {}
-            print(f"Loaded: {variables.annotation_contig}")
+            if startup:
+                print(f"Loaded: {variables.annotation_contig}")
             variables.genome_seq[variables.annotation_contig] = str(rec.seq)
 
 
 def domain_iterator(basket):
     ''' The function domain_iterator performs an iterative process to find 
     the optimal size of genomic regions to divide a genome for downstream analysis. 
     It starts by defining a maximum size of the genomic region, then iteratively
@@ -1282,15 +1374,14 @@
                     if basket[key].significant[domain].orient_pvalue != "N/A":
                         basket[key].significant[domain].orient_pvalue = fdr[1][p]
                         p += 1
             return basket
 
         basket = orientation_pvaluing(basket)
         pvalue_listing, euclidean_points = multi_pvalue_iter(basket)
-
         # point where TPR_sensitivity = 1 and 1-specificity = 0
         convergence = [[0] + [1]] * len(np.array(euclidean_points[0]))
 
         #lower is better
         distances = scipy.spatial.distance.cdist(
             np.array(euclidean_points[0]), np.array(convergence), 'euclidean')
 
@@ -1310,45 +1401,41 @@
         basket = domain_resizer(variables.domain_iteration[i], basket)
         basket = multi_annotater(basket)
         best_pvalue, best_distance, euclidean_points = ROC(basket)
         iterator_store.append(
             [current_gap] + [best_pvalue] + [best_distance] + [i] + [euclidean_points])
         return iterator_store
 
-    biggest_gene = 0
-    for gene in basket:
-        current = basket[gene].length
-        if current > biggest_gene:
-            biggest_gene = current
-
     euclidean_distances = []
     iterator_store = []
-    i, current_gap = 1, 0
+    i, current_gap = 0, 0
 
     try:
 
         iteration = 1
         for f in variables.domain_iteration:
-            if int(variables.genome_length / variables.total_insertions * f) <= biggest_gene:
+            if int(variables.genome_length / variables.total_insertions * f) <= variables.biggest_gene:
                 iteration += 1
     
-        while current_gap <= biggest_gene:
+        while (current_gap <= variables.biggest_gene) and (i+1 < len(variables.domain_iteration)):
             current_gap = int(variables.genome_length /
                               variables.total_insertions * variables.domain_iteration[i])
-            print(f"Current domain division iteration: {i} out {iteration}")
+            print(f"Current domain division iteration: {i+1} out {iteration}")
             iterator_store = iterating(
                 i, iterator_store, euclidean_distances, basket, current_gap)
             i += 1
             
+        # sort by best eucledian distance
+        sorted_optimal = sorted(iterator_store, key=lambda e: e[2])
+        variables.best_domain_size = sorted_optimal[0][0]
+        
     except Exception:
-        print("Make sure you have enough unique insertions in your library. It might not be saturating enough.")
-
-    # sort by best eucledian distance
-    sorted_optimal = sorted(iterator_store, key=lambda e: e[2])
-    variables.best_domain_size = sorted_optimal[0][0]
+        print("\nLow saturating library detected\n")
+        variables.best_domain_size = sorted_optimal[0]
+        
     print(f"Optimal domain division size: {variables.best_domain_size}bp")
     fig, ax1 = plt.subplots()
 
     plt.xlim(0, 1)
     plt.ylim(0, 1)
 
     ax1.set_xlabel("True Negative Rate")  # 1 - specificity
@@ -1363,28 +1450,25 @@
     ax1.tick_params(axis='y')
     ax1.set_title("Reciver Operator Curve (ROC)\nused to auto-determine the essentiality calling threshold for %s" %
                   variables.strain, size=9, pad=13)
     ax1.legend(legenda, loc="lower right")
     fig.tight_layout()
     plt.savefig(os.path.join(variables.directory,
                 "ROC_curves_iterator_%s.png" % variables.strain), dpi=300)
-
+    plt.close()
     best_index = int(sorted_optimal[0][3])
     output_writer(variables.directory, "Best_ROC_points{}".format(
         variables.output_name), iterator_store[best_index][4][0])
-    basket = domain_resizer(variables.domain_iteration[best_index], basket)
-    basket = multi_annotater(basket)
 
-    return basket, iterator_store[best_index][1], iterator_store[best_index][4]
-
-
-def gene_essentiality_compressor():
+    return best_index, iterator_store[best_index][1], iterator_store[best_index][4]
 
+def gene_essentiality_compressor(basket,genes_list):
+    
     essentials = pd.read_csv(f"{variables.directory}/{variables.output_name}.csv",
-                             skiprows=9)
+                             skiprows=9,low_memory=False)
 
     classifier = {'Essential': 1,
                   'Likelly Essential': 2,
                   'Probably Essential': 3,
                   'too small for assaying': 4,
                   'Non-Essential': 5}
 
@@ -1427,38 +1511,58 @@
     for gene_name, i in zip(essentials['Gene ID'], essentials.index):
         if gene_name in binned_essentiality:
             for j in range(1, 6):  # from the classifier dict
                 if j in binned_essentiality[gene_name]:
                     essentials.loc[i, 'Full gene essentiality'] = [
                         n for n in classifier if classifier[n] == j][0]
                     break
+    
+    final_out = [["Gene ID"] + ["Gene Name"] + ["Gene Orientation"] +
+                  ["Contig"] + ["Gene Lenght"] + ["Gene Product"] +
+                  ["Total Number of insertions"] + ["Essentiality"]]
 
-    essentials.to_csv(
-        f"{variables.directory}/{variables.output_name}_final.csv", index=False)
-
+    for gene in basket:
+        final_out.append([basket[gene].identity] +
+                          [basket[gene].gene] +
+                          [basket[gene].orientation] +
+                          [basket[gene].contig] +
+                          [basket[gene].length] +
+                          [basket[gene].product] +
+                          [sum(basket[gene].domain_insertions_total)] +
+                          [essentials[essentials["Gene ID"]==gene]["Full gene essentiality"].iloc[0]])
+    
+    output_writer(variables.directory, f"{variables.output_name}_final", final_out)
 
 def main(argv):
     ''' This function is the main function that calls all the other 
     functions in the program. It takes in a list of command-line arguments as 
     input (argv), sets up the necessary inputs and paths, loads the genome 
     sequence data, parses the transposon insertion data, constructs a basket 
     of genes, generates a matrix of gene insertions, iterates over different 
     domain sizes and identifies the optimal one, compiles the final results, 
     and prints the start and end times of the program execution. '''
-
-    print(f"\nStarting at: {datetime.datetime.now().strftime('%c')}")
+    
     inputs(argv)
     path_finder()
-    genome_loader()
-    insertions_parser()
+    genome_loader(startup=True)
+    insertions_parser(startup=True)
+    evaluator_basket = blast_maker()
+    if (len(variables.true_positives) != 0) and (len(variables.true_negatives) != 0):
+        evaluator_basket = gene_insertion_matrix(evaluator_basket)
+        best_index, pvalue, euclidean_points = domain_iterator(evaluator_basket)
+    else:
+        best_index, pvalue, euclidean_points = 0,variables.pvalue,[[[0,0],[0,0]]]
+
+    genome_loader(startup=False) # create a cleaner version where this doesnt need to repeat
+    insertions_parser(startup=False)
     basket = basket_storage()
     basket = gene_insertion_matrix(basket)
-    best_basket, pvalue, euclidean_points = domain_iterator(basket)
+    best_basket = domain_resizer(variables.domain_iteration[best_index], basket)
+    best_basket = multi_annotater(best_basket)
     final_compiler(best_basket, pvalue, euclidean_points)
-    print(f"Ended on: {datetime.datetime.now().strftime('%c')}")
 
 
 if __name__ == "__main__":
     if len(sys.argv) > 2:
         argv = sys.argv[1:]
     main(argv)
     multiprocessing.set_start_method("spawn")
```

### Comparing `tnseeker-1.0.5/tnseeker/__main__.py` & `tnseeker-1.0.7/tnseeker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os,glob
 import subprocess
 import multiprocessing
 from tnseeker import Essential_Finder,reads_trimer,sam_to_insertions,insertions_over_genome_plotter
 import argparse
-import time
+import datetime
 
 ''' Tnseeker is a pipeline for transposon insertion sequencing (Tn-Seq) analysis. 
     It performs various operations such as trimming the reads, 
     aligning the reads to a reference genome, extracting essential genes, 
     and plotting the insertions over the genome.
     
     The pipeline is started by calling the `variables_initializer()` function, 
@@ -101,15 +101,15 @@
     
         cpus = cpu()[1]
         send = ["bowtie2",
                 "--end-to-end",
                 "-x",f"{variables['index_dir']}{variables['strain']}",
                 "-U",f"{variables['fastq_trimed']}",
                 "-S",f"{variables['directory']}/alignment.sam",
-                "--no-unal",
+               # "--no-unal",
                 f"--threads {cpus}",
                 f"2>'{variables['directory']}/bowtie_align_log.log'"]
         
         subprocess_cmd(send)
         
     else:
         print(f'Found {variables["directory"]}/alignment.sam, skipping alignment')
@@ -124,15 +124,15 @@
         cpus = cpu()[1]
         send = ["bowtie2",
                 "--end-to-end",
                 "-x",f"{variables['index_dir']}{variables['strain']}",
                 "-1",f"{variables['fastq_trimed'][0]}",
                 "-2",f"{variables['fastq_trimed'][1]}",
                 "-S",f"{variables['directory']}/alignment.sam",
-                "--no-unal",
+                #"--no-unal",
                 f"--threads {cpus}",
                 f"2>'{variables['directory']}/bowtie_align_log.log'"]
         
         subprocess_cmd(send)
         
     else:
         print(f'Found {variables["directory"]}/alignment.sam, skipping alignment')
@@ -239,16 +239,16 @@
                                 f"{variables['intergenic_size_cutoff']}"])
 
 def essentials(variables):
     Essential_Finder.main([f'{variables["directory"]}',
                            f'{variables["strain"]}',
                            f'{variables["annotation_type"]}',
                            f'{variables["annotation_folder"]}',
-                           f'{variables["subdomain_length_down"]}',
                            f'{variables["subdomain_length_up"]}',
+                           f'{variables["subdomain_length_down"]}',
                            f'{variables["pvalue"]}',
                            f"{variables['intergenic_size_cutoff']}",
                            f"{variables['domain_uncertain_threshold']}"])
 
 def insertions_plotter(variables):     
     insertions_over_genome_plotter.main([f'{variables["directory"]}',
                                          f'{variables["seq_file"]}',
@@ -289,22 +289,22 @@
     parser.add_argument("--ig",nargs='?',const=0,help="The number of bp up and down stream of any gene to be considered an intergenic region")
     parser.add_argument("--dut",nargs='?',const=0,help="fraction of the minimal amount of 'too small domains' in a gene before the entire gene is deemed uncertain for essentiality inference")
     parser.add_argument("--pv",nargs='?',const=None,help="Essential Finder pvalue threshold for essentiality determination")
     parser.add_argument("--sl5",nargs='?',const=None,help="5' gene trimming percent for essentiality determination (number between 0 and 1)")
     parser.add_argument("--sl3",nargs='?',const=None,help="3' gene trimming percent for essentiality determination (number between 0 and 1)")
     
     args = parser.parse_args()
-
-    if (args.s is None) or (args.sd is None) or (args.ad is None) or (args.at is None) or (args.st is None):
-        print(parser.print_usage())
-        raise ValueError("No arguments given")
     
-    variables["version"]="1.0.5"
+    variables["version"]="1.0.7"
     print(f'\nVersion: {variables["version"]}\n')
     
+    if (args.s is None) or (args.sd is None) or (args.ad is None) or (args.at is None) or (args.st is None):
+        print(parser.print_usage())
+        raise ValueError("No arguments given")
+
     variables["full"]=True
     if args.e is not None:
         variables["full"] = False
         print("Running in essentials finder only mode\n")
         
     variables["trim"]=False
     variables["tn_mismatches"] = 0 
@@ -377,19 +377,19 @@
     if args.pv is not None:
         variables["pvalue"]=args.pv
         
     variables["domain_uncertain_threshold"]=0.75
     if args.dut is not None:
         variables["domain_uncertain_threshold"]=float(args.dut)
     
-    variables["subdomain_length_up"]=1
+    variables["subdomain_length_up"]=0
     if args.sl5 is not None:
         variables["subdomain_length_up"]=args.sl5
         
-    variables["subdomain_length_down"]=0
+    variables["subdomain_length_down"]=1
     if args.sl3 is not None:
         variables["subdomain_length_down"]=args.sl3
     
     if args.st == "PE":
         variables["sequencing_files_r"] = args.sd_2
         
     variables["sequencing_files"] = args.sd
@@ -410,14 +410,16 @@
     cmd_printer_path = os.path.join(variables['directory'],'cmd_input' + ".txt")
     with open(cmd_printer_path,'w+') as current:
         for key in variables:
             current.write(str(key)+':'+str(variables[key])+'\n')
     return variables
 
 def main():
+    print(f"\nStarting at: {datetime.datetime.now().strftime('%c')}")
+    
     variables = variables_initializer()
     
     if variables["full"]:
         variables = bowtie_index_maker(variables)
 
         if variables["seq_type"] == "PE":
             
@@ -442,17 +444,21 @@
                 
             print("Aligning Sequences")
             bowtie_aligner_maker_single(variables)
         
         print("Parsing insertions")
         sam_parser(variables)
         if variables["remove"]:
+            if variables["barcode"]:
+                os.remove(f"{variables['directory']}/barcoded_align.sam")
             os.remove(f"{variables['directory']}/alignment.sam")
     
         insertions_plotter(variables)
     
     if variables["essential_find"]:
         print("Finding Essentials")
         essentials(variables)
+        
+    print(f"Ended on: {datetime.datetime.now().strftime('%c')}")
     
 if __name__ == "__main__":
     main()
```

### Comparing `tnseeker-1.0.5/tnseeker/extras/possion_binom.py` & `tnseeker-1.0.7/tnseeker/extras/possion_binom.py`

 * *Files identical despite different names*

### Comparing `tnseeker-1.0.5/tnseeker/insertions_over_genome_plotter.py` & `tnseeker-1.0.7/tnseeker/insertions_over_genome_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,19 @@
                 else:
                     contig = line[1:-1]
                     genome_seq[contig] = 0
     else:
         for rec in SeqIO.parse(annotation, "gb"):
             genome_seq[rec.id] = len(rec.seq)
           
-    cmap = matplotlib.cm.get_cmap('jet') #gnuplot
+    cmap = matplotlib.colormaps['jet'] #gnuplot
     colour = ['.9','.6']*len(genome_seq)
     
     fig, ax = plt.subplots()  
+    ax.remove()
     grid = plt.GridSpec(1, 5, wspace=0.4, hspace=0.3)
     ax=plt.subplot(grid[0, :4])
     ax.set_ylim(1, 1000000)
     incremental_position=0
     genome_seq={k: v for k, v in sorted(genome_seq.items(), reverse=True,key=lambda item: item[1])}
     
     for i,contig in enumerate(genome_seq):
@@ -203,12 +204,13 @@
                y=np.log(df['reads']),
                fill=True, common_norm=False,
                alpha=.5, linewidth=0)
 
     adjust_spines(ax2, ['left', 'bottom'], (0, ax2.get_xlim()[1]), (ax2.get_ylim()))
     
     plt.savefig(f"{directory}/reads.png", dpi=300,bbox_inches='tight')
+    plt.close()
 
 if __name__ == "__main__":
     if len(sys.argv) > 2:
         argv = [sys.argv[1]]+[sys.argv[2]]+[sys.argv[3]]+[sys.argv[4]]
     main(argv)
```

### Comparing `tnseeker-1.0.5/tnseeker/reads_trimer.py` & `tnseeker-1.0.7/tnseeker/reads_trimer.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,20 +107,21 @@
                 read[3] = quality[start:end]
             else:
                 read[1] = sequence[start:]
                 read[3] = quality[start:]
 
             if (len(quality_set.intersection(quality)) == 0):
                 read[0],read[2] = str(read[0],"utf-8"),str(read[2],"utf-8")
+                read[0] = read[0].split(" ")[0]
                 processed_read.append(read)
                 if barcode_allow:
                     barcode = barcodeID(sequence,sequence_bin,borders,miss_up,miss_down)
                     if barcode is not None:
                         if (len(quality_set_bar_up.intersection(quality)) == 0) & (len(quality_set_bar_down.intersection(quality)) == 0):
-                            barcode_pool.append([barcode]+[read[0]])
+                            barcode_pool.append([f"{barcode}{read[0]}"])
 
     return [processed_read,barcode_pool]
                 
 def cpu():
     c = multiprocessing.cpu_count()
     if c >= 2:
         c -= 1
```

### Comparing `tnseeker-1.0.5/tnseeker/sam_to_insertions.py` & `tnseeker-1.0.7/tnseeker/sam_to_insertions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import csv
 import numpy as np
 import os, glob
 from regex import findall
 from matplotlib import pyplot as plt
 import argparse
 from Bio import SeqIO
+import multiprocessing
+import pkg_resources
+import subprocess
 
 """ This script processes and analyzes sequencing data from a SAM (Sequence Alignment/Map) file. 
     The main purpose is to extract information about transposon insertions in a given genome 
     and generate statistics, including the read histogram, for further analysis.
     
     Here's a high-level overview of the code:
 
@@ -120,47 +123,41 @@
     
     return statstics
 
 class Insertion():
     
     def __init__(self, contig=None, local=None, border=None, orientation=None,\
                  count=None,barcode=None,name=None,product=None,gene_orient=None,
-                 relative_gene_pos=None,mapQ=0):
+                 relative_gene_pos=None,mapQ=0,read_id=None):
         
         self.contig = contig
         self.local = local
         self.orientation = orientation
         self.seq = border
         self.count = count
         self.mapQ = mapQ
         self.barcode = barcode or {}
         self.name = name
         self.product = product
         self.gene_orient = gene_orient
         self.relative_gene_pos = relative_gene_pos
+        self.read_id = read_id
 
-def insertion_counter(current, contig, local, orientation, border):
-
-    compiled_local = contig + local + orientation
-    
-    if compiled_local not in current: 
-        current[compiled_local] = Insertion(contig, local, orientation, border, 1)
-        
-    else: 
-        current[compiled_local].count += 1
-
-    return current
-
-def read_count(dictionary):
-    count = 0
-
-    for key in dictionary:
-        count += dictionary[key].count
-        
-    return count
+def cpu():
+    c = multiprocessing.cpu_count()
+    if c >= 2:
+        c -= 1
+    pool = multiprocessing.Pool(processes = c)
+    return pool, c
+
+def subprocess_cmd(command):
+    try:
+        return subprocess.check_output(command)
+    except subprocess.CalledProcessError as e:
+        return e.output.decode()
 
 def extractor(name_folder, folder_path, pathing, paired_ended,barcode,\
               read_threshold,read_cut,annotation_file,ir_size_cutoff,map_quality_threshold = 42):
     
     def barcode_finder():
         read = ""
         barcode = {}
@@ -182,128 +179,182 @@
 
     aligned_reads, aligned_valid_reads = 0, 0
     insertion_count = {}
     
     flag_list = [0, 16]
     if paired_ended=="PE":
         flag_list = [83, 99] #[16] for single ended data #99 and 83 means that the read is the first in pair (only paired ended reads are considered as valid)
-
-    if barcode:
-        redundancy_barcode = {}
-        read_to_barcode = barcode_finder()
     
-    for file in pathing:
-        with open(file) as current:
-            for line in current:
-                sam = line.split('\t')
-                if (sam[0][0] != "@") and (sam[2] != '*'): #ignores headers and unaligned contigs
-                    local = sam[3]
-                    sequence = sam[9] 
-                    contig = sam[2]
-                    flag = int(sam[1])
-                    cigar = sam[5]
-                    map_quality = float(sam[4])
-                    border, orientation = "",""
-                    aligned_reads += 1
-                    multi = "XS:i:" in sam #multiple alignemnts
+    file = pathing[0]
+    if barcode:
+        print("Linking barcodes to insertion positions")
+        file = f"{folder_path}/barcoded_align.sam"
+        subprocess_cmd([pkg_resources.resource_filename(__name__, 'data/barcode2sam.sh'),
+                       f"{folder_path}/alignment.sam",
+                       f"{folder_path}/barcodes_1.txt",
+                       file,
+                       folder_path])
+        
+    with open(file) as current:
+        for line in current:
+            sam = line.split('\t')
+            if (sam[0][0] != "@") and (sam[2] != '*'): #ignores headers and unaligned contigs
+                local = sam[3]
+                sequence = sam[9] 
+                contig = sam[2]
+                flag = int(sam[1])
+                cigar = sam[5]
+                map_quality = float(sam[4])
+                border, orientation = "",""
+                aligned_reads += 1
+                multi = "XS:i:" in sam #multiple alignemnts
+
+                if (flag in flag_list) & (multi==False) & (map_quality >= map_quality_threshold): #only returns aligned reads witht he proper flag score
                     
-                    if (flag in flag_list) & (multi==False) & (map_quality >= map_quality_threshold): #only returns aligned reads witht he proper flag score
-                        
-                        aligned_valid_reads += 1
-                        
-                        if flag == flag_list[0]: #first read in pair oriented 5'to 3' (positive)
-                            orientation = "+"
-                            border = sequence[:2] 
-    
-                        elif flag == flag_list[1]: #first read in pair oriented 3'to 5' (negative)
-                            orientation = "-"
-                            border = sequence[::-1][:2] #needs to be reversed to make sure the start position is always the same
-
-                            #for CIGAR
-                            matches = findall(r'(\d+)([A-Z]{1})', cigar)
-                            clipped = 0
-                            for match in matches:
-                                if match[1] == "S":
-                                    clipped=int(match[0])
-                                    break #only consideres the first one at the start
-
-                            local=str(int(local)+len(sequence)-clipped)
-
-                        key = (contig, local, orientation)
-                        if key not in insertion_count: 
-                            insertion_count[key] = Insertion(contig=key[0], 
-                                                             local=key[1], 
-                                                             orientation=key[2], 
-                                                             count=1, 
-                                                             border=border,
-                                                             mapQ=map_quality)
-                        else: 
-                            insertion_count[key].count += 1
-                            insertion_count[key].mapQ += map_quality
-
-                        if barcode:
-                            if sam[0] in read_to_barcode:
-                                bar = read_to_barcode[sam[0]]
-                                if bar in insertion_count[key].barcode:
-                                    insertion_count[key].barcode[bar] += 1
-                                else:
-                                    insertion_count[key].barcode[bar] = 1
-                                    
-                                key = (contig, local, orientation, bar)
-                                if key in redundancy_barcode:
-                                    redundancy_barcode[key] = False
-                                else:
-                                    redundancy_barcode[key] = True
+                    aligned_valid_reads += 1
+                    
+                    if flag == flag_list[0]: #first read in pair oriented 5'to 3' (positive)
+                        orientation = "+"
+                        border = sequence[:2] 
+
+                    elif flag == flag_list[1]: #first read in pair oriented 3'to 5' (negative)
+                        orientation = "-"
+                        border = sequence[::-1][:2] #needs to be reversed to make sure the start position is always the same
+
+                        #for CIGAR
+                        matches = findall(r'(\d+)([A-Z]{1})', cigar)
+                        clipped = 0
+                        for match in matches:
+                            if match[1] == "S":
+                                clipped=int(match[0])
+                                break #only consideres the first one at the start
+
+                        local=str(int(local)+len(sequence)-clipped-1) # -1 to offsset bowtie alignement
+
+                    key = (contig, local, orientation)
+                    if key not in insertion_count: 
+                        insertion_count[key] = Insertion(contig=key[0], 
+                                                         local=key[1], 
+                                                         orientation=key[2], 
+                                                         count=1, 
+                                                         border=border,
+                                                         mapQ=map_quality)
+                    else: 
+                        insertion_count[key].count += 1
+                        insertion_count[key].mapQ += map_quality
+                    
+                    if barcode:
+                        bar = None
+                        if "BC:Z:" in sam[-1]:
+                            bar = sam[-1][:-1].split(":")[2]
+                        if bar != None:
+                            if bar in insertion_count[key].barcode:
+                                insertion_count[key].barcode[bar] += 1
+                            else:
+                                insertion_count[key].barcode[bar] = 1
+
+    for key in insertion_count:
+        insertion_count[key].mapQ = insertion_count[key].mapQ / insertion_count[key].count    
+
+    pool,cpus = cpu()
+    len_insertion_count_divider = int(len(insertion_count) / cpus)
+    batch_goals = {}
+    for i in range(cpus):
+        batch_goals[i] = set()
+        for j,key in enumerate(insertion_count):
+            if j >= len_insertion_count_divider * i:
+                if i != cpus-1:
+                    if len(batch_goals[i]) <= len_insertion_count_divider:
+                        batch_goals[i].add(key)
+                    else:
+                        break
+                else:
+                    batch_goals[i].add(key)
+
+    result_objs = []
+    for batch in batch_goals:
+
+        insertion_count_filtered = {}
+        for key in insertion_count:
+            if key in batch_goals[batch]:
+                insertion_count_filtered[key] = insertion_count[key]
+
+        result=pool.apply_async(annotation_processer, 
+                            args=((insertion_count_filtered, 
+                                   read_threshold,
+                                   read_cut,
+                                   barcode,
+                                   annotation_file,
+                                   ir_size_cutoff,
+                                   name_folder,
+                                   folder_path)))
+    
+        result_objs.append(result)
+    pool.close()
+    pool.join()
+        
+    result = [result.get() for result in result_objs]
+    
+    final_compiler = {}
+    barcoded_insertions_final = []
+    insertions_final = []
+
+    for entry in result:
+        insertion,barcoded,insert = entry
+        final_compiler = {**final_compiler, **insertion}
+        if barcode:
+            for a,b in zip(barcoded,insert):
+                barcoded_insertions_final.append(a)
+                insertions_final.append(b)
 
-    if read_threshold:
-        insertion_count,redundancy_barcode=dict_filter(insertion_count,read_cut,redundancy_barcode,barcode)
-    
-    if (annotation_file.endswith(".gb")) or (annotation_file.endswith(".gbk")):
-        insertion_count = gene_parser_genbank(annotation_file,insertion_count)
-        
-    elif annotation_file.endswith(".gff"):
-        insertion_count = gene_parser_gff(annotation_file,insertion_count)
-        
-    insertion_count = inter_gene_annotater(annotation_file,insertion_count,ir_size_cutoff)
-    
     if barcode:
-        insert_parser(insertion_count,name_folder,folder_path)
+        annotate_barcodes_writer(barcoded_insertions_final,insertions_final,name_folder,folder_path)
         
-    dictionary_parser(insertion_count,barcode,folder_path,name_folder)
+    dictionary_parser(final_compiler,barcode,folder_path,name_folder)
         
     q = plotter(insertion_count, f"Unique insertions_{name_folder}", folder_path)
 
     reads = f"Total Aligned Reads: {aligned_reads}\nTotal Quality Passed Reads: {aligned_valid_reads}\nFiltered Vs. Raw Read % ratio: {round(aligned_valid_reads/aligned_reads*100,2)}%\n"
-    
     e = "Number of total unique insertions: {}\n".format(len(insertion_count))
-    count = read_count(insertion_count)
-    f = f"Total number of reads attributed to unique insertions: {count}\n"
-    print(reads,e,f)
+    print(reads,e)
+
+    with open("{}/library_stats_{}.txt".format(folder_path,name_folder), "w+") as current:
+        current.write(reads+q+e)
+
+def annotation_processer(insertion_count_filtered,read_threshold,read_cut,
+                         barcode,annotation_file,ir_size_cutoff,name_folder,folder_path):
+
+    if read_threshold:
+        insertion_count_filtered=dict_filter(insertion_count_filtered,read_cut,barcode)
     
-    if barcode:
-        os.remove(f"{folder_path}/barcodes_1.txt")
+    if (annotation_file.endswith(".gb")) or (annotation_file.endswith(".gbk")):
+        insertion_count_filtered,genes,contigs = gene_parser_genbank(annotation_file,insertion_count_filtered)
+        
+    elif annotation_file.endswith(".gff"):
+        insertion_count_filtered,genes,contigs = gene_parser_gff(annotation_file,insertion_count_filtered)
+        
+    insertion_count_filtered = inter_gene_annotater(annotation_file,insertion_count_filtered,ir_size_cutoff,genes,contigs)
     
-    with open("{}/library_stats_{}.txt".format(folder_path,name_folder), "w+") as current:
-        current.write(reads+q+e+f)
+    barcoded_insertions,insertions = [],[]
+    if barcode:
+        barcoded_insertions,insertions = insert_parser(insertion_count_filtered,name_folder,folder_path)
 
-def dict_filter(dictionary,read_cut,redundancy_barcode,barcode):
+    return insertion_count_filtered,barcoded_insertions,insertions
+
+def dict_filter(dictionary,read_cut):
     for key in list(dictionary):
         if dictionary[key].count < read_cut:
             del dictionary[key]
-            if barcode:
-                for key1 in list(redundancy_barcode):
-                    if (key[0] == key1[0]) & (key[1] == key1[1]) & (key[2] == key1[2]):
-                        del redundancy_barcode[key1]
-    return dictionary,redundancy_barcode
+    return dictionary
 
 def insert_parser(insertion_count,name_folder,folder_path):    
     insertions,barcoded_insertions = [],[]
+
     for key in insertion_count: 
-        insertion_count[key].mapQ = insertion_count[key].mapQ / insertion_count[key].count
-        
+
         contig = [insertion_count[key].contig]
         local = [insertion_count[key].local]
         orientation = [insertion_count[key].orientation]
         count = [insertion_count[key].count]
         mapq = [insertion_count[key].mapQ]
         gene_name = [insertion_count[key].name]
         gene_product = [insertion_count[key].product]
@@ -319,14 +370,18 @@
             barcoded_insertions.append([bar] + [read] + contig + local +\
                                        orientation + count + mapq + gene_name + \
                                        gene_product + gene_orientation + relative_gene_pos)
             
         insertions.append(contig + local + orientation + count + mapq + \
                           gene_name + gene_product + gene_orientation + relative_gene_pos + \
                           [len(insertion_count[key].barcode)] + [reads] + [barcodes])
+            
+    return barcoded_insertions,insertions
+
+def annotate_barcodes_writer(barcoded_insertions,insertions,name_folder,folder_path):
     
     insertions.insert(0, ["#Contig"] + ["position"] + ["Orientation"] + ["Total Reads"] + \
                       ["Average MapQ"] + ["Gene Name"] + ["Gene Product"] + ["Gene Orientation"] + \
                       ["Relative Position in Gene (0-1)"] + ["Number of different barcodes in coordinate"] + \
                       ["Total barcode Reads"] + ["Barcodes (barcode:read)"])
     
     name = f"barcoded_insertions_{name_folder}.csv"
@@ -344,84 +399,16 @@
         
     name = f"annotated_barcodes_{name_folder}.csv"
     output_file_path = os.path.join(folder_path, name)
     with open(output_file_path, "w", newline='') as output:
         writer = csv.writer(output)
         writer.writerows(barcoded_insertions)
 
-def inter_gene_annotater(annotation_file,insertion_count,ir_size_cutoff):
-    
-    contigs = {}
-    genes = []
-    if annotation_file.endswith(".gff"):
-        with open(annotation_file) as current:
-            for line in current:
-                GB = line.split('\t') #len(GB)
-                if "#" not in GB[0][:3]: #ignores headers
+def inter_gene_annotater(annotation_file,insertion_count,ir_size_cutoff,genes,contigs):
 
-                    start = int(GB[3])
-                    end = int(GB[4])
-
-                    features = GB[8].split(";") #gene annotation file
-                    feature = {}
-                    for entry in features:
-                        entry = entry.split("=")
-                        feature[entry[0]] = entry[1].replace("\n","")
-                    if "gene" in feature:
-                        gene=feature["gene"]
-                    if "Name" in feature:
-                        gene=feature["Name"]
-                    else:
-                        gene=feature["ID"]
-
-                    contig = GB[0]
-                    orientation = GB[6] #orientation of the gene
-                    
-                    key = (start,end,orientation,gene,contig)
-                    genes.append((start,end,orientation,gene,contig))
-                else:
-                    if "sequence-region" in GB[0]:
-                        GB = GB[0].split(" ")
-                        contigs[GB[-3]] = int(GB[-1][:-1])
-                
-                if "##FASTA" in GB[0]:
-                    break
-    else:
-        for rec in SeqIO.parse(annotation_file, "gb"):
-            for feature in rec.features:
-                if feature.type != 'source':
-                    start = feature.location.start
-                    end = feature.location.end
-                    orientation = feature.location.strand
-                    if orientation == -1:
-                        orientation = '-'
-                    else:
-                        orientation = '+'
-                    try:
-                        identity = feature.qualifiers['locus_tag'][0]
-                    except KeyError:
-                        identity = 'Undefined'
-                        
-                    for key, val in feature.qualifiers.items():   
-                        if "pseudogene" in key:
-                            gene = identity
-                            break 
-                        elif "gene" in key:
-                            gene = feature.qualifiers['gene'][0]
-                            break 
-                        else:
-                            gene = identity
-                            
-                    key = (start,end,orientation,gene,rec.id)
-                    genes.append((start,end,orientation,gene,rec.id))
-            contigs[rec.id] = len(rec.seq)
-    
-    genes = list(dict.fromkeys(genes))
-    genes.sort(key=lambda x: (x[-1], x[0])) #sort by start position of the gene and contig
-    
     ir_annotation = {}
     count = 0
     for i,gene in enumerate(genes[:-1]):
         contig = gene[-1]
         if contig == genes[i+1][-1]: #same contigs
             gene_down_start_border = ir_size_cutoff + gene[1]
             gene_up_start_border = genes[i+1][0] - ir_size_cutoff
@@ -442,33 +429,35 @@
 
             domain_size = genes[i+1][0] - ir_size_cutoff
             if domain_size  >= 1:
                 count += 1
                 ir_name = f'IR_{count}_contig-start_{genes[0][3]}_{gene[2]}'
                 if ir_name not in ir_annotation:
                    ir_annotation[ir_name] = (0,genes[0][0],domain_size,contig)
-
+    
     for ir in ir_annotation:
         for key in insertion_count:
             if insertion_count[key].name is None:
                 if insertion_count[key].contig == ir_annotation[ir][3]:
                     if (int(insertion_count[key].local) >= ir_annotation[ir][0]) & (int(insertion_count[key].local) <= ir_annotation[ir][1]):
                         insertion_count[key].name = ir
                         insertion_count[key].relative_gene_pos = (int(insertion_count[key].local) - ir_annotation[ir][0]) / ir_annotation[ir][2]
-
+             
     return insertion_count
 
 def gene_parser_genbank(annotation_file,insertion_count):
     
     ''' The gene_info_parser_genbank function takes a genbank file as input and 
     extracts gene information, storing it in a dictionary with Gene class 
     instances as values. It parses the file using the SeqIO module, 
     retrieving attributes such as start, end, orientation, identity, 
     and product for each gene.''' 
     
+    contigs = {}
+    genes = []
     for rec in SeqIO.parse(annotation_file, "gb"):
         for feature in rec.features:
             if feature.type != 'source':
                 start = feature.location.start
                 end = feature.location.end
                 domain_size = end - start
                 
@@ -497,27 +486,34 @@
                         gene = identity
                         break #avoids continuing the iteration and passing to another key, which would make "gene" assume another value
                     elif "gene" in key:
                         gene = feature.qualifiers['gene'][0]
                         break #avoids continuing the iteration and passing to another key, which would make "gene" assume another value
                     else:
                         gene = identity
-                
+
+                genes.append((start,end,orientation,gene,rec.id))
+
                 for key in insertion_count:
                     if insertion_count[key].contig == rec.id:
                         if (int(insertion_count[key].local) >= start) & (int(insertion_count[key].local) <= end):
                             insertion_count[key].name = gene
                             insertion_count[key].product = product
                             insertion_count[key].gene_orient = orientation
                             insertion_count[key].relative_gene_pos = (int(insertion_count[key].local) - start) / domain_size
-                      
-    return insertion_count
+
+        contigs[rec.id] = len(rec.seq)
+        genes = list(dict.fromkeys(genes))
+        genes.sort(key=lambda x: (x[-1], x[0])) #sort by start position of the gene and contig
+    return insertion_count,genes,contigs
 
 def gene_parser_gff(annotation_file,insertion_count):
     
+    contigs = {}
+    genes = []
     with open(annotation_file) as current:
         for line in current:
             GB = line.split('\t') #len(GB)
             
             if "##FASTA" in GB[0]:
                 break
             
@@ -527,15 +523,16 @@
                 end = int(GB[4])
                 domain_size = end - start
                 
                 features = GB[8].split(";") #gene annotation file
                 feature = {}
                 for entry in features:
                     entry = entry.split("=")
-                    feature[entry[0]] = entry[1].replace("\n","")
+                    if len(entry) == 2:
+                        feature[entry[0]] = entry[1].replace("\n","")
                 if "gene" in feature:
                     gene=feature["gene"]
                 if "Name" in feature:
                     gene=feature["Name"]
                 else:
                     gene=feature["ID"]
                     
@@ -551,44 +548,55 @@
                 for key in insertion_count:
                     if insertion_count[key].contig == contig:
                         if (int(insertion_count[key].local) >= start) & (int(insertion_count[key].local) <= end):
                             insertion_count[key].name = gene
                             insertion_count[key].product =  feature['product']
                             insertion_count[key].gene_orient = orientation
                             insertion_count[key].relative_gene_pos = (int(insertion_count[key].local) - start) / domain_size
-                      
-    return insertion_count
+                            
+                contig = GB[0]
+                orientation = GB[6] #orientation of the gene
+                
+                key = (start,end,orientation,gene,contig)
+                genes.append(key)
+
+            if "sequence-region" in GB[0]:
+                GB = GB[0].split(" ")
+                contigs[GB[-3]] = int(GB[-1][:-1])
+                
+        genes = list(dict.fromkeys(genes))
+        genes.sort(key=lambda x: (x[-1], x[0])) #sort by start position of the gene and contig
+        
+    return insertion_count,genes,contigs
 
 def dictionary_parser(dictionary,barcode,folder_path,name_folder):
     
     insertions = []
 
     for key in dictionary:
-        if not barcode:
-            dictionary[key].mapQ = dictionary[key].mapQ / dictionary[key].count
-        
+
         contig = [dictionary[key].contig]
         local = [dictionary[key].local]
         orientation = [dictionary[key].orientation]
         border = [dictionary[key].seq]
         count = [dictionary[key].count]
         gene_name = [dictionary[key].name]
         gene_product = [dictionary[key].product]
         gene_orientation = [dictionary[key].gene_orient]
         relative_gene_pos = [dictionary[key].relative_gene_pos]
         mapQ = [dictionary[key].mapQ]
         
         insertions.append(contig + local + orientation + border + count + mapQ +\
                           gene_name + gene_product + gene_orientation + relative_gene_pos)
-            
+
     insertions.insert(0, ["#Contig"] + ["position"] + ["Orientation"] + \
                       ["Transposon Border Sequence"] + ["Read Counts"] + \
                       ["Average mapQ across reads"] + ["Gene Name"] + ["Gene Product"] + \
                       ["Gene Orientation"] + ["Relative Position in Gene (0-1)"])
-    
+
     getNextFilePath(folder_path, "all_insertions_"+name_folder, insertions) #all the unique insertions
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Process SAM aligned files and extract relevant information.")
     parser.add_argument("folder_path", help="Path to the folder containing SAM files.")
     parser.add_argument("name_folder", help="Name of the folder.")
     parser.add_argument("paired_ended", help="Type of data: 'PE' for paired-end or 'SE' for single-end.")
```

### Comparing `tnseeker-1.0.5/tnseeker.egg-info/PKG-INFO` & `tnseeker-1.0.7/tnseeker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: tnseeker
-Version: 1.0.5
+Version: 1.0.7
 Summary: TnSeeker
 Home-page: https://github.com/afombravo/tnseeker
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 Keywords: tn-seq,essentiality,rb-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.19.2
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numba>=0.53.1
-Requires-Dist: biopython>=1.81
-Requires-Dist: datetime
-Requires-Dist: argparse
-Requires-Dist: regex
-Requires-Dist: multiprocess
-Requires-Dist: pathlib
-Requires-Dist: scipy>=1.6.2
-Requires-Dist: seaborn>=0.12.1
-Requires-Dist: statsmodels>=0.12.2
+Requires-Dist: numpy==1.26.4
+Requires-Dist: matplotlib==3.8.2
+Requires-Dist: pandas==2.2.0
+Requires-Dist: numba==0.59.0
+Requires-Dist: biopython==1.83
+Requires-Dist: datetime==5.4
+Requires-Dist: argparse==1.4.0
+Requires-Dist: regex==2023.12.25
+Requires-Dist: multiprocess==0.70.16
+Requires-Dist: pathlib==1.0.1
+Requires-Dist: scipy==1.12.0
+Requires-Dist: seaborn==0.13.2
+Requires-Dist: statsmodels==0.14.1
 
 # Tnseeker
 Tnseeker is an advanced pipeline tailored for transposon insertion sequencing (Tn-Seq) analysis. It performs an array of tasks: from read trimming and alignment to associating genomic locations with transposon insertions, and inferring essential genes based on transposon insertion densities. Additionally, Tnseeker is adept at extracting barcodes from raw fastq files and linking them to corresponding transposon genomic locations for subsequent analysis. What truly distinguishes Tnseeker from other tools is its unique capability to automatically infer and adjust threshold/cutoff parameters. This negates the need for intricate user input, allowing for a more precise determination of gene essentiality based on the data. Compatible with any transposon disruption experiment, Tnseeker efficiently mitigates transposon-specific biases, including those seen with HIMAR. Hence, Tnseeker is versatile enough to handle all Tn-Seq datasets.
 
 Tnseeker is under active developement and is available as is. Contact me if you are interested in using the program or have any questions. Bugs can be expected. Please report any weird or unintented behaviour. 
 
 ## Requirements
```

