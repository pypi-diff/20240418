# Comparing `tmp/canuvit-0.5.0.tar.gz` & `tmp/canuvit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canuvit-0.5.0.tar", last modified: Sun Aug 27 07:47:37 2023, max compression
+gzip compressed data, was "canuvit-0.5.1.tar", last modified: Thu Apr 18 14:18:25 2024, max compression
```

## Comparing `canuvit-0.5.0.tar` & `canuvit-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-08-27 07:47:37.285212 canuvit-0.5.0/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 canuvit-0.5.0/LICENSE
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       34 2021-10-28 10:08:34.000000 canuvit-0.5.0/MANIFEST.in
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     6641 2023-08-27 07:47:37.286212 canuvit-0.5.0/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     6146 2023-03-25 10:28:20.000000 canuvit-0.5.0/README.md
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      104 2021-10-28 07:30:47.000000 canuvit-0.5.0/pyproject.toml
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      811 2023-08-27 07:47:37.286212 canuvit-0.5.0/setup.cfg
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-08-27 07:47:37.273212 canuvit-0.5.0/src/
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-08-27 07:47:37.275212 canuvit-0.5.0/src/canuvit/
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       96 2021-11-01 14:52:27.000000 canuvit-0.5.0/src/canuvit/__init__.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       66 2021-11-01 14:52:27.000000 canuvit-0.5.0/src/canuvit/__main__.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       80 2021-11-01 14:52:27.000000 canuvit-0.5.0/src/canuvit/_canuvit_version.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)    30432 2023-08-27 07:43:53.000000 canuvit-0.5.0/src/canuvit/canuvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     4217 2023-05-20 08:54:42.000000 canuvit-0.5.0/src/canuvit/cli.py
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)  1785600 2018-01-02 07:55:43.000000 canuvit-0.5.0/src/canuvit/td1_catalogue.fits
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-08-27 07:47:37.285212 canuvit-0.5.0/src/canuvit.egg-info/
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     6641 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      419 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/SOURCES.txt
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)        1 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/dependency_links.txt
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       44 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/entry_points.txt
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)       96 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/requires.txt
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)        8 2023-08-27 07:47:37.000000 canuvit-0.5.0/src/canuvit.egg-info/top_level.txt
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-18 14:18:25.717597 canuvit-0.5.1/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 canuvit-0.5.1/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       34 2021-10-28 10:08:34.000000 canuvit-0.5.1/MANIFEST.in
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     7248 2024-04-18 14:18:25.717597 canuvit-0.5.1/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     6552 2024-04-18 14:11:46.000000 canuvit-0.5.1/README.md
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      104 2021-10-28 07:30:47.000000 canuvit-0.5.1/pyproject.toml
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      811 2024-04-18 14:18:25.719597 canuvit-0.5.1/setup.cfg
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-18 14:18:25.621596 canuvit-0.5.1/src/
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-18 14:18:25.624596 canuvit-0.5.1/src/canuvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       96 2021-11-01 14:52:27.000000 canuvit-0.5.1/src/canuvit/__init__.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       66 2021-11-01 14:52:27.000000 canuvit-0.5.1/src/canuvit/__main__.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       80 2021-11-01 14:52:27.000000 canuvit-0.5.1/src/canuvit/_canuvit_version.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)    30471 2024-04-18 13:24:50.000000 canuvit-0.5.1/src/canuvit/canuvit.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     4217 2023-05-20 08:54:42.000000 canuvit-0.5.1/src/canuvit/cli.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)  1785600 2018-01-02 07:55:43.000000 canuvit-0.5.1/src/canuvit/td1_catalogue.fits
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-18 14:18:25.716597 canuvit-0.5.1/src/canuvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     7248 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      419 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       44 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/entry_points.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       96 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        8 2024-04-18 14:18:25.000000 canuvit-0.5.1/src/canuvit.egg-info/top_level.txt
```

### Comparing `canuvit-0.5.0/LICENSE` & `canuvit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canuvit-0.5.0/PKG-INFO` & `canuvit-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: canuvit
-Version: 0.5.0
+Version: 0.5.1
 Summary: UVIT safety checks
 Home-page: https://github.com/prajwel/canuvit
 Author: Prajwel Joseph
 Author-email: prajwel.pj@gmail.com
 Project-URL: Bug Tracker, https://github.com/prajwel/canuvit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2
