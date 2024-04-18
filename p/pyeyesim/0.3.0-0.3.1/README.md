# Comparing `tmp/pyeyesim-0.3.0.tar.gz` & `tmp/pyeyesim-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeyesim-0.3.0.tar", last modified: Tue Mar 12 16:58:36 2024, max compression
+gzip compressed data, was "pyeyesim-0.3.1.tar", last modified: Thu Apr 18 14:06:29 2024, max compression
```

## Comparing `pyeyesim-0.3.0.tar` & `pyeyesim-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-03-12 16:58:36.333078 pyeyesim-0.3.0/
--rw-r--r--   0 aratoj87   (501) staff       (20)     2684 2024-03-12 16:58:36.332908 pyeyesim-0.3.0/PKG-INFO
-drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-03-12 16:58:36.331783 pyeyesim-0.3.0/PyEyeSim/
--rw-r--r--   0 aratoj87   (501) staff       (20)    10022 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/__init__.py
--rw-r--r--   0 aratoj87   (501) staff       (20)    21582 2024-03-12 16:31:23.000000 pyeyesim-0.3.0/PyEyeSim/_comparegroups.py
--rw-r--r--   0 aratoj87   (501) staff       (20)    15435 2024-03-12 16:10:16.000000 pyeyesim-0.3.0/PyEyeSim/_dataproc.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     9028 2024-03-12 15:39:08.000000 pyeyesim-0.3.0/PyEyeSim/_hmm.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     5888 2024-03-12 16:31:01.000000 pyeyesim-0.3.0/PyEyeSim/_scanpathsim.py
--rw-r--r--   0 aratoj87   (501) staff       (20)    14228 2024-03-12 14:45:23.000000 pyeyesim-0.3.0/PyEyeSim/_stats.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     8963 2024-03-12 16:39:31.000000 pyeyesim-0.3.0/PyEyeSim/_visuals.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     1770 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/hmmhelper.py
--rw-r--r--   0 aratoj87   (501) staff       (20)    72855 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/pyeyesim.py
--rw-r--r--   0 aratoj87   (501) staff       (20)    71530 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/pyeyesim_old.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     4457 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/scanpathshelpdebug.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     4371 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/scanpathsimhelper.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     1801 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/statshelper.py
--rw-r--r--   0 aratoj87   (501) staff       (20)       28 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/test.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     3400 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/PyEyeSim/visualhelper.py
--rw-r--r--   0 aratoj87   (501) staff       (20)     2091 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/README.md
-drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-03-12 16:58:36.332661 pyeyesim-0.3.0/pyeyesim.egg-info/
--rw-r--r--   0 aratoj87   (501) staff       (20)     2684 2024-03-12 16:58:36.000000 pyeyesim-0.3.0/pyeyesim.egg-info/PKG-INFO
--rw-r--r--   0 aratoj87   (501) staff       (20)      539 2024-03-12 16:58:36.000000 pyeyesim-0.3.0/pyeyesim.egg-info/SOURCES.txt
--rw-r--r--   0 aratoj87   (501) staff       (20)        1 2024-03-12 16:58:36.000000 pyeyesim-0.3.0/pyeyesim.egg-info/dependency_links.txt
--rw-r--r--   0 aratoj87   (501) staff       (20)       43 2024-03-12 16:58:36.000000 pyeyesim-0.3.0/pyeyesim.egg-info/requires.txt
--rw-r--r--   0 aratoj87   (501) staff       (20)        9 2024-03-12 16:58:36.000000 pyeyesim-0.3.0/pyeyesim.egg-info/top_level.txt
--rw-r--r--   0 aratoj87   (501) staff       (20)      553 2024-03-12 16:57:50.000000 pyeyesim-0.3.0/pyproject.toml
--rw-r--r--   0 aratoj87   (501) staff       (20)       38 2024-03-12 16:58:36.333114 pyeyesim-0.3.0/setup.cfg
--rw-r--r--   0 aratoj87   (501) staff       (20)      243 2024-03-07 13:33:34.000000 pyeyesim-0.3.0/setup.py
+drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-04-18 14:06:29.806364 pyeyesim-0.3.1/
+-rw-r--r--   0 aratoj87   (501) staff       (20)     2684 2024-04-18 14:06:29.806205 pyeyesim-0.3.1/PKG-INFO
+drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-04-18 14:06:29.805219 pyeyesim-0.3.1/PyEyeSim/
+-rw-r--r--   0 aratoj87   (501) staff       (20)    10525 2024-04-18 14:06:08.000000 pyeyesim-0.3.1/PyEyeSim/__init__.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)    28987 2024-04-18 14:06:08.000000 pyeyesim-0.3.1/PyEyeSim/_comparegroups.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)    14659 2024-04-18 12:52:10.000000 pyeyesim-0.3.1/PyEyeSim/_dataproc.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     9028 2024-04-15 11:46:12.000000 pyeyesim-0.3.1/PyEyeSim/_hmm.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     7750 2024-04-15 14:53:06.000000 pyeyesim-0.3.1/PyEyeSim/_scanpathsim.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)    14383 2024-04-18 12:52:10.000000 pyeyesim-0.3.1/PyEyeSim/_stats.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     9903 2024-04-17 10:50:26.000000 pyeyesim-0.3.1/PyEyeSim/_visuals.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     1770 2024-03-07 13:33:34.000000 pyeyesim-0.3.1/PyEyeSim/hmmhelper.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)    72855 2024-04-10 13:33:29.000000 pyeyesim-0.3.1/PyEyeSim/pyeyesim.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)    71530 2024-03-07 13:33:34.000000 pyeyesim-0.3.1/PyEyeSim/pyeyesim_old.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     4457 2024-04-10 13:33:29.000000 pyeyesim-0.3.1/PyEyeSim/scanpathshelpdebug.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     4371 2024-04-10 13:33:29.000000 pyeyesim-0.3.1/PyEyeSim/scanpathsimhelper.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     2235 2024-04-17 08:18:26.000000 pyeyesim-0.3.1/PyEyeSim/statshelper.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)       28 2024-04-10 13:32:40.000000 pyeyesim-0.3.1/PyEyeSim/test.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     3504 2024-04-18 12:52:10.000000 pyeyesim-0.3.1/PyEyeSim/visualhelper.py
+-rw-r--r--   0 aratoj87   (501) staff       (20)     2091 2024-04-10 13:33:29.000000 pyeyesim-0.3.1/README.md
+drwxr-xr-x   0 aratoj87   (501) staff       (20)        0 2024-04-18 14:06:29.806027 pyeyesim-0.3.1/pyeyesim.egg-info/
+-rw-r--r--   0 aratoj87   (501) staff       (20)     2684 2024-04-18 14:06:29.000000 pyeyesim-0.3.1/pyeyesim.egg-info/PKG-INFO
+-rw-r--r--   0 aratoj87   (501) staff       (20)      539 2024-04-18 14:06:29.000000 pyeyesim-0.3.1/pyeyesim.egg-info/SOURCES.txt
+-rw-r--r--   0 aratoj87   (501) staff       (20)        1 2024-04-18 14:06:29.000000 pyeyesim-0.3.1/pyeyesim.egg-info/dependency_links.txt
+-rw-r--r--   0 aratoj87   (501) staff       (20)       43 2024-04-18 14:06:29.000000 pyeyesim-0.3.1/pyeyesim.egg-info/requires.txt
+-rw-r--r--   0 aratoj87   (501) staff       (20)        9 2024-04-18 14:06:29.000000 pyeyesim-0.3.1/pyeyesim.egg-info/top_level.txt
+-rw-r--r--   0 aratoj87   (501) staff       (20)      553 2024-04-17 15:12:47.000000 pyeyesim-0.3.1/pyproject.toml
+-rw-r--r--   0 aratoj87   (501) staff       (20)       38 2024-04-18 14:06:29.806405 pyeyesim-0.3.1/setup.cfg
+-rw-r--r--   0 aratoj87   (501) staff       (20)      243 2024-03-07 13:33:34.000000 pyeyesim-0.3.1/setup.py
```

### Comparing `pyeyesim-0.3.0/PKG-INFO` & `pyeyesim-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeyesim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Eye movement analysis and visualization package, with a focus on fixation map and scanpath similarity
 Author: jozsef arato
 Author-email: Jozsef Arato <jozsef.arato@gmail.com>
 Project-URL: Homepage, https://github.com/jozsarato/PyEyeSim
 Project-URL: Issues, https://github.com/jozsarato/PyEyeSim/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/__init__.py` & `pyeyesim-0.3.1/PyEyeSim/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,49 +9,48 @@
 import numpy as np
 import pandas as pd
 #% import  library helper functions
 
 from .visualhelper import MeanPlot,HistPlot
 
 from .statshelper import ScanpathL
-
+import warnings
 
 class EyeData:
 	
-    from ._visuals import VisScanPath,MySaccadeVis,VisLOOHMM,VisHMM,MyTrainTestVis,VisGrid,Hihglight_Sign
-    from ._dataproc import GetParams,GetStimuli,GetFixationData,GetDurations,GetGroups,GetCats,GetSaccades,GetEntropies,InferSize,Heatmap,FixCountCalc
+    from ._visuals import VisScanPath,MySaccadeVis,VisLOOHMM,VisHMM,MyTrainTestVis,VisGrid,Highlight_Sign,VisHeatmap
+    from ._dataproc import GetParams,GetStimuli,GetFixationData,GetDurations,GetGroups,GetCats,GetSaccades,GetEntropies,InferSize,Heatmap,FixCountCalc,GetStimSubjMap
     from ._stats import AngleCalc,AngtoPix,PixdoDeg,Entropy,FixDurProg,BinnedCount,GetInddiff,GetInddiff_v2,RunDiffDivs,GetBinnedStimFixS,StatPDiffInd2,StatPDiffInd1,CalcStatPs,CalcRets,CalcImmRets,BinnedDescriptives
-    from ._comparegroups import CompareGroupsFix,CompareWithinGroupsFix,FixDurProgGroups,BinnedDescriptivesGroups,CompareGroupsMat,CompareGroupsGridFix
-    from ._scanpathsim import AOIFix,SacSimPipeline,SacSim1Group,SaccadeSel
+    from ._comparegroups import CompareGroupsFix,CompareWithinGroupsFix,FixDurProgGroups,BinnedDescriptivesGroups,CompareGroupsMat,CompareGroupsGridFix,CompareStimHeatmap,CompareStimGridFix
+    from ._scanpathsim import AOIFix,SacSimPipeline,SacSim1Group,SaccadeSel,ScanpathSim2Groups
 
     try: 
-    	from ._hmm import DataArrayHmm,MyTrainTest,FitLOOHMM,FitVisHMM,FitVisHMMGroups,HMMSimPipeline
+        from ._hmm import DataArrayHmm,MyTrainTest,FitLOOHMM,FitVisHMM,FitVisHMMGroups,HMMSimPipeline
     except:
-    	print('hmmlearn not found, hidden markov model functionality will not work')
+        warnings.warn('hmmlearn not found, hidden markov model functionality will not work')
         
     try: 
         from ._comparegroups import CompareGroupsHeatmap
     except:
