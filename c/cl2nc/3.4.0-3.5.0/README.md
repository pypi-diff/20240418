# Comparing `tmp/cl2nc-3.4.0.tar.gz` & `tmp/cl2nc-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cl2nc-3.4.0.tar", last modified: Fri Mar 10 18:12:26 2023, max compression
+gzip compressed data, was "cl2nc-3.5.0.tar", last modified: Thu Apr 18 14:39:43 2024, max compression
```

## Comparing `cl2nc-3.4.0.tar` & `cl2nc-3.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-10 18:12:26.120416 cl2nc-3.4.0/
--rw-r--r--   0 peter     (1000) peter     (1000)       41 2023-03-10 18:10:58.000000 cl2nc-3.4.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)      715 2023-03-10 18:12:26.120416 cl2nc-3.4.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)    12718 2023-03-10 18:10:58.000000 cl2nc-3.4.0/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)     1060 2023-03-10 18:10:58.000000 cl2nc-3.4.0/cl2nc.1
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-03-10 18:12:26.120416 cl2nc-3.4.0/cl2nc.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      715 2023-03-10 18:12:25.000000 cl2nc-3.4.0/cl2nc.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      233 2023-03-10 18:12:26.000000 cl2nc-3.4.0/cl2nc.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-03-10 18:12:25.000000 cl2nc-3.4.0/cl2nc.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-03-10 18:12:25.000000 cl2nc-3.4.0/cl2nc.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       15 2023-03-10 18:12:25.000000 cl2nc-3.4.0/cl2nc.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        6 2023-03-10 18:12:25.000000 cl2nc-3.4.0/cl2nc.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)    21570 2023-03-10 18:10:58.000000 cl2nc-3.4.0/cl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)       79 2023-03-10 18:12:26.120416 cl2nc-3.4.0/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2023-03-10 18:10:58.000000 cl2nc-3.4.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 14:39:43.706040 cl2nc-3.5.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1074 2024-04-18 14:35:58.000000 cl2nc-3.5.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)       41 2024-04-18 14:35:58.000000 cl2nc-3.5.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)      662 2024-04-18 14:39:43.706040 cl2nc-3.5.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)    13768 2024-04-18 14:35:58.000000 cl2nc-3.5.0/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     1137 2024-04-18 14:35:58.000000 cl2nc-3.5.0/cl2nc.1
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 14:39:43.706040 cl2nc-3.5.0/cl2nc.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      662 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      244 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       37 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       21 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        6 2024-04-18 14:39:43.000000 cl2nc-3.5.0/cl2nc.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    24660 2024-04-18 14:35:58.000000 cl2nc-3.5.0/cl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       79 2024-04-18 14:39:43.706040 cl2nc-3.5.0/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      995 2024-04-18 14:35:58.000000 cl2nc-3.5.0/setup.py
```

### Comparing `cl2nc-3.4.0/PKG-INFO` & `cl2nc-3.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cl2nc
-Version: 3.4.0
-Summary: Convert Vaisala CL51 and CL31 dat files to NetCDF
+Version: 3.5.0
+Summary: Convert Vaisala CL51 and CL31 DAT and HIS L2 files to NetCDF
 Home-page: https://github.com/peterkuma/cl2nc
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
-Description: UNKNOWN
 Keywords: vaisala,ceilometer,cl51,cl31,netcdf,lidar
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+License-File: LICENSE.md
```

### Comparing `cl2nc-3.4.0/README.md` & `cl2nc-3.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,152 @@
 # cl2nc
 
 cl2nc is an open source command line Python program for converting Vaisala
-CL51 and CL31 ceilometer dat files to NetCDF.
+CL51 and CL31 ceilometer DAT and HIS L2 files to NetCDF.
 
 ## Example
 
 On the command-line:
 
 ```sh
 cl2nc input.dat output.nc
 ```
 
