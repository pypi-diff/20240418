# Comparing `tmp/pystorm3-0.1.5.tar.gz` & `tmp/pystorm3-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.5.tar", last modified: Fri Apr 12 13:03:51 2024, max compression
+gzip compressed data, was "pystorm3-0.1.6.tar", last modified: Wed Apr 17 17:49:19 2024, max compression
```

## Comparing `pystorm3-0.1.5.tar` & `pystorm3-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.5/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-12 13:03:51.240546 pystorm3-0.1.5/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.5/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1074 2024-04-12 11:34:02.000000 pystorm3-0.1.5/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/pystorm/signal_processing/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      652 2024-04-12 12:13:01.000000 pystorm3-0.1.5/pystorm/signal_processing/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     9434 2024-04-12 13:03:37.000000 pystorm3-0.1.5/pystorm/signal_processing/band_filter.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      761 2024-04-12 11:20:10.000000 pystorm3-0.1.5/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     6902 2024-04-12 12:55:13.000000 pystorm3-0.1.5/pystorm/timefreq/analytical_signal.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     4414 2024-04-12 12:54:52.000000 pystorm3-0.1.5/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      409 2024-04-12 11:26:22.000000 pystorm3-0.1.5/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    34849 2024-04-12 12:22:18.000000 pystorm3-0.1.5/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-12 13:03:45.000000 pystorm3-0.1.5/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 13:03:51.240546 pystorm3-0.1.5/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-12 13:03:51.000000 pystorm3-0.1.5/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      453 2024-04-12 13:03:51.000000 pystorm3-0.1.5/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-12 13:03:51.000000 pystorm3-0.1.5/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-12 13:03:51.000000 pystorm3-0.1.5/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-12 13:03:51.000000 pystorm3-0.1.5/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-12 13:03:51.240546 pystorm3-0.1.5/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.5/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.857699 pystorm3-0.1.6/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.6/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-04-17 17:49:19.857699 pystorm3-0.1.6/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1933 2024-04-17 17:48:22.000000 pystorm3-0.1.6/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.815699 pystorm3-0.1.6/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1102 2024-04-17 17:40:11.000000 pystorm3-0.1.6/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.836700 pystorm3-0.1.6/pystorm/connectivity/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      658 2024-04-17 17:43:32.000000 pystorm3-0.1.6/pystorm/connectivity/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4495 2024-04-17 17:43:16.000000 pystorm3-0.1.6/pystorm/connectivity/amplitude_envelope_correlation.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.836700 pystorm3-0.1.6/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      652 2024-04-12 12:13:01.000000 pystorm3-0.1.6/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    39786 2024-04-17 17:37:14.000000 pystorm3-0.1.6/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.855699 pystorm3-0.1.6/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      761 2024-04-12 11:20:10.000000 pystorm3-0.1.6/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    42449 2024-04-17 17:37:04.000000 pystorm3-0.1.6/pystorm/timefreq/analytical_signal.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4457 2024-04-16 12:53:00.000000 pystorm3-0.1.6/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.855699 pystorm3-0.1.6/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      409 2024-04-12 11:26:22.000000 pystorm3-0.1.6/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    37594 2024-04-16 14:52:01.000000 pystorm3-0.1.6/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-16 11:03:05.000000 pystorm3-0.1.6/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-17 17:49:19.856700 pystorm3-0.1.6/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2815 2024-04-17 17:49:19.000000 pystorm3-0.1.6/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      541 2024-04-17 17:49:19.000000 pystorm3-0.1.6/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-17 17:49:19.000000 pystorm3-0.1.6/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       69 2024-04-17 17:49:19.000000 pystorm3-0.1.6/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-17 17:49:19.000000 pystorm3-0.1.6/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-17 17:49:19.857699 pystorm3-0.1.6/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1572 2024-04-17 17:48:50.000000 pystorm3-0.1.6/setup.py
```

### Comparing `pystorm3-0.1.5/LICENSE` & `pystorm3-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.5/PKG-INFO` & `pystorm3-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
-Keywords: neuroscience,neuroimaging,neural oscillations,time series analysis,time frequency analysis,electrophysiology
+Keywords: neuroscience,neuroimaging,neural oscillations,time series analysis,time frequency analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.0
 Requires-Dist: numpy>=1.26
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: torchaudio>=2.2.0
+Requires-Dist: numba>=0.59
 
 # Pystorm
 Python implementation of various functions from the [Brainstorm](https://neuroimage.usc.edu/brainstorm/) [repository](https://github.com/brainstorm-tools/brainstorm3), often written for GPU compatibility and/or jit compilation.
 
 ## Note on the current scope of Pystorm
 Pystorm does not handle interactions with Brainstorm or matlab and, in its current state, does not handle loading of data files. 
 
@@ -42,15 +43,15 @@
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m)). Can only be applied on signal directly for now: does not work with (sensor, kernel) input.
 
 ### Coming soon
-- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.5/README.md` & `pystorm3-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m)). Can only be applied on signal directly for now: does not work with (sensor, kernel) input.
 
 ### Coming soon
-- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.5/pystorm/__init__.py` & `pystorm3-0.1.6/pystorm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 Currently contains: Welch PSD (sensor and source space), band pass filter, hilbert transform, minitorch (also available as 'mnt').
 """
 
 from .utils import *
 from .utils import minitorch as mnt
 from .signal_processing import *
 from .timefreq import *
+from .connectivity import *
 
 from .version import __version__
```

### Comparing `pystorm3-0.1.5/pystorm/signal_processing/__init__.py` & `pystorm3-0.1.6/pystorm/signal_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.5/pystorm/timefreq/__init__.py` & `pystorm3-0.1.6/pystorm/timefreq/__init__.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.5/pystorm/timefreq/welch_psd.py` & `pystorm3-0.1.6/pystorm/timefreq/welch_psd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pystorm.utils import minitorch as mnt
 from pystorm.utils.minitorch import ensure_numpy
+from sys import stderr 
 __all__ = ["welch_psd_source_space", "welch_psd_sensor_space"]
 
 def welch_psd_source_space(time_series, fs:int, ker = None, window_length=2000, overlap = 0.5, device = "cpu"):
 
     
     """ This function computes the PSD of source-space signals using the welch method. It can be called on the source time series directly or on the sensor time series with the imaging kernel
     
@@ -24,39 +25,38 @@
         Returns: 
             psd: numpy array                       
                 The PSD of the source signal
             freqs: numpy array                       
                 The frequencies of the PSD.
     """
 
-
     if ker is None:
         return welch_psd_sensor_space(time_series, fs, window_length=window_length, overlap = overlap, device = device)
     nTime = time_series.shape[-1]
     Lwin = round(window_length/1000*fs)
     Loverlap = round(Lwin * overlap)
     Lwin = Lwin - Lwin%2
     Nwin = int((nTime - Loverlap)/(Lwin-Loverlap))
 
     freqs = mnt.rfftfreq(Lwin,1/fs).to(device)
     ker_cuda = mnt.ensure_torch(ker, type_float=True).to(device).type(mnt.__default_complex_dtype__)
-    sensor_cuda = mnt.ensure_torch(time_series, type_float=True).to(device)
+    sensor_cuda = mnt.ensure_torch(time_series, type_float=True)
     hamming_window = (0.54 - 0.46 * mnt.cos(mnt.linspace(0,2*mnt.pi,Lwin))).to(device)
 
     win_noise_power_gain = (hamming_window**2).sum()
     scaling_term = (2/(win_noise_power_gain*fs)).sqrt()
     time_sequence = mnt.arange(0,Lwin, dtype = int)
 
     fft_blocks = 0
     for i in range(Nwin):
         iTimes =  time_sequence + (i - 1)*(Lwin-Loverlap)
-        block = sensor_cuda[:,iTimes]
-        source_ts = (block) * hamming_window
-        fft_res = mnt.rfft(source_ts,dim = -1) * scaling_term
-        fft_res[:,1:] /= 2**(1/2)
+        block = sensor_cuda[..., iTimes].to(device)
+        windowed_ts = (block) * hamming_window
+        fft_res = mnt.rfft(windowed_ts,dim = -1) * scaling_term
+        fft_res[..., 1:] /= 2**(1/2)
         fft_blocks += (ker_cuda @ fft_res).abs()**2/Nwin
         
     return ensure_numpy(fft_blocks), ensure_numpy(freqs)
 
 def welch_psd_sensor_space(time_series, fs:int, window_length=2000, overlap = 0.5, device = "cpu"):
     """ This function computes the PSD of sensor-space signals using the welch method.
     
@@ -82,24 +82,24 @@
     nTime = time_series.shape[-1]
     Lwin = round(window_length/1000*fs)
     Loverlap = round(Lwin * overlap)
     Lwin = Lwin - Lwin%2
     Nwin = int((nTime - Loverlap)/(Lwin-Loverlap))
 
     freqs = mnt.rfftfreq(Lwin,1/fs).to(device)
