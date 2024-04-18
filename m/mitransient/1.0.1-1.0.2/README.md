# Comparing `tmp/mitransient-1.0.1.tar.gz` & `tmp/mitransient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitransient-1.0.1.tar", last modified: Mon Apr  8 16:11:59 2024, max compression
+gzip compressed data, was "mitransient-1.0.2.tar", last modified: Thu Apr 18 12:20:14 2024, max compression
```

## Comparing `mitransient-1.0.1.tar` & `mitransient-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.404162 mitransient-1.0.1/
--rw-r--r--   0 droyo     (1000) droyo     (1000)    14068 2024-04-08 16:11:59.400162 mitransient-1.0.1/PKG-INFO
--rw-r--r--   0 droyo     (1000) droyo     (1000)    13739 2024-04-08 16:11:02.000000 mitransient-1.0.1/README.md
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      840 2024-04-08 16:11:02.000000 mitransient-1.0.1/mitransient/__init__.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient/films/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      877 2024-03-30 15:31:47.000000 mitransient-1.0.1/mitransient/films/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     5309 2024-03-30 15:31:52.000000 mitransient-1.0.1/mitransient/films/transient_hdr_film.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient/integrators/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      904 2024-03-30 15:31:54.000000 mitransient-1.0.1/mitransient/integrators/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    14232 2024-03-30 15:31:56.000000 mitransient-1.0.1/mitransient/integrators/common.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    22047 2024-03-30 15:31:58.000000 mitransient-1.0.1/mitransient/integrators/transient_prb_volpath.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    27872 2024-04-08 16:11:07.000000 mitransient-1.0.1/mitransient/integrators/transientnlospath.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    13233 2024-03-30 15:32:03.000000 mitransient-1.0.1/mitransient/integrators/transientpath.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1576 2024-03-30 18:48:01.000000 mitransient-1.0.1/mitransient/nlos.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient/render/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      877 2024-03-30 15:32:07.000000 mitransient-1.0.1/mitransient/render/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     8169 2024-03-30 15:32:06.000000 mitransient-1.0.1/mitransient/render/transient_block.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient/sensors/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      877 2024-03-30 15:32:09.000000 mitransient-1.0.1/mitransient/sensors/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     8184 2024-03-30 18:52:55.000000 mitransient-1.0.1/mitransient/sensors/nloscapturemeter.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)      319 2024-03-30 15:32:13.000000 mitransient-1.0.1/mitransient/sensors/nlossensor.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3365 2024-03-30 15:39:10.000000 mitransient-1.0.1/mitransient/utils.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1529 2024-04-08 16:11:17.000000 mitransient-1.0.1/mitransient/version.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2024-04-08 16:11:59.400162 mitransient-1.0.1/mitransient.egg-info/
--rw-r--r--   0 droyo     (1000) droyo     (1000)    14068 2024-04-08 16:11:59.000000 mitransient-1.0.1/mitransient.egg-info/PKG-INFO
--rw-r--r--   0 droyo     (1000) droyo     (1000)      730 2024-04-08 16:11:59.000000 mitransient-1.0.1/mitransient.egg-info/SOURCES.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)        1 2024-04-08 16:11:59.000000 mitransient-1.0.1/mitransient.egg-info/dependency_links.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)       15 2024-04-08 16:11:59.000000 mitransient-1.0.1/mitransient.egg-info/requires.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)       12 2024-04-08 16:11:59.000000 mitransient-1.0.1/mitransient.egg-info/top_level.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)       38 2024-04-08 16:11:59.404162 mitransient-1.0.1/setup.cfg
--rw-r--r--   0 droyo     (1000) droyo     (1000)      889 2024-04-08 16:11:02.000000 mitransient-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.063997 mitransient-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-18 12:20:14.063997 mitransient-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-04-18 12:20:10.000000 mitransient-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.055997 mitransient-1.0.2/mitransient/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.059997 mitransient-1.0.2/mitransient/films/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/films/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/films/transient_hdr_film.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.063997 mitransient-1.0.2/mitransient/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/integrators/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/integrators/transient_prb_volpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27872 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/integrators/transientnlospath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/integrators/transientpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/nlos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.063997 mitransient-1.0.2/mitransient/render/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/render/transient_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.063997 mitransient-1.0.2/mitransient/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/sensors/nloscapturemeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/sensors/nlossensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-18 12:20:10.000000 mitransient-1.0.2/mitransient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:20:14.063997 mitransient-1.0.2/mitransient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-18 12:20:14.000000 mitransient-1.0.2/mitransient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 12:20:14.000000 mitransient-1.0.2/mitransient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:20:14.000000 mitransient-1.0.2/mitransient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:20:14.000000 mitransient-1.0.2/mitransient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 12:20:14.000000 mitransient-1.0.2/mitransient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:20:14.063997 mitransient-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-18 12:20:10.000000 mitransient-1.0.2/setup.py
```

### Comparing `mitransient-1.0.1/PKG-INFO` & `mitransient-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: mitransient
-Version: 1.0.1
-Summary: Transient rendering extensions for Mitsuba 3
-Home-page: https://github.com/diegoroyo/mitsuba3-transient-nlos
-Author: Diego Royo, Miguel Crespo, Jorge García
-Author-email: droyo@unizar.es
-License: BSD
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 <div align="center">
 <img align="center" src="https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/logo_plain.png" width="90" height="90"/>
 </div>
 
 <!-- PROJECT LOGO -->
 <p align="center">
   <h1 align="center">Transient Mitsuba 3</h1>
@@ -20,94 +9,115 @@
   <p align="center">
     <a href="https://mcrespo.me"><strong>Miguel Crespo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://diego.contact"><strong>Diego Royo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://jgarciapueyo.github.io/"><strong>Jorge García</strong></a>
   </p>
-
-  <!-- <p align="center">
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Docs-passing-green?style=flat-square' alt='Project Page'>
-    </a>
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Project-Page-blue?style=flat-square' alt='Project Page'>
-    </a>
-  </p> -->
 </p>
 
 <br />
 
 <div align="center">
-  <img src=".images/cornell-box.png" width="200" height="200"/>
-  <img src=".images/cornell-box.gif" width="200" height="200"/>
-  <img src=".images/nlos-Z.png" width="200" height="200"/>
-  <img src=".images/nlos-Z.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif" width="200" height="200"/>
 </div>
 
 <br />
 
-# Introduction
+# Overview
 
-This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-line-of-sight (NLOS) data capture simulations.
+This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, with amazing support for non-line-of-sight (NLOS) data capture simulations.
 
-## Quick start:
+### Main features
+* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
+* **Easy interface** to convert your algorithms for the transient domain.
+* **Temporal domain** filtering.
+* **Python-only** library for doing transient rendering in both CPU and GPU.
+* **Several integrators have already been implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
 
-* [Installation](#installation)
-* [Usage](#usage) / [Documentation and examples](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples)
-* [License and citation](#license)
+<br>
 
+> **ℹ️ Check out our examples about how to use our library!** <br>
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples), [Line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-nlos/mitsuba3-transient-nlos.ipynb)
 
-## What is transient rendering?
+<br>
 
-Conventional rendering is referred as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumtion allowing to simulate light in motion (see the teaser image for a visual example).
+# License and citation
 
-For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives to the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
 
-*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+If you use our code in your project, please consider citing us using the following:
 
-# Main features
+```bibtex
+@misc{mitsuba3transient,
+	title        = {Transient Mitsuba 3},
+	author       = {Royo, Diego and Crespo, Miguel and Garcia, Jorge},
+	year         = 2023,
+	journal      = {GitHub repository},
+	publisher    = {GitHub},
+	howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
+}
+```
 
-* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
-* **Easy interface** to convert your algorithms for the transient domain.
-* **Temporal domain** filtering.
-* **Python only** library for doing transient rendering in both CPU and GPU.
-* **Several integrators already implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
+Additionally, the NLOS features were re-implemented from our publication [Non-line-of-sight transient rendering](https://doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use them:
 
-### Roadmap
+```bibtex
+@article{royo2022non,
+	title        = {Non-line-of-sight transient rendering},
+	author       = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo},
+	year         = 2022,
+	journal      = {Computers & Graphics},
+	doi          = {https://doi.org/10.1016/j.cag.2022.07.003},
+	issn         = {0097-8493},
+	url          = {https://www.sciencedirect.com/science/article/pii/S0097849322001200}
+}
+```
+
+# What is transient rendering?
+
+Conventional rendering is referred to as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumption allowing us to simulate light in motion (see the teaser image for a visual example).
+
+For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives at the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+
+*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+
+# Roadmap
 
 **Last update: Apr. 2024*
 
 - [ ] Importance sampling of the temporal domain
 - [ ] Differentiable transient rendering
 - [ ] Fluorescence BRDF
 - [X] Non-line-of-sight support (NLOS)
   - [X] `max_depth`
   - [X] `filter_depth`
   - [X] `discard_direct_paths`
   - [ ] `auto_detect_bins`
   - [ ] Faster implementation of exhaustive scanning
 
-# Requirements
-
-- `Python >= 3.8`
-- `Mitsuba3 >= 3.5.0`
-- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
-- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
-
 
 # Installation
 
 We provide the package via PyPI. To install `mitsuba3-transient-nlos` you need to run:
 
 ```bash
 pip install mitransient
 ```
 
-If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then we recommend that you compile Mitsuba 3 youself, enabling the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html).
+If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant which only propagates one wavelength), then we recommend that you compile Mitsuba 3 yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html) and enable the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`.
+
+## Requirements
+
+- `Python >= 3.8`
+- `Mitsuba3 >= 3.5.0`
+- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
+- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
 
 ## Old installation instructions (incl. Mitsuba 3 fork)
 
 <details>
 <summary>See details</summary>
 _NOTE: These instructions have been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully) without many problems_
 
@@ -135,25 +145,25 @@
       cmake \
           -GNinja \
           -DCMAKE_CXX_COMPILER=<path-to-c++-compiler> \
           -DCMAKE_C_COMPILER=<path-to-c-compiler> \
           -DPython_EXECUTABLE=<path-to-python-executable> \
           ..
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
+
     * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with ninja
       ```bash
       cmake <same arguments as before> ..
       ninja  # This will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     ```bash
     cd ../../..  # go back to initial mitsuba3-transient-nlos folder
     scripts/local_install.sh
     ```
 
 ### Windows users:
@@ -164,26 +174,26 @@
     ```
     * A recent version of Visual Studio 2022 is required. Cmake need to be installed manually
     * Check that the version of your Python is the correct one when you execute `python`
       ```powershell
       # Specifically ask for the 64 bit version of Visual Studio to be safe
       cmake -G "Visual Studio 17 2022" -A x64 -B build
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
-    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio. 
+
+    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio.
       ```powershell
       cmake <same arguments as before>
       # You can build from terminal with this, if you don't like opening Visual Studio
       cmake --build build --config Release  # this will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     * Step 2.1: You will need to edit your environment variables in Windows manually
       ```
       MITSUBA_DIR = <path-to-the-cloned-repository</mitsuba3-transient-nlos/ext/mitsuba3/build/Release
       Path = %Path%;%MITSUBA_DIR%
       PYTHON_PATH = %MITSUBA_DIR%/python
       ```