-where `input.dat` is a Vaisala CL51 or CL31 dat file and `output.nc` is the name
+where `input.dat` is a Vaisala CL51 or CL31 DAT file and `output.nc` is the name
 of a NetCDF output file.
 
 See [example.zip](example.zip) for an example input and output.
 
 ## Installation
 
-Supported operating systems:
+It is recommended to run cl2nc on Linux.
 
-- Linux
-- Windows
-- macOS
+### Linux
 
-Requirements:
+On Debian-derived distributions (Ubuntu, Devuan, ...), install the required
+system packages with:
 
-- Python 2.7 or Python 3
+```sh
+sudo apt install python3 python3-pip pipx
+```
 
-On Windows and macOS [Anaconda](https://www.anaconda.com/download/)
-distribution of Python is recommended. On Linux, use Python
-which comes with your Linux distribution (either built-in, or installed through
-a package manager).
+On Fedora, install the required system packages with:
 
-The following commands should be run in the **Terminal** (Linux and macOS)
-or **Anaconda Prompt** (Windows – you can find Anaconda Prompt in the
-Start menu). To install with Python 3 instead of Python 2, replace `pip` with
-`pip3` and `python` with `python3` in the commands below.
+```sh
+sudo yum install python3 pipx
+```
 
-To install from the
-[Python Package Index (PyPI)](https://pypi.python.org/pypi/cl2nc):
+Install cl2nc:
 
 ```sh
-pip install cl2nc
+pipx install cl2nc
+mkdir -p ~/.local/share/man/man1
+ln -s ~/.local/pipx/venvs/cl2nc/share/man/man1/cl2nc.1 ~/.local/share/man/man1/
 ```
 
-or to install in the user's home directory
-(make sure `~/.local/bin` is in the `PATH` environment variable):
+Make sure that `$HOME/.local/bin` is included in the `PATH` environment
+variable if not already. This can be done with `pipx ensurepath`.
+
+You should now be able to run `cl2nc` and see the manual page with `man cl2nc`.
+
+To uninstall:
 
 ```sh
-pip install cl2nc --user
+pipx uninstall cl2nc
+rm ~/.local/share/man/man1/cl2nc.1
 ```
 
-Alternatively, to install from source, download and unpack the latest
-[cl2nc](https://github.com/peterkuma/cl2nc/archive/master.zip) archive, or
-clone the repository from GitHub
-(`git clone https://github.com/peterkuma/cl2nc.git`). In the package
-directory, run the following commands:
+### macOS
+
+Open the Terminal. Install cl2nc with:
 
 ```sh
-pip install netCDF4
-python setup.py install
+python3 -m pip install cl2nc
+```
 
-# or to install in the user's home directory
-# (make sure `~/.local/bin` is in the `PATH` environment variable):
+Make sure that `/Users/<user>/Library/Python/<version>/bin` is included in the
+`PATH` environment variable if not already, where `<user>` is your system
+user name and `<version>` is the Python version. This path should be printed
+by the above command. This can be done by adding this line to the file
+`.zprofile` in your home directory and restart the Terminal:
 
-python setup.py install --user
+```sh
+PATH="$PATH:/Users/<user>/Library/Python/<version>/bin"
 ```
 
-You can also use the Python script `cl2nc` directly without installation
-(as long as netCDF4 is installed).
+You should now be able to run `cl2nc` and see the manual page with `man cl2nc`.
 
-Once installed, you should be able to run `cl2nc` in the Terminal
-(Linux and macOS) or Anaconda Prompt (Windows).
+To uninstall:
 
-## Usage
+```sh
+python3 -m pip uninstall cl2nc
+```
+
+### Windows
+
+Install [Python 3](https://www.python.org). In the installer, tick `Add
+python.exe to PATH`.
+
+Open Command Prompt from the Start menu. Install cl2nc with:
+
+```sh
+pip install cl2nc
+```
+
+You should now be able to run `cl2nc`.
+
+To uninstall:
 
 ```sh
-cl2nc [-chq] [--debug] [--help] <input> <output>
+pip uninstall cl2nc
 ```
 
-`<input>` is an input `.dat` file. `<output>` is an output `.nc` file.
-If directories are supplied for `<input>` and `<output>`, all `.dat` and `.DAT`
-files in `<input>` are converted to `.nc` files in `<output>`.
+## Usage
+
+cl2nc is a command line program to be run a terminal (Linux and macOS) or the
+Command Prompt (Windows).
+
+Synopsis:
+
+`cl2nc` [`-chq`] [`--debug`] *input* *output* \
+`cl2nc` `-h`|`--help`
+
+*input* is an input `.dat` or `.his` (L2) file. *output* is an output `.nc` file.
+If directories are supplied for *input* and *output*, all `.dat`, `.DAT`, `.his`
+and `.HIS` files in *input* are converted to `.nc` files in *output*.
 
 Options:
 
-- `-c`: Enable checksum verification (slow).
+- `-c`: Enable DAT checksum verification (slow).
 - `--debug`: Enable debugging output.
 - `-h`, `--help`: Show help message and exit.
 - `-q`: Run quietly (suppress output).
 
-A manual page is also available if cl2nc is installed on unix-like operating
-systems:
+On Linux and macOS, see also the manual page with:
 
 ```sh
 man cl2nc
 ```
 
 ## Variables
 
 Please see Vaisala CL51 User's Guide for a complete description of the
 variables.
 
 The DAT files can alternatively contain values in feet
 (instead of meters), in which case all values are converted by cl2nc to meters.
 
-Time in DAT files is assumed to be UTC.
+Time in DAT and HIS files is assumed to be UTC.
 
 Missing values are encoded as NaN (floating-point variables) or -2147483648
 (integer variables). The `_FillValue` attribute contains the missing value
 used in the given variable.
 
+DAT files produce the following NetCDF output:
+
 | Variable | Description | Units | Dimensions |
 | --- | --- | --- | --- |
 | [background_light](#background_light) | Background light | mV | time |
 | [backscatter](#backscatter) | Attenuated volume backscatter coefficient | km<sup>-1</sup>.sr<sup>-1</sup> | time, level |
 | [backscatter_sum](#backscatter_sum) | Backscatter sum | sr<sup>-1</sup> | time |
 | [cbh_1](#cbh_1) | Lowest cloud base height | m | time |
 | [cbh_2](#cbh_2) | Second lowest cloud base height | m | time |
@@ -144,14 +175,25 @@
 | [time](#time) | Time | seconds since 1970-01-01 00:00:00 UTC | time |
 | [time_utc](#time_utc) | Time (UTC) | ISO 8601 | time |
 | [unit](#unit) | Unit identification character | | time |
 | [vertical_resolution](#vertical_resolution) | Vertical resolution | m | time |
 | [vertical_visibility](#vertical_visibility) | Vertical visibility | m | time |
 | [window_transmission](#window_transmission) | Window transmission estimate | % | time |
 
+HIS L2 files produce the following NetCDF output:
+
+| Variable | Description | Units | Dimensions |
+| --- | --- | --- | --- |
+| [backscatter](#backscatter) | Attenuated volume backscatter coefficient | km<sup>-1</sup>.sr<sup>-1</sup> | time, level |
+| [ceilometer](#ceilometer) | Ceilometer name | | time |
+| [level](#level) | Level number | | level |
+| [period](#period) | Period | | time |
+| [time](#time) | Time | seconds since 1970-01-01 00:00:00 UTC | time |
+| [time_utc](#time_utc) | Time (UTC) | ISO 8601 | time |
+
 ### background_light
 
 Background light (mV)
 
 Millivolts at internal ADC input.
 
 ### backscatter
@@ -172,14 +214,18 @@
 
 Second lowest cloud base height (m)
 
 ### cbh_3
 
 Highest cloud base height (m)
 
+### ceilometer
+
+Ceilometer name (HIS L2 variable `CEILOMETER`).
+
 ### detection_status
 
 Detection status
 
 - `0` – no significant backscatter
 - `1` – one cloud base detected
 - `2` – two cloud bases detected
@@ -235,14 +281,18 @@
 ### message_subclass
 
 Message subclass
 
 - 6 – 10 m ⨉ 1540 samples, range 15400 m (msg1_10x1540)
 - 8 – without a backscatter profile (msg1_base)
 
+### period
+
+Period (HIS L2 variable `PERIOD`).
+
 ### pulse_energy
 
 Pulse energy (% of nominal factory setting)
 
 ### pulse_length
 
 Pulse length
@@ -416,14 +466,18 @@
 variables. You can use the `time` variable instead or use the MATLAB HDF
 functions to read the file (you may need to change the file extension to `.h5`).
 
 ## Changelog
 
 cl2nc follows [semantic versioning](http://semver.org/).
 
+### 3.5.0 (2024-04-18)
+
+- Added support for the HIS L2 format.
+
 ### 3.4.0 (2023-03-10)
 
 - Added support for a CL51 format as in R/V Polarstern data.
 
 ### 3.3.2 (2023-02-26)
 
 - Issue a warning when no output was created because an input file is empty.
@@ -482,9 +536,10 @@
 - Format time with `T` as delimiter to conform to ISO 8601.
 - Improved error handling.
 
 ## See also
 
 [ALCF](https://alcf-lidar.github.io),
 [ccplot](https://ccplot.org),
+[ccbrowse](https://github.com/peterkuma/ccbrowse),
 [mpl2nc](https://github.com/peterkuma/mpl2nc),
 [mrr2c](https://github.com/peterkuma/mrr2c)
```

### Comparing `cl2nc-3.4.0/cl2nc.1` & `cl2nc-3.5.0/cl2nc.1`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-.TH cl2nc "3.2.1" 08/02/2020
+.TH cl2nc "3.5.0" 04/18/2024
 
 .SH NAME
-cl2nc \- convert Vaisala CL51 and CL31 dat files to NetCDF
+cl2nc \- convert Vaisala CL51 and CL31 DAT and HIS L2 files to NetCDF
 
 .SH SYNOPSIS
 .B cl2nc
 .RB [ -chq ]
 .RB [ --debug ]
 .RB [ --help ]
 .I input
 .I output
 
 .SH DESCRIPTION
 
 .IR input
 is an input
 .I .dat
-file.
+or
+.I .his
+(L2) file.
 .IR output
 is an output
 .I .nc
 file.
 If directories are supplied for
 .I input
 and
 .IR output ,
 all
-.IR ".dat " "and " .DAT
+.IR .dat ,
+.IR .DAT ,
+.I .his
+and
+.I .HIS
 files in
 .I input
 are converted to
 .I .nc
 files in
 .IR output .
 
 .SH OPTIONS
 
 .TP
-.B -c 
-Enable checksum verification (slow).
+.B -c
+Enable DAT checksum verification (slow).
 .TP
 .B --debug
 Enable debugging output.
 .TP
 .TP
 .BR -h , " --help"
 Show help message and exit.
@@ -51,29 +57,32 @@
 Run quietly (suppress output).
 
 .SH EXAMPLES
 
 .B cl2nc input.dat outout.nc
 
 Convert
-.I input.dat 
+.I input.dat
 to
 .IR output.nc .
 
 .B cl2nc in out
 
 Convert dat files in the directory
 .I in
 to NetCDF files in the directory
 .IR out .
 
 .SH COPYRIGHT
 
-Copyright (C) 2018-2020 Peter Kuma.
+Copyright (C) 2018-2024 Peter Kuma.
 .PP
 This program is available under the terms of an MIT license (see LICENSE.md in the distribution).
 
 .SH SEE ALSO
 
-See <https://github.com/peterkuma/cl2nc>
+See
+.UR https://github.com/peterkuma/cl2nc
+cl2nc GitHub repository
+.UE
 for more information about
 .BR cl2nc .
```

### Comparing `cl2nc-3.4.0/cl2nc.egg-info/PKG-INFO` & `cl2nc-3.5.0/cl2nc.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cl2nc
-Version: 3.4.0
-Summary: Convert Vaisala CL51 and CL31 dat files to NetCDF
+Version: 3.5.0
+Summary: Convert Vaisala CL51 and CL31 DAT and HIS L2 files to NetCDF
 Home-page: https://github.com/peterkuma/cl2nc
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
-Description: UNKNOWN
 Keywords: vaisala,ceilometer,cl51,cl31,netcdf,lidar
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+License-File: LICENSE.md
```

### Comparing `cl2nc-3.4.0/cl2nc.py` & `cl2nc-3.5.0/cl2nc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
-__version__ = '3.4.0'
+__version__ = '3.5.0'
 
 import sys
 import signal
 signal.signal(signal.SIGINT, lambda signal, frame: sys.exit(0))
 import logging
 logging.basicConfig(format='%(name)s: %(message)s')
 log = logging.getLogger(sys.argv[0])
@@ -37,14 +37,16 @@
 re_line2 = re.compile(b'^(?P<detection_status>.)(?P<self_check>.) (?P<cbh_or_vertical_visibility>.{5}) (?P<cbh2_or_highest_signal>.{5}) (?P<cbh_3>.{5}) (?P<status_alarm>.{4})(?P<status_warning>.{4})(?P<status_internal>.{4})$')
 re_line3 = re.compile(b'^ (?P<sky_detection_status>..) +(?P<layer1_height>.{4}) +(?P<layer2_cloud_amount>.) +(?P<layer2_height>.{4}) +(?P<layer3_cloud_amount>.) +(?P<layer3_height>.{4}) +(?P<layer4_cloud_amount>.) +(?P<layer4_height>.{4}) +(?P<layer5_cloud_amount>.) +(?P<layer5_height>.{3,4})$')
 re_line4 = re.compile(b'^(?P<scale>.{5}) (?P<vertical_resolution>..) (?P<nsamples>.{4}) (?P<pulse_energy>...) (?P<laser_temperature>...) (?P<window_transmission>...) (?P<tilt_angle>..) (?P<background_light>.{4}) (?P<pulse_length>.)(?P<pulse_count>.{4})(?P<receiver_gain>.)(?P<receiver_bandwidth>.)(?P<sampling>..) (?P<backscatter_sum>...)$')
 re_line5 = re.compile(b'^(?P<backscatter>.*)$')
 re_line6 = re.compile(b'^\x03(?P<checksum>.{4})\x04$')
 re_none = re.compile(b'^/* *$')
 
+re_his_time = re.compile(b'^(?P<year>\d{4})-(?P<month>\d\d)-(?P<day>\d\d) (?P<hour>\d\d):(?P<minute>\d\d):(?P<second>\d\d)$')
+
 def fsencode(x):
     return os.fsencode(x) if sys.version_info[0] > 2 else x
 
 def fsdecode(x):
     return os.fsdecode(x) if sys.version_info[0] > 2 else x
 
 def is_none(s):
@@ -231,21 +233,27 @@
 
 def postprocess(d):
     for var in [
         'backscatter',
         'scale',
         'backscatter_sum',
     ]:
-        d[var] = int_to_float(d[var])
+        if var in d: d[var] = int_to_float(d[var])
+
+    d['scale'] = d.get('scale', 10)
 
-    d['backscatter'] = d['backscatter']/100000.0*(d['scale']/100.0)
-    d['backscatter_sum'] = d['backscatter_sum']/10000.0*(d['scale']/100.0)
+    if 'backscatter' in d:
+        d['backscatter'] = d['backscatter']/100000.0*(d['scale']/100.0)
 
-    d['units'] = 'm' if (d['status_internal'] & 0x0080) else 'ft'
-    layer_height_factor = 100 if d['units'] == 'ft' else 10
+    if 'backscatter_sum' in d:
+        d['backscatter_sum'] = d['backscatter_sum']/10000.0*(d['scale']/100.0)
+
+    if 'status_internal' in d:
+        d['units'] = 'm' if (d['status_internal'] & 0x0080) else 'ft'
+        layer_height_factor = 100 if d['units'] == 'ft' else 10
 
     if 'layer1_height' in d:
         d['layer_height'] = NA_INT32*np.ones(5)
         for i in range(5):
             d['layer_height'][i] = d['layer%d_height' % (i + 1)]
         d['layer_height'] = np.where(
             d['layer_height'] != NA_INT32,
@@ -254,52 +262,54 @@
         )
 
     if 'layer1_cloud_amount' in d:
         d['layer_cloud_amount'] = NA_INT32*np.ones(5)
         for i in range(5):
             d['layer_cloud_amount'][i] = d['layer%d_cloud_amount' % (i + 1)]
 
-    if d['units'] == 'ft':
+    if 'units' in d and d['units'] == 'ft':
         for var in [
             'vertical_visibility',
             'layer_height',
             'cbh_1',
             'cbh_2',
             'cbh_3',
         ]:
             if var in d:
                 d[var] = np.where(
                     d[var] != NA_INT32,
                     d[var]*0.3048,
                     NA_INT32
                 )
 
-    d['pulse_count'] = np.where(
-        d['pulse_count'] != NA_INT32,
-        d['pulse_count']*1024,
-        NA_INT32
-    )
+    if 'pulse_count' in d:
+        d['pulse_count'] = np.where(
+            d['pulse_count'] != NA_INT32,
+            d['pulse_count']*1024,
+            NA_INT32
+        )
 
     d['time_utc'] = d.get('time_utc', '')
-    d['time'] = NA_INT64 if d['time_utc'] == '' else (
-        dt.datetime.strptime(d['time_utc'].decode('ascii'), '%Y-%m-%dT%H:%M:%S')
-        - dt.datetime(1970, 1, 1)
-    ).total_seconds()
+    if 'time_utc' in d:
+        d['time'] = NA_INT64 if d['time_utc'] == '' else (
+            dt.datetime.strptime(d['time_utc'].decode('ascii'), '%Y-%m-%dT%H:%M:%S')
+            - dt.datetime(1970, 1, 1)
+        ).total_seconds()
 
 def crc16(buf):
     crc = 0xffff
     for i in range(len(buf)):
         crc = crc^(ord(buf[i:(i+1)]) << 8) & 0xffff
         for j in range(8):
             xmask = 0x1021 if (crc & 0x8000) else 0
             crc = (crc<<1) & 0xffff
             crc = (crc^xmask) & 0xffff
     return crc^0xffff;
 
-def read_input(filename, options={}):
+def read_dat(filename, options={}):
     options = dict({
         'check': False,
     }, **options)
 
     with open(filename, 'rb') as f:
         d = {}
         dd = []
@@ -387,33 +397,111 @@
                         line_number, e
                     ))
                     log.debug(traceback.format_exc())
                     stage = 0
                 break
         return dd
 
+def read_his_time(s):
+    m = re_his_time.match(s)
+    if m is not None:
+        g = m.groupdict()
+        return b'%s-%s-%sT%s:%s:%s' % (
+            g['year'],
+            g['month'],
+            g['day'],
+            g['hour'],
+            g['minute'],
+            g['second']
+        )
+    else:
+        raise ValueError('Invalid syntax for CREATEDATE field')
+
+def read_his_period(s):
+    try:
+        return int(s)
+    except ValueError:
+        raise ValueError('Invalid syntax for PERIOD field')
+
+def read_his_backscatter(s):
+    d2 = {}
+    d = {'backscatter': s}
+    read_hex_array(d, d2, 'backscatter', 5)
+    return d2['backscatter']
+
+def read_his(filename, options={}):
+    with open(filename, 'rb') as f:
+        dd = []
+        line_number = 0
+        header = None
+        for line in f.readlines():
+            line_number += 1
+            try:
+                d = {}
+                items = line.split(b',')
+                items = [x.strip() for x in items]
+                if items[0] == b'History file':
+                    continue
+                if header is None:
+                    header = items
+                    continue
+                for i, h in enumerate(header):
+                    s = items[i] if i < len(items) else b''
+                    if h == b'CREATEDATE':
+                        d['time_utc'] = read_his_time(s)
+                    elif h == b'CEILOMETER':
+                        d['ceilometer'] = s
+                    elif h == b'PERIOD':
+                        d['period'] = read_his_period(s)
+                    elif h == b'BS_PROFILE':
+                        d['backscatter'] = read_his_backscatter(s)
+                postprocess(d)
+                dd += [d]
+            except Exception as e:
+                t, v, tb = sys.exc_info()
+                log.warning('Error on line %d: %s' % (
+                    line_number, e
+                ))
+                log.debug(traceback.format_exc())
+    return dd
+
+def read(filename, options={}):
+    filename_lower = filename.lower()
+    if filename_lower.endswith(b'.his'):
+        return read_his(filename, options)
+    else:
+        return read_dat(filename, options)
+
 def write_output(dd, filename):
     n = len(dd)
     vars = list(set(itertools.chain(*[list(d.keys()) for d in dd])))
-    m = np.max([0] + [len(d['backscatter']) for d in dd])
 
     if os.path.dirname(filename) != b'' and \
         not os.path.exists(os.path.dirname(filename)):
         raise Exception('%s: No such file or directory' % fsdecode(filename))
 
     f = Dataset(fsdecode(filename), 'w', format='NETCDF4')
     f.createDimension('time', n)
-    f.createDimension('level', m)
-    f.createDimension('layer', 5)
-    level = np.arange(m)
-    layer = np.arange(5)
+
+    if 'backscatter' in vars:
+        m = np.max([0] + [len(d['backscatter']) for d in dd])
+        f.createDimension('level', m)
+        level = np.arange(m)
+
+    has_layers = 'layer_height' in vars or 'layer_cloud_amount' in vars
+    if has_layers:
+        f.createDimension('layer', 5)
+        layer = np.arange(5)
 
     def write_var(var, dtype, attributes={}):
         if not var in vars: return
         fill_value = NA_NETCDF.get(dtype)
+        if dtype == 'SX':
+            slen = max([len(d[var]) for d in dd])
+            dtype = 'S%d' % slen
         v = f.createVariable(var, dtype, ('time',), fill_value=fill_value)
         v[:] = np.array([d[var] for d in dd])
         v.setncatts(attributes)
 
     def write_profile(var, dtype, attributes={}):
         if not var in vars: return
         fill_value = NA_NETCDF.get(dtype)
@@ -441,20 +529,22 @@
         'long_name': 'Time (UTC)',
         'units': 'ISO 8601',
     })
     write_var('time', 'i8', {
         'long_name': 'Time',
         'units': 'seconds since 1970-01-01 00:00:00 UTC',
     })