-    sensor_cuda = mnt.ensure_torch(time_series).to(device)
+    sensor_cuda = mnt.ensure_torch(time_series)
     hamming_window = (0.54 - 0.46 * mnt.cos(mnt.linspace(0,2*mnt.pi,Lwin))).to(device)
 
     win_noise_power_gain = (hamming_window**2).sum()
     scaling_term = (2/(win_noise_power_gain*fs)).sqrt()
     time_sequence = mnt.arange(0,Lwin, dtype = int)
 
     fft_blocks = 0
     for i in range(Nwin):
         iTimes =  time_sequence + (i - 1)*(Lwin-Loverlap)
-        block = sensor_cuda[:,iTimes]
-        source_ts = (block) * hamming_window
-        fft_res = mnt.rfft(source_ts,dim = -1) * scaling_term
-        fft_res[:,1:] /= 2**(1/2)
+        block = sensor_cuda[..., iTimes].to(device)
+        windowed_ts = (block) * hamming_window
+        fft_res = mnt.rfft(windowed_ts,dim = -1) * scaling_term
+        fft_res[..., 1:] /= 2**(1/2)
         fft_blocks += (fft_res).abs()**2/Nwin
 
     return ensure_numpy(fft_blocks), ensure_numpy(freqs)
```

### Comparing `pystorm3-0.1.5/pystorm/utils/minitorch.py` & `pystorm3-0.1.6/pystorm/utils/minitorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,52 +26,77 @@
 from torch import eye as _eye
 from torch import argwhere as _argwhere
 from torchaudio.functional import convolve as _convolve
 from torchaudio.functional import fftconvolve as _fftconvolve
 from torch import float16,float32,float64
 from torch import set_default_dtype
 from numpy import ndarray as _ndarray
+from numpy import float32 as _np_float32
+from numpy import float64 as _np_float64
+from numpy import complex64 as _np_complex64
+from numpy import complex128 as _np_complex128
+from numpy import array as _np_array
 from torch import Tensor as _Tensor
+from torch.cuda import mem_get_info as _mem_get_info
+
+def _check_available_memory():
+    return _mem_get_info()[0]
+
 pi = _pi
 __all__=[
         "rfft","rfftfreq","fft","ifft","fftfreq","convolve","fftconvolve",
         "linspace","arange","argwhere",
         "cat","zeros","ones","zeros_like","ones_like","eye",
         "as_tensor","from_numpy","ensure_numpy","ensure_torch",
         "cos","pi",
-        "float16","float32","float64","complex64","complex128",
-        "set_minitorch_default_dtype","__default_dtype__","__default_complex_dtype__"
+        "float16","float32","float64","complex64","complex128","_np_float32","_np_float64",
+        "set_minitorch_default_dtype","__default_dtype__","__default_complex_dtype__","_check_available_memory"
 ]
 __default_dtype__ = float64
 __default_complex_dtype__ = complex128
+__default_np_dtype__ = _np_float64
+__default_np_complex_dtype__ = _np_complex128
+__default_dtype_str__ = "float64"
+__default_complex_dtype_str__ = "complex128"
+
 set_default_dtype(__default_dtype__)
 def set_minitorch_default_dtype(default_type: str = "float64"):
     """ This function allows for specifying a floating point precision (and its matching complex precision). Default is float64 and complex128.
 
         Args: 
             None
         Keyword Args: 
             default_type: str     
                 String that specifies the default floating point type of the pytorch backend
         Returns: 
             None
 
     """
 
-    global __default_dtype__, __default_complex_dtype__
+    global __default_dtype__, __default_complex_dtype__, __default_np_dtype__, __default_np_complex_dtype__, __default_dtype_str__, __default_complex_dtype_str__
     if default_type == "float16":
         __default_dtype__ = float16
-        print("Warning: Pytorch only supports FFT of signals whose length are powers of 2 in this float type")
+        __default_dtype_str__ = "float16"
+        print("Precision Type Warning [minitorch]: Most functions don't support this type (for now).")
     elif default_type == "float32":
         __default_dtype__ = float32
+        __default_np_dtype__ = _np_float32
+        __default_np_complex_dtype__ = _np_complex64
         __default_complex_dtype__ = complex64
+        __default_dtype_str__ = "float32"
+        __default_complex_dtype_str__ = "complex64"
     else:
         __default_dtype__ = float64
+        __default_np_dtype__ = _np_float64
+        __default_np_complex_dtype__ = _np_complex128
         __default_complex_dtype__ = complex128
+        __default_dtype_str__ = "float64"
+        __default_complex_dtype_str__ = "complex128"
     set_default_dtype(__default_dtype__)
