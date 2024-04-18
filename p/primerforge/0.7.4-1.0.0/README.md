# Comparing `tmp/primerforge-0.7.4.tar.gz` & `tmp/primerforge-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerforge-0.7.4.tar", last modified: Thu Mar 28 13:54:01 2024, max compression
+gzip compressed data, was "primerforge-1.0.0.tar", last modified: Thu Apr 18 18:10:50 2024, max compression
```

## Comparing `primerforge-0.7.4.tar` & `primerforge-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,25 @@
-drwx------   0 uma2     (1000984939) users      (529)        0 2024-03-28 13:54:01.813331 primerforge-0.7.4/
--rw-r--r--   0 uma2     (1000984939) users      (529)    11357 2024-01-11 14:26:06.000000 primerforge-0.7.4/LICENSE
--rw-r--r--   0 uma2     (1000984939) users      (529)     5305 2024-03-28 13:54:01.805939 primerforge-0.7.4/PKG-INFO
--rw-------   0 uma2     (1000984939) users      (529)     4793 2024-03-28 13:52:13.000000 primerforge-0.7.4/README.md
-drwx------   0 uma2     (1000984939) users      (529)        0 2024-03-28 13:54:01.723102 primerforge-0.7.4/bin/
--rw-------   0 uma2     (1000984939) users      (529)     9634 2024-03-13 14:57:21.000000 primerforge-0.7.4/bin/AnalysisData.py
--rw-------   0 uma2     (1000984939) users      (529)     6973 2024-03-28 12:55:56.000000 primerforge-0.7.4/bin/Clock.py
--rw-------   0 uma2     (1000984939) users      (529)     2354 2024-03-13 14:57:21.000000 primerforge-0.7.4/bin/Log.py
--rw-------   0 uma2     (1000984939) users      (529)    25046 2024-03-28 13:50:50.000000 primerforge-0.7.4/bin/Parameters.py
--rw-------   0 uma2     (1000984939) users      (529)     4585 2024-03-28 11:37:43.000000 primerforge-0.7.4/bin/Primer.py
--rw-------   0 uma2     (1000984939) users      (529)        0 2024-03-28 13:10:22.000000 primerforge-0.7.4/bin/__init__.py
--rw-------   0 uma2     (1000984939) users      (529)    14444 2024-03-13 14:57:21.000000 primerforge-0.7.4/bin/analysis.py
--rw-------   0 uma2     (1000984939) users      (529)    18304 2024-03-28 11:37:43.000000 primerforge-0.7.4/bin/getCandidateKmers.py
--rw-------   0 uma2     (1000984939) users      (529)    16993 2024-03-28 11:37:43.000000 primerforge-0.7.4/bin/getPrimerPairs.py
--rwx------   0 uma2     (1000984939) users      (529)    18470 2024-03-28 13:10:22.000000 primerforge-0.7.4/bin/main.py
--rw-------   0 uma2     (1000984939) users      (529)    10527 2024-03-28 11:37:43.000000 primerforge-0.7.4/bin/removeOutgroupPrimers.py
-drwx------   0 uma2     (1000984939) users      (529)        0 2024-03-28 13:54:01.759489 primerforge-0.7.4/bin/unit_tests/
--rw-------   0 uma2     (1000984939) users      (529)    13645 2024-03-08 03:16:52.000000 primerforge-0.7.4/bin/unit_tests/analysisData_test.py
--rw-r--r--   0 uma2     (1000984939) users      (529)     3384 2024-03-06 13:57:42.000000 primerforge-0.7.4/bin/unit_tests/clock_test.py
--rw-------   0 uma2     (1000984939) users      (529)    17061 2024-03-13 14:57:21.000000 primerforge-0.7.4/bin/unit_tests/parameters_test.py
--rw-------   0 uma2     (1000984939) users      (529)    10172 2024-03-28 11:37:43.000000 primerforge-0.7.4/bin/unit_tests/primer_test.py
--rw-------   0 uma2     (1000984939) users      (529)    46130 2024-03-28 13:10:22.000000 primerforge-0.7.4/bin/unit_tests/results_test.py
-drwx------   0 uma2     (1000984939) users      (529)        0 2024-03-28 13:54:01.799831 primerforge-0.7.4/primerforge.egg-info/
--rw-r--r--   0 uma2     (1000984939) users      (529)     5305 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/PKG-INFO
--rw-------   0 uma2     (1000984939) users      (529)      594 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/SOURCES.txt
--rw-------   0 uma2     (1000984939) users      (529)        1 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/dependency_links.txt
--rw-------   0 uma2     (1000984939) users      (529)       46 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/entry_points.txt
--rw-------   0 uma2     (1000984939) users      (529)       68 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/requires.txt
--rw-------   0 uma2     (1000984939) users      (529)        4 2024-03-28 13:54:01.000000 primerforge-0.7.4/primerforge.egg-info/top_level.txt
--rw-------   0 uma2     (1000984939) users      (529)       38 2024-03-28 13:54:01.814347 primerforge-0.7.4/setup.cfg
--rw-------   0 uma2     (1000984939) users      (529)      775 2024-03-28 13:10:22.000000 primerforge-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 18:10:43.000000 primerforge-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-18 18:10:50.584383 primerforge-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-18 18:10:43.000000 primerforge-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/AnalysisData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Primer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/getCandidateKmers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/getPrimerPairs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18470 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/removeOutgroupPrimers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/primerforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:10:50.584383 primerforge-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 18:10:43.000000 primerforge-1.0.0/setup.py
```

### Comparing `primerforge-0.7.4/LICENSE` & `primerforge-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/PKG-INFO` & `primerforge-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: primerforge
-Version: 0.7.4
+Version: 1.0.0
 Summary: software to identify primers that can be used to distinguish genomes
 Author: Joseph S. Wirth
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biopython==1.81
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: numpy
-Requires-Dist: primer3-py>=2.0
-Requires-Dist: scipy>=1.10
 
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
-### pip installation
+### `pip` installation
 ```shell
-pip install primerForge
+pip install primerforge
+```
+
+### `conda` installation
+```shell
+conda install -c bioconda primerforge
 ```
 
 ### Manual installation
 
 > [!NOTE]
 > This might take up to ten minutes.
 