@@ -193,76 +203,44 @@
       python -m pip install .
       ```
 
 </details>
 
 ## After installation
 
-At this point you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
-
-If it works, you're all set!
+At this point, you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
 
 For NLOS data capture simulations, see https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with an easier shell interface instead of directly from Python.
 
 ### If you use your own Mitsuba 3
 
-If you have opted for using a custom (non-default installation through `pip`) of Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
+If you have opted for using a custom (non-default installation through `pip`) Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
 
-* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
+* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
 * Another solution following the previous one is to directly set yourself the `PYTHONPATH` environment variable as you wish.
-* Another solution for having a custom version globally available is by using `pip install .--editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly for use. Please follow these instructions:
+* Another solution for having a custom version globally available is by using `pip install . --editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly to use. Please follow these instructions:
   * Go to `<mitsuba-path>/mitsuba3/build/python/drjit` and execute `pip install . --editable`.
   * Go to `<mitsuba-path>/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`.
-* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify on-site the PYTHON PATH for that specific notebook:
+* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify the notebook's `PYTHONPATH`:
 ```python
 import sys
 sys.path.insert(0, '<mitsuba-path>/mitsuba3/build/python')
 import mitsuba as mi
 ```
 
 # Usage
 
-Check out the `examples` folder for practical usage.
+> **ℹ️ Check out the `examples` folder for practical usage!** <br>
 
 As of November 2023, `mitsuba3-transient-nlos` implements the following plugins which can be used in scene XML files. To view a description of their parameters, click on the name of your desired plugin.
 * `film`:
   * [`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin.
 * `integrators`:
   * [`transient_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient path tracing for line-of-sight scenes. If you want to do NLOS simulations, use `transientnlospath` instead.
   * [`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/nlos-render)).
   * [`transient_prbvolpath`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transient_prb_volpath.py): Path Replay Backpropagation for volumetric path tracing. Implemented by Miguel Crespo, untested.
 * `sensor`:
   * [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of the scene's geometries, and measures uniformly-spaced points on such geometry (e.g. relay wall).
 
 ## Testing
 
-Our test suite can be ran using `pytest` on the root folder of the repo.
-
-# License and citation
-
-This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
-
-If you are using our code for transient NLOS simulations, we would be grateful if you cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003):
-
-```bibtex
-@article{royo2022non,
-    title = {Non-line-of-sight transient rendering},
-    journal = {Computers & Graphics},
-    year = {2022},
-    issn = {0097-8493},
-    doi = {https://doi.org/10.1016/j.cag.2022.07.003},
-    url = {https://www.sciencedirect.com/science/article/pii/S0097849322001200},
-    author = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo}
-```
-
-Otherwise you can cite this repository as:
-
-```bibtex
-@misc{mitsuba3transient,
-  author = {Royo, Diego and Garcia, Jorge and Crespo, Miguel},
-  title = {Mitsuba 3 Transient},
-  year = {2023},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
-}
-```
+Our test suite can be run using `pytest` on the root folder of the repo.
```

#### html2text {}

```diff
@@ -1,81 +1,101 @@
-Metadata-Version: 2.1 Name: mitransient Version: 1.0.1 Summary: Transient
-rendering extensions for Mitsuba 3 Home-page: https://github.com/diegoroyo/
-mitsuba3-transient-nlos Author: Diego Royo, Miguel Crespo, Jorge GarcÃ­a
-Author-email: droyo@unizar.es License: BSD Requires-Python: >=3.8 Description-
-Content-Type: text/markdown
      [https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/
                                 logo_plain.png]
                        ************ TTrraannssiieenntt MMiittssuubbaa 33 ************
                _MM_ii_gg_uu_ee_ll_ _CC_rr_ee_ss_pp_oo      _DD_ii_ee_gg_oo_ _RR_oo_yy_oo      _JJ_oo_rr_gg_ee_ _GG_aa_rr_cc_?Ã_?­_aa
 
-[.images/cornell-box.png][.images/cornell-box.gif][.images/nlos-Z.png][.images/
-                                  nlos-Z.gif]
+   [https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/
+  cornell-box.png][https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/
+    master/.images/cornell-box.gif][https://github.com/diegoroyo/mitsuba3-
+  transient-nlos/raw/master/.images/nlos-Z.png][https://github.com/diegoroyo/
+            mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif]
 
