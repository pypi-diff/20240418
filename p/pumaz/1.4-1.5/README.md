# Comparing `tmp/pumaz-1.4.tar.gz` & `tmp/pumaz-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-1.4.tar", last modified: Wed Apr 10 13:26:08 2024, max compression
+gzip compressed data, was "pumaz-1.5.tar", last modified: Thu Apr 18 12:47:06 2024, max compression
```

## Comparing `pumaz-1.4.tar` & `pumaz-1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.482655 pumaz-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-10 13:26:08.482655 pumaz-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-10 13:26:01.000000 pumaz-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.478654 pumaz-1.4/pumaz/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    42656 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/pumaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-10 13:26:01.000000 pumaz-1.4/pumaz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:26:08.478654 pumaz-1.4/pumaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 13:26:08.000000 pumaz-1.4/pumaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:26:08.482655 pumaz-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-10 13:26:01.000000 pumaz-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:47:06.190438 pumaz-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-18 12:47:06.190438 pumaz-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-04-18 12:47:01.000000 pumaz-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:47:06.190438 pumaz-1.5/pumaz/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/pumaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-18 12:47:01.000000 pumaz-1.5/pumaz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:47:06.190438 pumaz-1.5/pumaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 12:47:06.000000 pumaz-1.5/pumaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:47:06.190438 pumaz-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 12:47:01.000000 pumaz-1.5/setup.py
```

### Comparing `pumaz-1.4/PKG-INFO` & `pumaz-1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,184 +1,152 @@
-Metadata-Version: 2.1
-Name: pumaz
-Version: 1.4
-Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
-Home-page: https://github.com/QIMP-Team/PUMA
-Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
-Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
-License: GPLv3
-Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Requires-Dist: nibabel~=3.2.2
-Requires-Dist: halo~=0.0.31
-Requires-Dist: SimpleITK~=2.2.1
-Requires-Dist: pydicom~=2.2.2
-Requires-Dist: argparse~=1.4.0
-Requires-Dist: numpy
-Requires-Dist: mpire~=2.3.3
-Requires-Dist: openpyxl~=3.0.9
-Requires-Dist: matplotlib
-Requires-Dist: pyfiglet~=0.8.post1
-Requires-Dist: natsort~=8.1.0
-Requires-Dist: pillow>=9.2.0
-Requires-Dist: colorama~=0.4.6
-Requires-Dist: rich
-Requires-Dist: pandas
-Requires-Dist: dicom2nifti
-Requires-Dist: nifti2dicom
-Requires-Dist: requests
-Requires-Dist: moosez
-Requires-Dist: halo
-Requires-Dist: psutil
-Requires-Dist: gputil
-Requires-Dist: dask
-Requires-Dist: lionz
-
 ![Puma-logo](Images/Puma-logo.png)
 
