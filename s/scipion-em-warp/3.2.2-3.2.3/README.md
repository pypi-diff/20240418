# Comparing `tmp/scipion-em-warp-3.2.2.tar.gz` & `tmp/scipion-em-warp-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-warp-3.2.2.tar", last modified: Mon Feb 26 12:49:56 2024, max compression
+gzip compressed data, was "scipion-em-warp-3.2.3.tar", last modified: Thu Apr 18 12:45:36 2024, max compression
```

## Comparing `scipion-em-warp-3.2.2.tar` & `scipion-em-warp-3.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:49:56.806373 scipion-em-warp-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-26 12:49:56.806373 scipion-em-warp-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:49:56.802373 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-26 12:49:56.000000 scipion-em-warp-3.2.2/scipion_em_warp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 12:49:56.806373 scipion-em-warp-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:49:56.802373 scipion-em-warp-3.2.2/warp/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:49:56.806373 scipion-em-warp-3.2.2/warp/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_mics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_tomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:49:56.806373 scipion-em-warp-3.2.2/warp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/tests/test_protocols_tomo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-02-26 12:49:33.000000 scipion-em-warp-3.2.2/warp/warp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 12:45:36.000000 scipion-em-warp-3.2.3/scipion_em_warp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.239958 scipion-em-warp-3.2.3/warp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_mics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:45:36.243958 scipion-em-warp-3.2.3/warp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/tests/test_protocols_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-04-18 12:45:11.000000 scipion-em-warp-3.2.3/warp/warp_logo.png
```

### Comparing `scipion-em-warp-3.2.2/LICENSE` & `scipion-em-warp-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/PKG-INFO` & `scipion-em-warp-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-warp
-Version: 3.2.2
+Version: 3.2.3
 Summary: Plugin to use Warp within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-warp
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-warp/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-warp/
```

### Comparing `scipion-em-warp-3.2.2/README.rst` & `scipion-em-warp-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/scipion_em_warp.egg-info/PKG-INFO` & `scipion-em-warp-3.2.3/scipion_em_warp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-warp
-Version: 3.2.2
+Version: 3.2.3
 Summary: Plugin to use Warp within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-warp
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-warp/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-warp/
```

### Comparing `scipion-em-warp-3.2.2/scipion_em_warp.egg-info/SOURCES.txt` & `scipion-em-warp-3.2.3/scipion_em_warp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/setup.py` & `scipion-em-warp-3.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/__init__.py` & `scipion-em-warp-3.2.3/warp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pwem
 
 
-__version__ = '3.2.2'
+__version__ = '3.2.3'
 _references = ['Nickell2005', 'Tegunov2019']
 _logo = "warp_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-warp"
```

### Comparing `scipion-em-warp-3.2.2/warp/bibtex.py` & `scipion-em-warp-3.2.3/warp/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/protocols/__init__.py` & `scipion-em-warp-3.2.3/warp/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/protocols/protocol_base.py` & `scipion-em-warp-3.2.3/warp/protocols/protocol_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,24 +23,45 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 import mrcfile
 
+from pyworkflow.protocol import FloatParam, Positive, LEVEL_ADVANCED
 import pyworkflow.utils as pwutils
 from pwem.protocols import EMProtocol
 from pwem.emlib.image import ImageHandler
 
 from warp.utils import tom_deconv
 
 
 class ProtWarpBase(EMProtocol):
     _label = None
 
+    # -------------------------- DEFINE param functions -----------------------
+    @classmethod
+    def defineProcessParams(cls, form):
+        form.addParam('deconvstrength', FloatParam, validators=[Positive],
+                      default=1.0,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='Deconvolution strength',
+                      help='Strength parameter for the deconvolution filter.')
+        form.addParam('snrfalloff', FloatParam, validators=[Positive],
+                      default=1.1,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='SNR falloff',
+                      help='SNR falloff parameter for the deconvolution filter.')
+        form.addParam('highpassnyquist', FloatParam, validators=[Positive],
+                      default=0.02,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='High-pass fraction',
+                      help='Fraction of Nyquist frequency to be cut off on '
+                           'the lower end (since it will be boosted the most).')
+        
     # --------------------------- STEPS functions -----------------------------
     def _insertAllSteps(self):
         self._insertFunctionStep(self.deconvolveStep)
         self._insertFunctionStep(self.createOutputStep)
 
     def deconvolveStep(self):
         raise NotImplementedError
@@ -65,25 +86,31 @@
 
         voltage = acquisition.getVoltage()
         cs = acquisition.getSphericalAberration()
         ncpu = self.numberOfThreads.get()
         gpu = self.usesGpu()
         gpuid = self.getGpuList()[0]
 
