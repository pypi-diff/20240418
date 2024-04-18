# Comparing `tmp/niceplotpy-0.8.0.tar.gz` & `tmp/niceplotpy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niceplotpy-0.8.0.tar", last modified: Fri Apr 12 09:48:41 2024, max compression
+gzip compressed data, was "niceplotpy-0.8.1.tar", last modified: Thu Apr 18 10:14:31 2024, max compression
```

## Comparing `niceplotpy-0.8.0.tar` & `niceplotpy-0.8.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2397 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.714411 niceplotpy-0.8.0/niceplot/
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3789 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.715411 niceplotpy-0.8.0/niceplot/data/
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     7579 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     3486 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     4423 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     5079 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw1dratio.py
--rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw2dhist.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw2dscatter.py
--rw-rw-rw-   0 root         (0) root         (0)     6716 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/process_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     8445 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/niceplotpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      771 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:14:31.722756 niceplotpy-0.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-18 10:14:31.722756 niceplotpy-0.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2397 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:14:31.720756 niceplotpy-0.8.1/niceplot/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3859 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:14:31.721756 niceplotpy-0.8.1/niceplot/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     4423 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/draw1dratio.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/draw2dhist.py
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/draw2dscatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/process_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/niceplot/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:14:31.722756 niceplotpy-0.8.1/niceplotpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      771 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 10:14:31.000000 niceplotpy-0.8.1/niceplotpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 10:14:31.722756 niceplotpy-0.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-18 10:14:17.000000 niceplotpy-0.8.1/setup.py
```

### Comparing `niceplotpy-0.8.0/PKG-INFO` & `niceplotpy-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplotpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package collecting things to make nice plots from root files
 Home-page: https://gitlab.cern.ch/jwuerzin/nice-plot
 Author: Jonas Wuerzinger
 Author-email: jonas.wuerzinger@tum.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `niceplotpy-0.8.0/README.md` & `niceplotpy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/__main__.py` & `niceplotpy-0.8.1/niceplot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,18 @@
                 x=plot.x,
                 denominator=plot.denominator,
                 numerator=plot.numerator,
                 denomlab=utils.getaddinfo(reader.configurations, plot.denominator),
                 numlab=utils.getaddinfo(reader.configurations, plot.numerator),
                 nbins=plot.nbins,
                 range=plot.range,
+                xlab=plot.xlab,
                 ylab=plot.ylab,
                 suffix=f"{plot.denominator}_over_{plot.numerator}",
+                addinfo=plot.addinfo,
                 logy=plot.logy,
                 output_dir=reader.output_dir,
                 subdir=plot.subdir
             ) 
         elif plot.type == '2dhist':
             # Make one 2D (exclusion) Histogram for every dataframe configuration:
             for config in reader.configurations:
```

### Comparing `niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv` & `niceplotpy-0.8.1/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv` & `niceplotpy-0.8.1/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv` & `niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv` & `niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv` & `niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv` & `niceplotpy-0.8.1/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/draw1dratio.py` & `niceplotpy-0.8.1/niceplot/draw1dratio.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
   ax_top.legend(handles=[(new_handles[0], band_num), (new_handles[1], band_denom)] , labels=labels, loc='upper right')
 
   # Make ratio and error:  
   ratio, ratioerr = utils.saferatio(hist_num, hist_den)
   ax_bottom.errorbar(bincenters, ratio, yerr=ratioerr, fmt='ko', label='ratio', markersize=4, zorder=2)
   
   # Add dashed line at 1.0
-  xlinearr = np.linspace(ax_bottom.get_xlim()[0], ax_bottom.get_xlim()[1], 1000)
+  xlinearr = np.linspace(ax_top.get_xlim()[0], ax_top.get_xlim()[1], 1000)
   ylinearr = np.ones(1000)
   ax_bottom.plot(xlinearr, ylinearr, linestyle='dashed', color='grey', zorder=1)
   
   if logy:
     ax_top.set_yscale('log')
     ax_top.set_ylim(1., 2*max( [max(hist_den), max(hist_num)]) )
   else:
```

### Comparing `niceplotpy-0.8.0/niceplot/draw2dhist.py` & `niceplotpy-0.8.1/niceplot/draw2dhist.py`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/draw2dscatter.py` & `niceplotpy-0.8.1/niceplot/draw2dscatter.py`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/process_yaml.py` & `niceplotpy-0.8.1/niceplot/process_yaml.py`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/niceplot/reader.py` & `niceplotpy-0.8.1/niceplot/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import uproot
 import time
 import pandas
+import awkward as ak
 
 from niceplot.process_yaml import read_yaml
 
 class DotAccessibleDict:
     """Class for making dicts accessible by dots."""
     def __init__(self, dictionary):
         self._dict = dictionary
@@ -110,15 +111,17 @@
         dfdict = {}
         for config in self.configurations:
             starttime = time.time()
             # build one df for every configuration; copy other df if seed is provided.
             if config.seedfrom is not None:
                 dfdict[config.name] = dfdict[config.seedfrom]
             else:
-                dfdict[config.name] = susy.arrays(grab_columns, library='pd')
+                # Use uproot to read into simple pandas df. Might want to move to akarrays if performance issues arise for jagged inputs:
+                # dfdict[config.name] = susy.arrays(grab_columns, library='pd')
+                dfdict[config.name] = ak.to_dataframe(susy.arrays(grab_columns, library='ak'))
             
             # Add new variables to dataframe:
             if config.newvar is not None:
                 for var in config.newvar:
                     dfdict[config.name] = self.addnewvar(dfdict[config.name], var.varname, var.formula)  
             
             print(f"Time to read {config.name} into df: {time.time() - starttime:.2f} s")
```

### Comparing `niceplotpy-0.8.0/niceplot/utils.py` & `niceplotpy-0.8.1/niceplot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,19 +119,19 @@
         'GM2' : ["", "\\mathrm{ (GM2)}"],
     }
     
     for substr in string.split("_"):
         if substr in matchdict:
             leftlist += [matchdict[substr][0]]
             rightlist += [matchdict[substr][1]]
-        else:
-            leftlist += ["\\mathrm{"+substr+"}"]
-        # TODO: If no match found, might want to return input string instead:
+        # TODO: If no match found, might want to return input string instead of only using partials
         # else:
-        #     return string
+        #     leftlist += ["\\mathrm{"+substr+"}"]
+        else:
+            return string
     
     # Piece together full string from both lists:
     rightlist.reverse()
     fullstr = '$'+''.join(leftlist + rightlist)+'$'
     
     # Give last pass to re-change everything that may have been messed up by auto-gen:
     partdict = {
```

### Comparing `niceplotpy-0.8.0/niceplotpy.egg-info/PKG-INFO` & `niceplotpy-0.8.1/niceplotpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplotpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package collecting things to make nice plots from root files
 Home-page: https://gitlab.cern.ch/jwuerzin/nice-plot
 Author: Jonas Wuerzinger
 Author-email: jonas.wuerzinger@tum.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `niceplotpy-0.8.0/niceplotpy.egg-info/SOURCES.txt` & `niceplotpy-0.8.1/niceplotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.8.0/setup.py` & `niceplotpy-0.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='niceplotpy',
-    version='0.8.0',
+    version='0.8.1',
     description='A package collecting things to make nice plots from root files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.cern.ch/jwuerzin/nice-plot',
     author='Jonas Wuerzinger',
     author_email='jonas.wuerzinger@tum.de',
     packages=find_packages(),
     package_data={'': ['data/*.csv']},
     install_requires=['numpy',
                       'Click',
                       'matplotlib>=3.7.2',
                       'pyyaml',
-                      'uproot',
+                      'uproot>=5.0',
+                      'awkward>=2.6.3',
                       'pandas',
                       'atlasify',
                       'importlib-metadata',
                       'tqdm'
                       ],
 
     classifiers=[
```