-## PUMA 1.2 🐾 - Agile. Precision-Driven. Empowering 💪
-[![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/)
+## PUMA 1.0 🐾 -  One Image multiple perspectives 🎭
+[![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+**🌈 PET Reimagined: From Monochrome to a Palette of Possibilities with PUMA 1.0**
+
+Step into the vibrant new world of PET imaging with PUMA 1.0 🌟, where traditional monochrome scans are transformed into a dynamic spectrum of diagnostic data. 🎨
 
-Get ready for a leap in the world of Positron Emission Tomography (PET) imaging: introducing PUMA 1.2 🚀
+With PUMA 1.0, experience the power of multiplexing: a process that fuses multiple tracer images into a single, multicolored composite that reveals not just the presence of disease but its multifaceted physiological context. 🔄 The multiplexed approach provides a more comprehensive view, helping clinicians uncover nuanced insights about tumors and their microenvironments. 🔍
 
-PUMA 1.2 (PET Universal Multi-tracer Aligner) has been crafted with a strong focus on the challenges of clinical PET imaging.
+Whether you're in a high-tech lab or a remote clinic, PUMA 1.0 delivers high-quality, multiplexed PET scans that are as rich in detail as they are in color. 🏥 It’s not just an upgrade—it’s a whole new way of seeing PET data, turning every image into a detailed map of insight and opportunity. 🗺️
 
-⚡ It's Agile: PUMA operates across all operating systems and architectures, from x86 to ARM64 (Apple Silicon). It has no specific hardware needs, and with the requirement for Python 3.9 or above, PUMA 1.2 is ready to perform anywhere, anytime.
+## 🎉 Key Features
 
-🔍 It's Precision-Driven yet blazingly fast: Built upon the bedrock of nnUNet based MOOSE and advanced diffeomorphic registration techniques from the awesome 'greedy' library, PUMA 1.2 aligns multiplexed tracer images with high precision in less than a heartbeat, clocking in at under one minute, offering unrivaled clarity and accuracy in the diagnosis of patient pathology.
+### 🚀 Versatile and Powerful
+Run PUMA 1.0 on any device, any OS, from x86 to ARM64 (hello, Apple Silicon fans!). Whether you’re on a high-end GPU or a humble CPU, PUMA adapts to your needs without breaking a sweat.
 
-🗝️ It's Empowering: PUMA 1.2 enhances diagnostic capabilities with its multiplexed viewing angles, unlocking a new realm of diagnostic possibilities and empowering clinicians.
+### 🔍 Precision Meets Speed
+Harness the power of AI with MOOSE-driven segmentations and ‘greedy’ library’s wizardry for diffeomorphic image registration. PUMA 1.0 nails the perfect balance of sharp accuracy and zippy performance.
 
-Join us on this revolutionary journey with PUMA 1.2.
+### 🎨 Art of Imaging
+Why settle for ordinary when you can visualize in vibrant RGB? Each color shines a spotlight on a different tracer, turning complex data into a vivid, easy-to-interpret display. With processing times ranging from just 5 to 12 minutes, you're all set for a speedy yet thorough diagnostic journey.
 
 ## 🚀 PUMA's multiplexing in action
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
   <img alt="Shows an illustrated MOOSE story board adopted to different themes" src="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
 </picture>
 </div>
 
 ## Requirements ✅
 
-Before stepping into the future with PUMA 1.2, here's what you need for an optimal experience:
+Before stepping into the future with PUMA 1.0, here's what you need for an optimal experience:
 
-- **Operating System**: Windows, Mac, or Linux - PUMA 1.2 is versatile and works across all these platforms.
+- **Operating System**: Windows, Mac, or Linux - PUMA 1.0 is versatile and works across all these platforms.
 
 - **Memory**: Make sure your system has enough memory (8-16 GB) to run the tasks smoothly.
 
 - **GPU**: You need a cuda enabled GPU (NVIDIA), 8 GB or more!
 
-- **Python**: PUMA 1.2 operates with Python 3.10, staying in line with the latest updates.
+- **Python**: PUMA 1.0 operates with Python 3.10, staying in line with the latest updates.
 
-Once these specifications are met, you're all set to experience PUMA 1.2's capabilities.
+Once these specifications are met, you're all set to experience PUMA 1.0's capabilities.
 
 ## Installation Guide 🛠️
 
-Installation is a breeze on Windows, Linux, and MacOS. Follow the steps below to start your journey with PUMA 1.2.
+Installation is a breeze on Windows, Linux, and MacOS. Follow the steps below to start your journey with PUMA 1.0.
 
 ### For Linux and MacOS 🐧🍏
 
 1. Create a Python environment named 'puma-env' or as per your preference.
    ```bash
    python3 -m venv puma-env
    ```
 
 2. Activate the environment.
    ```bash
    source puma-env/bin/activate  # for Linux
    source puma-env/bin/activate  # for MacOS
    ```
 
-3. Install PUMA 1.2.
+3. Install PUMA 1.0.
    ```bash
    pip install pumaz
    ```
 
-Congratulations! You're all set to start using PUMA 1.2.
+Congratulations! You're all set to start using PUMA 1.0.
 
 ### For Windows 🪟
 
 1. Create a Python environment, e.g., 'puma-env'.
    ```bash
    python -m venv puma-env
    ```
 
 2. Activate the environment.
    ```bash
    .\puma-env\Scripts\activate
    ```
 
-3. Install PUMA 1.2.
+3. Install PUMA 1.0.
    ```bash
    pip install pumaz
    ```
 
-You're now ready to experience the precision and speed of PUMA 1.2.
+You're now ready to experience the precision and speed of PUMA 1.0.
 
 ## Usage Guide 📚
 
-Start your journey with PUMA 1.2 by using our straightforward command-line tool. It requires the directory path containing different tracer images, and each image should be stored in separate folders. Here's how you can get started:
+Start your journey with PUMA 1.0 by using our straightforward command-line tool. It requires the directory path containing different tracer images, and each image should be stored in separate folders. Here's how you can get started:
 
 ```bash
 
    pumaz \
        -d <path_to_image_dir>              # Directory path containing the images to be analyzed
        -ir <regions_to_ignore>             # Regions to ignore: arms, legs, head, none
        -m                                  # Optional: Enable multiplexed RGB image output
        -cs <color_selection>               # Optional: Custom color selection for RGB output (requires -m)
+       -c2d <convert_back_to_dicom>        # Optional: Once set, the generated nifti images will be converted back to DICOM
 ```
 
 - `<path_to_image_dir>` refers to the parent directory containing different tracer images in their respective sub-directories.
 
 - `-ir` specifies the regions to be ignored during registration. If you don't want to ignore any regions, use `none`. If you want to ignore the arms, legs, or head during registration, pass the corresponding regions delimited by a `,`. For example: `-ir head,arms` to ignore the head and arms.
 
 - `-m` will activate the output of a multiplexed RGB image of the combined tracer images.
 
-- `-cs`, when passed along with `-m`, PUMA will ask you to provide a custom order of color channels for the corresponding tracer images. That way, you can freely decide which tracer image is associated with which channel. 
+- `-cs`, when passed along with `-m`, PUMA will ask you to provide a custom order of color channels for the corresponding tracer images. That way, you can freely decide which tracer image is associated with which channel.
+- `-c2d`, when set the generated aligned nifti images will be converted back to DICOM.
+  
 For assistance or additional information, you can always type:
 
 ```bash
 pumaz -h
 ```
+
 ### Example usage:
 Apply PUMA to images in a directory, ignoring arms and legs, with multiplexed RGB output and custom colors:
 
 ```bash
-    pumaz -d /path/to/images -ir arms,legs -m -cs 
+    pumaz -d /path/to/images -ir arms,legs -m -cs -c2d 
 ```
 
 ## Directory Structure and Naming Conventions for PUMA 📂🏷️
 
-PUMA 1.2 requires your data to be structured in a certain way. It supports DICOM directories and NIFTI files. For NIFTI files, users need to ensure that the files are named with the correct modality tag at the start.
+PUMA 1.0 requires your data to be structured in a certain way. It supports DICOM directories and NIFTI files. For NIFTI files, users need to ensure that the files are named with the correct modality tag at the start.
 
 ### Required Directory Structure 🌳
 
-Here is the directory structure that PUMA 1.2 expects:
+Here is the directory structure that PUMA 1.0 expects:
 
 ```
 Parent_Directory
 │
-└───Tracer1
+└───Tracer1 # can be named anything
 │   │
-│   └───PET_DICOM_Directory or PT_xxxx.nii.gz
+│   └───PET_DICOM_Directory or PT_xxxx.nii.gz # If it's DICOM, the folder name can be anything, but if nifti use a prefix 'PT' for PET
 │   │
-│   └───CT_DICOM_Directory or CT_xxxx.nii.gz
+│   └───CT_DICOM_Directory or CT_xxxx.nii.gz # If it's DICOM, the folder name can be anything, but if nifti use a prefix 'CT' for CT
 │
 └───Tracer2
 │   │
 │   └───PET_DICOM_Directory or PT_xxxx.nii.gz
 │   │
 │   └───CT_DICOM_Directory or CT_xxxx.nii.gz
 ...
@@ -209,7 +177,29 @@
 
 Our PUMA package, for example, is named as 'pumaz', pronounced "puma-see". So, why 'Z'?
 
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
  
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/W7ebere"><img src="https://avatars.githubusercontent.com/u/166598214?v=4?s=100" width="100px;" alt="W7ebere"/><br /><sub><b>W7ebere</b></sub></a><br /><a href="https://github.com/LalithShiyam/PUMA/commits?author=W7ebere" title="Documentation">📖</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `pumaz-1.4/pumaz/constants.py` & `pumaz-1.5/pumaz/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 MOOSE_PREFIX_PUMA_CPU = 'Clin_CT_PUMA4_'
 MOOSE_LABEL_INDEX = {
     1: "legs",
     2: "body",
     3: "head",
     4: "arms"
 }
+MOOSE_FILLER_LABEL = 18
 
 # FOLDER NAMES
 
 PUMA_WORKING_FOLDER = 'PUMAZ-v1' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 ALIGNED_MASK_FOLDER = 'aligned_MASK'
 ALIGNED_CT_FOLDER = 'aligned_CT'
```

### Comparing `pumaz-1.4/pumaz/display.py` & `pumaz-1.5/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz/download.py` & `pumaz-1.5/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz/file_utilities.py` & `pumaz-1.5/pumaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz/image_conversion.py` & `pumaz-1.5/pumaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz/image_processing.py` & `pumaz-1.5/pumaz/image_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import psutil
 from lionz import lion
 from moosez import moose
 from mpire import WorkerPool
 from pumaz import constants
 from pumaz import file_utilities
 from pumaz.constants import (GREEDY_PATH, C3D_PATH, ANATOMICAL_MODALITIES, FUNCTIONAL_MODALITIES, RED_WEIGHT,
-                             GREEN_WEIGHT, BLUE_WEIGHT, LIONZ_MODEL)
+                             GREEN_WEIGHT, BLUE_WEIGHT, LIONZ_MODEL, MOOSE_FILLER_LABEL)
 from pumaz.file_utilities import (create_directory, move_file, remove_directory, move_files_to_directory, get_files,
                                   copy_reference_image, move_files, find_images, get_image_by_modality, get_modality)
 from pumaz.resources import check_device
 from rich.console import Console
 from rich.progress import Progress, BarColumn, TimeElapsedColumn
 from rich.table import Table
 
@@ -332,18 +332,61 @@
         change_mask_labels(new_mask_file, constants.MOOSE_LABEL_INDEX, regions_to_ignore)
 
     puma_mask_files = glob.glob(os.path.join(puma_mask_dir, moose_prefix_puma + '*nii*'))
     for puma_mask_file in puma_mask_files:
         new_mask_file = re.sub(rf'{moose_prefix_puma}', '', puma_mask_file)
         os.rename(puma_mask_file, new_mask_file)
         apply_mask(new_mask_file, os.path.join(body_mask_dir, os.path.basename(new_mask_file)), new_mask_file)
+        update_multilabel_mask(new_mask_file, os.path.join(body_mask_dir, os.path.basename(new_mask_file)),
+                               new_mask_file)
 
     return puma_working_dir, ct_dir, pt_dir, puma_mask_dir
 
 
+def update_multilabel_mask(multilabel_mask_path: str, body_mask_path: str, output_path: str) -> None:
+    """
+    Updates a multilabel mask by removing a specific label, converting to binary, and filling in gaps
+    from a binary body mask. The gaps are filled with a specified intensity label.
+
+    Args:
+    - multilabel_mask_path (str): Path to the multilabel mask file.
+    - body_mask_path (str): Path to the body mask file.
+    - output_path (str): Path where the updated mask will be saved.
+
+    Returns:
+    - None
+    """
+    # Load the masks
+    multilabel_mask = sitk.ReadImage(multilabel_mask_path, sitk.sitkUInt8)
+    body_mask = sitk.ReadImage(body_mask_path, sitk.sitkUInt8)
+
+    # Remove the filler label from the multilabel mask
+    multilabel_no_filler = sitk.BinaryThreshold(multilabel_mask, lowerThreshold=0,
+                                                upperThreshold=MOOSE_FILLER_LABEL - 1,
+                                                insideValue=1, outsideValue=0)
+
+    # Convert no filler mask back to the original values where filler label was removed
+    multilabel_no_filler = multilabel_no_filler * multilabel_mask
+
+    # Subtract the no filler binary mask from the binary body mask
+    binary_body_mask = body_mask > 0
+    remaining_mask = binary_body_mask - (multilabel_no_filler > 0)
+
+    # Scale the remaining mask with the filler label intensity
+    scaled_remaining_mask = remaining_mask * MOOSE_FILLER_LABEL
+
+    # Combine the multilabel mask with no filler label and the scaled remaining mask
+    final_mask = sitk.Add(multilabel_no_filler, scaled_remaining_mask)
+
+    # Write the resulting mask to the output path
+    sitk.WriteImage(final_mask, output_path)
+
+
+
+
 class ImageRegistration:
     """
     A class for performing image registration using the GREEDY algorithm.
 
     :param fixed_img: The path to the fixed image.
     :type fixed_img: str
     :param multi_resolution_iterations: The number of multi-resolution iterations to perform.
@@ -371,14 +414,15 @@
         :type update_transforms: bool
         """
         self.moving_img = moving_img
         if update_transforms:
             out_dir = pathlib.Path(self.moving_img).parent
             moving_img_filename = pathlib.Path(self.moving_img).name
             self.transform_files = {
+                'moments': os.path.join(out_dir, f"{moving_img_filename}_moment.mat"),
                 'rigid': os.path.join(out_dir, f"{moving_img_filename}_rigid.mat"),
                 'affine': os.path.join(out_dir, f"{moving_img_filename}_affine.mat"),
                 'warp': os.path.join(out_dir, f"{moving_img_filename}_warp.nii.gz"),
                 'inverse_warp': os.path.join(out_dir, f"{moving_img_filename}_inverse_warp.nii.gz")
             }
 
     def rigid(self) -> str:
@@ -387,21 +431,29 @@
 
         :return: The path to the rigid transform file.
         :rtype: str
         """
         mask_options = {'-gm': self.fixed_mask, '-mm': self.moving_mask}
         combined_mask_cmd = " ".join(f"{key} {re.escape(value)}" for key, value in mask_options.items() if value)
 
+        # Initialize the command with moments 1 <center of mass>
+
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -i " \
+                     fr"{self.fixed_img} {self.moving_img} " \
+                     f"{combined_mask_cmd} -moments 1 -o " \
+                     fr"{self.transform_files['moments']} "
+        subprocess.run(cmd_to_run, shell=True, capture_output=True)
+
         cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i " \
                      fr"{self.fixed_img} {self.moving_img} " \
-                     f"{combined_mask_cmd} -ia-image-centers -dof 6 -o " \
+                     f"{combined_mask_cmd} -ia {self.transform_files['moments']} -dof 6 -o " \
                      fr"{self.transform_files['rigid']} " \
                      f"-n {self.multi_resolution_iterations} -m SSD"
-
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
+
         logging.info(
             f"Rigid alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} | Aligned image: "
             f"moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['rigid']).name}")
         return self.transform_files['rigid']
 
     def affine(self) -> str:
         """
@@ -409,21 +461,30 @@
 
         :return: The path to the affine transform file.
         :rtype: str
         """
         mask_options = {'-gm': self.fixed_mask, '-mm': self.moving_mask}
         combined_mask_cmd = " ".join(f"{key} {re.escape(value)}" for key, value in mask_options.items() if value)
 
+        # Initialize the command with moments 1 <center of mass>
+
+        cmd_to_run = f"{GREEDY_PATH} -d 3 -i " \
+                     fr"{self.fixed_img} {self.moving_img} " \
+                     f"{combined_mask_cmd} -moments 1 -o " \
+                     fr"{self.transform_files['moments']} "
+
+        subprocess.run(cmd_to_run, shell=True, capture_output=True)
+
         cmd_to_run = f"{GREEDY_PATH} -d 3 -a -i " \
                      fr"{self.fixed_img} {self.moving_img} " \
-                     f"{combined_mask_cmd} -ia-image-centers -dof 12 -o " \
+                     f"{combined_mask_cmd} -ia {self.transform_files['moments']} -dof 12 -o " \
                      fr"{self.transform_files['affine']} " \
                      f"-n {self.multi_resolution_iterations} -m SSD"
-
         subprocess.run(cmd_to_run, shell=True, capture_output=True)
+
         logging.info(
             f"Affine alignment: {pathlib.Path(self.moving_img).name} -> {pathlib.Path(self.fixed_img).name} |"
             f" Aligned image: moco-{pathlib.Path(self.moving_img).name} | Transform file: {pathlib.Path(self.transform_files['affine']).name}")
         return self.transform_files['affine']
 
     def deformable(self) -> tuple:
         """
```

### Comparing `pumaz-1.4/pumaz/input_validation.py` & `pumaz-1.5/pumaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz/pumaz.py` & `pumaz-1.5/pumaz/pumaz.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
 
     # ----------------------------------
     # DISPLAYING INPUT CHOICES
     # ----------------------------------
     console.print(f' Multiplexing: {multiplex} | '
                   f'Custom Colors: {custom_colors} | '
                   f'Segment Tumors: {segment_tumors} | ',
-                  f'Convert to DICOM: {convert_to_dicom}',
+                  f'Convert to DICOM: {convert_to_dicom} | ',
+                  f'Regions to Ignore: {regions_to_ignore}',
                   style='bold magenta')
 
     # ----------------------------------
     # DOWNLOADING THE BINARIES
     # ----------------------------------
 
     print('')
```

### Comparing `pumaz-1.4/pumaz/resources.py` & `pumaz-1.5/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.4/pumaz.egg-info/PKG-INFO` & `pumaz-1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 1.4
+Version: 1.5
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Classifier: Development Status :: 4 - Beta
@@ -41,144 +41,157 @@
 Requires-Dist: psutil
 Requires-Dist: gputil
 Requires-Dist: dask
 Requires-Dist: lionz
 
 ![Puma-logo](Images/Puma-logo.png)
 
-## PUMA 1.2 🐾 - Agile. Precision-Driven. Empowering 💪
-[![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/)
+## PUMA 1.0 🐾 -  One Image multiple perspectives 🎭
+[![PyPI version](https://img.shields.io/pypi/v/pumaz?color=FF1493&style=flat-square&logo=pypi)](https://pypi.org/project/pumaz/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-red.svg?style=flat-square&logo=gnu&color=FF0000)](https://www.gnu.org/licenses/gpl-3.0) [![Monthly Downloads](https://img.shields.io/pypi/dm/pumaz?label=Downloads%20(Monthly)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) [![Daily Downloads](https://img.shields.io/pypi/dd/pumaz?label=Downloads%20(Daily)&color=9400D3&style=flat-square&logo=python)](https://pypi.org/project/pumaz/) <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
 
-Get ready for a leap in the world of Positron Emission Tomography (PET) imaging: introducing PUMA 1.2 🚀
+**🌈 PET Reimagined: From Monochrome to a Palette of Possibilities with PUMA 1.0**
 
-PUMA 1.2 (PET Universal Multi-tracer Aligner) has been crafted with a strong focus on the challenges of clinical PET imaging.
+Step into the vibrant new world of PET imaging with PUMA 1.0 🌟, where traditional monochrome scans are transformed into a dynamic spectrum of diagnostic data. 🎨
 
-⚡ It's Agile: PUMA operates across all operating systems and architectures, from x86 to ARM64 (Apple Silicon). It has no specific hardware needs, and with the requirement for Python 3.9 or above, PUMA 1.2 is ready to perform anywhere, anytime.
+With PUMA 1.0, experience the power of multiplexing: a process that fuses multiple tracer images into a single, multicolored composite that reveals not just the presence of disease but its multifaceted physiological context. 🔄 The multiplexed approach provides a more comprehensive view, helping clinicians uncover nuanced insights about tumors and their microenvironments. 🔍
 
-🔍 It's Precision-Driven yet blazingly fast: Built upon the bedrock of nnUNet based MOOSE and advanced diffeomorphic registration techniques from the awesome 'greedy' library, PUMA 1.2 aligns multiplexed tracer images with high precision in less than a heartbeat, clocking in at under one minute, offering unrivaled clarity and accuracy in the diagnosis of patient pathology.
+Whether you're in a high-tech lab or a remote clinic, PUMA 1.0 delivers high-quality, multiplexed PET scans that are as rich in detail as they are in color. 🏥 It’s not just an upgrade—it’s a whole new way of seeing PET data, turning every image into a detailed map of insight and opportunity. 🗺️
 
-🗝️ It's Empowering: PUMA 1.2 enhances diagnostic capabilities with its multiplexed viewing angles, unlocking a new realm of diagnostic possibilities and empowering clinicians.
+## 🎉 Key Features
 
-Join us on this revolutionary journey with PUMA 1.2.
+### 🚀 Versatile and Powerful
+Run PUMA 1.0 on any device, any OS, from x86 to ARM64 (hello, Apple Silicon fans!). Whether you’re on a high-end GPU or a humble CPU, PUMA adapts to your needs without breaking a sweat.
+
+### 🔍 Precision Meets Speed
+Harness the power of AI with MOOSE-driven segmentations and ‘greedy’ library’s wizardry for diffeomorphic image registration. PUMA 1.0 nails the perfect balance of sharp accuracy and zippy performance.
+
+### 🎨 Art of Imaging
+Why settle for ordinary when you can visualize in vibrant RGB? Each color shines a spotlight on a different tracer, turning complex data into a vivid, easy-to-interpret display. With processing times ranging from just 5 to 12 minutes, you're all set for a speedy yet thorough diagnostic journey.
 
 ## 🚀 PUMA's multiplexing in action
 
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
   <img alt="Shows an illustrated MOOSE story board adopted to different themes" src="https://github.com/Keyn34/PUMA/blob/master/Images/PUMA-Flex.gif">
 </picture>
 </div>
 
 ## Requirements ✅
 
-Before stepping into the future with PUMA 1.2, here's what you need for an optimal experience:
+Before stepping into the future with PUMA 1.0, here's what you need for an optimal experience:
 
-- **Operating System**: Windows, Mac, or Linux - PUMA 1.2 is versatile and works across all these platforms.
+- **Operating System**: Windows, Mac, or Linux - PUMA 1.0 is versatile and works across all these platforms.
 
 - **Memory**: Make sure your system has enough memory (8-16 GB) to run the tasks smoothly.
 
 - **GPU**: You need a cuda enabled GPU (NVIDIA), 8 GB or more!
 
-- **Python**: PUMA 1.2 operates with Python 3.10, staying in line with the latest updates.
+- **Python**: PUMA 1.0 operates with Python 3.10, staying in line with the latest updates.
 
-Once these specifications are met, you're all set to experience PUMA 1.2's capabilities.
+Once these specifications are met, you're all set to experience PUMA 1.0's capabilities.
 
 ## Installation Guide 🛠️
 
-Installation is a breeze on Windows, Linux, and MacOS. Follow the steps below to start your journey with PUMA 1.2.
+Installation is a breeze on Windows, Linux, and MacOS. Follow the steps below to start your journey with PUMA 1.0.
 
 ### For Linux and MacOS 🐧🍏
 
 1. Create a Python environment named 'puma-env' or as per your preference.
    ```bash
    python3 -m venv puma-env
    ```
 
 2. Activate the environment.
    ```bash
    source puma-env/bin/activate  # for Linux
    source puma-env/bin/activate  # for MacOS
    ```
 
-3. Install PUMA 1.2.
+3. Install PUMA 1.0.
    ```bash
    pip install pumaz
    ```
 
-Congratulations! You're all set to start using PUMA 1.2.
+Congratulations! You're all set to start using PUMA 1.0.
 
 ### For Windows 🪟
 
 1. Create a Python environment, e.g., 'puma-env'.
    ```bash
    python -m venv puma-env
    ```
 
 2. Activate the environment.
    ```bash
    .\puma-env\Scripts\activate
    ```
 
-3. Install PUMA 1.2.
+3. Install PUMA 1.0.
    ```bash
    pip install pumaz
    ```
 
-You're now ready to experience the precision and speed of PUMA 1.2.
+You're now ready to experience the precision and speed of PUMA 1.0.
 
 ## Usage Guide 📚
 
-Start your journey with PUMA 1.2 by using our straightforward command-line tool. It requires the directory path containing different tracer images, and each image should be stored in separate folders. Here's how you can get started:
+Start your journey with PUMA 1.0 by using our straightforward command-line tool. It requires the directory path containing different tracer images, and each image should be stored in separate folders. Here's how you can get started:
 
 ```bash
 
    pumaz \
        -d <path_to_image_dir>              # Directory path containing the images to be analyzed
        -ir <regions_to_ignore>             # Regions to ignore: arms, legs, head, none
        -m                                  # Optional: Enable multiplexed RGB image output
        -cs <color_selection>               # Optional: Custom color selection for RGB output (requires -m)
+       -c2d <convert_back_to_dicom>        # Optional: Once set, the generated nifti images will be converted back to DICOM
 ```
 
 - `<path_to_image_dir>` refers to the parent directory containing different tracer images in their respective sub-directories.
 
 - `-ir` specifies the regions to be ignored during registration. If you don't want to ignore any regions, use `none`. If you want to ignore the arms, legs, or head during registration, pass the corresponding regions delimited by a `,`. For example: `-ir head,arms` to ignore the head and arms.
 
 - `-m` will activate the output of a multiplexed RGB image of the combined tracer images.
 
-- `-cs`, when passed along with `-m`, PUMA will ask you to provide a custom order of color channels for the corresponding tracer images. That way, you can freely decide which tracer image is associated with which channel. 
+- `-cs`, when passed along with `-m`, PUMA will ask you to provide a custom order of color channels for the corresponding tracer images. That way, you can freely decide which tracer image is associated with which channel.
+- `-c2d`, when set the generated aligned nifti images will be converted back to DICOM.
+  
 For assistance or additional information, you can always type:
 
 ```bash
 pumaz -h
 ```
+
 ### Example usage:
 Apply PUMA to images in a directory, ignoring arms and legs, with multiplexed RGB output and custom colors:
 
 ```bash
-    pumaz -d /path/to/images -ir arms,legs -m -cs 
+    pumaz -d /path/to/images -ir arms,legs -m -cs -c2d 
 ```
 
 ## Directory Structure and Naming Conventions for PUMA 📂🏷️
 
-PUMA 1.2 requires your data to be structured in a certain way. It supports DICOM directories and NIFTI files. For NIFTI files, users need to ensure that the files are named with the correct modality tag at the start.
+PUMA 1.0 requires your data to be structured in a certain way. It supports DICOM directories and NIFTI files. For NIFTI files, users need to ensure that the files are named with the correct modality tag at the start.
 
 ### Required Directory Structure 🌳
 
-Here is the directory structure that PUMA 1.2 expects:
+Here is the directory structure that PUMA 1.0 expects:
 
 ```
 Parent_Directory
 │
-└───Tracer1
+└───Tracer1 # can be named anything
 │   │
-│   └───PET_DICOM_Directory or PT_xxxx.nii.gz
+│   └───PET_DICOM_Directory or PT_xxxx.nii.gz # If it's DICOM, the folder name can be anything, but if nifti use a prefix 'PT' for PET
 │   │
-│   └───CT_DICOM_Directory or CT_xxxx.nii.gz
+│   └───CT_DICOM_Directory or CT_xxxx.nii.gz # If it's DICOM, the folder name can be anything, but if nifti use a prefix 'CT' for CT
 │
 └───Tracer2
 │   │
 │   └───PET_DICOM_Directory or PT_xxxx.nii.gz
 │   │
 │   └───CT_DICOM_Directory or CT_xxxx.nii.gz
 ...
@@ -209,7 +222,29 @@
 
 Our PUMA package, for example, is named as 'pumaz', pronounced "puma-see". So, why 'Z'?
 
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
  
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/W7ebere"><img src="https://avatars.githubusercontent.com/u/166598214?v=4?s=100" width="100px;" alt="W7ebere"/><br /><sub><b>W7ebere</b></sub></a><br /><a href="https://github.com/LalithShiyam/PUMA/commits?author=W7ebere" title="Documentation">📖</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `pumaz-1.4/setup.py` & `pumaz-1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pumaz',
-    version='1.4',
+    version='1.5',
     author='Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, '
                  'Manuel.pires@meduniwien.ac.at',
     description='PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from '
                 'different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision '
                 'alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and '
                 'reproducibility of PET image studies.',
```