-        
-    	print('scikit image not found, compare groups heatmap will not work - scikit image needed for downsampling')
+        warnings.warn('scikit image not found, compare groups heatmap will not work - scikit image needed for downsampling')
 
 
     def __init__(self, name, design,data,x_size,y_size):
         ''' 
         Description: initalizing eye-tracking data object.
         
         Arguments:
         name (str): A name associated with the eye-tracking data.
         design (str): Information about the study design.
         data (pandas.DataFrame): The eye-tracking data.
         x_size (int): Screen size in pixels (width).
         y_size (int): Screen size in pixels (height).
         '''
         self.name = name
-        self.design = design
+        self.design = design  # remove design ?
         self.data=data
         self.x_size=x_size
         self.y_size=y_size
 
 
         print('dataset size: ',np.shape(self.data))
         print('study design: ',self.design)
@@ -77,59 +76,66 @@
 
     def data(self):
         ''' 
         Description: shows dataset.
         '''
         return self.data
     
+
+    def setColumns(self,Stimulus='Stimulus',subjectID='subjectID',mean_x='mean_x',mean_y='mean_y',FixDuration=0):
+        if type(FixDuration)!='int':
+            self.data=self.data.rename(columns={Stimulus:'Stimulus',subjectID:'subjectID',mean_x: 'mean_x',mean_y: 'mean_y',FixDuration: 'duration'})
+        else:
+            self.data=self.data.rename(columns={Stimulus:'Stimulus',subjectID:'subjectID',mean_x: 'mean_x',mean_y: 'mean_y'})
+ 
+
+    def setStimuliPath(self, StimPath = None, StimExt='.jpg',infersubpath=False):
+        if StimPath == None:
+            warnings.warn('Stim path not provided')
+            return
+        
+        self.GetStimuli(StimExt,StimPath,infersubpath=infersubpath)
+        print('stimuli loaded succesfully, access as self.images')
+
     
-    
-    def DataInfo(self,Stimulus='Stimulus',subjectID='subjectID',mean_x='mean_x',mean_y='mean_y',FixDuration=0,StimPath=0,StimExt='.jpg',infersubpath=False):
+    def setSubjStim(self):
+        try:
+            subjs,stims=self.GetParams()
+            print('info found for '+ str(len(subjs))+' subjects, and '+str(len(stims))+' stimuli')      
+        except:
+            warnings.warn('stimulus and subject info not found')
+
+
+    def DataInfo(self,Stimulus='Stimulus',subjectID='subjectID',mean_x='mean_x',mean_y='mean_y',FixDuration=0,StimPath=None,StimExt='.jpg',infersubpath=False, Visual=False):
+
         ''' 
         Description: Provide information about amount of stimuli and subjects.
         Arguments:
         Stimulus (str): Column name for stimulus information in the eye-tracking data.
         subjectID (str): Column name for subject ID information in the eye-tracking data.
         mean_x (str): Column name for mean x-coordinate of fixations in the eye-tracking data.
         mean_y (str): Column name for mean y-coordinate of fixations in the eye-tracking data.
         FixDuration (int or str): Column name or integers for fixation duration in the eye-tracking data.
             If an integer, fixation duration column is assumed absent. It will be renamed "duration" afterwards
         StimPath (str): Path to stimuli. Set to 0 if not provided.
         StimExt (str): File extension of stimuli (default: '.jpg').
         infersubpath (bool): Flag to infer stimulus subpaths based on subject IDs (default: False).  -- if stimuli are stored in subfolders for multiple categories
         '''
-       # print(type(FixDuration))
-       
-        if type(FixDuration)!='int':
-            self.data=self.data.rename(columns={Stimulus:'Stimulus',subjectID:'subjectID',mean_x: 'mean_x',mean_y: 'mean_y',FixDuration: 'duration'})
-        else:
-            self.data=self.data.rename(columns={Stimulus:'Stimulus',subjectID:'subjectID',mean_x: 'mean_x',mean_y: 'mean_y'})
- 
-        try:
-            subjs,stims=self.GetParams()
-            print('info found for '+ str(len(subjs))+' subjects, and '+str(len(stims))+' stimuli')
-            
-        except:
-            print('stimulus and subject info not found')
-            
-        if StimPath==0:
-            print('Stim path not provided')
-        else:
-         #  try: 
-            self.GetStimuli(StimExt,StimPath,infersubpath=infersubpath)
-            print('stimuli loaded succesfully, access as self.images')
-          # except:   
-           #    print('stimuli not found')
+
+        #pipeline
+        self.setColumns(Stimulus,subjectID,mean_x,mean_y,FixDuration)
+
+        self.setSubjStim()      
+
+        self.setStimuliPath(StimPath,StimExt,infersubpath)
+
+        print('run descriptive analysis')
+        self.RunDescriptiveFix(Visual=Visual)
         pass
   
-    
-    
-    
-   
-    
 
     def RunDescriptiveFix(self,Visual=0,duration=0):
         '''
         Description:  Calculate descriptive statistics for fixation data in dataset.
 
         Arguments:
         Visual (int): Flag indicating whether to generate visual plots (default: 0). Use 1 to show plots.
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/_comparegroups.py` & `pyeyesim-0.3.1/PyEyeSim/_comparegroups.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 # not all functions can do both ---- yet  
 
 import numpy as np
 from numpy import matlib
 from scipy import stats,ndimage
 import pandas as pd
 import matplotlib.pyplot as plt
+import warnings
 
 import copy
 
 # import  library helper functions. 
-from .statshelper import SaliencyMapFilt,SaccadesTrial,ScanpathL,StatEntropy,BonfHolm
+from .statshelper import SaliencyMapFilt,SaccadesTrial,ScanpathL,StatEntropy,BonfHolm,ReduceCounts
 from .scanpathsimhelper import AOIbounds,CreatAoiRects,Rect,SaccadeLine,CalcSim ,CheckCoor
 from .visualhelper import VisBinnedProg,PlotDurProg,JointBinnedPlot,MeanPlot,draw_ellipse,HistPlot
 
 
 
 
 def CompareGroupsFix(self,betwcond):
@@ -94,207 +95,309 @@
                 print('Saccade amplitudes t=',np.round(t,4),', p=',np.round(p,4))
                 print(' ')
 
     
     return 
 
     
-def CompareGroupsHeatmap(self,Stim,betwcond,StimPath='',SD=25,CutArea=0,Conds=0,substring=False,cmap='plasma',alpha=.5,cutoff='median',downsample=8, Nrand=100):
+
+
+    
+    
+def CompareWithinGroupsFix(self,withinColName):
+    '''
+    Description: Run fixation comparisons within groups defined by a category column. Makes plots and prints descriptive stats.
+    
+    Arguments:
+    withinColName (str): The name of the categorical column defining groups for analysis.
+    '''
+    
+    WhichC=self.GetCats(withinColName)
+
+    if hasattr(self,'entropies')==False:   # check if entropy has already been calculated
+        print('Calculating entropy')
+        Entropies,self.entropmax,self.entropies_ind=self.GetEntropies()
+    #Cols=['darkred','cornflowerblue']
+#        plt.figure(figsize=(8,8))
+    
+    Entrs=[]
+    Fixies=[]
+    ScanpLs=[]
+    SaccAmpls=[] 
+    for cc,c in enumerate(self.WithinConds):
+        print(cc,'Category',c)
+        Idx=np.nonzero(WhichC==c)[0]
+        FixGr=np.array(self.nfix[:,Idx])
+        EntrGr=self.entropies_ind[:,Idx]
+        Entrs.append(np.nanmean(EntrGr,1))
+        Fixies.append(np.nanmean(FixGr,1))
+        ScanpLs.append(np.nanmean(self.len_scanpath[:,Idx],1))
+        SaccAmpls.append(np.nanmean(self.sacc_ampl[:,Idx],1))
+     
+        
+        print(cc,c,'Num fix= ',np.round(np.mean(np.nanmean(FixGr,1)),2),'+/-',np.round(np.std(np.nanmean(FixGr,1)),2))
+        print(cc,c,'Entropy= ',np.round(np.mean(np.nanmean(EntrGr,1)),2),'+/-',np.round(np.std(np.nanmean(EntrGr,1)),2))
+        print(cc,c,'tot scanpath len = ',np.round(np.mean(np.nanmean(self.len_scanpath[:,Idx],1)),2),'+/-',np.round(np.std(np.nanmean(self.len_scanpath[:,Idx],1)),2),'pix')
+        print(cc,c,'saccade amplitude = ',np.round(np.mean(np.nanmean(self.sacc_ampl[:,Idx],1)),2),'+/-',np.round(np.std(np.nanmean(self.sacc_ampl[:,Idx],1)),2),'pix')
+        print('')
+    return
+ 
+   
+def CompareGroupsHeatmap(self,Stim,betwcond,SD=25,CutArea=0,Conds=0,cmap_ind='plasma',cmap_diff='RdYlBu',cmap_abs='Greens',alpha=.5,cutoff='median',downsample=8, Nrand=100):
     ''' 
     DESCRIPTION: visualize  heatmap fopr two groups, 
     subplot 1: group 1
     subplot 2: group 2
     subplot 3: difference heatmap (raw value)
     subplot 4: difference heatmap (absolute value)
     
 
     ARGUMENTS:
     
-    Stim (str): The stimulus for which the heatmap is generated.
+    Stim (str): The stimulus name
     betwcond (str): The condition for between-group heatmap comparison.
-    
+
     
     OPTIONAL PARAMETERS
+    
     StimPath (str, optional): Path to the stimulus. Default is an empty string. if stimuli loaded before, this is not necessary
     SD (int, optional): Optional parameter for heatmap smoothness, in pixels. Default is 25.
     CutArea (int, optional): Cut fixations. For example if you use '1', it shows 99% percentile of fixations. Default is 0. SEt to 1, if stimulus does not cover the screen size eg: for  portrait orientation
     Conds (int or list, optional): use automatically detected conditions conditions, as provided in betweencond column