-# Introduction This library adds support to [Mitsuba 3](https://github.com/
-mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-
-line-of-sight (NLOS) data capture simulations. ## Quick start: * [Installation]
-(#installation) * [Usage](#usage) / [Documentation and examples](https://
-github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples) * [License and
-citation](#license) ## What is transient rendering? Conventional rendering is
-referred as steady state, where the light propagation speed is assumed to be
-infinite. In contrast, transient rendering breaks this assumtion allowing to
-simulate light in motion (see the teaser image for a visual example). For
-example, path tracing algorithms integrate over multiple paths that connect a
-light source with the camera. For a known path, transient path tracing uses the
-*very complex* formula of `time = distance / speed` (see [[Two New Sciences by
-Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the
-`time` when each photon arrives to the camera from the path's `distance` and
-light's `speed`. This adds a new `time` dimension to the captured images (i.e.
-it's a video now). The simulations now take new parameters as input: when to
-start recording the video, how long is each time step (framerate), and how many
+# Overview This library adds support to [Mitsuba 3](https://github.com/mitsuba-
+renderer/mitsuba3) for doing transient simulations, with amazing support for
+non-line-of-sight (NLOS) data capture simulations. ### Main features * **Cross-
+platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64,
+x86_64), and Windows (x86_64). * **Easy interface** to convert your algorithms
+for the transient domain. * **Temporal domain** filtering. * **Python-only**
+library for doing transient rendering in both CPU and GPU. * **Several
+integrators have already been implemented** including path tracing (also
+adapted for NLOS scenes) and volumetric path-tracing.
+> **â¹ï¸ Check out our examples about how to use our library!**
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-
+nlos/tree/main/examples), [Line-of-sight transient rendering](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/
+render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https:/
+/github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-
+nlos/mitsuba3-transient-nlos.ipynb)
+# License and citation This project was created by [Miguel Crespo](https://
+mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge
+GarcÃ­a](https://jgarciapueyo.github.io/). If you use our code in your project,
+please consider citing us using the following: ```bibtex @misc
+{mitsuba3transient, title = {Transient Mitsuba 3}, author = {Royo, Diego and
+Crespo, Miguel and Garcia, Jorge}, year = 2023, journal = {GitHub repository},
+publisher = {GitHub}, howpublished = {\url{https://github.com/diegoroyo/
+mitsuba3-transient-nlos}} } ``` Additionally, the NLOS features were re-
+implemented from our publication [Non-line-of-sight transient rendering](https:
+//doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use
+them: ```bibtex @article{royo2022non, title = {Non-line-of-sight transient
+rendering}, author = {Diego Royo and Jorge GarcÃ­a and Adolfo MuÃ±oz and Adrian
+Jarabo}, year = 2022, journal = {Computers & Graphics}, doi = {https://doi.org/
+10.1016/j.cag.2022.07.003}, issn = {0097-8493}, url = {https://
+www.sciencedirect.com/science/article/pii/S0097849322001200} } ``` # What is
+transient rendering? Conventional rendering is referred to as steady state,
+where the light propagation speed is assumed to be infinite. In contrast,
+transient rendering breaks this assumption allowing us to simulate light in
+motion (see the teaser image for a visual example). For example, path tracing
+algorithms integrate over multiple paths that connect a light source with the
+camera. For a known path, transient path tracing uses the *very complex*
+formula of `time = distance / speed` (see [[Two New Sciences by Galileo]]
+(https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when
+each photon arrives at the camera from the path's `distance` and light's
+`speed`. This adds a new `time` dimension to the captured images (i.e. it's a
+video now). The simulations now take new parameters as input: when to start
+recording the video, how long is each time step (framerate), and how many
 frames to record. *Note: note that the `time` values we need to compute are
 very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter),
 `time` is usually measured in optical path distance. See [Wikipedia](https://
 en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl =
-distance * refractive_index`* # Main features * **Cross-platform:** Mitsuba 3
-has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows
-(x86_64). * **Easy interface** to convert your algorithms for the transient
-domain. * **Temporal domain** filtering. * **Python only** library for doing
-transient rendering in both CPU and GPU. * **Several integrators already
-implemented** including path tracing (also adapted for NLOS scenes) and
-volumetric path-tracing. ### Roadmap **Last update: Apr. 2024* - [ ] Importance
-sampling of the temporal domain - [ ] Differentiable transient rendering - [ ]
-Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X] `max_depth` -
-[X] `filter_depth` - [X] `discard_direct_paths` - [ ] `auto_detect_bins` - [ ]
-Faster implementation of exhaustive scanning # Requirements - `Python >= 3.8` -
-`Mitsuba3 >= 3.5.0` - (optional) For computation on the GPU: `Nvidia driver >=
-495.89` - (optional) For vectorized / parallel computation on the CPU: `LLVM >=
-11.1` # Installation We provide the package via PyPI. To install `mitsuba3-
-transient-nlos` you need to run: ```bash pip install mitransient ``` If you
-have installed Mitsuba 3 via `pip` you will only have access to the
-`llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants
-(e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then
-we recommend that you compile Mitsuba 3 youself, enabling the following
-variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono",
-"cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb",
-"cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/
-src/developer_guide/compiling.html). ## Old installation instructions (incl.
-Mitsuba 3 fork) See details _NOTE: These instructions have been tested on Linux
-and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully)
-without many problems_ After cloning the repo, navigate to the root folder and
-execute the following commands to build the custom version of Mitsuba 3 * Step
-0: Clone the repo (including the mitsuba3 custom fork submodule) ```bash git
-clone git@github.com:diegoroyo/mitsuba3-transient-nlos.git mitsuba3-transient-
-nlos cd mitsuba3-transient-nlos git submodule update --init --recursive ``` ##
-Now the steps are different for Linux and Windows users ### Linux users: * Step
-1: Compile mitsuba3 (ext/mitsuba3) from source * This is for Linux. for other
-OSes, check: https://mitsuba.readthedocs.io/en/latest/src/developer_guide/
-compiling.html ```bash cd ext/mitsuba3 mkdir -p build && cd build ``` * You
-might want to set the C++/C compiler (probably you want this e.g. if `cmake`
-complains about your version of g++). Always set `C_COMPILER` version to the
-same version as `CXX_COMPILER` (e.g. if you use `g++-12`, then also set `gcc-
-12`) * If you have multiple Python versions installed, also set
-Python_EXECUTABLE to ensure that the program is compiled for your specific
-version of Python ```bash cmake \ -GNinja \ -DCMAKE_CXX_COMPILER=
+distance * refractive_index`* # Roadmap **Last update: Apr. 2024* - [ ]
+Importance sampling of the temporal domain - [ ] Differentiable transient
+rendering - [ ] Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X]
+`max_depth` - [X] `filter_depth` - [X] `discard_direct_paths` - [ ]
+`auto_detect_bins` - [ ] Faster implementation of exhaustive scanning #
+Installation We provide the package via PyPI. To install `mitsuba3-transient-
+nlos` you need to run: ```bash pip install mitransient ``` If you have
+installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb`
+and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS
+simulations can greatly benefit from the `llvm_mono` variant which only
+propagates one wavelength), then we recommend that you compile Mitsuba 3
+yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/
+src/developer_guide/compiling.html) and enable the following variants: `
+["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono",
+"scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. ##
+Requirements - `Python >= 3.8` - `Mitsuba3 >= 3.5.0` - (optional) For
+computation on the GPU: `Nvidia driver >= 495.89` - (optional) For vectorized /
+parallel computation on the CPU: `LLVM >= 11.1` ## Old installation
+instructions (incl. Mitsuba 3 fork) See details _NOTE: These instructions have
+been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS
+probably (hopefully) without many problems_ After cloning the repo, navigate to
+the root folder and execute the following commands to build the custom version
+of Mitsuba 3 * Step 0: Clone the repo (including the mitsuba3 custom fork
+submodule) ```bash git clone git@github.com:diegoroyo/mitsuba3-transient-
+nlos.git mitsuba3-transient-nlos cd mitsuba3-transient-nlos git submodule
+update --init --recursive ``` ## Now the steps are different for Linux and
+Windows users ### Linux users: * Step 1: Compile mitsuba3 (ext/mitsuba3) from
+source * This is for Linux. for other OSes, check: https://
+mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html ```bash cd
+ext/mitsuba3 mkdir -p build && cd build ``` * You might want to set the C++/
+C compiler (probably you want this e.g. if `cmake` complains about your version
+of g++). Always set `C_COMPILER` version to the same version as `CXX_COMPILER`
+(e.g. if you use `g++-12`, then also set `gcc-12`) * If you have multiple
+Python versions installed, also set Python_EXECUTABLE to ensure that the
+program is compiled for your specific version of Python ```bash cmake \ -GNinja
+\ -DCMAKE_CXX_COMPILER=
 +-compiler> \ -DCMAKE_C_COMPILER= \ -DPython_EXECUTABLE= \ .. ``` * Step 1.1:
 You should see a message that a file was created on "build/mitsuba.conf". Open
 the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/
 en/latest/src/key_topics/variants.html * Recommended variants: `"scalar_mono",
 "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb",
 "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`. * IMPORTANT: At least
 one *_ad_* variant needs to be specified. * Step 1.2: Re-run the cmake command
@@ -100,69 +120,55 @@
 --config Release # this will take some time ``` * Step 2: Install `mitsuba3-
 transient-nlos` (a.k.a. `mitransient` Python library) * Step 2.1: You will need
 to edit your environment variables in Windows manually ``` MITSUBA_DIR =
 /mitsuba3-transient-nlos/ext/mitsuba3/build/Release Path = %Path%;%MITSUBA_DIR%
 PYTHON_PATH = %MITSUBA_DIR%/python ``` * Step 2.2: Install `mitsuba3-transient-
 nlos` (a.k.a. `mitransient` Python library) ```powershell cd ../../ # go back
 to initial mitsuba3-transient-nlos folder python -m pip install . ``` ## After
-installation At this point you should be able to `import mitsuba` and `import
+installation At this point, you should be able to `import mitsuba` and `import
 mitransient` in your Python code (careful about setting the correct `PATH`
 environment variable if you have compiled Mitsuba 3 yourself, see the section
-below). If it works, you're all set! For NLOS data capture simulations, see
-https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create
-and simulate NLOS scenes with an easier shell interface instead of directly
-from Python. ### If you use your own Mitsuba 3 If you have opted for using a
-custom (non-default installation through `pip`) of Mitsuba 3, you have several
-options for it. The idea here is to be able to control which version of Mitsuba
-will be loaded on demand. * One solution is to directly execute `setpath.sh`
-provided after the compilation of the Mitsuba 3 repo [(More info)](https://
-mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This
-shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to
-load first this version of Mitsuba. * Another solution following the previous
-one is to directly set yourself the `PYTHONPATH` environment variable as you
-wish. * Another solution for having a custom version globally available is by
-using `pip install .--editable`. This will create a symlink copy of the package
-files inside the corresponding `site-packages` folder and will be listed as a
-package installed of `pip` and will be available as other packages installed.
-If you recompile them, you will still have the newest version directly for use.
-Please follow these instructions: * Go to `/mitsuba3/build/python/drjit` and
-execute `pip install . --editable`. * Go to `/mitsuba3/build/python/mitsuba`
-and execute `pip install . --editable`. * If you are a user of Jupyter
-Notebooks, the easiest solution will be to add the following snippet of code to
-modify on-site the PYTHON PATH for that specific notebook: ```python import sys
-sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi ``` # Usage
-Check out the `examples` folder for practical usage. As of November 2023,
-`mitsuba3-transient-nlos` implements the following plugins which can be used in
-scene XML files. To view a description of their parameters, click on the name
-of your desired plugin. * `film`: * [`transient_hdr_film`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/
-transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin. *
-`integrators`: * [`transient_path`](https://github.com/diegoroyo/mitsuba3-
-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient
-path tracing for line-of-sight scenes. If you want to do NLOS simulations, use
-`transientnlospath` instead. * [`transient_nlos_path`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
-transientnlospath.py): Transient path tracing with specific sampling routines
-for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-
-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/
-nlos-render)). * [`transient_prbvolpath`](https://github.com/diegoroyo/
-mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+below). For NLOS data capture simulations, see https://github.com/diegoroyo/
+tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with
+an easier shell interface instead of directly from Python. ### If you use your
+own Mitsuba 3 If you have opted for using a custom (non-default installation
+through `pip`) Mitsuba 3, you have several options for it. The idea here is to
+be able to control which version of Mitsuba will be loaded on demand. * One
+solution is to directly execute `setpath.sh` provided after the compilation of
+the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/
+developer_guide/compiling.html). This shell script will modify the `PATH` and
+`PYTHONPATH` variables to load first this version of Mitsuba. * Another
+solution following the previous one is to directly set yourself the
+`PYTHONPATH` environment variable as you wish. * Another solution for having a
+custom version globally available is by using `pip install . --editable`. This
+will create a symlink copy of the package files inside the corresponding `site-
+packages` folder and will be listed as a package installed of `pip` and will be
+available as other packages installed. If you recompile them, you will still
+have the newest version directly to use. Please follow these instructions: * Go
+to `/mitsuba3/build/python/drjit` and execute `pip install . --editable`. * Go
+to `/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`. *
+If you are a user of Jupyter Notebooks, the easiest solution will be to add the
+following snippet of code to modify the notebook's `PYTHONPATH`: ```python
+import sys sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi
+``` # Usage > **â¹ï¸ Check out the `examples` folder for practical usage!**
+As of November 2023, `mitsuba3-transient-nlos` implements the following plugins
+which can be used in scene XML files. To view a description of their
+parameters, click on the name of your desired plugin. * `film`: *
+[`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of
+Mitsuba 3's `hdrfilm` plugin. * `integrators`: * [`transient_path`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+transientpath.py): Transient path tracing for line-of-sight scenes. If you want
+to do NLOS simulations, use `transientnlospath` instead. *
+[`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing
+with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden
+geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https:
+//diego.contact/publications/nlos-render)). * [`transient_prbvolpath`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
 transient_prb_volpath.py): Path Replay Backpropagation for volumetric path
 tracing. Implemented by Miguel Crespo, untested. * `sensor`: *
 [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
 blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of
 the scene's geometries, and measures uniformly-spaced points on such geometry
-(e.g. relay wall). ## Testing Our test suite can be ran using `pytest` on the
-root folder of the repo. # License and citation This project was created by
-[Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://
-diego.contact) and [Jorge GarcÃ­a](https://jgarciapueyo.github.io/). If you are
-using our code for transient NLOS simulations, we would be grateful if you
-cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003): ```bibtex
-@article{royo2022non, title = {Non-line-of-sight transient rendering}, journal
-= {Computers & Graphics}, year = {2022}, issn = {0097-8493}, doi = {https://
-doi.org/10.1016/j.cag.2022.07.003}, url = {https://www.sciencedirect.com/
-science/article/pii/S0097849322001200}, author = {Diego Royo and Jorge GarcÃ­a
-and Adolfo MuÃ±oz and Adrian Jarabo} ``` Otherwise you can cite this repository
-as: ```bibtex @misc{mitsuba3transient, author = {Royo, Diego and Garcia, Jorge
-and Crespo, Miguel}, title = {Mitsuba 3 Transient}, year = {2023}, publisher =
-{GitHub}, journal = {GitHub repository}, howpublished = {\url{https://
-github.com/diegoroyo/mitsuba3-transient-nlos}} } ```
+(e.g. relay wall). ## Testing Our test suite can be run using `pytest` on the
+root folder of the repo.
```

### Comparing `mitransient-1.0.1/README.md` & `mitransient-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: mitransient
+Version: 1.0.2
+Summary: Transient rendering extensions for Mitsuba 3
+Home-page: https://github.com/diegoroyo/mitsuba3-transient-nlos
+Author: Miguel Crespo, Diego Royo, Jorge García
+Author-email: droyo@unizar.es
+License: BSD
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: mitsuba>=3.5.0
+
 <div align="center">
 <img align="center" src="https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/logo_plain.png" width="90" height="90"/>
 </div>
 
 <!-- PROJECT LOGO -->
 <p align="center">
   <h1 align="center">Transient Mitsuba 3</h1>
@@ -9,94 +21,115 @@
   <p align="center">
     <a href="https://mcrespo.me"><strong>Miguel Crespo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://diego.contact"><strong>Diego Royo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://jgarciapueyo.github.io/"><strong>Jorge García</strong></a>
   </p>
-
-  <!-- <p align="center">
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Docs-passing-green?style=flat-square' alt='Project Page'>
-    </a>
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Project-Page-blue?style=flat-square' alt='Project Page'>
-    </a>
-  </p> -->
 </p>
 
 <br />
 
 <div align="center">
-  <img src=".images/cornell-box.png" width="200" height="200"/>
-  <img src=".images/cornell-box.gif" width="200" height="200"/>
-  <img src=".images/nlos-Z.png" width="200" height="200"/>
-  <img src=".images/nlos-Z.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif" width="200" height="200"/>
 </div>
 
 <br />
 
-# Introduction
+# Overview
 
-This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-line-of-sight (NLOS) data capture simulations.
+This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, with amazing support for non-line-of-sight (NLOS) data capture simulations.
 
-## Quick start:
+### Main features
+* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
+* **Easy interface** to convert your algorithms for the transient domain.
+* **Temporal domain** filtering.
+* **Python-only** library for doing transient rendering in both CPU and GPU.
+* **Several integrators have already been implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
 
-* [Installation](#installation)
-* [Usage](#usage) / [Documentation and examples](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples)
-* [License and citation](#license)
+<br>
 
+> **ℹ️ Check out our examples about how to use our library!** <br>
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples), [Line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-nlos/mitsuba3-transient-nlos.ipynb)
 
-## What is transient rendering?
+<br>
 
-Conventional rendering is referred as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumtion allowing to simulate light in motion (see the teaser image for a visual example).
+# License and citation
 
-For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives to the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
 
-*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+If you use our code in your project, please consider citing us using the following:
 
-# Main features
+```bibtex
+@misc{mitsuba3transient,
+	title        = {Transient Mitsuba 3},
+	author       = {Royo, Diego and Crespo, Miguel and Garcia, Jorge},
+	year         = 2023,
+	journal      = {GitHub repository},
+	publisher    = {GitHub},
+	howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
+}
+```
 
-* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
-* **Easy interface** to convert your algorithms for the transient domain.
-* **Temporal domain** filtering.
-* **Python only** library for doing transient rendering in both CPU and GPU.
-* **Several integrators already implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
+Additionally, the NLOS features were re-implemented from our publication [Non-line-of-sight transient rendering](https://doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use them:
 
-### Roadmap
+```bibtex
+@article{royo2022non,
+	title        = {Non-line-of-sight transient rendering},
+	author       = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo},
+	year         = 2022,
+	journal      = {Computers & Graphics},
+	doi          = {https://doi.org/10.1016/j.cag.2022.07.003},
+	issn         = {0097-8493},
+	url          = {https://www.sciencedirect.com/science/article/pii/S0097849322001200}
+}
+```
+
+# What is transient rendering?
+
+Conventional rendering is referred to as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumption allowing us to simulate light in motion (see the teaser image for a visual example).
+
+For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives at the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+
+*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+
+# Roadmap
 
 **Last update: Apr. 2024*
 
 - [ ] Importance sampling of the temporal domain
 - [ ] Differentiable transient rendering
 - [ ] Fluorescence BRDF
 - [X] Non-line-of-sight support (NLOS)
   - [X] `max_depth`
   - [X] `filter_depth`
   - [X] `discard_direct_paths`
   - [ ] `auto_detect_bins`
   - [ ] Faster implementation of exhaustive scanning
 
-# Requirements
-
-- `Python >= 3.8`
-- `Mitsuba3 >= 3.5.0`
-- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
-- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
-
 
 # Installation
 
 We provide the package via PyPI. To install `mitsuba3-transient-nlos` you need to run:
 
 ```bash
 pip install mitransient
 ```
 
-If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then we recommend that you compile Mitsuba 3 youself, enabling the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html).
+If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant which only propagates one wavelength), then we recommend that you compile Mitsuba 3 yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html) and enable the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`.
+
+## Requirements
+
+- `Python >= 3.8`
+- `Mitsuba3 >= 3.5.0`
+- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
+- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
 
 ## Old installation instructions (incl. Mitsuba 3 fork)
 
 <details>
 <summary>See details</summary>
 _NOTE: These instructions have been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully) without many problems_
 
@@ -124,25 +157,25 @@
       cmake \
           -GNinja \
           -DCMAKE_CXX_COMPILER=<path-to-c++-compiler> \
           -DCMAKE_C_COMPILER=<path-to-c-compiler> \
           -DPython_EXECUTABLE=<path-to-python-executable> \
           ..
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
+
     * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with ninja
       ```bash
       cmake <same arguments as before> ..
       ninja  # This will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     ```bash
     cd ../../..  # go back to initial mitsuba3-transient-nlos folder
     scripts/local_install.sh
     ```
 
 ### Windows users:
@@ -153,26 +186,26 @@
     ```
     * A recent version of Visual Studio 2022 is required. Cmake need to be installed manually
     * Check that the version of your Python is the correct one when you execute `python`
       ```powershell
       # Specifically ask for the 64 bit version of Visual Studio to be safe
       cmake -G "Visual Studio 17 2022" -A x64 -B build
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
-    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio. 
+
+    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio.
       ```powershell
       cmake <same arguments as before>
       # You can build from terminal with this, if you don't like opening Visual Studio
       cmake --build build --config Release  # this will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     * Step 2.1: You will need to edit your environment variables in Windows manually
       ```
       MITSUBA_DIR = <path-to-the-cloned-repository</mitsuba3-transient-nlos/ext/mitsuba3/build/Release
       Path = %Path%;%MITSUBA_DIR%
       PYTHON_PATH = %MITSUBA_DIR%/python
       ```
@@ -182,76 +215,44 @@
       python -m pip install .
       ```
 
 </details>
 
 ## After installation
 
-At this point you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
-
-If it works, you're all set!
+At this point, you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
 
 For NLOS data capture simulations, see https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with an easier shell interface instead of directly from Python.
 
 ### If you use your own Mitsuba 3
 
-If you have opted for using a custom (non-default installation through `pip`) of Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
+If you have opted for using a custom (non-default installation through `pip`) Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
 
-* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
+* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
 * Another solution following the previous one is to directly set yourself the `PYTHONPATH` environment variable as you wish.
-* Another solution for having a custom version globally available is by using `pip install .--editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly for use. Please follow these instructions:
+* Another solution for having a custom version globally available is by using `pip install . --editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly to use. Please follow these instructions:
   * Go to `<mitsuba-path>/mitsuba3/build/python/drjit` and execute `pip install . --editable`.
   * Go to `<mitsuba-path>/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`.
-* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify on-site the PYTHON PATH for that specific notebook:
+* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify the notebook's `PYTHONPATH`:
 ```python
 import sys
 sys.path.insert(0, '<mitsuba-path>/mitsuba3/build/python')
 import mitsuba as mi
 ```
 
 # Usage
 
-Check out the `examples` folder for practical usage.
+> **ℹ️ Check out the `examples` folder for practical usage!** <br>
 
 As of November 2023, `mitsuba3-transient-nlos` implements the following plugins which can be used in scene XML files. To view a description of their parameters, click on the name of your desired plugin.
 * `film`:
   * [`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin.
 * `integrators`:
   * [`transient_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient path tracing for line-of-sight scenes. If you want to do NLOS simulations, use `transientnlospath` instead.
   * [`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/nlos-render)).
   * [`transient_prbvolpath`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transient_prb_volpath.py): Path Replay Backpropagation for volumetric path tracing. Implemented by Miguel Crespo, untested.
 * `sensor`:
   * [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of the scene's geometries, and measures uniformly-spaced points on such geometry (e.g. relay wall).
 
 ## Testing
 
-Our test suite can be ran using `pytest` on the root folder of the repo.
-
-# License and citation
-
-This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
-
-If you are using our code for transient NLOS simulations, we would be grateful if you cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003):
-
-```bibtex
-@article{royo2022non,
-    title = {Non-line-of-sight transient rendering},
-    journal = {Computers & Graphics},
-    year = {2022},
-    issn = {0097-8493},
-    doi = {https://doi.org/10.1016/j.cag.2022.07.003},
-    url = {https://www.sciencedirect.com/science/article/pii/S0097849322001200},
-    author = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo}
-```
-
-Otherwise you can cite this repository as:
-
-```bibtex
-@misc{mitsuba3transient,
-  author = {Royo, Diego and Garcia, Jorge and Crespo, Miguel},
-  title = {Mitsuba 3 Transient},
-  year = {2023},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
-}
-```
+Our test suite can be run using `pytest` on the root folder of the repo.
```

#### html2text {}

```diff
@@ -1,76 +1,106 @@
+Metadata-Version: 2.1 Name: mitransient Version: 1.0.2 Summary: Transient
+rendering extensions for Mitsuba 3 Home-page: https://github.com/diegoroyo/
+mitsuba3-transient-nlos Author: Miguel Crespo, Diego Royo, Jorge GarcÃ­a
+Author-email: droyo@unizar.es License: BSD Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Requires-Dist: mitsuba>=3.5.0
      [https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/
                                 logo_plain.png]
                        ************ TTrraannssiieenntt MMiittssuubbaa 33 ************
                _MM_ii_gg_uu_ee_ll_ _CC_rr_ee_ss_pp_oo      _DD_ii_ee_gg_oo_ _RR_oo_yy_oo      _JJ_oo_rr_gg_ee_ _GG_aa_rr_cc_?Ã_?­_aa
 
-[.images/cornell-box.png][.images/cornell-box.gif][.images/nlos-Z.png][.images/
-                                  nlos-Z.gif]
+   [https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/
+  cornell-box.png][https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/
+    master/.images/cornell-box.gif][https://github.com/diegoroyo/mitsuba3-
+  transient-nlos/raw/master/.images/nlos-Z.png][https://github.com/diegoroyo/
+            mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif]
 
-# Introduction This library adds support to [Mitsuba 3](https://github.com/
-mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-
-line-of-sight (NLOS) data capture simulations. ## Quick start: * [Installation]
-(#installation) * [Usage](#usage) / [Documentation and examples](https://
-github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples) * [License and
-citation](#license) ## What is transient rendering? Conventional rendering is
-referred as steady state, where the light propagation speed is assumed to be
-infinite. In contrast, transient rendering breaks this assumtion allowing to
-simulate light in motion (see the teaser image for a visual example). For
-example, path tracing algorithms integrate over multiple paths that connect a
-light source with the camera. For a known path, transient path tracing uses the
-*very complex* formula of `time = distance / speed` (see [[Two New Sciences by
-Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the
-`time` when each photon arrives to the camera from the path's `distance` and
-light's `speed`. This adds a new `time` dimension to the captured images (i.e.
-it's a video now). The simulations now take new parameters as input: when to
-start recording the video, how long is each time step (framerate), and how many
+# Overview This library adds support to [Mitsuba 3](https://github.com/mitsuba-
+renderer/mitsuba3) for doing transient simulations, with amazing support for
+non-line-of-sight (NLOS) data capture simulations. ### Main features * **Cross-
+platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64,
+x86_64), and Windows (x86_64). * **Easy interface** to convert your algorithms
+for the transient domain. * **Temporal domain** filtering. * **Python-only**
+library for doing transient rendering in both CPU and GPU. * **Several
+integrators have already been implemented** including path tracing (also
+adapted for NLOS scenes) and volumetric path-tracing.
+> **â¹ï¸ Check out our examples about how to use our library!**
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-
+nlos/tree/main/examples), [Line-of-sight transient rendering](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/
+render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https:/
+/github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-
+nlos/mitsuba3-transient-nlos.ipynb)
+# License and citation This project was created by [Miguel Crespo](https://
+mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge
+GarcÃ­a](https://jgarciapueyo.github.io/). If you use our code in your project,
+please consider citing us using the following: ```bibtex @misc
+{mitsuba3transient, title = {Transient Mitsuba 3}, author = {Royo, Diego and
+Crespo, Miguel and Garcia, Jorge}, year = 2023, journal = {GitHub repository},
+publisher = {GitHub}, howpublished = {\url{https://github.com/diegoroyo/
+mitsuba3-transient-nlos}} } ``` Additionally, the NLOS features were re-
+implemented from our publication [Non-line-of-sight transient rendering](https:
+//doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use
+them: ```bibtex @article{royo2022non, title = {Non-line-of-sight transient
+rendering}, author = {Diego Royo and Jorge GarcÃ­a and Adolfo MuÃ±oz and Adrian
+Jarabo}, year = 2022, journal = {Computers & Graphics}, doi = {https://doi.org/
+10.1016/j.cag.2022.07.003}, issn = {0097-8493}, url = {https://
+www.sciencedirect.com/science/article/pii/S0097849322001200} } ``` # What is
+transient rendering? Conventional rendering is referred to as steady state,
+where the light propagation speed is assumed to be infinite. In contrast,
+transient rendering breaks this assumption allowing us to simulate light in
+motion (see the teaser image for a visual example). For example, path tracing
+algorithms integrate over multiple paths that connect a light source with the
+camera. For a known path, transient path tracing uses the *very complex*
+formula of `time = distance / speed` (see [[Two New Sciences by Galileo]]
+(https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when
+each photon arrives at the camera from the path's `distance` and light's
+`speed`. This adds a new `time` dimension to the captured images (i.e. it's a
+video now). The simulations now take new parameters as input: when to start
+recording the video, how long is each time step (framerate), and how many
 frames to record. *Note: note that the `time` values we need to compute are
 very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter),
 `time` is usually measured in optical path distance. See [Wikipedia](https://
 en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl =
-distance * refractive_index`* # Main features * **Cross-platform:** Mitsuba 3
-has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows
-(x86_64). * **Easy interface** to convert your algorithms for the transient
-domain. * **Temporal domain** filtering. * **Python only** library for doing
-transient rendering in both CPU and GPU. * **Several integrators already
-implemented** including path tracing (also adapted for NLOS scenes) and
-volumetric path-tracing. ### Roadmap **Last update: Apr. 2024* - [ ] Importance
-sampling of the temporal domain - [ ] Differentiable transient rendering - [ ]
-Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X] `max_depth` -
-[X] `filter_depth` - [X] `discard_direct_paths` - [ ] `auto_detect_bins` - [ ]
-Faster implementation of exhaustive scanning # Requirements - `Python >= 3.8` -
-`Mitsuba3 >= 3.5.0` - (optional) For computation on the GPU: `Nvidia driver >=
-495.89` - (optional) For vectorized / parallel computation on the CPU: `LLVM >=
-11.1` # Installation We provide the package via PyPI. To install `mitsuba3-
-transient-nlos` you need to run: ```bash pip install mitransient ``` If you
-have installed Mitsuba 3 via `pip` you will only have access to the
-`llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants
-(e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then
-we recommend that you compile Mitsuba 3 youself, enabling the following
-variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono",
-"cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb",
-"cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/
-src/developer_guide/compiling.html). ## Old installation instructions (incl.
-Mitsuba 3 fork) See details _NOTE: These instructions have been tested on Linux
-and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully)
-without many problems_ After cloning the repo, navigate to the root folder and
-execute the following commands to build the custom version of Mitsuba 3 * Step
-0: Clone the repo (including the mitsuba3 custom fork submodule) ```bash git
-clone git@github.com:diegoroyo/mitsuba3-transient-nlos.git mitsuba3-transient-
-nlos cd mitsuba3-transient-nlos git submodule update --init --recursive ``` ##
-Now the steps are different for Linux and Windows users ### Linux users: * Step
-1: Compile mitsuba3 (ext/mitsuba3) from source * This is for Linux. for other
-OSes, check: https://mitsuba.readthedocs.io/en/latest/src/developer_guide/
-compiling.html ```bash cd ext/mitsuba3 mkdir -p build && cd build ``` * You
-might want to set the C++/C compiler (probably you want this e.g. if `cmake`
-complains about your version of g++). Always set `C_COMPILER` version to the
-same version as `CXX_COMPILER` (e.g. if you use `g++-12`, then also set `gcc-
-12`) * If you have multiple Python versions installed, also set
-Python_EXECUTABLE to ensure that the program is compiled for your specific
-version of Python ```bash cmake \ -GNinja \ -DCMAKE_CXX_COMPILER=
+distance * refractive_index`* # Roadmap **Last update: Apr. 2024* - [ ]
+Importance sampling of the temporal domain - [ ] Differentiable transient
+rendering - [ ] Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X]
+`max_depth` - [X] `filter_depth` - [X] `discard_direct_paths` - [ ]
+`auto_detect_bins` - [ ] Faster implementation of exhaustive scanning #
+Installation We provide the package via PyPI. To install `mitsuba3-transient-
+nlos` you need to run: ```bash pip install mitransient ``` If you have
+installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb`
+and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS
+simulations can greatly benefit from the `llvm_mono` variant which only
+propagates one wavelength), then we recommend that you compile Mitsuba 3
+yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/
+src/developer_guide/compiling.html) and enable the following variants: `
+["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono",
+"scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. ##
+Requirements - `Python >= 3.8` - `Mitsuba3 >= 3.5.0` - (optional) For
+computation on the GPU: `Nvidia driver >= 495.89` - (optional) For vectorized /
+parallel computation on the CPU: `LLVM >= 11.1` ## Old installation
+instructions (incl. Mitsuba 3 fork) See details _NOTE: These instructions have
+been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS
+probably (hopefully) without many problems_ After cloning the repo, navigate to
+the root folder and execute the following commands to build the custom version
+of Mitsuba 3 * Step 0: Clone the repo (including the mitsuba3 custom fork
+submodule) ```bash git clone git@github.com:diegoroyo/mitsuba3-transient-
+nlos.git mitsuba3-transient-nlos cd mitsuba3-transient-nlos git submodule
+update --init --recursive ``` ## Now the steps are different for Linux and
+Windows users ### Linux users: * Step 1: Compile mitsuba3 (ext/mitsuba3) from
+source * This is for Linux. for other OSes, check: https://
+mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html ```bash cd
+ext/mitsuba3 mkdir -p build && cd build ``` * You might want to set the C++/
+C compiler (probably you want this e.g. if `cmake` complains about your version
+of g++). Always set `C_COMPILER` version to the same version as `CXX_COMPILER`
+(e.g. if you use `g++-12`, then also set `gcc-12`) * If you have multiple
+Python versions installed, also set Python_EXECUTABLE to ensure that the
+program is compiled for your specific version of Python ```bash cmake \ -GNinja
+\ -DCMAKE_CXX_COMPILER=
 +-compiler> \ -DCMAKE_C_COMPILER= \ -DPython_EXECUTABLE= \ .. ``` * Step 1.1:
 You should see a message that a file was created on "build/mitsuba.conf". Open
 the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/
 en/latest/src/key_topics/variants.html * Recommended variants: `"scalar_mono",
 "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb",
 "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`. * IMPORTANT: At least
 one *_ad_* variant needs to be specified. * Step 1.2: Re-run the cmake command
@@ -95,69 +125,55 @@
 --config Release # this will take some time ``` * Step 2: Install `mitsuba3-
 transient-nlos` (a.k.a. `mitransient` Python library) * Step 2.1: You will need
 to edit your environment variables in Windows manually ``` MITSUBA_DIR =
 /mitsuba3-transient-nlos/ext/mitsuba3/build/Release Path = %Path%;%MITSUBA_DIR%
 PYTHON_PATH = %MITSUBA_DIR%/python ``` * Step 2.2: Install `mitsuba3-transient-
 nlos` (a.k.a. `mitransient` Python library) ```powershell cd ../../ # go back
 to initial mitsuba3-transient-nlos folder python -m pip install . ``` ## After
-installation At this point you should be able to `import mitsuba` and `import
+installation At this point, you should be able to `import mitsuba` and `import
 mitransient` in your Python code (careful about setting the correct `PATH`
 environment variable if you have compiled Mitsuba 3 yourself, see the section
-below). If it works, you're all set! For NLOS data capture simulations, see
-https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create
-and simulate NLOS scenes with an easier shell interface instead of directly
-from Python. ### If you use your own Mitsuba 3 If you have opted for using a
-custom (non-default installation through `pip`) of Mitsuba 3, you have several
-options for it. The idea here is to be able to control which version of Mitsuba
-will be loaded on demand. * One solution is to directly execute `setpath.sh`
-provided after the compilation of the Mitsuba 3 repo [(More info)](https://
-mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This
-shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to
-load first this version of Mitsuba. * Another solution following the previous
-one is to directly set yourself the `PYTHONPATH` environment variable as you
-wish. * Another solution for having a custom version globally available is by
-using `pip install .--editable`. This will create a symlink copy of the package
-files inside the corresponding `site-packages` folder and will be listed as a
-package installed of `pip` and will be available as other packages installed.
-If you recompile them, you will still have the newest version directly for use.
-Please follow these instructions: * Go to `/mitsuba3/build/python/drjit` and
-execute `pip install . --editable`. * Go to `/mitsuba3/build/python/mitsuba`
-and execute `pip install . --editable`. * If you are a user of Jupyter
-Notebooks, the easiest solution will be to add the following snippet of code to
-modify on-site the PYTHON PATH for that specific notebook: ```python import sys
-sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi ``` # Usage
-Check out the `examples` folder for practical usage. As of November 2023,
-`mitsuba3-transient-nlos` implements the following plugins which can be used in
-scene XML files. To view a description of their parameters, click on the name
-of your desired plugin. * `film`: * [`transient_hdr_film`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/
-transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin. *
-`integrators`: * [`transient_path`](https://github.com/diegoroyo/mitsuba3-
-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient
-path tracing for line-of-sight scenes. If you want to do NLOS simulations, use
-`transientnlospath` instead. * [`transient_nlos_path`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
-transientnlospath.py): Transient path tracing with specific sampling routines
-for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-
-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/
-nlos-render)). * [`transient_prbvolpath`](https://github.com/diegoroyo/
-mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+below). For NLOS data capture simulations, see https://github.com/diegoroyo/
+tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with
+an easier shell interface instead of directly from Python. ### If you use your
+own Mitsuba 3 If you have opted for using a custom (non-default installation
+through `pip`) Mitsuba 3, you have several options for it. The idea here is to
+be able to control which version of Mitsuba will be loaded on demand. * One
+solution is to directly execute `setpath.sh` provided after the compilation of
+the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/
+developer_guide/compiling.html). This shell script will modify the `PATH` and
+`PYTHONPATH` variables to load first this version of Mitsuba. * Another
+solution following the previous one is to directly set yourself the
+`PYTHONPATH` environment variable as you wish. * Another solution for having a
+custom version globally available is by using `pip install . --editable`. This
+will create a symlink copy of the package files inside the corresponding `site-
+packages` folder and will be listed as a package installed of `pip` and will be
+available as other packages installed. If you recompile them, you will still
+have the newest version directly to use. Please follow these instructions: * Go
+to `/mitsuba3/build/python/drjit` and execute `pip install . --editable`. * Go
+to `/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`. *
+If you are a user of Jupyter Notebooks, the easiest solution will be to add the
+following snippet of code to modify the notebook's `PYTHONPATH`: ```python
+import sys sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi
+``` # Usage > **â¹ï¸ Check out the `examples` folder for practical usage!**
+As of November 2023, `mitsuba3-transient-nlos` implements the following plugins
+which can be used in scene XML files. To view a description of their
+parameters, click on the name of your desired plugin. * `film`: *
+[`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of
+Mitsuba 3's `hdrfilm` plugin. * `integrators`: * [`transient_path`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+transientpath.py): Transient path tracing for line-of-sight scenes. If you want
+to do NLOS simulations, use `transientnlospath` instead. *
+[`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing
+with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden
+geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https:
+//diego.contact/publications/nlos-render)). * [`transient_prbvolpath`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
 transient_prb_volpath.py): Path Replay Backpropagation for volumetric path
 tracing. Implemented by Miguel Crespo, untested. * `sensor`: *
 [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
 blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of
 the scene's geometries, and measures uniformly-spaced points on such geometry
-(e.g. relay wall). ## Testing Our test suite can be ran using `pytest` on the
-root folder of the repo. # License and citation This project was created by
-[Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://
-diego.contact) and [Jorge GarcÃ­a](https://jgarciapueyo.github.io/). If you are
-using our code for transient NLOS simulations, we would be grateful if you
-cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003): ```bibtex
-@article{royo2022non, title = {Non-line-of-sight transient rendering}, journal
-= {Computers & Graphics}, year = {2022}, issn = {0097-8493}, doi = {https://
-doi.org/10.1016/j.cag.2022.07.003}, url = {https://www.sciencedirect.com/
-science/article/pii/S0097849322001200}, author = {Diego Royo and Jorge GarcÃ­a
-and Adolfo MuÃ±oz and Adrian Jarabo} ``` Otherwise you can cite this repository
-as: ```bibtex @misc{mitsuba3transient, author = {Royo, Diego and Garcia, Jorge
-and Crespo, Miguel}, title = {Mitsuba 3 Transient}, year = {2023}, publisher =
-{GitHub}, journal = {GitHub repository}, howpublished = {\url{https://
-github.com/diegoroyo/mitsuba3-transient-nlos}} } ```
+(e.g. relay wall). ## Testing Our test suite can be run using `pytest` on the
+root folder of the repo.
```

### Comparing `mitransient-1.0.1/mitransient/__init__.py` & `mitransient-1.0.2/mitransient/__init__.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/films/__init__.py` & `mitransient-1.0.2/mitransient/films/__init__.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/films/transient_hdr_film.py` & `mitransient-1.0.2/mitransient/films/transient_hdr_film.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/integrators/__init__.py` & `mitransient-1.0.2/mitransient/integrators/__init__.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/integrators/common.py` & `mitransient-1.0.2/mitransient/integrators/common.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/integrators/transient_prb_volpath.py` & `mitransient-1.0.2/mitransient/integrators/transient_prb_volpath.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/integrators/transientnlospath.py` & `mitransient-1.0.2/mitransient/integrators/transientnlospath.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/integrators/transientpath.py` & `mitransient-1.0.2/mitransient/integrators/transientpath.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/nlos.py` & `mitransient-1.0.2/mitransient/nlos.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/render/__init__.py` & `mitransient-1.0.2/mitransient/render/__init__.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/render/transient_block.py` & `mitransient-1.0.2/mitransient/render/transient_block.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/sensors/__init__.py` & `mitransient-1.0.2/mitransient/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/sensors/nloscapturemeter.py` & `mitransient-1.0.2/mitransient/sensors/nloscapturemeter.py`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/mitransient/utils.py` & `mitransient-1.0.2/mitransient/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,15 @@
         value = getattr(value, item)
     return value
 
 
 def get_module(class_):
     return get_class(class_.__module__)
 
-if mi.variant() is None:
-    # e.g. pip installation does not set mi.variant()
-    # does not matter as it does not use Array variants
-    pass
-elif mi.variant().startswith('scalar'):
+if mi.variant().startswith('scalar'):
     ArrayXf = dr.scalar.ArrayXf
     ArrayXu = dr.scalar.ArrayXu
     ArrayXi = dr.scalar.ArrayXi
     Array2f = dr.scalar.Array2f
     Array2u = dr.scalar.Array2u
     Array3f = dr.scalar.Array3f
 else:
@@ -108,16 +104,14 @@
 
     num_frames = data.shape[axis_video]
     for i in range(num_frames):
         mi.Bitmap(data[generate_index(axis_video, len(data.shape), i)]).write(
             f'{folder}/{i:03d}.exr')
 
 # Indent output of subobjects
-
-
 def indent(obj, amount=2):
     output = str(obj)
     result = ""
     lines = output.splitlines(keepends=True)
     if len(lines) == 1:
         result += lines[0]
     else:
```

### Comparing `mitransient-1.0.1/mitransient/version.py` & `mitransient-1.0.2/mitransient/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MiTransient version
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 # Mitsuba minimum compatible version
 __mi_version__ = '3.5.0'
 
 
 class Version:
     def __init__(self, string) -> None:
```

### Comparing `mitransient-1.0.1/mitransient.egg-info/PKG-INFO` & `mitransient-1.0.2/mitransient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mitransient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transient rendering extensions for Mitsuba 3
 Home-page: https://github.com/diegoroyo/mitsuba3-transient-nlos
-Author: Diego Royo, Miguel Crespo, Jorge García
+Author: Miguel Crespo, Diego Royo, Jorge García
 Author-email: droyo@unizar.es
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: mitsuba>=3.5.0
 
 <div align="center">
 <img align="center" src="https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/logo_plain.png" width="90" height="90"/>
 </div>
 
 <!-- PROJECT LOGO -->
 <p align="center">
@@ -20,94 +21,115 @@
   <p align="center">
     <a href="https://mcrespo.me"><strong>Miguel Crespo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://diego.contact"><strong>Diego Royo</strong></a>
     &nbsp;&nbsp;&nbsp;&nbsp;
     <a href="https://jgarciapueyo.github.io/"><strong>Jorge García</strong></a>
   </p>
-
-  <!-- <p align="center">
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Docs-passing-green?style=flat-square' alt='Project Page'>
-    </a>
-    <a href='' style='padding-left: 0.5rem;'>
-      <img src='https://img.shields.io/badge/Project-Page-blue?style=flat-square' alt='Project Page'>
-    </a>
-  </p> -->
 </p>
 
 <br />
 
 <div align="center">
-  <img src=".images/cornell-box.png" width="200" height="200"/>
-  <img src=".images/cornell-box.gif" width="200" height="200"/>
-  <img src=".images/nlos-Z.png" width="200" height="200"/>
-  <img src=".images/nlos-Z.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/cornell-box.gif" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.png" width="200" height="200"/>
+  <img src="https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif" width="200" height="200"/>
 </div>
 
 <br />
 
-# Introduction
+# Overview
 
-This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-line-of-sight (NLOS) data capture simulations.
+This library adds support to [Mitsuba 3](https://github.com/mitsuba-renderer/mitsuba3) for doing transient simulations, with amazing support for non-line-of-sight (NLOS) data capture simulations.
 
-## Quick start:
+### Main features
+* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
+* **Easy interface** to convert your algorithms for the transient domain.
+* **Temporal domain** filtering.
+* **Python-only** library for doing transient rendering in both CPU and GPU.
+* **Several integrators have already been implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
 
-* [Installation](#installation)
-* [Usage](#usage) / [Documentation and examples](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples)
-* [License and citation](#license)
+<br>
 
+> **ℹ️ Check out our examples about how to use our library!** <br>
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples), [Line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-nlos/mitsuba3-transient-nlos.ipynb)
 
-## What is transient rendering?
+<br>
 
-Conventional rendering is referred as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumtion allowing to simulate light in motion (see the teaser image for a visual example).
+# License and citation
 
-For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives to the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
 
-*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+If you use our code in your project, please consider citing us using the following:
 
-# Main features
+```bibtex
+@misc{mitsuba3transient,
+	title        = {Transient Mitsuba 3},
+	author       = {Royo, Diego and Crespo, Miguel and Garcia, Jorge},
+	year         = 2023,
+	journal      = {GitHub repository},
+	publisher    = {GitHub},
+	howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
+}
+```
 
-* **Cross-platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows (x86_64).
-* **Easy interface** to convert your algorithms for the transient domain.
-* **Temporal domain** filtering.
-* **Python only** library for doing transient rendering in both CPU and GPU.
-* **Several integrators already implemented** including path tracing (also adapted for NLOS scenes) and volumetric path-tracing.
+Additionally, the NLOS features were re-implemented from our publication [Non-line-of-sight transient rendering](https://doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use them:
 
-### Roadmap
+```bibtex
+@article{royo2022non,
+	title        = {Non-line-of-sight transient rendering},
+	author       = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo},
+	year         = 2022,
+	journal      = {Computers & Graphics},
+	doi          = {https://doi.org/10.1016/j.cag.2022.07.003},
+	issn         = {0097-8493},
+	url          = {https://www.sciencedirect.com/science/article/pii/S0097849322001200}
+}
+```
+
+# What is transient rendering?
+
+Conventional rendering is referred to as steady state, where the light propagation speed is assumed to be infinite. In contrast, transient rendering breaks this assumption allowing us to simulate light in motion (see the teaser image for a visual example).
+
+For example, path tracing algorithms integrate over multiple paths that connect a light source with the camera. For a known path, transient path tracing uses the *very complex* formula of `time = distance / speed` (see [[Two New Sciences by Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when each photon arrives at the camera from the path's `distance` and light's `speed`. This adds a new `time` dimension to the captured images (i.e. it's a video now). The simulations now take new parameters as input: when to start recording the video, how long is each time step (framerate), and how many frames to record.
+
+*Note: note that the `time` values we need to compute are very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter), `time` is usually measured in optical path distance. See [Wikipedia](https://en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl = distance * refractive_index`*
+
+# Roadmap
 
 **Last update: Apr. 2024*
 
 - [ ] Importance sampling of the temporal domain
 - [ ] Differentiable transient rendering
 - [ ] Fluorescence BRDF
 - [X] Non-line-of-sight support (NLOS)
   - [X] `max_depth`
   - [X] `filter_depth`
   - [X] `discard_direct_paths`
   - [ ] `auto_detect_bins`
   - [ ] Faster implementation of exhaustive scanning
 
-# Requirements
-
-- `Python >= 3.8`
-- `Mitsuba3 >= 3.5.0`
-- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
-- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
-
 
 # Installation
 
 We provide the package via PyPI. To install `mitsuba3-transient-nlos` you need to run:
 
 ```bash
 pip install mitransient
 ```
 
-If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then we recommend that you compile Mitsuba 3 youself, enabling the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html).
+If you have installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant which only propagates one wavelength), then we recommend that you compile Mitsuba 3 yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html) and enable the following variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`.
+
+## Requirements
+
+- `Python >= 3.8`
+- `Mitsuba3 >= 3.5.0`
+- (optional) For computation on the GPU: `Nvidia driver >= 495.89`
+- (optional) For vectorized / parallel computation on the CPU: `LLVM >= 11.1`
 
 ## Old installation instructions (incl. Mitsuba 3 fork)
 
 <details>
 <summary>See details</summary>
 _NOTE: These instructions have been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully) without many problems_
 
@@ -135,25 +157,25 @@
       cmake \
           -GNinja \
           -DCMAKE_CXX_COMPILER=<path-to-c++-compiler> \
           -DCMAKE_C_COMPILER=<path-to-c-compiler> \
           -DPython_EXECUTABLE=<path-to-python-executable> \
           ..
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
+
     * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with ninja
       ```bash
       cmake <same arguments as before> ..
       ninja  # This will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     ```bash
     cd ../../..  # go back to initial mitsuba3-transient-nlos folder
     scripts/local_install.sh
     ```
 
 ### Windows users:
@@ -164,26 +186,26 @@
     ```
     * A recent version of Visual Studio 2022 is required. Cmake need to be installed manually
     * Check that the version of your Python is the correct one when you execute `python`
       ```powershell
       # Specifically ask for the 64 bit version of Visual Studio to be safe
       cmake -G "Visual Studio 17 2022" -A x64 -B build
       ```
-  
+
     * Step 1.1: You should see a message that a file was created on "build/mitsuba.conf". Open the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/en/latest/src/key_topics/variants.html
       * Recommended variants: `"scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`.
       * IMPORTANT: At least one *_ad_* variant needs to be specified.
-  
-    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio. 
+
+    * Step 1.2: Re-run the cmake command to read the updated mitsuba.conf and compile the code with Visual Studio.
       ```powershell
       cmake <same arguments as before>
       # You can build from terminal with this, if you don't like opening Visual Studio
       cmake --build build --config Release  # this will take some time
       ```
-  
+
   * Step 2: Install `mitsuba3-transient-nlos` (a.k.a. `mitransient` Python library)
     * Step 2.1: You will need to edit your environment variables in Windows manually
       ```
       MITSUBA_DIR = <path-to-the-cloned-repository</mitsuba3-transient-nlos/ext/mitsuba3/build/Release
       Path = %Path%;%MITSUBA_DIR%
       PYTHON_PATH = %MITSUBA_DIR%/python
       ```
@@ -193,76 +215,44 @@
       python -m pip install .
       ```
 
 </details>
 
 ## After installation
 
-At this point you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
-
-If it works, you're all set!
+At this point, you should be able to `import mitsuba` and `import mitransient` in your Python code (careful about setting the correct `PATH` environment variable if you have compiled Mitsuba 3 yourself, see the section below).
 
 For NLOS data capture simulations, see https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with an easier shell interface instead of directly from Python.
 
 ### If you use your own Mitsuba 3
 
-If you have opted for using a custom (non-default installation through `pip`) of Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
+If you have opted for using a custom (non-default installation through `pip`) Mitsuba 3, you have several options for it. The idea here is to be able to control which version of Mitsuba will be loaded on demand.
 
-* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
+* One solution is to directly execute `setpath.sh` provided after the compilation of the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This shell script will modify the `PATH` and `PYTHONPATH` variables to load first this version of Mitsuba.
 * Another solution following the previous one is to directly set yourself the `PYTHONPATH` environment variable as you wish.
-* Another solution for having a custom version globally available is by using `pip install .--editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly for use. Please follow these instructions:
+* Another solution for having a custom version globally available is by using `pip install . --editable`. This will create a symlink copy of the package files inside the corresponding `site-packages` folder and will be listed as a package installed of `pip` and will be available as other packages installed. If you recompile them, you will still have the newest version directly to use. Please follow these instructions:
   * Go to `<mitsuba-path>/mitsuba3/build/python/drjit` and execute `pip install . --editable`.
   * Go to `<mitsuba-path>/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`.
-* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify on-site the PYTHON PATH for that specific notebook:
+* If you are a user of Jupyter Notebooks, the easiest solution will be to add the following snippet of code to modify the notebook's `PYTHONPATH`:
 ```python
 import sys
 sys.path.insert(0, '<mitsuba-path>/mitsuba3/build/python')
 import mitsuba as mi
 ```
 
 # Usage
 
-Check out the `examples` folder for practical usage.
+> **ℹ️ Check out the `examples` folder for practical usage!** <br>
 
 As of November 2023, `mitsuba3-transient-nlos` implements the following plugins which can be used in scene XML files. To view a description of their parameters, click on the name of your desired plugin.
 * `film`:
   * [`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin.
 * `integrators`:
   * [`transient_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient path tracing for line-of-sight scenes. If you want to do NLOS simulations, use `transientnlospath` instead.
   * [`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/nlos-render)).
   * [`transient_prbvolpath`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/transient_prb_volpath.py): Path Replay Backpropagation for volumetric path tracing. Implemented by Miguel Crespo, untested.
 * `sensor`:
   * [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of the scene's geometries, and measures uniformly-spaced points on such geometry (e.g. relay wall).
 
 ## Testing
 
-Our test suite can be ran using `pytest` on the root folder of the repo.
-
-# License and citation
-
-This project was created by [Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge García](https://jgarciapueyo.github.io/).
-
-If you are using our code for transient NLOS simulations, we would be grateful if you cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003):
-
-```bibtex
-@article{royo2022non,
-    title = {Non-line-of-sight transient rendering},
-    journal = {Computers & Graphics},
-    year = {2022},
-    issn = {0097-8493},
-    doi = {https://doi.org/10.1016/j.cag.2022.07.003},
-    url = {https://www.sciencedirect.com/science/article/pii/S0097849322001200},
-    author = {Diego Royo and Jorge García and Adolfo Muñoz and Adrian Jarabo}
-```
-
-Otherwise you can cite this repository as:
-
-```bibtex
-@misc{mitsuba3transient,
-  author = {Royo, Diego and Garcia, Jorge and Crespo, Miguel},
-  title = {Mitsuba 3 Transient},
-  year = {2023},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/diegoroyo/mitsuba3-transient-nlos}}
-}
-```
+Our test suite can be run using `pytest` on the root folder of the repo.
```

#### html2text {}

```diff
@@ -1,81 +1,106 @@
-Metadata-Version: 2.1 Name: mitransient Version: 1.0.1 Summary: Transient
+Metadata-Version: 2.1 Name: mitransient Version: 1.0.2 Summary: Transient
 rendering extensions for Mitsuba 3 Home-page: https://github.com/diegoroyo/
-mitsuba3-transient-nlos Author: Diego Royo, Miguel Crespo, Jorge GarcÃ­a
+mitsuba3-transient-nlos Author: Miguel Crespo, Diego Royo, Jorge GarcÃ­a
 Author-email: droyo@unizar.es License: BSD Requires-Python: >=3.8 Description-
-Content-Type: text/markdown
+Content-Type: text/markdown Requires-Dist: mitsuba>=3.5.0
      [https://github.com/mitsuba-renderer/mitsuba2/raw/master/docs/images/
                                 logo_plain.png]
                        ************ TTrraannssiieenntt MMiittssuubbaa 33 ************
                _MM_ii_gg_uu_ee_ll_ _CC_rr_ee_ss_pp_oo      _DD_ii_ee_gg_oo_ _RR_oo_yy_oo      _JJ_oo_rr_gg_ee_ _GG_aa_rr_cc_?Ã_?­_aa
 
-[.images/cornell-box.png][.images/cornell-box.gif][.images/nlos-Z.png][.images/
-                                  nlos-Z.gif]
+   [https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/master/.images/
+  cornell-box.png][https://github.com/diegoroyo/mitsuba3-transient-nlos/raw/
+    master/.images/cornell-box.gif][https://github.com/diegoroyo/mitsuba3-
+  transient-nlos/raw/master/.images/nlos-Z.png][https://github.com/diegoroyo/
+            mitsuba3-transient-nlos/raw/master/.images/nlos-Z.gif]
 
-# Introduction This library adds support to [Mitsuba 3](https://github.com/
-mitsuba-renderer/mitsuba3) for doing transient simulations, and especially non-
-line-of-sight (NLOS) data capture simulations. ## Quick start: * [Installation]
-(#installation) * [Usage](#usage) / [Documentation and examples](https://
-github.com/diegoroyo/mitsuba3-transient-nlos/tree/main/examples) * [License and
-citation](#license) ## What is transient rendering? Conventional rendering is
-referred as steady state, where the light propagation speed is assumed to be
-infinite. In contrast, transient rendering breaks this assumtion allowing to
-simulate light in motion (see the teaser image for a visual example). For
-example, path tracing algorithms integrate over multiple paths that connect a
-light source with the camera. For a known path, transient path tracing uses the
-*very complex* formula of `time = distance / speed` (see [[Two New Sciences by
-Galileo]](https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the
-`time` when each photon arrives to the camera from the path's `distance` and
-light's `speed`. This adds a new `time` dimension to the captured images (i.e.
-it's a video now). The simulations now take new parameters as input: when to
-start recording the video, how long is each time step (framerate), and how many
+# Overview This library adds support to [Mitsuba 3](https://github.com/mitsuba-
+renderer/mitsuba3) for doing transient simulations, with amazing support for
+non-line-of-sight (NLOS) data capture simulations. ### Main features * **Cross-
+platform:** Mitsuba 3 has been tested on Linux (x86_64), macOS (aarch64,
+x86_64), and Windows (x86_64). * **Easy interface** to convert your algorithms
+for the transient domain. * **Temporal domain** filtering. * **Python-only**
+library for doing transient rendering in both CPU and GPU. * **Several
+integrators have already been implemented** including path tracing (also
+adapted for NLOS scenes) and volumetric path-tracing.
+> **â¹ï¸ Check out our examples about how to use our library!**
+> Featuring [General Usage](https://github.com/diegoroyo/mitsuba3-transient-
+nlos/tree/main/examples), [Line-of-sight transient rendering](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient/
+render_cbox_diffuse.ipynb), and [Non-line-of-sight transient rendering](https:/
+/github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/examples/transient-
+nlos/mitsuba3-transient-nlos.ipynb)
+# License and citation This project was created by [Miguel Crespo](https://
+mcrespo.me) and expanded by [Diego Royo](https://diego.contact) and [Jorge
+GarcÃ­a](https://jgarciapueyo.github.io/). If you use our code in your project,
+please consider citing us using the following: ```bibtex @misc
+{mitsuba3transient, title = {Transient Mitsuba 3}, author = {Royo, Diego and
+Crespo, Miguel and Garcia, Jorge}, year = 2023, journal = {GitHub repository},
+publisher = {GitHub}, howpublished = {\url{https://github.com/diegoroyo/
+mitsuba3-transient-nlos}} } ``` Additionally, the NLOS features were re-
+implemented from our publication [Non-line-of-sight transient rendering](https:
+//doi.org/10.1016/j.cag.2022.07.003). Please also consider citing us if you use
+them: ```bibtex @article{royo2022non, title = {Non-line-of-sight transient
+rendering}, author = {Diego Royo and Jorge GarcÃ­a and Adolfo MuÃ±oz and Adrian
+Jarabo}, year = 2022, journal = {Computers & Graphics}, doi = {https://doi.org/
+10.1016/j.cag.2022.07.003}, issn = {0097-8493}, url = {https://
+www.sciencedirect.com/science/article/pii/S0097849322001200} } ``` # What is
+transient rendering? Conventional rendering is referred to as steady state,
+where the light propagation speed is assumed to be infinite. In contrast,
+transient rendering breaks this assumption allowing us to simulate light in
+motion (see the teaser image for a visual example). For example, path tracing
+algorithms integrate over multiple paths that connect a light source with the
+camera. For a known path, transient path tracing uses the *very complex*
+formula of `time = distance / speed` (see [[Two New Sciences by Galileo]]
+(https://en.wikipedia.org/wiki/Two_New_Sciences)) to compute the `time` when
+each photon arrives at the camera from the path's `distance` and light's
+`speed`. This adds a new `time` dimension to the captured images (i.e. it's a
+video now). The simulations now take new parameters as input: when to start
+recording the video, how long is each time step (framerate), and how many
 frames to record. *Note: note that the `time` values we need to compute are
 very small (e.g. light takes only ~3.33 * 10^-9 seconds to travel 1 meter),
 `time` is usually measured in optical path distance. See [Wikipedia](https://
 en.wikipedia.org/wiki/Optical_path_length) for more information. TL;DR `opl =
-distance * refractive_index`* # Main features * **Cross-platform:** Mitsuba 3
-has been tested on Linux (x86_64), macOS (aarch64, x86_64), and Windows
-(x86_64). * **Easy interface** to convert your algorithms for the transient
-domain. * **Temporal domain** filtering. * **Python only** library for doing
-transient rendering in both CPU and GPU. * **Several integrators already
-implemented** including path tracing (also adapted for NLOS scenes) and
-volumetric path-tracing. ### Roadmap **Last update: Apr. 2024* - [ ] Importance
-sampling of the temporal domain - [ ] Differentiable transient rendering - [ ]
-Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X] `max_depth` -
-[X] `filter_depth` - [X] `discard_direct_paths` - [ ] `auto_detect_bins` - [ ]
-Faster implementation of exhaustive scanning # Requirements - `Python >= 3.8` -
-`Mitsuba3 >= 3.5.0` - (optional) For computation on the GPU: `Nvidia driver >=
-495.89` - (optional) For vectorized / parallel computation on the CPU: `LLVM >=
-11.1` # Installation We provide the package via PyPI. To install `mitsuba3-
-transient-nlos` you need to run: ```bash pip install mitransient ``` If you
-have installed Mitsuba 3 via `pip` you will only have access to the
-`llvm_ad_rgb` and `cuda_ad_rgb` variants. If you want to use other variants
-(e.g. NLOS simulations can greatly benefit from the `llvm_mono` variant), then
-we recommend that you compile Mitsuba 3 youself, enabling the following
-variants: `["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono",
-"cuda_ad_mono", "scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb",
-"cuda_ad_rgb"]`. [Here's more info](https://mitsuba.readthedocs.io/en/latest/
-src/developer_guide/compiling.html). ## Old installation instructions (incl.
-Mitsuba 3 fork) See details _NOTE: These instructions have been tested on Linux
-and Windows 11 (Powershell), but can be adapted to MacOS probably (hopefully)
-without many problems_ After cloning the repo, navigate to the root folder and
-execute the following commands to build the custom version of Mitsuba 3 * Step
-0: Clone the repo (including the mitsuba3 custom fork submodule) ```bash git
-clone git@github.com:diegoroyo/mitsuba3-transient-nlos.git mitsuba3-transient-
-nlos cd mitsuba3-transient-nlos git submodule update --init --recursive ``` ##
-Now the steps are different for Linux and Windows users ### Linux users: * Step
-1: Compile mitsuba3 (ext/mitsuba3) from source * This is for Linux. for other
-OSes, check: https://mitsuba.readthedocs.io/en/latest/src/developer_guide/
-compiling.html ```bash cd ext/mitsuba3 mkdir -p build && cd build ``` * You
-might want to set the C++/C compiler (probably you want this e.g. if `cmake`
-complains about your version of g++). Always set `C_COMPILER` version to the
-same version as `CXX_COMPILER` (e.g. if you use `g++-12`, then also set `gcc-
-12`) * If you have multiple Python versions installed, also set
-Python_EXECUTABLE to ensure that the program is compiled for your specific
-version of Python ```bash cmake \ -GNinja \ -DCMAKE_CXX_COMPILER=
+distance * refractive_index`* # Roadmap **Last update: Apr. 2024* - [ ]
+Importance sampling of the temporal domain - [ ] Differentiable transient
+rendering - [ ] Fluorescence BRDF - [X] Non-line-of-sight support (NLOS) - [X]
+`max_depth` - [X] `filter_depth` - [X] `discard_direct_paths` - [ ]
+`auto_detect_bins` - [ ] Faster implementation of exhaustive scanning #
+Installation We provide the package via PyPI. To install `mitsuba3-transient-
+nlos` you need to run: ```bash pip install mitransient ``` If you have
+installed Mitsuba 3 via `pip` you will only have access to the `llvm_ad_rgb`
+and `cuda_ad_rgb` variants. If you want to use other variants (e.g. NLOS
+simulations can greatly benefit from the `llvm_mono` variant which only
+propagates one wavelength), then we recommend that you compile Mitsuba 3
+yourself [following this tutorial](https://mitsuba.readthedocs.io/en/latest/
+src/developer_guide/compiling.html) and enable the following variants: `
+["scalar_mono", "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono",
+"scalar_rgb", "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"]`. ##
+Requirements - `Python >= 3.8` - `Mitsuba3 >= 3.5.0` - (optional) For
+computation on the GPU: `Nvidia driver >= 495.89` - (optional) For vectorized /
+parallel computation on the CPU: `LLVM >= 11.1` ## Old installation
+instructions (incl. Mitsuba 3 fork) See details _NOTE: These instructions have
+been tested on Linux and Windows 11 (Powershell), but can be adapted to MacOS
+probably (hopefully) without many problems_ After cloning the repo, navigate to
+the root folder and execute the following commands to build the custom version
+of Mitsuba 3 * Step 0: Clone the repo (including the mitsuba3 custom fork
+submodule) ```bash git clone git@github.com:diegoroyo/mitsuba3-transient-
+nlos.git mitsuba3-transient-nlos cd mitsuba3-transient-nlos git submodule
+update --init --recursive ``` ## Now the steps are different for Linux and
+Windows users ### Linux users: * Step 1: Compile mitsuba3 (ext/mitsuba3) from
+source * This is for Linux. for other OSes, check: https://
+mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html ```bash cd
+ext/mitsuba3 mkdir -p build && cd build ``` * You might want to set the C++/
+C compiler (probably you want this e.g. if `cmake` complains about your version
+of g++). Always set `C_COMPILER` version to the same version as `CXX_COMPILER`
+(e.g. if you use `g++-12`, then also set `gcc-12`) * If you have multiple
+Python versions installed, also set Python_EXECUTABLE to ensure that the
+program is compiled for your specific version of Python ```bash cmake \ -GNinja
+\ -DCMAKE_CXX_COMPILER=
 +-compiler> \ -DCMAKE_C_COMPILER= \ -DPython_EXECUTABLE= \ .. ``` * Step 1.1:
 You should see a message that a file was created on "build/mitsuba.conf". Open
 the file and look for "enabled" variants. Docs: https://mitsuba.readthedocs.io/
 en/latest/src/key_topics/variants.html * Recommended variants: `"scalar_mono",
 "llvm_mono", "llvm_ad_mono", "cuda_mono", "cuda_ad_mono", "scalar_rgb",
 "llvm_rgb", "llvm_ad_rgb", "cuda_rgb", "cuda_ad_rgb"`. * IMPORTANT: At least
 one *_ad_* variant needs to be specified. * Step 1.2: Re-run the cmake command
@@ -100,69 +125,55 @@
 --config Release # this will take some time ``` * Step 2: Install `mitsuba3-
 transient-nlos` (a.k.a. `mitransient` Python library) * Step 2.1: You will need
 to edit your environment variables in Windows manually ``` MITSUBA_DIR =
 /mitsuba3-transient-nlos/ext/mitsuba3/build/Release Path = %Path%;%MITSUBA_DIR%
 PYTHON_PATH = %MITSUBA_DIR%/python ``` * Step 2.2: Install `mitsuba3-transient-
 nlos` (a.k.a. `mitransient` Python library) ```powershell cd ../../ # go back
 to initial mitsuba3-transient-nlos folder python -m pip install . ``` ## After
-installation At this point you should be able to `import mitsuba` and `import
+installation At this point, you should be able to `import mitsuba` and `import
 mitransient` in your Python code (careful about setting the correct `PATH`
 environment variable if you have compiled Mitsuba 3 yourself, see the section
-below). If it works, you're all set! For NLOS data capture simulations, see
-https://github.com/diegoroyo/tal. `tal` is a toolkit that allows you to create
-and simulate NLOS scenes with an easier shell interface instead of directly
-from Python. ### If you use your own Mitsuba 3 If you have opted for using a
-custom (non-default installation through `pip`) of Mitsuba 3, you have several
-options for it. The idea here is to be able to control which version of Mitsuba
-will be loaded on demand. * One solution is to directly execute `setpath.sh`
-provided after the compilation of the Mitsuba 3 repo [(More info)](https://
-mitsuba.readthedocs.io/en/latest/src/developer_guide/compiling.html). This
-shell script (on Linux) will modify the `PATH` and `PYTHONPATH` variables to
-load first this version of Mitsuba. * Another solution following the previous
-one is to directly set yourself the `PYTHONPATH` environment variable as you
-wish. * Another solution for having a custom version globally available is by
-using `pip install .--editable`. This will create a symlink copy of the package
-files inside the corresponding `site-packages` folder and will be listed as a
-package installed of `pip` and will be available as other packages installed.
-If you recompile them, you will still have the newest version directly for use.
-Please follow these instructions: * Go to `/mitsuba3/build/python/drjit` and
-execute `pip install . --editable`. * Go to `/mitsuba3/build/python/mitsuba`
-and execute `pip install . --editable`. * If you are a user of Jupyter
-Notebooks, the easiest solution will be to add the following snippet of code to
-modify on-site the PYTHON PATH for that specific notebook: ```python import sys
-sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi ``` # Usage
-Check out the `examples` folder for practical usage. As of November 2023,
-`mitsuba3-transient-nlos` implements the following plugins which can be used in
-scene XML files. To view a description of their parameters, click on the name
-of your desired plugin. * `film`: * [`transient_hdr_film`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/films/
-transient_hdr_film.py): Transient equivalent of Mitsuba 3's `hdrfilm` plugin. *
-`integrators`: * [`transient_path`](https://github.com/diegoroyo/mitsuba3-
-transient-nlos/blob/main/mitransient/integrators/transientpath.py): Transient
-path tracing for line-of-sight scenes. If you want to do NLOS simulations, use
-`transientnlospath` instead. * [`transient_nlos_path`](https://github.com/
-diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
-transientnlospath.py): Transient path tracing with specific sampling routines
-for NLOS scenes (e.g. laser sampling and hidden geometry sampling of the ["Non-
-Line-of-Sight Transient Rendering" paper](https://diego.contact/publications/
-nlos-render)). * [`transient_prbvolpath`](https://github.com/diegoroyo/
-mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+below). For NLOS data capture simulations, see https://github.com/diegoroyo/
+tal. `tal` is a toolkit that allows you to create and simulate NLOS scenes with
+an easier shell interface instead of directly from Python. ### If you use your
+own Mitsuba 3 If you have opted for using a custom (non-default installation
+through `pip`) Mitsuba 3, you have several options for it. The idea here is to
+be able to control which version of Mitsuba will be loaded on demand. * One
+solution is to directly execute `setpath.sh` provided after the compilation of
+the Mitsuba 3 repo [(More info)](https://mitsuba.readthedocs.io/en/latest/src/
+developer_guide/compiling.html). This shell script will modify the `PATH` and
+`PYTHONPATH` variables to load first this version of Mitsuba. * Another
+solution following the previous one is to directly set yourself the
+`PYTHONPATH` environment variable as you wish. * Another solution for having a
+custom version globally available is by using `pip install . --editable`. This
+will create a symlink copy of the package files inside the corresponding `site-
+packages` folder and will be listed as a package installed of `pip` and will be
+available as other packages installed. If you recompile them, you will still
+have the newest version directly to use. Please follow these instructions: * Go
+to `/mitsuba3/build/python/drjit` and execute `pip install . --editable`. * Go
+to `/mitsuba3/build/python/mitsuba` and execute `pip install . --editable`. *
+If you are a user of Jupyter Notebooks, the easiest solution will be to add the
+following snippet of code to modify the notebook's `PYTHONPATH`: ```python
+import sys sys.path.insert(0, '/mitsuba3/build/python') import mitsuba as mi
+``` # Usage > **â¹ï¸ Check out the `examples` folder for practical usage!**
+As of November 2023, `mitsuba3-transient-nlos` implements the following plugins
+which can be used in scene XML files. To view a description of their
+parameters, click on the name of your desired plugin. * `film`: *
+[`transient_hdr_film`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/films/transient_hdr_film.py): Transient equivalent of
+Mitsuba 3's `hdrfilm` plugin. * `integrators`: * [`transient_path`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
+transientpath.py): Transient path tracing for line-of-sight scenes. If you want
+to do NLOS simulations, use `transientnlospath` instead. *
+[`transient_nlos_path`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
+blob/main/mitransient/integrators/transientnlospath.py): Transient path tracing
+with specific sampling routines for NLOS scenes (e.g. laser sampling and hidden
+geometry sampling of the ["Non-Line-of-Sight Transient Rendering" paper](https:
+//diego.contact/publications/nlos-render)). * [`transient_prbvolpath`](https://
+github.com/diegoroyo/mitsuba3-transient-nlos/blob/main/mitransient/integrators/
 transient_prb_volpath.py): Path Replay Backpropagation for volumetric path
 tracing. Implemented by Miguel Crespo, untested. * `sensor`: *
 [`nlos_capture_meter`](https://github.com/diegoroyo/mitsuba3-transient-nlos/
 blob/main/mitransient/sensors/nloscapturemeter.py): Can be attached to one of
 the scene's geometries, and measures uniformly-spaced points on such geometry
-(e.g. relay wall). ## Testing Our test suite can be ran using `pytest` on the
-root folder of the repo. # License and citation This project was created by
-[Miguel Crespo](https://mcrespo.me) and expanded by [Diego Royo](https://
-diego.contact) and [Jorge GarcÃ­a](https://jgarciapueyo.github.io/). If you are
-using our code for transient NLOS simulations, we would be grateful if you
-cited [our publication](https://doi.org/10.1016/j.cag.2022.07.003): ```bibtex
-@article{royo2022non, title = {Non-line-of-sight transient rendering}, journal
-= {Computers & Graphics}, year = {2022}, issn = {0097-8493}, doi = {https://
-doi.org/10.1016/j.cag.2022.07.003}, url = {https://www.sciencedirect.com/
-science/article/pii/S0097849322001200}, author = {Diego Royo and Jorge GarcÃ­a
-and Adolfo MuÃ±oz and Adrian Jarabo} ``` Otherwise you can cite this repository
-as: ```bibtex @misc{mitsuba3transient, author = {Royo, Diego and Garcia, Jorge
-and Crespo, Miguel}, title = {Mitsuba 3 Transient}, year = {2023}, publisher =
-{GitHub}, journal = {GitHub repository}, howpublished = {\url{https://
-github.com/diegoroyo/mitsuba3-transient-nlos}} } ```
+(e.g. relay wall). ## Testing Our test suite can be run using `pytest` on the
+root folder of the repo.
```

### Comparing `mitransient-1.0.1/mitransient.egg-info/SOURCES.txt` & `mitransient-1.0.2/mitransient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitransient-1.0.1/setup.py` & `mitransient-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     exec(f.read())
 
 setup(
     name='mitransient',
     version=__version__,
     description='Transient rendering extensions for Mitsuba 3',
     url='https://github.com/diegoroyo/mitsuba3-transient-nlos',
-    author='Diego Royo, Miguel Crespo, Jorge García',
+    author='Miguel Crespo, Diego Royo, Jorge García',
     author_email='droyo@unizar.es',
     license='BSD',
     packages=find_packages(),
     install_requires=[f"mitsuba>={__mi_version__}"],
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires=">=3.8"
```