+Requires-Dist: numpy>=1.13
+Requires-Dist: matplotlib>=2
+Requires-Dist: astropy>=2
+Requires-Dist: beautifulsoup4>=4.4
+Requires-Dist: click>=2
+Requires-Dist: astroquery>=0.4.5
 
 # **CanUVIT**
 > To check whether a field can be safely observed with UVIT.
 
 <p align="center">
 <img src="https://i.imgur.com/b0hoB04.png" width="400"/>
 </p>
@@ -40,24 +47,26 @@
 ```python
 >>> import canuvit
 >>> canuvit.observe('uvit', '12:12:12', '12:12:12')
 ```
 
 > **Note:** In general, `canuvit.observe(instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt', 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in sexagesimal format.
 
+> **IMPORTANT:** Make sure you choose the correct **primary instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+
 For the above example, you should get an output as shown below. Please also check the working directory for the output GALEX images with sources marked in the primary instrument field of view.
 
 ```
-=========================================================
-Payload: uvit, Coordinates: 12:12:12, 12:12:12
-=========================================================
+===================================================================
+Primary instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+===================================================================
 
 ### VIS
 
-sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7  
+sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7
 ----- ---------- ----------- ---- --- -------- ------ ----- ----- ---- ------
     1 12:11:52.8 +12:07:47.5 11.1 0.9       K1 1333.0 124.4  88.6 29.7 1624.9
     2 12:12:22.9 +12:17:23.9 11.1 0.8       K0 1296.7 121.0  86.2 28.9 1580.6
     3 12:11:35.0 +12:12:04.6 11.4 0.5       F5 1457.4 234.9 180.9 32.8 1915.2
     4 12:11:01.7 +12:08:35.9 11.9 0.7       G5  754.3  89.1  69.2 16.8  950.9
     5 12:11:11.5 +12:03:14.0 12.2 0.3       F0  803.1 143.5 101.4 18.2 1061.7
     6 12:12:05.5 +12:19:09.8 12.3 0.8       K0  452.9  42.3  30.1 10.1  552.1