+        snrfalloff = self.snrfalloff.get()
+        deconvstrength = self.deconvstrength.get()
+        highpassnyquist = self.highpassnyquist.get()
+
         for item in inputList:
             key = item[keyName]
             if key in ctfDict:
                 fileName = item["_filename"]
                 defocus = ctfDict[key] / 10000
                 outputFn = self._getOutputFn(fileName)
                 self.info(f"Deconvolving {fileName}")
 
                 func = self._processStack if isTS else self._processImage
                 func(fileName, outputFn, angpix=pixSize, voltage=voltage,
-                     cs=cs, defocus=defocus, ncpu=ncpu, gpu=gpu, gpuid=gpuid)
+                     cs=cs, defocus=defocus, ncpu=ncpu, gpu=gpu, gpuid=gpuid,
+                     snrfalloff=snrfalloff, deconvstrength=deconvstrength,
+                     highpassnyquist=highpassnyquist)
             else:
                 self.warning(f"No CTF found for: {key}")
 
     # --------------------------- INFO functions ------------------------------
     def _warnings(self):
         warnings = []
 
@@ -99,26 +126,26 @@
     def _updateItem(self, item, row):
         outputFn = self._getOutputFn(item.getFileName())
         if os.path.exists(outputFn):
             item.setFileName(outputFn)
         else:
             item._appendItem = False
 
-    @classmethod
-    def _processImage(cls, inputFn, outputFn, **kwargs):
+    @staticmethod
+    def _processImage(inputFn, outputFn, **kwargs):
         ih = ImageHandler()
         inputData = ih.read(inputFn).getData()
         result = tom_deconv(inputData, **kwargs)
         with mrcfile.new(outputFn) as mrcOut:
             mrcOut.set_data(result)
             mrcOut.voxel_size = kwargs["angpix"]
             mrcOut.update_header_from_data()
 
-    @classmethod
-    def _processStack(cls, inputFn, outputFn, **kwargs):
+    @staticmethod
+    def _processStack(inputFn, outputFn, **kwargs):
         ih = ImageHandler()
         x, y, z, n = ih.getDimensions(inputFn)
         stack_shape = (n, y, x)
         mrc = mrcfile.new_mmap(outputFn, shape=stack_shape,
                                mrc_mode=2, overwrite=True)
         for i in range(n):
             inputData = ih.read((i + 1, inputFn)).getData()
```

### Comparing `scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_mics.py` & `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_mics.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         form.addParam('ctfRelations', params.RelationParam,
                       important=True,
                       relationName=RELATION_CTF,
                       attributeName='getInputMicrographs',
                       label='CTF estimation',
                       help='Choose a CTF estimation '
                            'related to the input micrographs.')
-
+        
+        self.defineProcessParams(form)
         form.addParallelSection(threads=8, mpi=0)
 
     # --------------------------- STEPS functions -----------------------------
     def deconvolveStep(self):
         """ Load input CTFs and micrograph sets, then run deconvolution. """
         ctfDict = dict()
         for ctf in self.ctfRelations.get():
```

### Comparing `scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_tomo.py` & `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_tomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
                       params.PointerParam,
                       pointerClass='SetOfCTFTomoSeries',
                       important=True,
                       label='CTF tomo series',
                       help='Set of CTFs that correspond to the '
                            'input above. The matching is done using tsId.')
 
+        self.defineProcessParams(form)
         form.addParallelSection(threads=8, mpi=0)
+        
 
     # --------------------------- STEPS functions -----------------------------
     def deconvolveStep(self):
         """ Load CTF and tomograms sets, match by tsId before processing. """
         tomoSet = self.getInputTomos()
         ctfSet = self.inputCTFs.get()
         acq = tomoSet.getAcquisition()
```

### Comparing `scipion-em-warp-3.2.2/warp/protocols/protocol_deconv_ts.py` & `scipion-em-warp-3.2.3/warp/protocols/protocol_deconv_ts.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         form.addParam('inputCTFs',
                       params.PointerParam,
                       pointerClass='SetOfCTFTomoSeries',
                       important=True,
                       label='CTF tomo series',
                       help='Set of CTFs that correspond to the '
                            'input above. The matching is done using tsId.')
-
+        
+        self.defineProcessParams(form)
         form.addParallelSection(threads=8, mpi=0)
 
     # --------------------------- STEPS functions -----------------------------
     def deconvolveStep(self):
         """ Load CTF and TS sets, match by tsId before processing. """
         tsSet = self.getInputTS()
         ctfSet = self.inputCTFs.get()
```

### Comparing `scipion-em-warp-3.2.2/warp/protocols.conf` & `scipion-em-warp-3.2.3/warp/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/tests/__init__.py` & `scipion-em-warp-3.2.3/warp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/tests/test_protocols.py` & `scipion-em-warp-3.2.3/warp/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/tests/test_protocols_tomo.py` & `scipion-em-warp-3.2.3/warp/tests/test_protocols_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/utils.py` & `scipion-em-warp-3.2.3/warp/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-warp-3.2.2/warp/warp_logo.png` & `scipion-em-warp-3.2.3/warp/warp_logo.png`

 * *Files identical despite different names*