@@ -90,25 +90,27 @@
                 GC{"GC in
                  range?"}
                 Tm{"Tm in
                 range?"}
                 homo{"repeats
                 ≤ 3bp?"}
                 hair{"no hairpins?"}
-                GC-->Tm-->homo-->hair
+                dime{"no homo-
+                dimers?"}
+                GC-->Tm-->homo-->hair-->dime
             end
         end
     end
 
     %% connections up to candidate kmers
     sharedKmers --> B
     dump1[/"dump to file"/]
     sharedKmers --> dump1
     candidates(["unique, shared kmers; one per start position"])
-    hair --> candidates
+    dime --> candidates
 
     %% get primer pairs
     subgraph C["for each genome"]
         bin1["bin overlapping kmers (64bp max)"]
         bin2["get bin pairs"]
         candPair(["candidate primer pairs"])
         sharePair(["shared primer pairs"])
@@ -116,29 +118,33 @@
         %% evaluate one kmer pair
         subgraph C0["for each bin pair"]
             size{"is PCR
             size ok?"}
             subgraph C4["for each primer pair"]
                 prime{"is 3' end
                 G or C?"}
+                temp{"is Tm
+                difference ok?"}
+                hetero{"no hetero-
+                dimers?"}
             end
             size --> C4
         end
 
 
         %% get shared primer pairs
         subgraph C2["for each candidate primer pair"]
             subgraph C3["for each other genome"]
                 pcr{"PCR size ok?"}
             end
         end
 
         bin1 --> bin2
         bin2 --> C0
-        prime --> candPair
+        prime --> temp --> hetero --> candPair
         candPair --> C2
         pcr --> sharePair
     end
 
     allSharePair(["all shared primer pairs"])
     dump2[/"dump to file"/]
     dump3[/"dump to file"/]
```

### Comparing `primerforge-0.7.4/README.md` & `primerforge-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
-### pip installation
+### `pip` installation
 ```shell
-pip install primerForge
+pip install primerforge
+```
+
+### `conda` installation
+```shell
+conda install -c bioconda primerforge
 ```
 
 ### Manual installation
 
 > [!NOTE]
 > This might take up to ten minutes.
 
@@ -74,25 +79,27 @@
                 GC{"GC in
                  range?"}
                 Tm{"Tm in
                 range?"}
                 homo{"repeats
                 ≤ 3bp?"}
                 hair{"no hairpins?"}
-                GC-->Tm-->homo-->hair
+                dime{"no homo-
+                dimers?"}
+                GC-->Tm-->homo-->hair-->dime
             end
         end
     end
 
     %% connections up to candidate kmers
     sharedKmers --> B
     dump1[/"dump to file"/]
     sharedKmers --> dump1
     candidates(["unique, shared kmers; one per start position"])
-    hair --> candidates
+    dime --> candidates
 
     %% get primer pairs
     subgraph C["for each genome"]
         bin1["bin overlapping kmers (64bp max)"]
         bin2["get bin pairs"]
         candPair(["candidate primer pairs"])
         sharePair(["shared primer pairs"])
@@ -100,29 +107,33 @@
         %% evaluate one kmer pair
         subgraph C0["for each bin pair"]
             size{"is PCR
             size ok?"}
             subgraph C4["for each primer pair"]
                 prime{"is 3' end
                 G or C?"}
+                temp{"is Tm
+                difference ok?"}
+                hetero{"no hetero-
+                dimers?"}
             end
             size --> C4
         end
 
 
         %% get shared primer pairs
         subgraph C2["for each candidate primer pair"]
             subgraph C3["for each other genome"]
                 pcr{"PCR size ok?"}
             end
         end
 
         bin1 --> bin2
         bin2 --> C0
-        prime --> candPair
+        prime --> temp --> hetero --> candPair
         candPair --> C2
         pcr --> sharePair
     end
 
     allSharePair(["all shared primer pairs"])
     dump2[/"dump to file"/]
     dump3[/"dump to file"/]
```

### Comparing `primerforge-0.7.4/bin/AnalysisData.py` & `primerforge-1.0.0/bin/AnalysisData.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/Clock.py` & `primerforge-1.0.0/bin/Clock.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,13 +224,20 @@
         # restart the clock
         self.restart()
     
     def printDone(self) -> None:
         """prints the end message and the duration
         """
         # stop spinning the wheel if necessary
-        if self.__spin:
-            self.__WHEEL.stop()
-            
+        self._killWheel()
+        
         # print the done string
         print(f"done {self.getTimeString()}")
         sys.stdout.flush()
+    
+    def _killWheel(self) -> None:
+        """kills any spinning clocks
+        """
+        try:
+            self.__WHEEL.stop()
+        except:
+            pass
```

### Comparing `primerforge-0.7.4/bin/Log.py` & `primerforge-1.0.0/bin/Log.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/Parameters.py` & `primerforge-1.0.0/bin/Parameters.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/Primer.py` & `primerforge-1.0.0/bin/Primer.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/analysis.py` & `primerforge-1.0.0/bin/analysis.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/getCandidateKmers.py` & `primerforge-1.0.0/bin/getCandidateKmers.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/getPrimerPairs.py` & `primerforge-1.0.0/bin/getPrimerPairs.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/bin/main.py` & `primerforge-1.0.0/bin/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bin.AnalysisData import AnalysisData
 from bin.getCandidateKmers import _getAllCandidateKmers
 from bin.removeOutgroupPrimers import _removeOutgroupPrimers
 from bin.getPrimerPairs import _getPrimerPairs, _keepOnePairPerBinPair
 from bin.analysis import _initializeAnalysisData, _updateAnalysisData, _plotAnalysisData
 
 # global constants
-__version__ = "0.7.4"
+__version__ = "1.0.0"
 __author__ = "Joseph S. Wirth"
 __SHARED_NUM = 0
 __CAND_NUM   = 1
 __PAIR_1_NUM = 2
 __PAIR_2_NUM = 3
 __PAIR_3_NUM = 4
 __ANAL_NUM   = 5
```

### Comparing `primerforge-0.7.4/bin/removeOutgroupPrimers.py` & `primerforge-1.0.0/bin/removeOutgroupPrimers.py`

 * *Files identical despite different names*

### Comparing `primerforge-0.7.4/primerforge.egg-info/PKG-INFO` & `primerforge-1.0.0/primerforge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: primerforge
-Version: 0.7.4
+Version: 1.0.0
 Summary: software to identify primers that can be used to distinguish genomes
 Author: Joseph S. Wirth
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biopython==1.81
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: numpy
-Requires-Dist: primer3-py>=2.0
-Requires-Dist: scipy>=1.10
 
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
-### pip installation
+### `pip` installation
 ```shell
-pip install primerForge
+pip install primerforge
+```
+
+### `conda` installation
+```shell
+conda install -c bioconda primerforge
 ```
 
 ### Manual installation
 
 > [!NOTE]
 > This might take up to ten minutes.
 
@@ -90,25 +90,27 @@
                 GC{"GC in
                  range?"}
                 Tm{"Tm in
                 range?"}
                 homo{"repeats
                 ≤ 3bp?"}
                 hair{"no hairpins?"}
-                GC-->Tm-->homo-->hair
+                dime{"no homo-
+                dimers?"}
+                GC-->Tm-->homo-->hair-->dime
             end
         end
     end
 
     %% connections up to candidate kmers
     sharedKmers --> B
     dump1[/"dump to file"/]
     sharedKmers --> dump1
     candidates(["unique, shared kmers; one per start position"])
-    hair --> candidates
+    dime --> candidates
 
     %% get primer pairs
     subgraph C["for each genome"]
         bin1["bin overlapping kmers (64bp max)"]
         bin2["get bin pairs"]
         candPair(["candidate primer pairs"])
         sharePair(["shared primer pairs"])
@@ -116,29 +118,33 @@
         %% evaluate one kmer pair
         subgraph C0["for each bin pair"]
             size{"is PCR
             size ok?"}
             subgraph C4["for each primer pair"]
                 prime{"is 3' end
                 G or C?"}
+                temp{"is Tm
+                difference ok?"}
+                hetero{"no hetero-
+                dimers?"}
             end
             size --> C4
         end
 
 
         %% get shared primer pairs
         subgraph C2["for each candidate primer pair"]
             subgraph C3["for each other genome"]
                 pcr{"PCR size ok?"}
             end
         end
 
         bin1 --> bin2
         bin2 --> C0
-        prime --> candPair
+        prime --> temp --> hetero --> candPair
         candPair --> C2
         pcr --> sharePair
     end
 
     allSharePair(["all shared primer pairs"])
     dump2[/"dump to file"/]
     dump3[/"dump to file"/]
```

### Comparing `primerforge-0.7.4/setup.py` & `primerforge-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='primerforge',
-    version='0.7.4',
+    version='1.0.0',
     author='Joseph S. Wirth',
     packages=find_packages(),
     description='software to identify primers that can be used to distinguish genomes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'biopython==1.81',
```