@@ -89,14 +98,16 @@
     5 12:11:35.0 +12:12:04.7 16.5          14.8 23.0 19.6     14.5    5.1
 
 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2', 'Sapphire', 'Silica']
 ```
 
 Please choose the VIS filters such that none of the stars in the field gives >4800 counts/second. Further, for good tracking of the aspect, there should be at least two stars within a 12 arcminute radius of the target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid saturation) in the chosen filter. Please also avoid configuring multiple VIS filters. 
 
+> **Note:** You will receive a warning if there are pairs of stars that are closer than 10 arcseconds in the VIS channel. In such cases, ensure the total count rate from the pairs of stars does not exceed the 4800 counts/seconds limit.
+
 Two additional functions are also available, which takes the same input arguments as `canuvit.observe()`.
 
 * `canuvit.observe_VIS()`: to find safe VIS filters.
 * `canuvit.observe_UV()`: to find safe UV filters.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1 Name: canuvit Version: 0.5.0 Summary: UVIT safety checks
+Metadata-Version: 2.1 Name: canuvit Version: 0.5.1 Summary: UVIT safety checks
 Home-page: https://github.com/prajwel/canuvit Author: Prajwel Joseph Author-
 email: prajwel.pj@gmail.com Project-URL: Bug Tracker, https://github.com/
 prajwel/canuvit/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # **CanUVIT** > To check whether a
-field can be safely observed with UVIT.
+Type: text/markdown License-File: LICENSE Requires-Dist: requests>=2 Requires-
+Dist: numpy>=1.13 Requires-Dist: matplotlib>=2 Requires-Dist: astropy>=2
+Requires-Dist: beautifulsoup4>=4.4 Requires-Dist: click>=2 Requires-Dist:
+astroquery>=0.4.5 # **CanUVIT** > To check whether a field can be safely
+observed with UVIT.
                        [https://i.imgur.com/b0hoB04.png]
 You can install the CanUVIT Python package using the following command. ```bash
 pip install canuvit --upgrade ``` > **IMPORTANT:** Even if you have CanUVIT
 already installed, make sure you use the latest version by running the above
 command. Current version of CanUVIT is shown on the badge below:
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_c_a_n_u_v_i_t_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 > **Note:** If you don't want to install CanUVIT or are facing problems during
@@ -19,52 +22,57 @@
 After installation, you can run CanUVIT on a Python command prompt or as a
 script. For example, if your primary instrument is UVIT and the RA, DEC
 coordinates of the field are (12:12:12, 12:12:12), you may run the CanUVIT
 package as follows. ```python >>> import canuvit >>> canuvit.observe('uvit',
 '12:12:12', '12:12:12') ``` > **Note:** In general, `canuvit.observe
 (instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt',
 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in
-sexagesimal format. For the above example, you should get an output as shown
-below. Please also check the working directory for the output GALEX images with
-sources marked in the primary instrument field of view. ```
-========================================================= Payload: uvit,
-Coordinates: 12:12:12, 12:12:12
-========================================================= ### VIS sl_no ra_hms
-dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- ----------- --
--- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:07:47.5 11.1
-0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1 0.8 K0
-1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5 1457.4 234.9
-180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1 69.2 16.8
-950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2 1061.7 6 12:
-12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe filters:
-['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be absent!
-Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag Mag_corrected
-silica b4 b13 b15 n2 ----- ---------- ----------- ---- ------------- ------ --
-- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1 0.1 2 12:11:
-11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:14:58.3 16.2
-16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6 0.3 0.4 0.1
-0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe filters in
-NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-N2'] ###
-FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica ----- ----
------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:12:32.4
-+12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2 14.6 28.2
-23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4 12:12:
-15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5 14.8
-23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
+sexagesimal format. > **IMPORTANT:** Make sure you choose the correct **primary
+instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+For the above example, you should get an output as shown below. Please also
+check the working directory for the output GALEX images with sources marked in
+the primary instrument field of view. ```
+=================================================================== Primary
+instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+=================================================================== ### VIS
+sl_no ra_hms dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- -
+---------- ---- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:
+07:47.5 11.1 0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1
+0.8 K0 1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5
+1457.4 234.9 180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1
+69.2 16.8 950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2
+1061.7 6 12:12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe
+filters: ['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be
+absent! Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag
+Mag_corrected silica b4 b13 b15 n2 ----- ---------- ----------- ---- ----------
+--- ------ --- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1
+0.1 2 12:11:11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:
+14:58.3 16.2 16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6
+0.3 0.4 0.1 0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe
+filters in NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-
+N2'] ### FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica -
+---- ---------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:
+12:32.4 +12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2
+14.6 28.2 23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4
+12:12:15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5
+14.8 23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
 'Sapphire', 'Silica'] ``` Please choose the VIS filters such that none of the
 stars in the field gives >4800 counts/second. Further, for good tracking of the
 aspect, there should be at least two stars within a 12 arcminute radius of the
 target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid
 saturation) in the chosen filter. Please also avoid configuring multiple VIS
-filters. Two additional functions are also available, which takes the same
-input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find safe
-VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ### Command
-Line Interface After installation with pip, you can also access CanUVIT from
-the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12" -
-d "12:12:12" ``` The help page of the command-line tool can be accessed as
+filters. > **Note:** You will receive a warning if there are pairs of stars
+that are closer than 10 arcseconds in the VIS channel. In such cases, ensure
+the total count rate from the pairs of stars does not exceed the 4800 counts/
+seconds limit. Two additional functions are also available, which takes the
+same input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find
+safe VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ###
+Command Line Interface After installation with pip, you can also access CanUVIT
+from the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12"
+-d "12:12:12" ``` The help page of the command-line tool can be accessed as
 follows: ```bash canuvit -h ``` ``` Usage: canuvit [OPTIONS] Program to check
 if a given coordinate can be safely observed using UVIT. Example usage: canuvit
 -r "13:12:14" -d "-14:15:13" Options: --all Check safety for all filters.
 [default: all] --vis Check saftey for only visible filters. --uv Check safety
 for only UV filters. -r, --ra RA Right ascension of the coordinate. Format: hh:
 mm:ss[.ss] e.g. "00:54:53.45" [required] -d, --dec DEC Declination of the
 coordinate. Format: [-]dd:mm:ss[.ss] e.g. "-37:41:03.23". [required] -i, --
```

### Comparing `canuvit-0.5.0/README.md` & `canuvit-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,26 @@
 ```python
 >>> import canuvit
 >>> canuvit.observe('uvit', '12:12:12', '12:12:12')
 ```
 
 > **Note:** In general, `canuvit.observe(instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt', 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in sexagesimal format.
 
+> **IMPORTANT:** Make sure you choose the correct **primary instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+
 For the above example, you should get an output as shown below. Please also check the working directory for the output GALEX images with sources marked in the primary instrument field of view.
 
 ```
-=========================================================
-Payload: uvit, Coordinates: 12:12:12, 12:12:12
-=========================================================
+===================================================================
+Primary instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+===================================================================
 
 ### VIS
 
-sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7  
+sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7
 ----- ---------- ----------- ---- --- -------- ------ ----- ----- ---- ------
     1 12:11:52.8 +12:07:47.5 11.1 0.9       K1 1333.0 124.4  88.6 29.7 1624.9
     2 12:12:22.9 +12:17:23.9 11.1 0.8       K0 1296.7 121.0  86.2 28.9 1580.6
     3 12:11:35.0 +12:12:04.6 11.4 0.5       F5 1457.4 234.9 180.9 32.8 1915.2
     4 12:11:01.7 +12:08:35.9 11.9 0.7       G5  754.3  89.1  69.2 16.8  950.9
     5 12:11:11.5 +12:03:14.0 12.2 0.3       F0  803.1 143.5 101.4 18.2 1061.7
     6 12:12:05.5 +12:19:09.8 12.3 0.8       K0  452.9  42.3  30.1 10.1  552.1
@@ -74,14 +76,16 @@
     5 12:11:35.0 +12:12:04.7 16.5          14.8 23.0 19.6     14.5    5.1
 
 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2', 'Sapphire', 'Silica']
 ```
 
 Please choose the VIS filters such that none of the stars in the field gives >4800 counts/second. Further, for good tracking of the aspect, there should be at least two stars within a 12 arcminute radius of the target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid saturation) in the chosen filter. Please also avoid configuring multiple VIS filters. 
 
+> **Note:** You will receive a warning if there are pairs of stars that are closer than 10 arcseconds in the VIS channel. In such cases, ensure the total count rate from the pairs of stars does not exceed the 4800 counts/seconds limit.
+
 Two additional functions are also available, which takes the same input arguments as `canuvit.observe()`.
 
 * `canuvit.observe_VIS()`: to find safe VIS filters.
 * `canuvit.observe_UV()`: to find safe UV filters.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -12,52 +12,57 @@
 After installation, you can run CanUVIT on a Python command prompt or as a
 script. For example, if your primary instrument is UVIT and the RA, DEC
 coordinates of the field are (12:12:12, 12:12:12), you may run the CanUVIT
 package as follows. ```python >>> import canuvit >>> canuvit.observe('uvit',
 '12:12:12', '12:12:12') ``` > **Note:** In general, `canuvit.observe
 (instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt',
 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in
-sexagesimal format. For the above example, you should get an output as shown
-below. Please also check the working directory for the output GALEX images with
-sources marked in the primary instrument field of view. ```
-========================================================= Payload: uvit,
-Coordinates: 12:12:12, 12:12:12
-========================================================= ### VIS sl_no ra_hms
-dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- ----------- --
--- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:07:47.5 11.1
-0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1 0.8 K0
-1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5 1457.4 234.9
-180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1 69.2 16.8
-950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2 1061.7 6 12:
-12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe filters:
-['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be absent!
-Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag Mag_corrected
-silica b4 b13 b15 n2 ----- ---------- ----------- ---- ------------- ------ --
-- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1 0.1 2 12:11:
-11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:14:58.3 16.2
-16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6 0.3 0.4 0.1
-0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe filters in
-NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-N2'] ###
-FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica ----- ----
------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:12:32.4
-+12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2 14.6 28.2
-23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4 12:12:
-15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5 14.8
-23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
+sexagesimal format. > **IMPORTANT:** Make sure you choose the correct **primary
+instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+For the above example, you should get an output as shown below. Please also
+check the working directory for the output GALEX images with sources marked in
+the primary instrument field of view. ```
+=================================================================== Primary
+instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+=================================================================== ### VIS
+sl_no ra_hms dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- -
+---------- ---- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:
+07:47.5 11.1 0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1
+0.8 K0 1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5
+1457.4 234.9 180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1
+69.2 16.8 950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2
+1061.7 6 12:12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe
+filters: ['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be
+absent! Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag
+Mag_corrected silica b4 b13 b15 n2 ----- ---------- ----------- ---- ----------
+--- ------ --- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1
+0.1 2 12:11:11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:
+14:58.3 16.2 16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6
+0.3 0.4 0.1 0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe
+filters in NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-
+N2'] ### FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica -
+---- ---------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:
+12:32.4 +12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2
+14.6 28.2 23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4
+12:12:15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5
+14.8 23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
 'Sapphire', 'Silica'] ``` Please choose the VIS filters such that none of the
 stars in the field gives >4800 counts/second. Further, for good tracking of the
 aspect, there should be at least two stars within a 12 arcminute radius of the
 target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid
 saturation) in the chosen filter. Please also avoid configuring multiple VIS
-filters. Two additional functions are also available, which takes the same
-input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find safe
-VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ### Command
-Line Interface After installation with pip, you can also access CanUVIT from
-the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12" -
-d "12:12:12" ``` The help page of the command-line tool can be accessed as
+filters. > **Note:** You will receive a warning if there are pairs of stars
+that are closer than 10 arcseconds in the VIS channel. In such cases, ensure
+the total count rate from the pairs of stars does not exceed the 4800 counts/
+seconds limit. Two additional functions are also available, which takes the
+same input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find
+safe VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ###
+Command Line Interface After installation with pip, you can also access CanUVIT
+from the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12"
+-d "12:12:12" ``` The help page of the command-line tool can be accessed as
 follows: ```bash canuvit -h ``` ``` Usage: canuvit [OPTIONS] Program to check
 if a given coordinate can be safely observed using UVIT. Example usage: canuvit
 -r "13:12:14" -d "-14:15:13" Options: --all Check safety for all filters.
 [default: all] --vis Check saftey for only visible filters. --uv Check safety
 for only UV filters. -r, --ra RA Right ascension of the coordinate. Format: hh:
 mm:ss[.ss] e.g. "00:54:53.45" [required] -d, --dec DEC Declination of the
 coordinate. Format: [-]dd:mm:ss[.ss] e.g. "-37:41:03.23". [required] -i, --
```

### Comparing `canuvit-0.5.0/setup.cfg` & `canuvit-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = canuvit
-version = 0.5.0
+version = 0.5.1
 author = Prajwel Joseph
 author_email = prajwel.pj@gmail.com
 description = UVIT safety checks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/prajwel/canuvit
 project_urls =
```

### Comparing `canuvit-0.5.0/src/canuvit/canuvit.py` & `canuvit-0.5.1/src/canuvit/canuvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1010,13 +1010,13 @@
         j = j + 1
 
     fuv_declaration = "Safe filters in FUV: {}".format(fuv_safe)
     print("\n{}".format(fuv_declaration))
 
 
 def observe(instrument, RA, DEC):
-    print("\n=========================================================")
-    print("Payload: {}, Coordinates: {}, {}".format(instrument, RA, DEC))
-    print("=========================================================")
+    print("\n===================================================================")
+    print("Primary instrument: {}, Coordinates: {}, {}".format(instrument.upper(), RA, DEC))
+    print("===================================================================")
 
     observe_VIS(instrument, RA, DEC)
     observe_UV(instrument, RA, DEC)
```

### Comparing `canuvit-0.5.0/src/canuvit/cli.py` & `canuvit-0.5.1/src/canuvit/cli.py`

 * *Files identical despite different names*

### Comparing `canuvit-0.5.0/src/canuvit/td1_catalogue.fits` & `canuvit-0.5.1/src/canuvit/td1_catalogue.fits`

 * *Files identical despite different names*

### Comparing `canuvit-0.5.0/src/canuvit.egg-info/PKG-INFO` & `canuvit-0.5.1/src/canuvit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: canuvit
-Version: 0.5.0
+Version: 0.5.1
 Summary: UVIT safety checks
 Home-page: https://github.com/prajwel/canuvit
 Author: Prajwel Joseph
 Author-email: prajwel.pj@gmail.com
 Project-URL: Bug Tracker, https://github.com/prajwel/canuvit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2
+Requires-Dist: numpy>=1.13
+Requires-Dist: matplotlib>=2
+Requires-Dist: astropy>=2
+Requires-Dist: beautifulsoup4>=4.4
+Requires-Dist: click>=2
+Requires-Dist: astroquery>=0.4.5
 
 # **CanUVIT**
 > To check whether a field can be safely observed with UVIT.
 
 <p align="center">
 <img src="https://i.imgur.com/b0hoB04.png" width="400"/>
 </p>
@@ -40,24 +47,26 @@
 ```python
 >>> import canuvit
 >>> canuvit.observe('uvit', '12:12:12', '12:12:12')
 ```
 
 > **Note:** In general, `canuvit.observe(instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt', 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in sexagesimal format.
 
+> **IMPORTANT:** Make sure you choose the correct **primary instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+
 For the above example, you should get an output as shown below. Please also check the working directory for the output GALEX images with sources marked in the primary instrument field of view.
 
 ```
-=========================================================
-Payload: uvit, Coordinates: 12:12:12, 12:12:12
-=========================================================
+===================================================================
+Primary instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+===================================================================
 
 ### VIS
 
-sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7  
+sl_no   ra_hms     dec_dms   mag  B-V SpecType  VIS3   VIS2  VIS1 ND1   BK7
 ----- ---------- ----------- ---- --- -------- ------ ----- ----- ---- ------
     1 12:11:52.8 +12:07:47.5 11.1 0.9       K1 1333.0 124.4  88.6 29.7 1624.9
     2 12:12:22.9 +12:17:23.9 11.1 0.8       K0 1296.7 121.0  86.2 28.9 1580.6
     3 12:11:35.0 +12:12:04.6 11.4 0.5       F5 1457.4 234.9 180.9 32.8 1915.2
     4 12:11:01.7 +12:08:35.9 11.9 0.7       G5  754.3  89.1  69.2 16.8  950.9
     5 12:11:11.5 +12:03:14.0 12.2 0.3       F0  803.1 143.5 101.4 18.2 1061.7
     6 12:12:05.5 +12:19:09.8 12.3 0.8       K0  452.9  42.3  30.1 10.1  552.1
@@ -89,14 +98,16 @@
     5 12:11:35.0 +12:12:04.7 16.5          14.8 23.0 19.6     14.5    5.1
 
 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2', 'Sapphire', 'Silica']
 ```
 
 Please choose the VIS filters such that none of the stars in the field gives >4800 counts/second. Further, for good tracking of the aspect, there should be at least two stars within a 12 arcminute radius of the target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid saturation) in the chosen filter. Please also avoid configuring multiple VIS filters. 
 
+> **Note:** You will receive a warning if there are pairs of stars that are closer than 10 arcseconds in the VIS channel. In such cases, ensure the total count rate from the pairs of stars does not exceed the 4800 counts/seconds limit.
+
 Two additional functions are also available, which takes the same input arguments as `canuvit.observe()`.
 
 * `canuvit.observe_VIS()`: to find safe VIS filters.
 * `canuvit.observe_UV()`: to find safe UV filters.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1 Name: canuvit Version: 0.5.0 Summary: UVIT safety checks
+Metadata-Version: 2.1 Name: canuvit Version: 0.5.1 Summary: UVIT safety checks
 Home-page: https://github.com/prajwel/canuvit Author: Prajwel Joseph Author-
 email: prajwel.pj@gmail.com Project-URL: Bug Tracker, https://github.com/
 prajwel/canuvit/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # **CanUVIT** > To check whether a
-field can be safely observed with UVIT.
+Type: text/markdown License-File: LICENSE Requires-Dist: requests>=2 Requires-
+Dist: numpy>=1.13 Requires-Dist: matplotlib>=2 Requires-Dist: astropy>=2
+Requires-Dist: beautifulsoup4>=4.4 Requires-Dist: click>=2 Requires-Dist:
+astroquery>=0.4.5 # **CanUVIT** > To check whether a field can be safely
+observed with UVIT.
                        [https://i.imgur.com/b0hoB04.png]
 You can install the CanUVIT Python package using the following command. ```bash
 pip install canuvit --upgrade ``` > **IMPORTANT:** Even if you have CanUVIT
 already installed, make sure you use the latest version by running the above
 command. Current version of CanUVIT is shown on the badge below:
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_c_a_n_u_v_i_t_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 > **Note:** If you don't want to install CanUVIT or are facing problems during
@@ -19,52 +22,57 @@
 After installation, you can run CanUVIT on a Python command prompt or as a
 script. For example, if your primary instrument is UVIT and the RA, DEC
 coordinates of the field are (12:12:12, 12:12:12), you may run the CanUVIT
 package as follows. ```python >>> import canuvit >>> canuvit.observe('uvit',
 '12:12:12', '12:12:12') ``` > **Note:** In general, `canuvit.observe
 (instrument, RA, DEC)` where the `instrument` can be either 'uvit', 'sxt',
 'czti', or 'laxpc' and `RA` and `DEC` field coordinates should be in
-sexagesimal format. For the above example, you should get an output as shown
-below. Please also check the working directory for the output GALEX images with
-sources marked in the primary instrument field of view. ```
-========================================================= Payload: uvit,
-Coordinates: 12:12:12, 12:12:12
-========================================================= ### VIS sl_no ra_hms
-dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- ----------- --
--- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:07:47.5 11.1
-0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1 0.8 K0
-1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5 1457.4 234.9
-180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1 69.2 16.8
-950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2 1061.7 6 12:
-12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe filters:
-['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be absent!
-Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag Mag_corrected
-silica b4 b13 b15 n2 ----- ---------- ----------- ---- ------------- ------ --
-- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1 0.1 2 12:11:
-11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:14:58.3 16.2
-16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6 0.3 0.4 0.1
-0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe filters in
-NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-N2'] ###
-FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica ----- ----
------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:12:32.4
-+12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2 14.6 28.2
-23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4 12:12:
-15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5 14.8
-23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
+sexagesimal format. > **IMPORTANT:** Make sure you choose the correct **primary
+instrument**. Incorrect choice of `instrument` may lead to proposal rejection.
+For the above example, you should get an output as shown below. Please also
+check the working directory for the output GALEX images with sources marked in
+the primary instrument field of view. ```
+=================================================================== Primary
+instrument: UVIT, Coordinates: 12:12:12, 12:12:12
+=================================================================== ### VIS
+sl_no ra_hms dec_dms mag B-V SpecType VIS3 VIS2 VIS1 ND1 BK7 ----- ---------- -
+---------- ---- --- -------- ------ ----- ----- ---- ------ 1 12:11:52.8 +12:
+07:47.5 11.1 0.9 K1 1333.0 124.4 88.6 29.7 1624.9 2 12:12:22.9 +12:17:23.9 11.1
+0.8 K0 1296.7 121.0 86.2 28.9 1580.6 3 12:11:35.0 +12:12:04.6 11.4 0.5 F5
+1457.4 234.9 180.9 32.8 1915.2 4 12:11:01.7 +12:08:35.9 11.9 0.7 G5 754.3 89.1
+69.2 16.8 950.9 5 12:11:11.5 +12:03:14.0 12.2 0.3 F0 803.1 143.5 101.4 18.2
+1061.7 6 12:12:05.5 +12:19:09.8 12.3 0.8 K0 452.9 42.3 30.1 10.1 552.1 Safe
+filters: ['VIS3', 'VIS2', 'VIS1', 'ND1', 'BK7'] FUV observations seem to be
+absent! Using M_fuv = M_nuv - 1.65. ### NUV sl_no ra_hms dec_dms Mag
+Mag_corrected silica b4 b13 b15 n2 ----- ---------- ----------- ---- ----------
+--- ------ --- --- --- --- 1 12:12:32.4 +12:07:27.4 19.3 19.3 1.9 0.4 0.5 0.1
+0.1 2 12:11:11.7 +12:03:14.8 16.2 16.2 31.8 7.0 8.6 2.3 1.7 3 12:12:41.1 +12:
+14:58.3 16.2 16.2 34.7 7.6 9.4 2.6 1.9 4 12:12:15.3 +12:29:18.1 19.5 19.5 1.6
+0.3 0.4 0.1 0.1 5 12:11:35.0 +12:12:04.7 16.5 16.5 25.9 5.7 7.0 1.9 1.4 Safe
+filters in NUV: ['Silica', 'NUV-grating', 'NUV-B4', 'NUV-B13', 'NUV-B15', 'NUV-
+N2'] ### FUV sl_no ra_hms dec_dms Mag Mag_corrected caf2 baf2 sapphire silica -
+---- ---------- ----------- ---- ------------- ---- ---- -------- ------ 1 12:
+12:32.4 +12:07:27.4 19.3 17.7 1.7 1.4 1.0 0.4 2 12:11:11.7 +12:03:14.8 16.2
+14.6 28.2 23.9 17.7 6.2 3 12:12:41.1 +12:14:58.3 16.2 14.5 30.7 26.1 19.4 6.8 4
+12:12:15.3 +12:29:18.1 19.5 17.8 1.4 1.2 0.9 0.3 5 12:11:35.0 +12:12:04.7 16.5
+14.8 23.0 19.6 14.5 5.1 Safe filters in FUV: ['CaF2', 'FUV-grating', 'BaF2',
 'Sapphire', 'Silica'] ``` Please choose the VIS filters such that none of the
 stars in the field gives >4800 counts/second. Further, for good tracking of the
 aspect, there should be at least two stars within a 12 arcminute radius of the
 target with >30 counts/second (for good S/N) and <1000 counts/second (to avoid
 saturation) in the chosen filter. Please also avoid configuring multiple VIS
-filters. Two additional functions are also available, which takes the same
-input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find safe
-VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ### Command
-Line Interface After installation with pip, you can also access CanUVIT from
-the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12" -
-d "12:12:12" ``` The help page of the command-line tool can be accessed as
+filters. > **Note:** You will receive a warning if there are pairs of stars
+that are closer than 10 arcseconds in the VIS channel. In such cases, ensure
+the total count rate from the pairs of stars does not exceed the 4800 counts/
+seconds limit. Two additional functions are also available, which takes the
+same input arguments as `canuvit.observe()`. * `canuvit.observe_VIS()`: to find
+safe VIS filters. * `canuvit.observe_UV()`: to find safe UV filters. ###
+Command Line Interface After installation with pip, you can also access CanUVIT
+from the command line. Here's an example: ```bash canuvit -i uvit -r "12:12:12"
+-d "12:12:12" ``` The help page of the command-line tool can be accessed as
 follows: ```bash canuvit -h ``` ``` Usage: canuvit [OPTIONS] Program to check
 if a given coordinate can be safely observed using UVIT. Example usage: canuvit
 -r "13:12:14" -d "-14:15:13" Options: --all Check safety for all filters.
 [default: all] --vis Check saftey for only visible filters. --uv Check safety
 for only UV filters. -r, --ra RA Right ascension of the coordinate. Format: hh:
 mm:ss[.ss] e.g. "00:54:53.45" [required] -d, --dec DEC Declination of the
 coordinate. Format: [-]dd:mm:ss[.ss] e.g. "-37:41:03.23". [required] -i, --
```