-    write_dim('level', 'i4', level, {
-        'long_name': 'Level number',
-    })
-    write_dim('layer', 'i4', layer, {
-        'long_name': 'Layer number',
-    })
+    if 'backscatter' in vars:
+        write_dim('level', 'i4', level, {
+            'long_name': 'Level number',
+        })
+    if has_layers:
+        write_dim('layer', 'i4', layer, {
+            'long_name': 'Layer number',
+        })
     write_profile('backscatter', 'f4', {
         'long_name': 'Attenuated volume backscatter coefficient',
         'units': 'km^-1.sr^-1',
     })
     write_var('unit', 'S1', {
         'long_name': 'Unit identification character',
     })
@@ -562,14 +652,20 @@
         'flag_meanings': 'narrow wide'
     })
     write_var('backscatter_sum', 'f4', {
         'long_name': 'Backscatter sum',
         'units': 'sr^-1',
         'comment': 'Sum of detected and normalized backscatter',
     })
+    write_var('ceilometer', 'SX', {
+        'long_name': 'Ceilometer name',
+    })
+    write_var('period', 'i4', {
+        'long_name': 'Period',
+    })
     write_layer('layer_height', 'i4', {
         'long_name': 'Layer height',
         'units': 'm',
         'comment': 'Sky condition algorithm',
     })
     write_layer('layer_cloud_amount', 'i4', {
         'long_name': 'Layer cloud amount',
@@ -580,19 +676,19 @@
     f.software = 'cl2nc (https://github.com/peterkuma/cl2nc)'
     f.version = __version__
     f.created = dt.datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
 
     f.close()
 
 def main():
-    parser = argparse.ArgumentParser(description='Convert Vaisala CL51 and CL31 dat files to NetCDF')
+    parser = argparse.ArgumentParser(description='Convert Vaisala CL51 and CL31 DAT and HIS L2 files to NetCDF')
     parser.add_argument('-c',
         dest='check',
         action='store_true',
-        help='enable checksum verification (slow)'
+        help='enable DAT checksum verification (slow)'
     )
     parser.add_argument('-q',
         dest='quiet',
         action='store_true',
         help='run quietly (suppress output)'
     )
     parser.add_argument('--debug',
@@ -608,35 +704,36 @@
         log.setLevel('DEBUG')
 
     input_ = fsencode(args.input)
     output = fsencode(args.output)
 
     if os.path.isdir(input_):
         for file_ in sorted([fsencode(x) for x in os.listdir(input_)]):
-            if not (file_.endswith(b'.dat') or file_.endswith(b'.DAT')):
+            file_lower = file_.lower()
+            if not (file_lower.endswith(b'.dat') or file_lower.endswith(b'.his')):
                 continue
             input_filename = os.path.join(input_, file_)
             output_filename = os.path.join(
                 output,
                 os.path.splitext(file_)[0] + b'.nc'
             )
             if not args.quiet:
                 print(fsdecode(input_filename))
             try:
-                dd = read_input(input_filename, {'check': args.check})
+                dd = read(input_filename, {'check': args.check})
                 if len(dd) > 0:
                     write_output(dd, output_filename)
                 else:
                     log.warning('No output was created because the input file has no records')
             except Exception as e:
                 log.error(e)
                 log.debug(traceback.format_exc())
     else:
         try:
-            dd = read_input(input_, {'check': args.check})
+            dd = read(input_, {'check': args.check})
             if len(dd) > 0:
                 write_output(dd, output)
             else:
                 log.warning('No output was created because the input file has no records')
         except Exception as e:
             log.error(e)
             log.debug(traceback.format_exc())
```

### Comparing `cl2nc-3.4.0/setup.py` & `cl2nc-3.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='cl2nc',
-    version='3.4.0',
-    description='Convert Vaisala CL51 and CL31 dat files to NetCDF',
+    version='3.5.0',
+    description='Convert Vaisala CL51 and CL31 DAT and HIS L2 files to NetCDF',
     author='Peter Kuma',
     author_email='peter@peterkuma.net',
     license='MIT',
     py_modules=['cl2nc'],
     entry_points={
         'console_scripts': ['cl2nc=cl2nc:main'],
     },
     data_files=[('share/man/man1', ['cl2nc.1'])],
-    install_requires=['netCDF4>=1.2.9'],
+    install_requires=[
+        'numpy',
+        'netCDF4>=1.2.9'
+    ],
     keywords=['vaisala', 'ceilometer', 'cl51', 'cl31', 'netcdf', 'lidar'],
     url='https://github.com/peterkuma/cl2nc',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Atmospheric Science',
     ]
 )
```