+    print("Type Warning: All previously defined tensors or arrays might have incompatible types with the new default, this could cause some functions to crash, especially those that depend on numba.")
     
 
 def ensure_torch(x, type_float: bool = False, type_complex: bool = False):
     """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype').
     
         Args: 
             x: list/numpy array/torch tensor/primitive type that can be contained in a torch tensor (e.g., float, int, bool)
@@ -109,14 +134,68 @@
                 x = x.type(dtype_setting)
             return x
         except:
             pass
     return x
 
 
+def ensure_numpy(x, type_float: bool = False, type_complex: bool = False):
+    """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype').
+    
+        Args: 
+            x: list/numpy array/torch tensor/primitive type that can be contained in a torch tensor (e.g., float, int, bool)
+                Input variable.
+        Keyword Args: 
+            type_float: bool          
+                Specifies whether to set the type of the tensor.
+            type_complex: bool        
+                Specifies if the type of the tensor is meant to be complex
+        Returns:
+            x: Torch tensor
+                The input ensured to be a torch tensor.
+
+    """
+    dtype_setting = __default_np_dtype__
+    if type_complex:
+        dtype_setting = __default_np_complex_dtype__
+    if isinstance(x, _ndarray):
+        if not type_float:
+            return x
+        try:
+            x = x.astype(dtype_setting)
+            return x
+        except:
+            pass
+    try:
+        x = x.detach()
+    except:
+        pass
+    try:
+        x = x.cpu()
+    except:
+        pass
+    try:
+        x = x.numpy()
+    except:
+        pass
+    if type_float:
+        try:
+            x = x.astype(dtype_setting)
+            return x
+        except:
+            pass
+    try:
+        x = _np_array(x)
+        if type_float:
+            x = x.astype(dtype_setting)
+        return x
+    except:
+        pass
+    return x
+
 def _ensure_torch(x, type_float: bool = False, type_complex: bool = False):
     """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype'). Differs from 'ensure_torch' by returning False if it could not cast it as a tensor instead of returning the input.
     
         Args: 
             x: list/numpy array/torch tensor/primitive type that can be contained in a torch tensor (e.g., float, int, bool)
                 Input variable.
         Keyword Args: 
@@ -153,15 +232,15 @@
             if type_float:
                 x = x.type(dtype_setting)
             return True, x
         except:
             pass
     return False, x
 
-def ensure_numpy(x):
+def _ensure_numpy_old(x):
     """ This function ensures that the variable is a numpy array. 
     
         Args: 
             x: list/numpy array/torch tensor/primitive type that can be contained in a numpy array (e.g., float, int, bool)
                 Input variable.
         Keyword Args: 
             None
@@ -181,15 +260,14 @@
         x = x.cpu()
     except:
         pass
     
     try:
         x = x.numpy()
     except:
-        # Handle the case where it's a list
         try:
             is_torch_now, x = _ensure_torch(x)
             if is_torch_now: # Avoids infinite loop if for some reason casting fails
                 x = ensure_numpy(x)
                 return x
             else:
                 return x
```

### Comparing `pystorm3-0.1.5/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.6/pystorm3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
-Keywords: neuroscience,neuroimaging,neural oscillations,time series analysis,time frequency analysis,electrophysiology
+Keywords: neuroscience,neuroimaging,neural oscillations,time series analysis,time frequency analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.0
 Requires-Dist: numpy>=1.26
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: torchaudio>=2.2.0
+Requires-Dist: numba>=0.59
 
 # Pystorm
 Python implementation of various functions from the [Brainstorm](https://neuroimage.usc.edu/brainstorm/) [repository](https://github.com/brainstorm-tools/brainstorm3), often written for GPU compatibility and/or jit compilation.
 
 ## Note on the current scope of Pystorm
 Pystorm does not handle interactions with Brainstorm or matlab and, in its current state, does not handle loading of data files. 
 
@@ -42,15 +43,15 @@
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m)). Can only be applied on signal directly for now: does not work with (sensor, kernel) input.
 
 ### Coming soon
-- Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.5/setup.py` & `pystorm3-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,24 +21,24 @@
    maintainer_email='dominic.boutet@mail.mcgill.ca',
    url='https://github.com/NeuroLife77/pystorm',
    packages=find_packages(),
    install_requires=[
                         'torch>=2.2.0',
                         'numpy>=1.26',
                         'scipy>=1.13.0',
-                        'torchaudio>=2.2.0'
+                        'torchaudio>=2.2.0',
+                        "numba>=0.59"
     ],
    python_requires='>=3.9',
    keywords = [
                     'neuroscience',
                     'neuroimaging',
                     'neural oscillations',
                     'time series analysis',
                     'time frequency analysis',
-                    'electrophysiology'
     ],
    classifiers=[
                 'Development Status :: 1 - Planning',
                 'Intended Audience :: Science/Research',
                 'Topic :: Scientific/Engineering',
                 'Operating System :: Unix',
                 'Programming Language :: Python',
```