-        othewise Conds=['MyCond1' MyCond2'], if we want to specify the order of access for betweencond column.
+        othewise Conds=['MyCond1' MyCond2'], if we want to specify the order of access for betweencond column.  (could be useful if there are more then 2 conditions, and we want to select 2 to contrast)
     center: if stimulus area does not start at pixel 0, shifts image display using the plt.imshow(image, extent=)
-    cmap=colormap (see matplotlib colormaps for options: https://matplotlib.org/stable/users/explain/colors/colormaps.html)
+    cmap_ind=colormap for  each of the two group heatmaps (see matplotlib colormaps for options: https://matplotlib.org/stable/users/explain/colors/colormaps.html) (two top figures)
+    cmap_diff: colormap of difference heatmap (raw) in two directions (bottom left figure)
+    cmap_abs: colormap of absolute difference heatmap (bottom right figure)
+
     alpha= transparency- 0-1 higher values less transparent
     cutoff: shows areas below this threshold as blank
-    substring: match stimuli based on part of string --- if we want to compare two differently named stimuli, with part of the stimulus name matching
+    twostim: compare two similar stimuli, either provided as list or  match stimuli based on part of string --- if we want to compare two differently named stimuli, with part of the stimulus name matching
     downsample: downampling size 8 reduced by a factor of 8*8 pixels for example (using skimage)
     Nrand: number of random permutations to compute, default 100, for actual stats long run time and at least 1000 permutations are recommended, if set to 0 random permutation comparisonno performed
-    
+    # optional paramter to control color of difference heatmap
     '''
-    from skimage import measure
 
-    if substring:
-        self.stimuli=self.stimuli.astype('str')
-        stimn=np.char.find(self.stimuli,Stim)
-        Stims=self.stimuli[stimn>-1]
-        stimn=np.nonzero(stimn>-1)[0]
-        stimShow=Stims[0]
-        print('stimns found:',stimn,Stims)
-    else:
-        stimShow=copy.copy(Stim)
-
-    WhichC,WhichCN=self.GetGroups(betwcond)
-      
-    if hasattr(self,'boundsX')==0:
-        self.RunDescriptiveFix()
-    
     if hasattr(self,'subjects')==0:
-        self.GetParams()    
-    #Cols=['darkred','cornflowerblue']
-    fig,ax=plt.subplots(ncols=2,nrows=2,figsize=(10,8)) 
-    
-    if CutArea:
-        FixCounts=self.FixCountCalc(Stim,CutAct=1,substring=substring) 
-    else:
-        FixCounts=self.FixCountCalc(Stim,CutAct=0,substring=substring) 
+        self.GetParams()   
+        
+  
+
+    FixCounts=self.FixCountCalc(Stim,CutAct=CutArea) 
     assert np.sum(FixCounts)>0,'!!no fixations found'
     print('dimensions=',np.shape(FixCounts))
-    hmaps=[]
-    hmapsred=[]## reduced heatmaps, downsampled with scikit image (mean based downsampling)
+    Reduced=ReduceCounts(FixCounts,downsample)
 
-    red1=measure.block_reduce(FixCounts[0,:,:], (downsample,downsample), np.mean)  # just to get dimensions for the output
-    RedAll=np.zeros((np.shape(FixCounts)[0],np.shape(red1)[0],np.shape(red1)[1]))
-    for s in range(np.shape(FixCounts)[0]):
-        RedAll[s,:,:]=measure.block_reduce(FixCounts[s,:,:], (downsample,downsample), np.mean)
-        
-        
+    print('reduced dims',np.shape(Reduced))
+
+
+    WhichC,WhichCN=self.GetGroups(betwcond)
     if type(Conds)==int:    
         Conditions=np.copy(self.Conds)
     else:
-        print('use provided conditions: ' ,Conds)
+        print('use provided conditions: ' ,Conds) 
         Conditions=np.copy(Conds)
     N1=np.sum(WhichCN==Conditions[0])
-    N2=np.sum(WhichCN==Conditions[1])
     print(f'num observers in group 1: {N1}') 
-    print(f'num observers in group 2: {N2}') 
+    print(f'num observers in group 2: {np.sum(WhichCN==Conditions[1])}') 
 
+
+    fig,ax=plt.subplots(ncols=2,nrows=2,figsize=(10,8)) 
+    hmaps=[]
+    hmapsred=[]## reduced heatmaps, downsampled with scikit image (mean based downsampling)
     for cc,c in enumerate(Conditions):
+            
         Idx=np.nonzero(WhichCN==c)[0]   
-        if substring:
-            if np.sum(self.data.Stimulus[self.data['group']==self.Conds[cc]]==Stims[0])>0:
-                stims=Stims[0] # select which of the two  image files to show (assuming two similar named image files)
-            else:
-                stims=Stims[1]
-        else:
-            stims=copy.copy(Stim)
-        print(cc,c,stims)
-        hmap=self.Heatmap(stims,SD=SD,Ind=0,Vis=1,FixCounts=FixCounts[Idx,:,:],CutArea=CutArea,substring=False,ax=ax[0,cc],cmap=cmap,alpha=alpha,cutoff=cutoff)
+        heatmap=SaliencyMapFilt(FixCounts[Idx,:,:],SD=SD,Ind=0)
+        hmaps.append(heatmap)
+        
+        self.VisHeatmap(Stim,heatmap,ax=ax[0,cc],cutoff=cutoff,alpha=alpha,cmap=cmap_ind,title=c)
         
-        hmap_red=self.Heatmap(stims,SD=8,Ind=0,Vis=0,FixCounts=RedAll[Idx,:,:])#,CutArea=CutArea)
-        hmapsred.append(hmap_red)
         
-        ax[0,cc].set_title(c)
-       # ax[0,cc].colorbar()
-        hmaps.append(hmap)
-    if hasattr(self,'images'):
-        ax[1,0].imshow( self.images[stimShow])
+        redcount=ReduceCounts(FixCounts[Idx,:,:],downsample)
+        hmap_red=SaliencyMapFilt(redcount,SD=8,Ind=0)
+        hmapsred.append(hmap_red)
+   
+    # difference heatmp
+    Diff=hmaps[0]-hmaps[1]
+
 
     
-    Diff=hmaps[0]-hmaps[1]
+    colorbarlabel=str(Conditions[0])+'<---->'+str(Conditions[1])
+   
+    self.VisHeatmap(Stim,Diff,ax=ax[1,0],cutoff=cutoff,alpha=alpha,cmap=cmap_diff,cbar=True,cbarlabel=colorbarlabel,title='difference')
+    
+    self.VisHeatmap(Stim,np.abs(Diff),ax=ax[1,1],cutoff=cutoff,alpha=alpha,cmap=cmap_abs,cbar=True,cbarlabel=' ',title='absolute difference')
+    
+    
+    
     DiffRed=hmapsred[0]-hmapsred[1]
-    im=ax[1,0].imshow(Diff,cmap='RdBu', vmin=-np.nanmax(np.abs(Diff)), vmax=np.nanmax(np.abs(Diff)),alpha=alpha)
    
-    ax[1,0].set_title(str(Conditions[0])+' - '+str(Conditions[1]))
-    cbar=plt.colorbar(im,ax=ax[1,0], shrink=.6)
-    cbar.ax.get_yaxis().set_ticks([])
-    cbar.ax.get_yaxis().labelpad = 15
-    cbar.ax.set_ylabel(str(Conditions[0])+'<---->'+str(Conditions[1]), rotation=270)
-  
     ### calculate permuted difference heatmaps
     DiffPerm=np.zeros(Nrand)
     print(f'{Nrand} permutations starting')
     if Nrand>0:
         for n in range(Nrand):
-            Idxs=np.random.permutation(N1+N2)
-            hmap1=self.Heatmap(stims,SD=8,Ind=0,Vis=0,FixCounts=RedAll[Idxs[0:N1],:,:])#,CutArea=CutArea)
-            hmap2=self.Heatmap(stims,SD=8,Ind=0,Vis=0,FixCounts=RedAll[Idxs[N1:],:,:])#,CutArea=CutArea)
+            Idxs=np.random.permutation(np.shape(Reduced)[0])         
+            hmap1=SaliencyMapFilt(Reduced[Idxs[0:N1],:,:],SD=downsample,Ind=0)
+            hmap2=SaliencyMapFilt(Reduced[Idxs[N1:],:,:],SD=downsample,Ind=0)
             DiffPerm[n]=np.nansum(np.abs(hmap1-hmap2))
         
-    
-    if hasattr(self,'images'):
-       
-        ax[1,1].imshow(self.images[stimShow])
-    im=ax[1,1].imshow(np.abs(Diff), vmin=0, vmax=np.nanmax(np.abs(Diff)),alpha=alpha)
    
-    plt.colorbar(im,ax=ax[1,1], shrink=.6)
-    ax[1,1].set_title('Absolute diff: '+str(np.round(np.nansum(np.abs(Diff)),3)))
-    plt.tight_layout()
-    
-    for hora in range(2):
-        for vera in range(2):
-            ax[hora,vera].set_xlim(0,np.shape(self.images[stimShow])[1])
-            ax[hora,vera].set_ylim(np.shape(self.images[stimShow])[0],0)
 
-            ax[hora,vera].set_xticks([])
-            ax[hora,vera].set_yticks([])
-    
+
     truereddiff=np.nansum(np.abs(DiffRed))
     # visualize permuted difference heatmap distribution
     
     if Nrand>0:
-        fig,ax2=plt.subplots()
-        ax2.hist(DiffPerm,color='olive')
-        ax2.axvline(np.nansum(np.abs(DiffRed)),color='k')
-        ax2.text(truereddiff,Nrand/20,'true difference')
-        ax2.set_title(f' {Stim} permuted {Nrand} vs true diff - p={np.sum(DiffPerm>truereddiff)/Nrand}')
-        ax2.set_xlabel('group difference')
-        ax2.set_ylabel('num random permutations')
+        
+        HistPlot(DiffPerm,xtickL='group difference',ax=0,ylab='num random permutations',verline=truereddiff,title=f' {Stim} permuted {Nrand} vs true diff - p={np.sum(DiffPerm>truereddiff)/Nrand}',mean=False)
+        
+   
 
-    return np.nansum(np.abs(Diff)),truereddiff,DiffPerm
+    return np.nansum(np.abs(Diff))#,truereddiff,DiffPerm
 
+def CompareStimHeatmap(self,Stim,SD=25,CutArea=0,Conds=0,cmap_ind='plasma',cmap_diff='RdYlBu',cmap_abs='Greens',alpha=.5,cutoff='median',downsample=8, Nrand=100):
+    ''' 
+    DESCRIPTION: visualize  heatmap fopr two groups, 
+    subplot 1: group 1
+    subplot 2: group 2
+    subplot 3: difference heatmap (raw value)
+    subplot 4: difference heatmap (absolute value)
     
+
+    ARGUMENTS:
     
-def CompareWithinGroupsFix(self,withinColName):
-    '''
-    Description: Run fixation comparisons within groups defined by a category column. Makes plots and prints descriptive stats.
+    Stim (str): list of two stimuli for which the heatmap is generated, it can also find similarly named stimuli based on common substring
     
-    Arguments:
-    withinColName (str): The name of the categorical column defining groups for analysis.
+    
+    
+    OPTIONAL PARAMETERS
+    
+    
+    SD (int, optional): Optional parameter for heatmap smoothness, in pixels. Default is 25.
+    CutArea (int, optional): Cut fixations. For example if you use '1', it shows 99% percentile of fixations. Default is 0. SEt to 1, if stimulus does not cover the screen size eg: for  portrait orientation
+    Conds (int or list, optional): use automatically detected conditions conditions, as provided in betweencond column
+        othewise Conds=['MyCond1' MyCond2'], if we want to specify the order of access for betweencond column.  (could be useful if there are more then 2 conditions, and we want to select 2 to contrast)
+    center: if stimulus area does not start at pixel 0, shifts image display using the plt.imshow(image, extent=)
+    cmap_ind=colormap for  each of the two group heatmaps (see matplotlib colormaps for options: https://matplotlib.org/stable/users/explain/colors/colormaps.html) (two top figures)
+    cmap_diff: colormap of difference heatmap (raw) in two directions (bottom left figure)
+    cmap_abs: colormap of absolute difference heatmap (bottom right figure)
+
+    alpha= transparency- 0-1 higher values less transparent
+    cutoff: shows areas below this threshold as blank
+    twostim: compare two similar stimuli, either provided as list or  match stimuli based on part of string --- if we want to compare two differently named stimuli, with part of the stimulus name matching
+    downsample: downampling size 8 reduced by a factor of 8*8 pixels for example (using skimage)
+    Nrand: number of random permutations to compute, default 100, for actual stats long run time and at least 1000 permutations are recommended, if set to 0 random permutation comparisonno performed
+    # optional paramter to control color of difference heatmap
     '''
+
+    if hasattr(self,'subjects')==0:
+        self.GetParams()   
     
-    WhichC=self.GetCats(withinColName)
+    if type(Stim)==list:
+        assert len(Stim)==2,' length 2 list expected'
+        Stims=np.array(Stim)
+        stimn=np.zeros(2)
+        for cs,s in enumerate(Stims):
+            stimn[cs]=np.nonzero(self.stimuli==s)[0]
+            assert stimn[cs]>-1, 'stim not found'
+    else:
+        self.stimuli=self.stimuli.astype('str')
+        stimn=np.char.find(self.stimuli,Stim)
+        Stims=self.stimuli[stimn>-1]
+        stimn=np.nonzero(stimn>-1)[0]
+        print('stimns found:',stimn,Stims)
+    stimn=np.intp(stimn)
+    stimShow=Stims[0]  # for comparison figures, first figure is used
+    StimIdxs=self.GetStimSubjMap(Stims)
 
-    if hasattr(self,'entropies')==False:   # check if entropy has already been calculated
-        print('Calculating entropy')
-        Entropies,self.entropmax,self.entropies_ind=self.GetEntropies()
-    #Cols=['darkred','cornflowerblue']
-#        plt.figure(figsize=(8,8))
+
+  
     
-    Entrs=[]
-    Fixies=[]
-    ScanpLs=[]
-    SaccAmpls=[] 
-    for cc,c in enumerate(self.WithinConds):
-        print(cc,'Category',c)
-        Idx=np.nonzero(WhichC==c)[0]
-        FixGr=np.array(self.nfix[:,Idx])
-        EntrGr=self.entropies_ind[:,Idx]
-        Entrs.append(np.nanmean(EntrGr,1))
-        Fixies.append(np.nanmean(FixGr,1))
-        ScanpLs.append(np.nanmean(self.len_scanpath[:,Idx],1))
-        SaccAmpls.append(np.nanmean(self.sacc_ampl[:,Idx],1))
-     
+
+    FixCounts=[]
+    for s in Stims:
+        fixcount=self.FixCountCalc(s,CutAct=0)
+        assert np.sum(fixcount)>0,'!!no fixations found'
+        HasFixIdx=np.sum(np.sum(fixcount,2),1)>0
+        fixcount=fixcount[HasFixIdx,:,:]
+        FixCounts.append(fixcount)
+        print(s,np.shape(FixCounts[-1]))
+    Reduced1=ReduceCounts(FixCounts[0],downsample)
+    Reduced2=ReduceCounts(FixCounts[1],downsample)
+    Reduced=np.concatenate((Reduced1,Reduced2),axis=0)
+
+
+    print('reduced dims',np.shape(Reduced))
+    
+    N1=len(StimIdxs[0])
+    print(f'num observers seen stimulus {Stims[0]}: {N1}') 
+    print(f'num observers seen stimulus {Stims[1]}: {len(StimIdxs[1])}') 
+
+
+
+    fig,ax=plt.subplots(ncols=2,nrows=2,figsize=(10,8)) 
+    hmaps=[]
+    hmapsred=[]## reduced heatmaps, downsampled with scikit image (mean based downsampling)
+    
+    for cs,s in enumerate(stimn):
+            
         
-        print(cc,c,'Num fix= ',np.round(np.mean(np.nanmean(FixGr,1)),2),'+/-',np.round(np.std(np.nanmean(FixGr,1)),2))
-        print(cc,c,'Entropy= ',np.round(np.mean(np.nanmean(EntrGr,1)),2),'+/-',np.round(np.std(np.nanmean(EntrGr,1)),2))
-        print(cc,c,'tot scanpath len = ',np.round(np.mean(np.nanmean(self.len_scanpath[:,Idx],1)),2),'+/-',np.round(np.std(np.nanmean(self.len_scanpath[:,Idx],1)),2),'pix')
-        print(cc,c,'saccade amplitude = ',np.round(np.mean(np.nanmean(self.sacc_ampl[:,Idx],1)),2),'+/-',np.round(np.std(np.nanmean(self.sacc_ampl[:,Idx],1)),2),'pix')
-        print('')
-    return
- 
+        heatmap=SaliencyMapFilt(FixCounts[cs],SD=SD,Ind=0)
+        hmaps.append(heatmap)
+        self.VisHeatmap(Stims[cs],heatmap,ax=ax[0,cs],cutoff=cutoff,alpha=alpha,cmap=cmap_ind,title=self.stimuli[s])
+        
+        
+        redcount=ReduceCounts(FixCounts[cs],downsample)
+        hmap_red=SaliencyMapFilt(redcount,SD=8,Ind=0)
+        hmapsred.append(hmap_red)
+   
+    # difference heatmp
+    Diff=hmaps[0]-hmaps[1]
+
+
+    colorbarlabel=str(Stims[0])+'<---->'+str(Stims[1])
+
+    self.VisHeatmap(stimShow,Diff,ax=ax[1,0],cutoff=cutoff,alpha=alpha,cmap=cmap_diff,cbar=True,cbarlabel=colorbarlabel,title='difference')
+    
+    self.VisHeatmap(stimShow,np.abs(Diff),ax=ax[1,1],cutoff=cutoff,alpha=alpha,cmap=cmap_abs,cbar=True,cbarlabel=' ',title='absolute difference')
+    
+    
+    
+    DiffRed=hmapsred[0]-hmapsred[1]
    
+    ### calculate permuted difference heatmaps
+    DiffPerm=np.zeros(Nrand)
+    print(f'{Nrand} permutations starting')
+    if Nrand>0:
+        for n in range(Nrand):
+            Idxs=np.random.permutation(np.shape(Reduced)[0])         
+            hmap1=SaliencyMapFilt(Reduced[Idxs[0:N1],:,:],SD=downsample,Ind=0)
+            hmap2=SaliencyMapFilt(Reduced[Idxs[N1:],:,:],SD=downsample,Ind=0)
+            DiffPerm[n]=np.nansum(np.abs(hmap1-hmap2))
+        
+   
+
+
+    truereddiff=np.nansum(np.abs(DiffRed))
+    # visualize permuted difference heatmap distribution
+    
+    if Nrand>0:
+        
+        HistPlot(DiffPerm,xtickL='group difference',ax=0,ylab='num random permutations',verline=truereddiff,title=f' {Stim} permuted {Nrand} vs true diff - p={np.sum(DiffPerm>truereddiff)/Nrand}',mean=False)
+        
+      
+
+    return np.nansum(np.abs(Diff))#,truereddiff,DiffPerm
+
+    
+ 
     
+ 
     
 def FixDurProgGroups(self,colName,nfixmax=10,between=0):
     ''' 
     Description: Calculate and visualize fixation duration progression within or between groups defined by a category column, for the first x number of fixations of each trial
 
     Arguments:
     colName (str): The name of the category column defining groups for analysis.
@@ -330,52 +433,78 @@
 
 
 
 
 def BinnedDescriptivesGroups(self,colName,between=0):
     ''' time-binned within trial descriptive progression, groups of stimuli or between groups of participants'''
     if hasattr(self,'binFixL')==False: 
-        print('run BinnedDescriptives first, than call this function for group wise visualization')
+        
+        warnings.warn('run BinnedDescriptives first to specify time columns and bins, than call this function for group wise visualization')
+        self.BinnedDescriptives()
     if between:
          print('running between group comparison')
 
          WhichC,WhichCN=self.GetGroups(colName)
     else:
          print('running within group comparison, provide between=True for between group comparisons')
 
          WhichC=self.GetCats(colName)
  #   print(WhichC)
     Colors=['navy','salmon','olive','orange','gray']
+    
+    Measures=[self.binFixL,self.saccadeAmp,self.totLscanpath]
+    MeasureNames=['fixation duration (ms)','saccade ampl (pixel)','scanpath length (pixel)']
     fig,ax=plt.subplots(nrows=3,ncols=1,figsize=(4,10))
+    
+    Dats=[{},{}]
+   
     for cc,c in enumerate(self.WithinConds):
         if between:
             Idx=np.nonzero(WhichC==cc)[0]
             print(Idx)
         else:
             Idx=np.nonzero(WhichC==c)[0]
-            
+        for cm,m in enumerate(Measures):
+   
+            if between:
+                dat=np.nanmean(m[Idx,:,:],1)
+                if cm==0:
+                    ax1,ax2=JointBinnedPlot(self.tbins,np.nanmean(self.binFixL[Idx,:,:],1),np.nanmean(self.saccadeAmp[Idx,:,:],1),ylabel1='fixation duration (ms)',ylabel2='saccade ampl (pixel)')
+            else:
+                dat=np.nanmean(m[:,Idx,:],1)
+                if cm==0:
+                    ax1,ax2=JointBinnedPlot(self.tbins,np.nanmean(self.binFixL[:,Idx,:],1),np.nanmean(self.saccadeAmp[:,Idx,:],1),ylabel1='fixation duration (ms)',ylabel2='saccade ampl (pixel)')
+            axout=VisBinnedProg(self.tbins,dat,MeasureNames[cm],col=Colors[cc],label=c,axin=ax[cm])
+            Dats[cc][MeasureNames[cm]]=dat
+        ax1.set_title(c)
+    tvals={}
+    pvals={}
+    for cm,m in enumerate(Measures):
         if between:
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.binFixL[Idx,:,:],1),'fixation duration (ms)',col=Colors[cc],label=c,axin=ax[0])
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.saccadeAmp[Idx,:,:],1),'saccade ampl (pixel)',col=Colors[cc],label=c,axin=ax[1])
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.totLscanpath[Idx,:,:],1),'scanpath length (pixel)',col=Colors[cc],label=c,axin=ax[2])
-          
-            ax1,ax2=JointBinnedPlot(self.tbins,np.nanmean(self.binFixL[Idx,:,:],1),np.nanmean(self.saccadeAmp[Idx,:,:],1),ylabel1='fixation duration (ms)',ylabel2='saccade ampl (pixel)')
+            t,p=stats.ttest_ind(Dats[0][MeasureNames[cm]],Dats[1][MeasureNames[cm]])
         else:
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.binFixL[:,Idx,:],1),'fixation duration (ms)',col=Colors[cc],label=c,axin=ax[0])
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.saccadeAmp[:,Idx,:],1),'saccade ampl (pixel)',col=Colors[cc],label=c,axin=ax[1])
-            axout=VisBinnedProg(self.tbins,np.nanmean(self.totLscanpath[:,Idx,:],1),'scanpath length (pixel)',col=Colors[cc],label=c,axin=ax[2])
+            t,p=stats.ttest_rel(Dats[0][MeasureNames[cm]],Dats[1][MeasureNames[cm]])
+        tvals[MeasureNames[cm]]=t
+        pvals[MeasureNames[cm]]=p
+        ypos=np.nanmean(np.concatenate((Dats[0][MeasureNames[cm]],Dats[1][MeasureNames[cm]])))
+        for c,p_i in enumerate(p):
+            xpos=(self.tbins[c]+self.tbins[c+1])/2
+            if p_i<.01:
+                ax[cm].scatter(xpos,ypos,marker='*', s=30,color='k')
+            elif  p_i<.05:
+                ax[cm].scatter(xpos,ypos,marker='*', s=17,color='k')
+
+
+   #     print(cm,MeasureNames[cm],t,p)
             
-            ax1,ax2=JointBinnedPlot(self.tbins,np.nanmean(self.binFixL[:,Idx,:],1),np.nanmean(self.saccadeAmp[:,Idx,:],1),ylabel1='fixation duration (ms)',ylabel2='saccade ampl (pixel)')
-        ax1.set_title(c)
-        
 
-    ax[0].legend()
-    ax[1].legend()
-    ax[2].legend()
+    for a in range(3):
+        ax[a].legend()
     plt.tight_layout()      
+    return tvals, pvals
     
     
          
     
 def CompareGroupsMat(self,group,indsimmat):
     ''' 
     calculates  average within and between group values from inividual matrix differences
@@ -389,123 +518,181 @@
         for cg2,gr2 in enumerate(grs):
             for cs in range(self.np):
                 Diffs[cs,cg1,cg2]=np.nanmean(indsimmat[cs,groups==cg1,:][:,groups==cg2])
     return Diffs
         
 
 
-def CompareGroupsGridFix(self,Stim,betwcond,Conds=0,nhor=5,nver=5,substring=False,cmap_ind='plasma',cmap_diff='RdYlBu',alpha=.5,t_abs=False,timemin=0, timemax=np.inf, timecol=0): 
+def CompareGroupsGridFix(self,Stim,betwcond,Conds=0,nhor=5,nver=5,cmap_ind='plasma',cmap_diff='RdYlBu',alpha=.5,t_abs=False,timemin=0, timemax=np.inf, timecol=0,useT=True,cutoff=-1): 
     ''' 
 
     Stim: stimulus name
     betwcond: between subject condition (if substring=True, this is not used)
     
     Conds: explicitly provide conditions (if there are more than 2, this is necessary)
     t_abs: default=False,  absolute t value vs raw t-values grid
     nhor: number of horizonal cells for the grid
     nver: number of vertical cells for the grid
     center (true): stimulus position correction (based on difference between stimulus and screen resolution), stimulus must be presented centrally!
-    substring: if paired stimuli have to found based on common part in stimulusID
+    substring: if two different stimuli are compared,  can be paired stimuli have to found based on common part in stimulusID
     cmap_ind: colormap for the heatmap of each group, default: 'plasma'
     cmap_diff: colormap for difference heatmaps- default 'RdYlBu'--- ideally use divergent heatmaps
     
 
     '''
-
-    if substring:
-        self.stimuli=self.stimuli.astype('str')
-        stimn=np.char.find(self.stimuli,Stim)
-        Stims=self.stimuli[stimn>-1]
-        stimn=np.nonzero(stimn>-1)[0]
-        stimShow=Stims[0]
-        print('stimns found:',stimn,Stims)
-    else:
-        stimShow=copy.copy(Stim)
-        stimn=np.nonzero(self.stimuli==Stim)[0]
-        print('stimns found:',stimn,stimShow)
-
+   
+    stimn=np.nonzero(self.stimuli==Stim)[0]
 
     WhichC,WhichCN=self.GetGroups(betwcond)
 
     if type(Conds)==int:    
         Conditions=np.copy(self.Conds)
     else:
         print('use provided conditions: ' ,Conds)
         Conditions=np.copy(Conds)
       
-    if hasattr(self,'boundsX')==0:
-        self.RunDescriptiveFix()
-    
-    if hasattr(self,'subjects')==0:
-        self.GetParams()   
    
     statPMat,statEntropyMat=self.CalcStatPs(nhor,nver,MinFix=5,InferS=2,timemin=timemin, timemax=timemax, timecol=timecol)
 
    # if substring and len(stimn)==2:
 
     fig,ax=plt.subplots(nrows=2,ncols=2,figsize=(10,8))
     statmats=[]
-    if substring:
-        for cs,s in enumerate(stimn):
-            Statpm=np.nanmean(statPMat[:,s,:,:],0)
-            Statpm[Statpm<np.nanpercentile(Statpm,30)]=np.NAN
-            self.VisGrid(Statpm,Stims[cs],ax=ax[0,cs],alpha=alpha,cmap=cmap_ind)
-            ax[0,cs].set_title(Stims[cs])
+    
+    for ccond,cond in enumerate(Conditions):
+        Idx=WhichCN==cond
+        print(np.shape(np.nanmean(statPMat[Idx,stimn,:,:],0)))
+        Statpm=np.nanmean(statPMat[Idx,stimn,:,:],0)
+        if cutoff>-1:
+            Statpm[Statpm<np.nanpercentile(Statpm,cutoff)]=np.NAN
+        self.VisGrid(Statpm,Stim,ax=ax[0,ccond],alpha=alpha,cmap=cmap_ind)
+        ax[0,ccond].set_title(cond)
+        statmats.append(statPMat[Idx,stimn,:,:])
+    diffmat=np.nanmean(statmats[0],0)-np.nanmean(statmats[1],0) 
+
+    tt,pp=np.zeros((nver,nhor)),np.zeros((nver,nhor))
+    for ch in range(nhor):
+        for cv in range(nver):
+            d1,d2=statmats[0][:,cv,ch],statmats[1][:,cv,ch]
            
-            statmats.append(statPMat[:,s,:,:])
+            tt[cv,ch],pp[cv,ch] = stats.ttest_ind(d1[np.isfinite(d1)],d2[np.isfinite(d2)])
+
+    cbar=self.VisGrid(diffmat,Stim,ax=ax[1,0],alpha=.7,cmap=cmap_diff,vmax=np.nanmax(np.abs(diffmat)),cbar=True)
+    cbar.ax.get_yaxis().set_ticks([])
+    cbar.ax.get_yaxis().labelpad = 15
+    cbar.ax.set_ylabel(str(Conditions[0])+'<---->'+str(Conditions[1]), rotation=270)
+
+    ax[1,0].set_title('difference')
+    if useT:
+        if t_abs:
+            cbar=self.VisGrid(np.abs(tt),Stim,ax=ax[1,1],alpha=.7,cmap='Greens',cbar=True)
+            ax[1,1].set_title('abs t-values')
+        else:
+            cbar=self.VisGrid(tt,Stim,ax=ax[1,1],alpha=.7,cmap=cmap_diff,vmax=4,cbar=True)
+            ax[1,1].set_title('t-value')
+            cbar.ax.get_yaxis().labelpad = 30
+            cbar.ax.set_ylabel(str(Conditions[0])+'<---->'+str(Conditions[1]), rotation=270)
 
+    else:
+        cbar=self.VisGrid(np.log(pp),Stim,ax=ax[1,1],alpha=.7,cmap='Greens',cbar=True)
+        ax[1,1].set_title('log(p)')
+
+    self.Highlight_Sign(Stim,pp,ax[1,1]) # highlight significant cells, by showing grid buondaries (dashed (p<.05) or solid line (p<.01) 
+    
+    print('num significant uncorrected: ',np.sum(pp<.05))
+    print('num significant Bonferroni - Holm corrected: ',BonfHolm(pp))
 
-        diffmat=np.nanmean(statPMat[:,stimn[0],:,:],0)-np.nanmean(statPMat[:,stimn[1],:,:],0) 
+    return tt,pp
+
+
+def CompareStimGridFix(self,Stim,Conds=0,nhor=5,nver=5,cmap_ind='plasma',cmap_diff='RdYlBu',alpha=.5,t_abs=False,timemin=0, timemax=np.inf, timecol=0,useT=True,cutoff=-1): 
+    ''' 
+
+    Stim: slist of two stimulus names to compare, or common substring to find pairs of stimuli (for the latter two options)
+    
+    Conds: explicitly provide conditions (if there are more than 2, this is necessary)
+    t_abs: default=False,  absolute t value vs raw t-values grid
+    nhor: number of horizonal cells for the grid
+    nver: number of vertical cells for the grid
+    center (true): stimulus position correction (based on difference between stimulus and screen resolution), stimulus must be presented centrally!
+    substring: if two different stimuli are compared,  can be paired stimuli have to found based on common part in stimulusID
+    cmap_ind: colormap for the heatmap of each group, default: 'plasma'
+    cmap_diff: colormap for difference heatmaps- default 'RdYlBu'--- ideally use divergent heatmaps
+    
+
+    '''
+    
+    
+    if type(Stim)==list:
+        assert len(Stim)==2,' length 2 list expected'
+        Stims=np.array(Stim)
+        stimn=np.zeros(2)
+        for cs,s in enumerate(Stims):
+            stimn[cs]=np.nonzero(self.stimuli==s)[0]
+            assert stimn[cs]>-1, 'stim not found'
+    else:    
+        self.stimuli=self.stimuli.astype('str')
+        stimn=np.char.find(self.stimuli,Stim)
         
+        Stims=self.stimuli[stimn>-1]
+        stimn=np.nonzero(stimn>-1)[0]
+    stimn=np.intp(stimn)
+    stimShow=Stims[0]
+    print('stimns found:',stimn,Stims)
+   
+    statPMat,statEntropyMat=self.CalcStatPs(nhor,nver,MinFix=5,InferS=2,timemin=timemin, timemax=timemax, timecol=timecol)
+
+   # if substring and len(stimn)==2:
+
+    fig,ax=plt.subplots(nrows=2,ncols=2,figsize=(10,8))
+    statmats=[]
+    for cs,s in enumerate(stimn):
+        Statpm=np.nanmean(statPMat[:,s,:,:],0)
+        if cutoff>-1:
+            Statpm[Statpm<np.nanpercentile(Statpm,cutoff)]=np.NAN
+        self.VisGrid(Statpm,Stims[cs],ax=ax[0,cs],alpha=alpha,cmap=cmap_ind)
+        ax[0,cs].set_title(Stims[cs])
+        statmats.append(statPMat[:,s,:,:])
+
+
+    diffmat=np.nanmean(statPMat[:,stimn[0],:,:],0)-np.nanmean(statPMat[:,stimn[1],:,:],0) 
+    
   
-    else:
-        for ccond,cond in enumerate(Conditions):
-            Idx=WhichCN==cond
-            print(np.shape(np.nanmean(statPMat[Idx,stimn,:,:],0)))
-            Statpm=np.nanmean(statPMat[Idx,stimn,:,:],0)
-            Statpm[Statpm<np.nanpercentile(Statpm,30)]=np.NAN
-            self.VisGrid(Statpm,stimShow,ax=ax[0,ccond],alpha=alpha,cmap=cmap_ind)
-            ax[0,ccond].set_title(cond)
-            statmats.append(statPMat[Idx,stimn,:,:])
-        diffmat=np.nanmean(statmats[0],0)-np.nanmean(statmats[1],0) 
 
     tt,pp=np.zeros((nver,nhor)),np.zeros((nver,nhor))
     for ch in range(nhor):
         for cv in range(nver):
             d1,d2=statmats[0][:,cv,ch],statmats[1][:,cv,ch]
-           
-
             tt[cv,ch],pp[cv,ch] = stats.ttest_ind(d1[np.isfinite(d1)],d2[np.isfinite(d2)])
 
 
 
     cbar=self.VisGrid(diffmat,stimShow,ax=ax[1,0],alpha=.7,cmap=cmap_diff,vmax=np.nanmax(np.abs(diffmat)),cbar=True)
     cbar.ax.get_yaxis().set_ticks([])
     cbar.ax.get_yaxis().labelpad = 15
-    if substring:
-        cbar.ax.set_ylabel(str(Stims[0])+'<---->'+str(Stims[1]), rotation=270)
-    else:
-        cbar.ax.set_ylabel(str(Conditions[0])+'<---->'+str(Conditions[1]), rotation=270)
-
+    cbar.ax.set_ylabel(str(Stims[0])+'<---->'+str(Stims[1]), rotation=270)
+  
     ax[1,0].set_title('difference')
-    if t_abs:
-        cbar=self.VisGrid(np.abs(tt),stimShow,ax=ax[1,1],alpha=.7,cmap='Greens',cbar=True)
-        ax[1,1].set_title('abs t-values')
-    else:
-        cbar=self.VisGrid(tt,stimShow,ax=ax[1,1],alpha=.7,cmap=cmap_diff,vmax=4,cbar=True)
-        ax[1,1].set_title('t-value')
-        cbar.ax.get_yaxis().labelpad = 30
-
-        if substring:
-            cbar.ax.set_ylabel(str(Stims[0])+'<---->'+str(Stims[1]), rotation=270)
+    if useT:
+        if t_abs:
+            cbar=self.VisGrid(np.abs(tt),stimShow,ax=ax[1,1],alpha=.7,cmap='Greens',cbar=True)
+            ax[1,1].set_title('abs t-values')
         else:
-            cbar.ax.set_ylabel(str(Conditions[0])+'<---->'+str(Conditions[1]), rotation=270)
-
+            cbar=self.VisGrid(tt,stimShow,ax=ax[1,1],alpha=.7,cmap=cmap_diff,vmax=4,cbar=True)
+            ax[1,1].set_title('t-value')
+            cbar.ax.get_yaxis().labelpad = 30
+            cbar.ax.set_ylabel(str(Stims[0])+'<---->'+str(Stims[1]), rotation=270)       
 
+    else:
+        cbar=self.VisGrid(np.log(pp),stimShow,ax=ax[1,1],alpha=.7,cmap='Greens',cbar=True)
+        ax[1,1].set_title('log(p)')
 
-    self.Hihglight_Sign(stimShow,pp,ax[1,1]) # highlight significant cells, by showing grid buondaries (dashed (p<.05) or solid line (p<.01) 
-    
+  
+    self.Highlight_Sign(stimShow,pp,ax[1,1]) # highlight significant cells, by showing grid buondaries (dashed (p<.05) or solid line (p<.01) 
     
+    print('num significant uncorrected: ',np.sum(pp<.05))
+    print('num significant Bonferroni - Holm corrected: ',BonfHolm(pp))
+
     return tt,pp
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/_dataproc.py` & `pyeyesim-0.3.1/PyEyeSim/_dataproc.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from numpy import matlib
 #from scipy import stats,ndimage
 import pandas as pd
 import matplotlib.pyplot as plt
 from .statshelper import SaliencyMapFilt,SaccadesTrial
 from .scanpathshelpdebug import CreatAoiRects,SaccadeLine
 import platform
+import warnings
 
 
 def GetParams(self):
     """ Get stimulus and subject info of dataset """  
     assert  'subjectID' in self.data.columns , 'subjectID column not found- DataInfo(subjectID=Your Column)'
     assert  'Stimulus' in self.data.columns, 'Stimulus column not found- DataInfo(Stimulus=Your Column'
 
@@ -105,62 +106,46 @@
 
        
         
     pass 
  
 
   
-def FixCountCalc(self,Stim,CutAct=1,substring=False):
+def FixCountCalc(self,Stim,CutAct=False):
     ''' Pixelwise fixation count for each participant, but for single stimulus  (Stim) 
     output: subjects*y*x --> num of fixaiton for each pixel
     if CutAct==1 in the end, only the within bounds areas is returned for further calculations
     optional parameter, substring for stimulus names containing the same substring'''
-    if substring==False:
-        assert np.sum(self.data['Stimulus']==Stim)>0, 'stimulus not found'
-        stimn=np.nonzero(self.stimuli==Stim)[0]
-        print('stimns found:',stimn,Stim)
-        idims=np.shape(self.images[Stim])
-
-
-    elif substring==True:  
-        self.stimuli=self.stimuli.astype('str')
-        stimn=np.char.find(self.stimuli,Stim)
-        Stims=self.stimuli[stimn>-1]
-        stimn=np.nonzero(stimn>-1)[0]
-        print('stimns found:',stimn,Stims)
-        
-        idims=np.shape(self.images[Stims[0]])
+ 
+    
+    if hasattr(self,'images')==False:
+         idims=np.array([self.y_size,self.x_size])
+    else:
+         idims=np.shape(self.images[Stim])
+    stimn=np.nonzero(self.stimuli==Stim)[0]
     yimsize,ximsize=idims[0],idims[1]
     print('resolution x =', ximsize, ' y =',yimsize)
 
     FixCountInd=np.zeros(((self.ns,yimsize,ximsize)))
     
     
     for cs,s in enumerate(self.subjects):
-        if substring:
-            x,y=np.intp(self.GetFixationData(s,Stims[0]))
-            if len(x)==0: # if length of first match is zero
-                x,y=np.intp(self.GetFixationData(s,Stims[1])) # get second match
-                stimIdx=1
-            else:
-                stimIdx=0
-            Valid=np.nonzero((x<ximsize)&(x>0)&(y>0)&(y<yimsize))[0]
-
-        else:
-            x,y=np.intp(self.GetFixationData(s,Stim))
-         #   Valid=np.nonzero((x<self.boundsX[stimn,1])&(x>self.boundsX[stimn,0])&(y>self.boundsY[stimn,0])&(y<self.boundsY[stimn,1]))[0]
-            Valid=np.nonzero((x<ximsize)&(x>0)&(y>0)&(y<yimsize))[0]
-        X,Y=x[Valid],y[Valid]
-        FixCountInd[cs,Y,X]+=1
-   # self.boundsX[stimn,0]:self.boundsX[stimn,1]
-   # if CutAct:
-    #    if len(stimn)>0:
-     #       stimn=stimn[0] # cut based on the bounds of the first if there are more matching stimuli
-      #  FixCountInd=FixCountInd[:,:,int(np.round(self.boundsX[stimn,0])):int(np.round(self.boundsX[stimn,1]))]  # cut X
-       # FixCountInd=FixCountInd[:,int(np.round(self.boundsY[stimn,0])):int(np.round(self.boundsY[stimn,1])),:] # cut Y
+      
+        x,y=np.intp(self.GetFixationData(s,Stim))
+        if len(x)>0:
+            Valid=np.nonzero((x<ximsize)&(x>=0)&(y>=0)&(y<yimsize))[0]
+            X,Y=x[Valid],y[Valid]
+            for xx,yy in zip(X,Y):
+                FixCountInd[cs,yy,xx]+=1
+        #if np.sum(FixCountInd[cs,:,:])==0:
+            #print('no fixations for', s ,'with', Stim)
+      
+    if CutAct:
+        FixCountInd=FixCountInd[:,:,int(np.round(self.boundsX[stimn,0])):int(np.round(self.boundsX[stimn,1]))]  # cut X
+        FixCountInd=FixCountInd[:,int(np.round(self.boundsY[stimn,0])):int(np.round(self.boundsY[stimn,1])),:] # cut Y
     return FixCountInd
 
 
 
 def GetFixationData(self,subj,stim,timemin=0,timemax=np.inf,timecol=0):
     """get X,Y fixation sequence for a subject and stimulus
     output 1: array of pixel x for sequence of fixations
@@ -199,29 +184,47 @@
             if PPc==self.Conds[cc]:
                 WhichC[cs]=cc
                 WhichCN.append(c)
     self.whichC=WhichC
     return WhichC,np.array(WhichCN)
 
 def GetCats(self,condColumn):
-    ''' Between group comparison- 2 groups expected
+    ''' Within group comparison- 
     get conditions from between group column, check if mapping of participants to conditions is unique'''
     self.WithinConds=np.unique(self.data[condColumn])
     print('Conditions',self.WithinConds)
     WhichCat=[]# np.zeros(self.np)
 
     for cp,p in enumerate(self.stimuli):
         AssignCat=np.unique(self.data[condColumn][self.data['Stimulus']==p])
        # print(cp,p,AssignCat)
         #assert len(AssignCat)==1, ' category mapping not unique for a stimulus'
         WhichCat.append(AssignCat)
     WhichCat=np.array(WhichCat)
     assert len(np.unique(WhichCat))==len(np.unique(self.WithinConds)), 'stimulus category mapping problem'
     return WhichCat
 
+def GetStimSubjMap(self,Stims):
+    StimIdxs=[[],[]]  # check which participant saw which stimulus
+    for cs,s in enumerate(self.subjects):
+        x1,y1=np.intp(self.GetFixationData(s,Stims[0]))
+        x2,y2=np.intp(self.GetFixationData(s,Stims[1]))
+        if len(x1)>0 and len(x2)>0:
+            warnings.warn('non unique stimulus - subject mapping error')
+        if len(x1)>0:
+            StimIdxs[0].append(cs)
+        elif len(x2)>0:
+            StimIdxs[1].append(cs)
+           
+    StimIdxs[0]=np.intp(np.array(StimIdxs[0]))    
+    StimIdxs[1]=np.intp(np.array(StimIdxs[1]))    
+    return StimIdxs
+    
+
+
 def GetSaccades(self):
     ''' from fixations, make approximate saccades, and store it as saccade objects'''
     SaccadeObj=[]
     
     self.nsac=np.zeros((self.ns,self.np))
     self.saccadelenghts=np.zeros((self.ns,self.np))
     for cs,s in enumerate(self.subjects):
@@ -279,35 +282,30 @@
 
   
 def Heatmap(self,Stim,SD=25,Ind=0,Vis=0,FixCounts=0,cutoff='median',CutArea=0,ax=False,substring=False,cmap='plasma',alpha=.5):
     ''' Pipeline for  heatmap calculation, FixCounts are calculated for stimulus, or passed pre-calcualted as optional parameter
     output: heatmap for a stimulus
     
     Vis:  if 1 Heatmap visual shows up- otherwise no visualization, but returns the heatmap values
-    
+    Ind: independent heatmap for each participant
     cutarea option: 1 only use active area (99% percentile of fixations), 0- use all of the area - set it to 1, if stimulus does not cover the whole screen
     cutoff=median: median cutoff, otherwise percetile of values to replace with nans, goal--> clear visualization
     substring: use part of file name (expected for mathcing paired files)
     cmap=colormap (see matplotlib colormaps for options: https://matplotlib.org/stable/users/explain/colors/colormaps.html)
     alpha= transparency- 0-1 higher values less transparent
     '''
   #  if hasattr(self,'fixcounts'):
    #     FixCountIndie=self.fixcounts['Stim']
     #else:    
-    if substring==False:
-        stimn=np.nonzero(self.stimuli==Stim)[0]
-        stimShow=Stim
-        idims=np.shape(self.images[Stim])
+    stimn=np.nonzero(self.stimuli==Stim)[0]
+    if hasattr(self,'images')==False:
+        idims=np.array([self.y_size,self.x_size])
     else:
-        self.stimuli=self.stimuli.astype('str')
-        stimn=np.char.find(self.stimuli,Stim)
-        Stims=self.stimuli[stimn>-1]
-        stimn=np.nonzero(stimn>-1)[0]
-        stimShow=Stims[0]
-        idims=np.shape(self.images[Stims[0]])
+        idims=np.shape(self.images[Stim])
+        
     yimsize,ximsize=idims[0],idims[1]
 
     if hasattr(self,'boundsX')==False:
         print('run RunDescriptiveFix first- without visuals')
         self.RunDescriptiveFix()
     if type(FixCounts)==int:
         if CutArea:
@@ -316,39 +314,26 @@
             FixCounts=self.FixCountCalc(Stim,CutAct=0,substring=substring) 
     assert np.sum(FixCounts)>0,'!!no fixations found'
 
     if np.sum(FixCounts)<10:
         print('WARNING NUM FIX FOUND: ',np.sum(FixCounts))
     if Ind==0:
         smap=SaliencyMapFilt(FixCounts,SD=SD,Ind=0)
-        if cutoff=='median':
-             cutThr=np.median(smap)
-        elif cutoff>0:
-             cutThr=np.percentile(smap,cutoff) 
-        else:
-            cutThr=0
         if CutArea:
             smapall=np.zeros((yimsize,ximsize))
+            smapall[:]=np.NAN
             if len(stimn)>0:
                 stimn=stimn[0]
             smapall[int(self.boundsY[stimn,0]):int(self.boundsY[stimn,1]),int(self.boundsX[stimn,0]):int(self.boundsX[stimn,1])]=smap
         else:
             smapall=np.copy(smap)
     else:
         smap=np.zeros_like(FixCounts)
         for cs,s in enumerate(self.subjects):
-            smap[cs,:,:]=SaliencyMapFilt(FixCounts[cs,:,:],SD=SD,Ind=1)       
-    if Vis:
-        smapall[smapall<cutThr]=np.NAN  # replacing below threshold with NAN
+            smap[cs,:,:]=SaliencyMapFilt(FixCounts[cs,:,:],SD=SD,Ind=1)
+        smapall=np.nanmean(smap,0)
        
-        if ax==False:
-            fig,ax=plt.subplots()
-#
-        ax.imshow(self.images[stimShow])
-        ax.imshow(smapall,alpha=alpha,cmap=cmap) 
-        ax.set_xticks([])
-        ax.set_yticks([])
-        #ax.set_xlim([xs1,xs2])
-       # ax.set_ylim([ys2,ys1])
-            
+    
+    if Vis:
+        self.VisHeatmap(Stim,smapall,ax=ax,cutoff=cutoff,cmap=cmap,alpha=alpha)
     return smapall
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/_hmm.py` & `pyeyesim-0.3.1/PyEyeSim/_hmm.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/_scanpathsim.py` & `pyeyesim-0.3.1/PyEyeSim/_scanpathsim.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,88 +56,135 @@
             WhichAOI[x]=AOInums[np.intp(WhichAOIV[x]),np.intp(WhichAOIH[x])]  # get combined vertival and horizontal
     for st in range(nAOI): # gaze transition start
         StatNtrial[st]=np.sum(WhichAOI==st)  # get count in AOI
         StatPtrial[st]=np.sum(WhichAOI==st)/np.sum(np.isfinite(WhichAOI)) # calculate stationary P for each AOI    
     return NFix,StatPtrial,StatNtrial
 
     
-def SaccadeSel(self,SaccadeObj,nDiv,InferS=True): 
+def SaccadeSel(self,SaccadeObj,nHor,nVer=0,InferS=False): 
     ''' select saccades for angle comparison method'''
-    nH,nV=nDiv,nDiv
+    if nVer==0:
+        nVer=nHor  # if number of vertical divisions not provided -- use same as the number of horizontal
     SaccadeAOIAngles=[]
     SaccadeAOIAnglesCross=[]
     if InferS:
         if hasattr(self,'boundsX')==False:
             print('runnnig descriptives to get bounds')
             self.RunDescriptiveFix()  
-        AOIRects=CreatAoiRects(nH,nV,self.boundsX,self.boundsY)
+        AOIRects=CreatAoiRects(nHor,nVer,self.boundsX,self.boundsY)
     else:
-        AOIRects=CreatAoiRects(nH,nV,self.x_size,self.y_size)
+        AOIRects=CreatAoiRects(nHor,nVer,self.x_size,self.y_size)
 
-    Saccades=np.zeros((((self.ns,self.np,nH,nV))),dtype=np.ndarray)  # store an array of saccades that cross the cell, for each AOI rectangle of each trial for each partiicpant
+    Saccades=np.zeros((((self.ns,self.np,nVer,nHor))),dtype=np.ndarray)  # store an array of saccades that cross the cell, for each AOI rectangle of each trial for each partiicpant
     for s in np.arange(self.ns):
         SaccadeAOIAngles.append([])
         SaccadeAOIAnglesCross.append([])
         for p in range(self.np):
-            SaccadeAOIAngles[s].append(np.zeros(((int(self.nsac[s,p]),nH,nV))))
+            SaccadeAOIAngles[s].append(np.zeros(((int(self.nsac[s,p]),nVer,nHor))))
            # print(s,p,NSac[s,p])
             SaccadeAOIAngles[s][p][:]=np.NAN
-            SaccadeAOIAnglesCross[s].append(np.zeros(((int(self.nsac[s,p]),nH,nV))))
+            SaccadeAOIAnglesCross[s].append(np.zeros(((int(self.nsac[s,p]),nVer,nHor))))
             SaccadeAOIAnglesCross[s][p][:]=np.NAN
             for sac in range(len(SaccadeObj[s][p])):
                 SaccadeDots=SaccadeObj[s][p][sac].LinePoints()
                 
                 
-                for h in range(nH):
-                    for v in range(nV):
+                for h in range(nHor):
+                    for v in range(nVer):
                        # print(h,v)
                         if AOIRects[p][h][v].Cross(SaccadeDots)==True:
                           #  print(h,v,SaccadeObj[s][p][sac].Angle())
-                            SaccadeAOIAngles[s][p][sac,h,v]=SaccadeObj[s][p][sac].Angle()  # get the angle of the sacccade
+                            SaccadeAOIAngles[s][p][sac,v,h]=SaccadeObj[s][p][sac].Angle()  # get the angle of the sacccade
 
                 if np.sum(SaccadeAOIAngles[s][p][sac,:,:]>0)>1:  # select saccaded that use multiple cells
                     #print('CrossSel',SaccadeAOIAngles[s][p][sac,:,:])
                     SaccadeAOIAnglesCross[s][p][sac,:,:]=SaccadeAOIAngles[s][p][sac,:,:]
 
-            for h in range(nH):
-                for v in range(nV):
-                    if np.sum(np.isfinite(SaccadeAOIAnglesCross[s][p][:,h,v]))>0:
-                        Saccades[s,p,h,v]=np.array(SaccadeAOIAnglesCross[s][p][~np.isnan(SaccadeAOIAnglesCross[s][p][:,h,v]),h,v])
+            for h in range(nHor):
+                for v in range(nVer):
+                    if np.sum(np.isfinite(SaccadeAOIAnglesCross[s][p][:,v,h]))>0:
+                        Saccades[s,p,v,h]=np.array(SaccadeAOIAnglesCross[s][p][~np.isnan(SaccadeAOIAnglesCross[s][p][:,v,h]),v,h])
                     else:
-                        Saccades[s,p,h,v]=np.array([])
+                        Saccades[s,p,v,h]=np.array([])
     return Saccades
 
 
-def SacSim1Group(self,Saccades,nDiv,Thr=5):
-    ''' calculate saccade similarity for each stimulus, betwween each pair of participants '''
-    nHor,nVer=nDiv,nDiv
-    SimSacP=np.zeros((self.ns,self.ns,self.np,nHor,nVer))  
+def SacSim1Group(self,Saccades,Thr=5,p='all',normalize='add'):
+    ''' calculate saccade similarity for each stimulus, between each pair of participants ,
+    needs saccades stored as PyEyeSim saccade objects stored in AOIs as input,
+    vertical and horizontal dimensions are inferred from the input
+    Thr=5: threshold for similarity'''
+    
+    nVer=np.shape(Saccades)[2]
+    nHor=np.shape(Saccades)[3]
+        
+    SimSacP=np.zeros((self.ns,self.ns,self.np,nVer,nHor))  
     SimSacP[:]=np.NaN
     for s1 in range(self.ns):
         for s2 in range(self.ns):
             if s1!=s2:
                 for p1 in range(self.np):
                     if self.nsac[s1,p1]>5 and self.nsac[s2,p1]>5:                    
                         for h in range(nHor):
                             for v in range(nVer):
-                                if len(Saccades[s1,p1,h,v])>0 and len(Saccades[s2,p1,h,v])>0:
+                                if len(Saccades[s1,p1,v,h])>0 and len(Saccades[s2,p1,v,h])>0:
                                         
-                                    simsacn=CalcSim(Saccades[s1,p1,h,v],Saccades[s2,p1,h,v],Thr=Thr)
-                                    SimSacP[s1,s2,p1,h,v]=simsacn/(len(Saccades[s1,p1,h,v])+len(Saccades[s2,p1,h,v]))
+                                    simsacn=CalcSim(Saccades[s1,p1,v,h],Saccades[s2,p1,v,h],Thr=Thr)
+                                    if normalize=='add':
+                                        SimSacP[s1,s2,p1,v,h]=simsacn/(len(Saccades[s1,p1,v,h])+len(Saccades[s2,p1,v,h]))
+                                    else:
+                                        SimSacP[s1,s2,p1,v,h]=simsacn/(len(Saccades[s1,p1,v,h])*len(Saccades[s2,p1,v,h]))
+ 
     return SimSacP
 
   
 
 
 def SacSimPipeline(self,divs=[4,5,7,9],Thr=5,InferS=True):
     SaccadeObj=self.GetSaccades()
     StimSims=np.zeros((len(divs),self.np))
     StimSimsInd=np.zeros((len(divs),self.ns,self.np))
 
     for cd,ndiv in enumerate(divs):
         print(cd,ndiv)
         sacDivSel=self.SaccadeSel(SaccadeObj,ndiv,InferS=InferS)
-        SimSacP=self.SacSim1Group(sacDivSel,ndiv,Thr=Thr)
+        SimSacP=self.SacSim1Group(sacDivSel,Thr=Thr)
         StimSimsInd[cd,:,:]=np.nanmean(np.nanmean(np.nanmean(SimSacP,4),3),0)
         StimSims[cd,:]=np.nanmean(np.nanmean(np.nanmean(np.nanmean(SimSacP,4),3),0),0)
     return StimSims,np.nanmean(StimSimsInd,0)
+
+
+def ScanpathSim2Groups(self,stim,betwcond,nHor=5,nVer=0,inferS=False,Thr=5,normalize='add'):
+    if hasattr(self,'subjects')==0:
+        self.GetParams()  
+    SaccadeObj=self.GetSaccades()
+    if type(stim)==str:
+        if stim=='all':
+            stimn=np.arange(self.ns)  # all stimuli
+        else:
+            stimn=np.nonzero(self.stimuli==stim)[0]
+
+    else:    
+        stimn=np.nonzero(self.stimuli==stim)[0]
+        
+    if nVer==0:
+        nVer=nHor  #
+    
+    SaccadeDiv=self.SaccadeSel(SaccadeObj,nHor=nHor,nVer=nVer,InferS=inferS)    
+    SimSacP=self.SacSim1Group(SaccadeDiv,Thr=Thr,normalize=normalize)
+    WhichC,WhichCN=self.GetGroups(betwcond)
+    Idxs=[]
    
+      
+    #Cols=['darkred','cornflowerblue']
+    fig,ax=plt.subplots(ncols=2,nrows=2,figsize=(10,8))
+                        
+    for cc,cond in enumerate(self.Conds):
+        Idxs.append(np.nonzero(WhichCN==cond)[0])
+    for cgr1,gr1 in enumerate(self.Conds):
+        for cgr2,gr2 in enumerate(self.Conds):
+            
+            Vals=np.nanmean(np.nanmean(SimSacP[Idxs[cgr1],:,stimn,:,:][:,Idxs[cgr2],:,:],0),0)  
+            self.VisGrid(Vals,stim,ax=ax[cgr1,cgr2],cbar=True,inferS=inferS,alpha=.8)
+            ax[cgr1,cgr2].set_title(gr1+' '+gr2)
+    
+    return
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/_stats.py` & `pyeyesim-0.3.1/PyEyeSim/_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,21 +283,21 @@
     return np.sum(immret),Dist1
 
 
 
     
     
 
-def BinnedDescriptives(self,length,binsize,timecol,durcol,startime=0):
+def BinnedDescriptives(self,length=5000,binsize=500,timecol='CURRENT_FIX_START',durcol='duration',startime=0):
     ''' time-binned within trial descriptive progression
     INPUTS
-    length: maximum trial length of interest in ms
-    binsize: length of timebin 
+    length: maximum trial length of interest in ms  (default 5000ms)
+    binsize: length of timebin  (default 500 ms)
     timecol: name of column with time length information
-    durcol: name of column with fixation duration information '''
+    durcol: name of column with fixation duration information -- if this is already provided during initalization should not be provided again'''
     Bins=np.arange(startime,length+binsize,binsize)
     print(f'Bins {Bins}')
     self.tbins=Bins
     self.binFixL=np.zeros((self.ns,self.np,len(Bins)-1))
     self.saccadeAmp=np.zeros((self.ns,self.np,len(Bins)-1))
     self.totLscanpath=np.zeros((self.ns,self.np,len(Bins)-1))
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/_visuals.py` & `pyeyesim-0.3.1/PyEyeSim/_visuals.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,55 +149,58 @@
             titStr='subj '+str(int(self.suseHMM[totest][0]))
         else:
             titStr='n subj '+str(len(totest))
 
     self.MySaccadeVis(ax[1],DatTest,lenTest,title='test data '+titStr)
     return 
 
-def VisGrid(self,vals,Stim,ax=0,alpha=.3,cmap='inferno',cbar=0,vmax=0):
+def VisGrid(self,vals,Stim,ax=0,alpha=.3,cmap='inferno',cbar=0,vmax=0,inferS=0):
     '''  
-    visualize grid on image
+    visualize transparent grid of values on stimulus image
 
     Arguments:
     vals: values to lay over image
-    stimn: stimulus number
+    Stim: stimulus name
 
 
     optional:
-
-    center: needed if not full screen images
+    ax: provide axis to plot, if not new figure is opened
+    alpha: transparency
+    inferS: needed if not full screen images, with background--> not calculating value for full image in this case, but using BoundsX&Y
     cb: visualize colorbar --> also returned   
+    vmax: to fix colormap max and minimum values at x/- vmax(for stimulus comparabilty)
+    
     '''
     if type(ax)==int:
         fig,ax=plt.subplots()
     idims=np.shape(self.images[Stim])
     yimsize,ximsize=idims[0],idims[1]
     
     ax.imshow(self.images[Stim])
+    if inferS==0:
+        horcells=np.linspace(0,ximsize,np.shape(vals)[1]+1)
+        vercells=np.linspace(0,yimsize,np.shape(vals)[0]+1)
+    else:
+        stimId=np.nonzero(self.stimuli==Stim)[0]   
+        horcells=np.linspace(self.boundsX[stimId,0],self.boundsX[stimId,1],np.shape(vals)[1]+1).flatten()
+        vercells=np.linspace(self.boundsY[stimId,0],self.boundsY[stimId,1],np.shape(vals)[0]+1).flatten()
     if vmax==0:
-        cols=ax.pcolormesh(np.linspace(0,ximsize,np.shape(vals)[1]+1),np.linspace(0,yimsize,np.shape(vals)[0]+1),vals,alpha=alpha,cmap=cmap)
+        cols=ax.pcolormesh(horcells,vercells,vals,alpha=alpha,cmap=cmap)
     else:
-        cols=ax.pcolormesh(np.linspace(0,ximsize,np.shape(vals)[1]+1),np.linspace(0,yimsize,np.shape(vals)[0]+1),vals,alpha=alpha,cmap=cmap,vmin=-vmax,vmax=vmax)
-
-#    else:
- #       stimId=self.stimuli==Stim
-  #      if vmax==0:
-   #         cols=ax.pcolormesh(np.linspace(self.boundsX[stimId,0],self.boundsX[stimId,1],np.shape(vals)[1]+1),np.linspace(self.boundsY[stimId,0],self.boundsY[stimId,1],np.shape(vals)[0]+1),vals,alpha=alpha,cmap=cmap)
-    #    else:
-     #       cols=ax.pcolormesh(np.linspace(self.boundsX[stimId,0],self.boundsX[stimId,1],np.shape(vals)[1]+1),np.linspace(self.boundsY[stimId,0],self.boundsY[stimId,1],np.shape(vals)[0]+1),vals,alpha=alpha,cmap=cmap,vmin=-vmax,vmax=vmax)
+        cols=ax.pcolormesh(horcells,vercells,vals,alpha=alpha,cmap=cmap,vmin=-vmax,vmax=vmax)
     ax.set_xticks([])
     ax.set_yticks([])
     if cbar:
         cb=plt.colorbar(cols,ax=ax,shrink=.6)
     else:
         cb=0
     return cb
         
 
-def Hihglight_Sign(self,Stim,pvals,axis):
+def Highlight_Sign(self,Stim,pvals,axis):
     idims=np.shape(self.images[Stim])
     yimsize,ximsize=idims[0],idims[1]
     x,y=np.linspace(0,ximsize,np.shape(pvals)[1]+1),np.linspace(0,yimsize,np.shape(pvals)[0]+1)
     for i in range(len(x) - 1):
         for j in range(len(y) - 1):
             if pvals[j,i]<.05:
                 if pvals[j,i]<.01:
@@ -210,8 +213,38 @@
                 if i<len(x):
                     axis.plot([x[i+1], x[i+1]], [y[j], y[j + 1]], color='k',linestyle=linestyle)  # Vertical lines
                 if j <len(y):
                     axis.plot([x[i], x[i + 1]], [y[j+1], y[j+1]], color='k',linestyle=linestyle)  # Horizontal lines
     axis.set_xlabel(f'num sign p<.05: {np.sum(pvals<.05)} ,chance expectation: {np.round(np.shape(pvals)[0]*np.shape(pvals)[1]*.05,1)} ')  
     return 
 
+
+def VisHeatmap(self,Stim,smap,ax=0,cutoff=0,alpha=.5,cmap='plasma',cbar=False,cbarlabel=False,title=''):
+    if cutoff=='median':
+        cutThr=np.median(smap)
+    elif cutoff>0:
+        cutThr=np.percentile(smap,cutoff) 
+    else:
+        cutThr=0
+    smap[smap<cutThr]=np.NAN  # replacing below threshold with NAN
+    if ax==False:
+        fig,ax=plt.subplots()
+    if hasattr(self,'images')==True:
+        ax.imshow(self.images[Stim])
+    cols=ax.imshow(smap,alpha=alpha,cmap=cmap) 
+    if cbar:
+        cb=plt.colorbar(cols,ax=ax,shrink=.6)
+        if cbarlabel!=' ':
+            cb.ax.get_yaxis().set_ticks([])
+            cb.ax.get_yaxis().labelpad = 15
+            cb.ax.set_ylabel(cbarlabel, rotation=270)
+
+    ax.set_xticks([])
+    ax.set_yticks([])
+    ax.set_xlim(0,np.shape(self.images[Stim])[1])
+    ax.set_ylim(np.shape(self.images[Stim])[0],0)
+    ax.set_title(title)
+   
+    return
+
+
 # %%
```

### Comparing `pyeyesim-0.3.0/PyEyeSim/hmmhelper.py` & `pyeyesim-0.3.1/PyEyeSim/hmmhelper.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/pyeyesim.py` & `pyeyesim-0.3.1/PyEyeSim/pyeyesim.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/pyeyesim_old.py` & `pyeyesim-0.3.1/PyEyeSim/pyeyesim_old.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/scanpathshelpdebug.py` & `pyeyesim-0.3.1/PyEyeSim/scanpathshelpdebug.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/scanpathsimhelper.py` & `pyeyesim-0.3.1/PyEyeSim/scanpathsimhelper.py`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/PyEyeSim/visualhelper.py` & `pyeyesim-0.3.1/PyEyeSim/visualhelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,37 @@
         ax.set_xticks(np.arange(N),labels=xtickL,fontsize=9,rotation=60)
     ax.set_xlabel('Stimulus',fontsize=14)
     ax.set_ylabel(yLab,fontsize=14)
     return None
 
 
 
-def HistPlot(Y,xtickL=0,ax=0):
+def HistPlot(Y,xtickL=0,ax=0,ylab='Num of observers',verline=False,mean=True,title=''):
     ''' expected data format: row-  subjects column- stimuli '''
-    assert len(np.shape(Y))==2, '2d data is expected: observer*stimulus'
     if type(ax)==int:
         fig,ax=plt.subplots()
-    ax.hist(np.nanmean(Y,1),color='darkred')
+        
+    if mean:
+        Y=np.nanmean(Y,1)
+        
+    ax.hist(Y,color='darkred')
     ax.set_xlabel(xtickL,fontsize=14)
-    ax.set_ylabel('Num observers',fontsize=13)
+    ax.set_ylabel(ylab,fontsize=13)
+    if verline:
+        ax.axvline(verline,color='k')
+    ax.set_title(title)
     return None
 
 
+
     
 def VisBinnedProg(bins,Y,ylabel,col='navy',label='',axin=0):
     if type(axin)==int:
         fig,axin=plt.subplots()
-    axin.errorbar((bins[0:-1]+bins[1:])/2,np.nanmean(Y,0),stats.sem(Y,0,nan_policy='omit'),color=col,linewidth=2,label=label)
+    axin.errorbar((bins[0:-1]+bins[1:])/2,np.nanmean(Y,0),stats.sem(Y,0,nan_policy='omit'),color=col,linewidth=2,label=label,alpha=.5)
     axin.set_xlabel('time (ms)')
     axin.yaxis.set_major_locator(ticker.MaxNLocator(5))
     axin.set_ylabel(ylabel)
     return axin
```

### Comparing `pyeyesim-0.3.0/README.md` & `pyeyesim-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/pyeyesim.egg-info/PKG-INFO` & `pyeyesim-0.3.1/pyeyesim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeyesim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Eye movement analysis and visualization package, with a focus on fixation map and scanpath similarity
 Author: jozsef arato
 Author-email: Jozsef Arato <jozsef.arato@gmail.com>
 Project-URL: Homepage, https://github.com/jozsarato/PyEyeSim
 Project-URL: Issues, https://github.com/jozsarato/PyEyeSim/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `pyeyesim-0.3.0/pyeyesim.egg-info/SOURCES.txt` & `pyeyesim-0.3.1/pyeyesim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyeyesim-0.3.0/pyproject.toml` & `pyeyesim-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyeyesim"
-version = "0.3.0"
+version = "0.3.1"
 requires-python = ">=3.8"
 authors = [
   { name="Jozsef Arato", email="jozsef.arato@gmail.com" },
 ]
 description = "Eye movement analysis and visualization package, with a focus on fixation map and scanpath similarity"
 readme = "README.md"
 classifiers = [
```

