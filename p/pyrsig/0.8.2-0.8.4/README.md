# Comparing `tmp/pyrsig-0.8.2.tar.gz` & `tmp/pyrsig-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsig-0.8.2.tar", last modified: Mon Apr  8 16:54:44 2024, max compression
+gzip compressed data, was "pyrsig-0.8.4.tar", last modified: Thu Apr 18 20:30:58 2024, max compression
```

## Comparing `pyrsig-0.8.2.tar` & `pyrsig-0.8.4.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.709510 pyrsig-0.8.2/
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.8.2/LICENSE
--rw-r--r--   0 bhenders (83225) romo       (131)     3678 2024-04-08 16:54:44.709256 pyrsig-0.8.2/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)     3180 2024-04-08 16:48:39.000000 pyrsig-0.8.2/README.md
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.701291 pyrsig-0.8.2/pyrsig/
--rw-r--r--   0 bhenders (83225) romo       (131)    53734 2024-04-08 16:48:46.000000 pyrsig-0.8.2/pyrsig/__init__.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.705100 pyrsig-0.8.2/pyrsig/cmaq/
--rw-r--r--   0 bhenders (83225) romo       (131)     7162 2024-03-07 22:09:38.000000 pyrsig-0.8.2/pyrsig/cmaq/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     5581 2024-03-11 19:31:34.000000 pyrsig-0.8.2/pyrsig/cmaq/pair.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.708890 pyrsig-0.8.2/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.8.2/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-12-14 22:29:06.000000 pyrsig-0.8.2/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.8.2/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3129 2023-06-08 20:39:38.000000 pyrsig-0.8.2/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 19:56:26.000000 pyrsig-0.8.2/pyrsig/tests/test_gui.py
--rw-r--r--   0 bhenders (83225) romo       (131)     3576 2023-10-10 18:23:29.000000 pyrsig-0.8.2/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.8.2/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     8301 2024-03-11 21:02:29.000000 pyrsig-0.8.2/pyrsig/utils.py
--rw-r--r--   0 bhenders (83225) romo       (131)    20959 2024-04-08 13:39:40.000000 pyrsig-0.8.2/pyrsig/xdr.py
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-08 16:54:44.704062 pyrsig-0.8.2/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)     3678 2024-04-08 16:54:44.701941 pyrsig-0.8.2/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)      456 2024-04-08 16:54:44.702486 pyrsig-0.8.2/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-08 16:54:44.703028 pyrsig-0.8.2/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2024-04-08 16:54:44.703596 pyrsig-0.8.2/pyrsig.egg-info/requires.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2024-04-08 16:54:44.704138 pyrsig-0.8.2/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2024-04-08 16:54:44.709732 pyrsig-0.8.2/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 20:59:18.000000 pyrsig-0.8.2/setup.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.742769 pyrsig-0.8.4/
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.8.4/LICENSE
+-rw-r--r--   0 bhenders (83225) romo       (131)       32 2024-04-15 14:22:45.000000 pyrsig-0.8.4/MANIFEST.in
+-rw-r--r--   0 bhenders (83225) romo       (131)     4025 2024-04-18 20:30:58.742498 pyrsig-0.8.4/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)     3527 2024-04-17 18:36:29.000000 pyrsig-0.8.4/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.724761 pyrsig-0.8.4/pyrsig/
+-rw-r--r--   0 bhenders (83225) romo       (131)    37419 2024-04-17 18:35:22.000000 pyrsig-0.8.4/pyrsig/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.729708 pyrsig-0.8.4/pyrsig/cmaq/
+-rw-r--r--   0 bhenders (83225) romo       (131)     8054 2024-04-17 18:34:45.000000 pyrsig-0.8.4/pyrsig/cmaq/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     5581 2024-03-11 19:31:34.000000 pyrsig-0.8.4/pyrsig/cmaq/pair.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.733921 pyrsig-0.8.4/pyrsig/data/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.736419 pyrsig-0.8.4/pyrsig/data/.ipynb_checkpoints/
+-rw-r--r--   0 bhenders (83225) romo       (131)   977294 2024-04-15 14:05:54.000000 pyrsig-0.8.4/pyrsig/data/.ipynb_checkpoints/DescribeCoverage-checkpoint.csv
+-rw-r--r--   0 bhenders (83225) romo       (131)     6105 2024-04-17 18:34:14.000000 pyrsig-0.8.4/pyrsig/data/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 bhenders (83225) romo       (131)   977294 2024-04-15 14:05:54.000000 pyrsig-0.8.4/pyrsig/data/DescribeCoverage.csv
+-rw-r--r--   0 bhenders (83225) romo       (131)     6105 2024-04-17 18:34:14.000000 pyrsig-0.8.4/pyrsig/data/__init__.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.737089 pyrsig-0.8.4/pyrsig/data/__pycache__/
+-rw-r--r--   0 bhenders (83225) romo       (131)     4117 2024-04-17 18:35:46.000000 pyrsig-0.8.4/pyrsig/data/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.742039 pyrsig-0.8.4/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.8.4/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-12-14 22:29:06.000000 pyrsig-0.8.4/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.8.4/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3420 2024-04-10 12:28:13.000000 pyrsig-0.8.4/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-11-16 19:56:26.000000 pyrsig-0.8.4/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     3576 2023-10-10 18:23:29.000000 pyrsig-0.8.4/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      147 2024-04-15 15:01:26.000000 pyrsig-0.8.4/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    17099 2024-04-15 19:40:13.000000 pyrsig-0.8.4/pyrsig/utils.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    32866 2024-04-17 18:33:57.000000 pyrsig-0.8.4/pyrsig/xdr.py
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2024-04-18 20:30:58.728285 pyrsig-0.8.4/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)     4025 2024-04-18 20:30:58.725547 pyrsig-0.8.4/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)      719 2024-04-18 20:30:58.726130 pyrsig-0.8.4/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-18 20:30:58.726641 pyrsig-0.8.4/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2024-04-17 18:30:39.000000 pyrsig-0.8.4/pyrsig.egg-info/not-zip-safe
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2024-04-18 20:30:58.727773 pyrsig-0.8.4/pyrsig.egg-info/requires.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2024-04-18 20:30:58.728359 pyrsig-0.8.4/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2024-04-18 20:30:58.743046 pyrsig-0.8.4/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     1016 2024-04-15 15:53:11.000000 pyrsig-0.8.4/setup.py
```

### Comparing `pyrsig-0.8.2/LICENSE` & `pyrsig-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/PKG-INFO` & `pyrsig-0.8.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyrsig
-Version: 0.8.2
-Summary: Python interface to RSIG Web API
-Home-page: https://github.com/barronh/pyrsig
-Author: Barron H. Henderson
-Author-email: barronh@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyrsig
 
 Python interface to RSIG Web API
 
 ## Install
 
 From pypi.org (most stable):
@@ -105,14 +90,19 @@
 # 3875
 ```
 
 ## Change Log
 
 Not all changes are listed, but notable changes are itemized for ease of review.
 
+* v0.8.4: Added support for Subset 9.0 CMAQ and Grid 1.0 xdr formats.
+          Updated keys to rely on descriptions (via DescribeCoverage).
+          Added utilites for basic polygon/cmaq intersections for HMS.
+* v0.8.3: Added xdr Polygon 1.0 format capability, added package
+          DescribeCoverage in data module and restructured utilities.
 * v0.8.2: Added xdr CALIPSO 1.0 format capability.
 * v0.8.1: Added xdr Point 1.0 format capability.
 * v0.8.0: Restructuring module code and adding CMAQ pairing.
 * v0.7.0: Added offline descriptions for review of space/time coverage.
 * v0.7.0: Added TEMPO options for screening
 * v0.6.0: Added latitude longitude grid pass thru support.
 * v0.5.1: Added convenience function for opening many IOAPI files at once.
```

### Comparing `pyrsig-0.8.2/pyrsig/__init__.py` & `pyrsig-0.8.4/pyrsig/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,19 @@
 __all__ = ['RsigApi', 'RsigGui', 'open_ioapi', 'open_mfioapi', 'cmaq']
-__version__ = '0.8.2'
+__version__ = '0.8.4'
 
 from . import cmaq
 from .cmaq import open_ioapi, open_mfioapi
 import pandas as pd
-import requests
 from .utils import customize_grid, def_grid_kw as _def_grid_kw
+from .utils import coverages_from_xml, legacy_get
 
-# Used to shorten pandora names for 80 character PEP
-_trvca = 'tropospheric_vertical_column_amount'
 
-_keys = (
-    'airnow.pm25', 'airnow.pm10', 'airnow.ozone', 'airnow.no', 'airnow.no2',
-    'airnow.nox', 'airnow.so2', 'airnow.co', 'airnow.temperature',
-    'airnow.pressure', 'airnow.rh', 'airnow2.pm25', 'airnow2.ozone',
-    'airnow2.no2', 'airnow2.so2', 'airnow2.co',
-    'aqs.pm25', 'aqs.pm25_daily_average', 'aqs.pm25_daily_filter', 'aqs.pm10',
-    'aqs.ozone', 'aqs.ozone_8hour_average', 'aqs.ozone_daily_8hour_maximum',
-    'aqs.co', 'aqs.so2', 'aqs.no2', 'aqs.nox', 'aqs.noy', 'aqs.rh',
-    'aqs.temperature', 'aqs.pressure',
-    'ceilometer.aerosol_layer_heights',
-    'cmaq.equates.conus.aconc.O3', 'cmaq.equates.conus.aconc.NO2',
-    'cmaq.equates.conus.aconc.PM25',
-    'hms.fire_ecosys', 'hms.fire_power', 'hms.smoke',
-    'metar.elevation', 'metar.visibility', 'metar.seaLevelPress',
-    'metar.temperature', 'metar.dewpoint', 'metar.relativeHumidity',
-    'metar.windDir', 'metar.windSpeed', 'metar.windGustSpeed', 'metar.wind',
-    'metar.altimeter', 'metar.minTemp24Hour', 'metar.maxTemp24Hour',
-    'metar.precip1Hour', 'metar.precip3Hour', 'metar.precip6Hour',
-    'metar.precip24Hour', 'metar.pressChange3Hour', 'metar.snowCover'
-    'nesdis.pm25', 'nesdis.co', 'nesdis.co2', 'nesdis.ch4', 'nesdis.n2o',
-    'nesdis.nh3', 'nesdis.nox', 'nesdis.so2', 'nesdis.tnmhc',
-    'pandora.ozone'
-    f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}',
-    f'pandora.L2_rfuh5p1_8.formaldehyde_{_trvca}_uncertainty',
-    'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor',
-    'pandora.L2_rfus5p1_8.direct_formaldehyde_air_mass_factor_uncertainty',
-    'pandora.L2_rfus5p1_8.formaldehyde_total_vertical_column_amount',
-    'pandora.L2_rfus5p1_8.formaldehyde_vertical_column_amount_uncertainty',
-    f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}',
-    f'pandora.L2_rnvh3p1_8.water_vapor_{_trvca}_uncertainty',
-    'pandora.L2_rnvs3p1_8.nitrogen_dioxide_vertical_column_amount',
-    'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide',
-    'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide_uncertainty',
-    'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor',
-    'pandora.L2_rnvs3p1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
-    'pandora.L2_rout2p1_8.ozone_vertical_column_amount',
-    'pandora.L2_rout2p1_8.direct_ozone_air_mass_factor',
-    'pandora.L2_rout2p1_8.ozone_air_mass_factor_uncertainty',
-    'pandora.L2_rsus1p1_8.sulfur_dioxide_vertical_column_amount',
-    'pandora.L2_rsus1p1_8.direct_sulfur_dioxide_air_mass_factor',
-    'pandora.L2_rsus1p1_8.sulfur_dioxide_air_mass_factor_uncertainty',
-    'pandora.L2_rnvssp1_8.nitrogen_dioxide_vertical_column_amount',
-    'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor',
-    'pandora.L2_rnvssp1_8.direct_nitrogen_dioxide_air_mass_factor_uncertainty',
-    'purpleair.pm25_corrected',
-    'purpleair.pm25_corrected_hourly', 'purpleair.pm25_corrected_daily',
-    'purpleair.pm25_corrected_monthly', 'purpleair.pm25_corrected_yearly',
-    'regridded.conus.monthly.tropomi.offl.no2',
-    'regridded.conus.monthly.tropomi.offl.hcho',
-    'regridded.conus.monthly.tropomi.offl.ch4',
-    'regridded.conus.monthly.tropomi.offl.co',
-    'regridded.conus.monthly.tropomi.rpro.no2',
-    'regridded.conus.seasonal.tropomi.offl.no2',
-    'regridded.conus.seasonal.tropomi.offl.hcho',
-    'regridded.conus.seasonal.tropomi.offl.ch4',
-    'regridded.conus.seasonal.tropomi.offl.co',
-    'regridded.conus.seasonal.tropomi.rpro.no2',
-    'tempo.proxy_l2.no2.vertical_column_total',
-    'tempo.proxy_l2.no2.vertical_column_total_uncertainty',
-    'tempo.proxy_l2.no2.vertical_column_troposphere',
-    'tempo.proxy_l2.no2.vertical_column_stratosphere',
-    'tempo.proxy_l2.no2.amf_total',
-    'tempo.proxy_l2.no2.amf_total_uncertainty',
-    'tempo.proxy_l2.no2.amf_troposphere',
-    'tempo.proxy_l2.no2.amf_stratosphere',
-    'tempo.proxy_l2.no2.ground_pixel_quality_flag',
-    'tempo.proxy_l2.hcho.vertical_column',
-    'tempo.proxy_l2.hcho.vertical_column_uncertainty',
-    'tempo.proxy_l2.hcho.amf',
-    'tempo.proxy_l2.hcho.amf_uncertainty',
-    'tempo.proxy_l2.o3p.total_ozone_column',
-    'tempo.proxy_l2.o3p.troposphere_ozone_column',
-    'tempo.proxy_l2.o3p.stratosphere_ozone_column',
-    'tempo.proxy_l2.o3p.ozone_information_content',
-    'tempo.proxy_l2.o3p.ground_pixel_quality_flag',
-    'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
-    'tropomi.offl.no2.air_mass_factor_troposphere',
-    'tropomi.offl.hcho.formaldehyde_tropospheric_vertical_column',
-    'tropomi.offl.co.carbonmonoxide_total_column',
-    'tropomi.offl.ch4.methane_mixing_ratio',
-    'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
-    'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
-)
-
-_nocorner_prefixes = (
-    'airnow', 'aqs', 'purpleair', 'pandora', 'cmaq', 'regridded',
-    'calipso'
+_corner_prefixes = (
+    'gasp', 'goes', 'modis', 'omibehr', 'tempo', 'tropomi', 'viirs'
 )
 _nolonlats_prefixes = ('cmaq', 'regridded')
 _noregrid_prefixes = ('cmaq', 'regridded')
 
 
 def _actionf(msg, action, ErrorTyp=None):
     """
@@ -127,233 +40,14 @@
         ErrorTyp = ValueError
     if action == 'error':
         raise ErrorTyp(msg)
     elif action == 'warn':
         warnings.warn(msg)
 
 
-def parsexml(root):
-    """Recursive xml parsing:
-    Given a root, return dictionaries for each element and its children.
-    Each element has children, attributes (attr), tag, and text.
-    If any of these has no elements, it will be removed.
-    """
-    out = {}
-    out['tag'] = root.tag.split('}')[-1]
-    out['attr'] = root.attrib
-    out['text'] = root.text
-    out['children'] = []
-
-    for child in root:
-        childd = parsexml(child)
-        out['children'].append(childd)
-
-    if len(out['children']) == 0:
-        del out['children']
-    if out['text'] is None:
-        out['text'] = ''
-
-    out['text'] = out['text'].strip()
-    if len(out['text']) == 0:
-        del out['text']
-    if len(out['attr']) == 0:
-        del out['attr']
-
-    return out
-
-
-def coverages_from_xml(txt):
-    """Based on xml text, create coverage data"""
-    import xml.etree.ElementTree as ET
-
-    root = ET.fromstring(txt)
-
-    xmlout = parsexml(root)
-    out = []
-    for c in xmlout['children']:
-        record = {k: v for k, v in c.items() if k != 'children'}
-        kids = c['children']
-        for e in kids:
-            if 'attr' not in e and len(e.get('children', [])) == 0:
-                record[e['tag']] = e.get('text', '')
-
-            if e['tag'] == 'lonLatEnvelope':
-                envtxt = ''
-                for p in e['children']:
-                    envtxt += ' ' + p['text']
-                record['bbox_str'] = envtxt.strip()
-
-            if e['tag'] == 'domainSet':
-                for s in e['children']:
-                    if s['tag'] == 'temporalDomain':
-                        for tp in s['children']:
-                            for te in tp['children']:
-                                record[te['tag']] = te['text']
-
-        out.append(record)
-
-    return out
-
-
-def _progress(blocknum, readsize, totalsize):
-    """
-    Display progress using dots or % indicator.
-
-    Arguments
-    ---------
-    blocknum : int
-        block number of blocks to be read
-    readsize : int
-        chunksize read
-    totalsize : int
-        -1 unknown or size of file
-    """
-    totalblocks = (totalsize // readsize) + 1
-    pblocks = totalblocks // 10
-    if pblocks <= 0:
-        pblocks = 100
-    if totalsize > 0:
-        print(
-            '\r' + 'Retrieving {:.0f}'.format(readsize/totalsize*100), end='',
-            flush=True
-        )
-    else:
-        if blocknum == 0:
-            print('Retrieving .', end='', flush=True)
-        if (blocknum % pblocks) == 0:
-            print('.', end='', flush=True)
-
-
-def _create_unverified_tls_context(*args, **kwds):
-    """
-    Thin wrapper around ssl._create_unverified_context that adds the option to
-    use TLS negotiation, which is currently used by RSIG servers.
-    """
-    import ssl
-    # Set up SSL context to allow legacy TLS versions
-    ctx = ssl._create_unverified_context(*args, **kwds)
-    ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
-    return ctx
-
-
-class LegacyAdapter(requests.adapters.HTTPAdapter):
-    # "Transport adapter" that allows us to use custom ssl_context.
-
-    def __init__(self, **kwargs):
-        import ssl
-        def_ctx = ssl._create_default_https_context
-        ssl._create_default_https_context = _create_unverified_tls_context
-        ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
-        ctx.options |= 0x4  # OP_LEGACY_SERVER_CONNECT
-        self.ssl_context = ctx
-        ssl._create_default_https_context = def_ctx
-        super().__init__(**kwargs)
-
-    def init_poolmanager(self, connections, maxsize, block=False):
-        import urllib3
-        self.poolmanager = urllib3.poolmanager.PoolManager(
-            num_pools=connections, maxsize=maxsize,
-            block=block, ssl_context=self.ssl_context)
-
-
-def legacy_get(url, *args, **kwds):
-    import copy
-    session = requests.session()
-    la = LegacyAdapter()
-
-    # Maple has a bad certificate, so here if you are using maple
-    # I disable the certificate, but no the warning
-    if 'maple' in url:
-        la.ssl_context.check_hostname = False
-        kwds = copy.copy(kwds)
-        kwds.setdefault('verify', False)
-
-    session.mount('https://', la)
-
-    return session.get(url, *args, **kwds)
-
-
-def _getfile(url, outpath, maxtries=5, verbose=1, overwrite=False):
-    """
-    Download file from RSIG using fault tolerance and optional caching
-    when overwrite is False.
-
-    Arguments
-    ---------
-    url : str
-        path to retrieve
-    outpath : str
-        path to save file to
-    maxtries : int
-        try this many times before quitting
-    verbose : int
-        Level of verbosity
-    overwrite : bool
-        If True, overwrite existing files.
-        If False, reuse existing files.
-
-    Returns
-    -------
-    None
-    """
-    import time
-    from urllib.request import urlretrieve
-    import ssl
-    import os
-
-    # If the file exists, get the current size
-    if not overwrite and os.path.exists(outpath):
-        stat = os.stat(outpath)
-        dlsize = stat.st_size
-    else:
-        dlsize = 0
-
-    # if the size is non-zero, assume it is good
-    if dlsize > 0:
-        print('Using cached:', outpath)
-        return
-
-    _def_https_context = ssl._create_default_https_context
-    ssl._create_default_https_context = _create_unverified_tls_context
-
-    # Try to download the file maxtries times
-    tries = 0
-    if verbose > 0:
-        reporthook = _progress
-    else:
-        reporthook = None
-    while dlsize <= 0 and tries < maxtries:
-        # Remove 0-sized files.
-        outdir = os.path.dirname(outpath)
-        if os.path.exists(outpath):
-            os.remove(outpath)
-        os.makedirs(outdir, exist_ok=True)
-        if verbose:
-            print('Calling RSIG', outpath, '')
-        t0 = time.time()
-        urlretrieve(
-            url=url,
-            filename=outpath,
-            reporthook=reporthook,
-        )
-        # Check timing
-        t1 = time.time()
-        stat = os.stat(outpath)
-        dlsize = stat.st_size
-
-        if dlsize == 0:
-            print('Failed', url, t1 - t0)
-        tries += 1
-
-        if verbose > 0:
-            print('')
-
-    ssl._create_default_https_context = _def_https_context
-
-
 class RsigApi:
     def __init__(
         self, key=None, bdate=None, edate=None, bbox=None, grid_kw=None,
         tropomi_kw=None, purpleair_kw=None, viirsnoaa_kw=None, tempo_kw=None,
         pandora_kw=None, calipso_kw=None,
         server='ofmpub.epa.gov', compress=1, corners=1, encoding=None,
         overwrite=False, workdir='.', gridfit=False
@@ -438,17 +132,15 @@
           Dictionary of filter properties and api_key. Unlike other options,
           purpleair_kw will not work with the defaults. The user *must* update
           teh api_key property to their own key. Contact PurpleAir for more
           details.
 
         """
         self._description = {}
-        self._keys = None
         self._capabilities = None
-        self._describecoverages = None
         self._coveragesdf = None
         self._capabilitiesdf = None
         self.server = server
         self.key = key
         self.compress = compress
         self.workdir = workdir
         self.encoding = encoding
@@ -617,15 +309,15 @@
             coverages['prefix'] = coverages['name'].apply(
                 lambda x: x.split('.')[0]
             )
             coverages = coverages.drop('tag', axis=1)
 
         return coverages
 
-    def descriptions(self, as_dataframe=True, refresh=False, verbose=0):
+    def descriptions(self, refresh=False, verbose=0):
         """
         Experimental and may change.
 
         descriptions returns details about all coverages. Details include
         spatial bounding box, time coverage, time resolution, variable label,
         and a short description.
 
@@ -634,17 +326,14 @@
         DescribeCoverage.
 
         Currently cleaning up data xml elements that are bad and doing a
         per-coverage parsing to increase fault tolerance in the xml.
 
         Arguments
         ---------
-        as_dataframe : bool
-            Defaults to True and descriptions are returned as a dataframe.
-            If False, returns a list of elements.
         refresh : bool
             If True, get new copy and save to ~/.pyrsig/descriptons.xml
             If False (default), reload from saved if available.
         verbose : int
             If verbose is greater than 0, show warnings from parsing.
 
         Returns
@@ -658,150 +347,20 @@
             rsigapi = pyrsig.RsigApi()
             desc = rsigapi.descriptions()
             print(desc.query('prefix == "tropomi"').name.unique())
             # ['tropomi.nrti.no2.nitrogendioxide_tropospheric_column'
             #  ... 43 other name here
             #  'tropomi.rpro.ch4.methane_mixing_ratio_bias_corrected']
         """
-        import re
-        import pandas as pd
-        import warnings
-        import os
-
-        descpath = os.path.expanduser('~/.pyrsig/DescribeCoverage.csv')
-        if not refresh and as_dataframe:
-            if self._coveragesdf is not None:
-                return self._coveragesdf
-            elif os.path.exists(descpath):
-                self._coveragesdf = pd.read_csv(descpath)
-                return self._coveragesdf
-
-        print('Refreshing descriptions...')
-        # Start Cleaning Section
-        # BHH 2023-05-10
-        # This section provides "cleaning" to the xml content provided by
-        # DescribeCoverage. This should not have to happen and should be
-        # removable at some point in the future.
-        # Working with TP to fix xml
-
-        descmidre = re.compile(
-            r'\</CoverageDescription\>.+?\<CoverageDescription.+?\>',
-            flags=re.MULTILINE + re.DOTALL
-        )
-        mismatchtempre = re.compile(
-            r'\</lonLatEnvelope\>\s+\</spatialDomain\>',
-            flags=re.MULTILINE + re.DOTALL
-        )
-
-        # Regex, replacement
-        resubsdesc = [
-            (descmidre, ''),  # concated coverages have extra open/close tags
-            (re.compile('<='), '&lt;='),  # associated with <= 32 in Modis
-            (re.compile('qa_value <'), 'qa_value &lt;'),  # w/ tropomi.ntri
-            (
-                mismatchtempre,
-                '</lonLatEnvelope><domainSet><spatialDomain></spatialDomain>',
-            ),  # Missing open block for spatialDomain in goes (eg imager.calb)
-            (
-                re.compile(r'</CoverageOffering>\s+</CoverageOfferingBrief>'),
-                '</CoverageOffering>',
-            ),  # Ceiliometers have wrong opening tags and extra close tag
-            (
-                re.compile('CoverageOfferingBrief'), 'CoverageOffering'
-            ),  # Ceiliometers have wrong opening tags and extra close tag
-            (
-                re.compile(
-                    r'<rangeSet>\s+<RangeSet>\s+<supportedCRSs>',
-                    flags=re.MULTILINE + re.DOTALL
-                ),
-                '<rangeSet><RangeSet></RangeSet></rangeSet><supportedCRSs>'
-            ),  # Ceiliometers have missing rangeset content and closing tags
-        ]
-
-        if self._describecoverages is None or refresh:
-            if verbose > 1:
-                print('Requesting...', flush=True)
-            self._describecoverages = legacy_get(
-                f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
-                '1.0.0&REQUEST=DescribeCoverage'
-            ).text
-
-            ctext = self._describecoverages
-
-            for reg, sub in resubsdesc:
-                ctext = reg.sub(sub, ctext)
-
-            # End Cleaning Section
-            self._describecoverages = ctext
-
-        ctext = self._describecoverages
-
-        # Selecting coverages and removing garbage when necessary.
-        cleanre = re.compile(
-            r'\</name\>.+?\</CoverageOffering\>',
-            flags=re.MULTILINE + re.DOTALL
-        )
-        # <CoverageOffering>.+?</CoverageOffering>
-        coverre = re.compile(
-            r'\<CoverageOffering\>.+?\</CoverageOffering\>',
-            flags=re.MULTILINE + re.DOTALL
-        )
-
-        coverages = []
-        limited_details = []
-        for rex in coverre.finditer(ctext):
-            secttxt = ctext[rex.start():rex.end()]
-            secttxt = (
-                '<CoverageDescription version="1.0.0"'
-                + ' xmlns="http://www.opengeospatial.org/standards/wcs"'
-                + ' xmlns:gml="http://www.opengis.net/gml"'
-                + ' xmlns:xlink="http://www.w3.org/1999/xlink">'
-                + secttxt + '</CoverageDescription>'
-            )
-            try:
-                coverage = coverages_from_xml(secttxt)
-                coverages.extend(coverage)
-            except Exception as e:
-                try:
-                    secttxt = cleanre.sub(
-                        '</name></CoverageOffering>', secttxt
-                    )
-                    coverage = coverages_from_xml(secttxt)
-                    coverages.extend(coverage)
-                    limited_details.append(coverage[0]["name"])
-                except Exception as e2:
-                    # If a secondary error was raised, print it... but raise
-                    # the original error
-                    print(e)
-                    raise e2
-
-        nlimited = len(limited_details)
-        if nlimited > 0 and verbose > 0:
-            limitedstr = ', '.join(limited_details)
-            warnings.warn(
-                f'Limited details for {nlimited} coverages: {limitedstr}'
-            )
-
-        if as_dataframe:
-            coverages = pd.DataFrame.from_records(coverages)
-            coverages['bbox_str'] = coverages['bbox_str'].fillna(
-                '-180 -90 180 90'
-            )
-            coverages['endPosition'] = coverages['endPosition'].fillna('now')
-            coverages['prefix'] = coverages['name'].apply(
-                lambda x: x.split('.')[0]
+        from .data import get_descriptions
+        if self._coveragesdf is None:
+            self._coveragesdf = get_descriptions(
+                server=self.server, refresh=refresh
             )
-            coverages = coverages.drop('tag', axis=1)
-            self._coveragesdf = coverages
-            # If you have arrived here, it means the file did not exist
-            # or was intended to be refreshed. So, make it.
-            os.makedirs(os.path.dirname(descpath), exist_ok=True)
-            self._coveragesdf.to_csv(descpath, index=False)
-
-        return coverages
+        return self._coveragesdf
 
     def capabilities(self, as_dataframe=True, refresh=False, verbose=0):
         """
         At this time, the capabilities does not list cmaq.*
         """
         import re
         import pandas as pd
@@ -877,40 +436,38 @@
         Arguments
         ---------
         offline : bool
             If True, uses small cached set of tested coverages.
             If False, finds all coverages from capabilities service.
 
         """
-        if offline:
-            keys = tuple(_keys)
-        else:
-            keys = sorted(self.capabilities(refresh=True).name.unique())
-
+        descdf = self.descriptions(refresh=not offline)
+        keys = tuple(sorted(descdf['name'].unique()))
         return keys
 
     def get_file(
         self, formatstr, key=None, bdate=None, edate=None, bbox=None,
         grid=False, request='GetCoverage', compress=0, overwrite=None,
         verbose=0
     ):
         """
         Build url, outpath, and download the file. Returns outpath
 
         """
+        from .utils import get_file
         if overwrite is None:
             overwrite = self.overwrite
         url, outpath = self._build_url(
             formatstr, key=key, bdate=bdate, edate=edate, bbox=bbox,
             grid=grid, request=request, compress=compress
         )
         if verbose > 0:
             print(url)
 
-        _getfile(url, outpath, verbose=verbose, overwrite=overwrite)
+        get_file(url, outpath, verbose=verbose, overwrite=overwrite)
 
         return outpath
 
     def _build_url(
         self, formatstr, key=None, bdate=None, edate=None, bbox=None,
         grid=False, request='GetCoverage',
         compress=1
@@ -1029,18 +586,18 @@
                 '{maximum_difference}&MAXIMUM_RATIO={maximum_ratio}'
                 '&AGGREGATE={freq}&MINIMUM_AGGREGATION_COUNT_PERCENTAGE='
                 '{agg_pct}&DEFAULT_HUMIDITY={default_humidity}&KEY={api_key}'
             ).format(**purpleair_kw)
         else:
             purpleairstr = ''
 
-        if any([key.startswith(pre) for pre in _nocorner_prefixes]):
-            cornerstr = ''
-        else:
+        if any([key.startswith(pre) for pre in _corner_prefixes]):
             cornerstr = f'&CORNERS={corners}'
+        else:
+            cornerstr = ''
 
         if any([key.startswith(pre) for pre in _nolonlats_prefixes]):
             nolonlatsstr = '&NOLONLATS=1'
         else:
             nolonlatsstr = ''
 
         url = (
@@ -1138,14 +695,16 @@
         -------
         df : pandas.DataFrame
             Results from download
 
         """
         from . import xdr
         assert backend in {'ascii', 'xdr'}
+        if key.startswith('hms.'):
+            backend = 'xdr'
         outpath = self.get_file(
             backend, key=key, bdate=bdate, edate=edate, bbox=bbox,
             grid=False, verbose=verbose,
             compress=1
         )
         if backend == 'ascii':
             df = pd.read_csv(outpath, delimiter='\t', na_values=[-9999., -999])
```

### Comparing `pyrsig-0.8.2/pyrsig/cmaq/__init__.py` & `pyrsig-0.8.4/pyrsig/cmaq/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,19 +42,34 @@
         ods.attrs['FTYPE'] = 1
     elif 'PERIM' in ds[outkeys[0]].dims:
         ods.attrs['FTYPE'] = 2
 
     assert len(set([k[:16] for k in outkeys])) == nv
     varlist = ''.join([k[:16].ljust(16) for k in outkeys])
     dates = pd.to_datetime(ds.TSTEP.values)
-    dt = np.diff(dates).astype('d').max() / 1e9
+    if len(dates) == 1:
+        if 'TSTEP' in ds.attrs:
+            # A bit circular here, but parsing TSTEP as definitive when there
+            # is no time coordinate.
+            tstep = ds.attrs['TSTEP']
+            tstepstr = f'{tstep:06d}'
+            dts = int(tstepstr[-2:])
+            dtm = int(tstepstr[-4:-2])
+            dth = int(tstepstr[:-4])
+            dt = dth * 3600 + dtm * 60 + dts
+        else:
+            # Assume 24h, which is like typical rsig
+            dt = 24 * 3600
+    else:
+        dt = np.diff(dates).astype('d').max() / 1e9
 
     dth = dt // 3600
     dtm = (dt % 3600) // 60
     dts = (dt % 60) // 1
+    tstepstr = f'{dth:.0f}{dtm:02.0f}{dts:02.0f}'
     timec = pd.to_datetime(
         ds.TSTEP.min().values
         + np.arange(len(dates)) * pd.to_timedelta(dt, unit='s')
     )
     jdays = timec.strftime('%Y%j').astype('i')
     hms = timec.strftime('%H%M%S').astype('i')
     ods['TFLAG'] = xr.DataArray(
@@ -62,50 +77,56 @@
         attrs=dict(
             long_name='TFLAG'.ljust(16), units='<YYYYJJJ,HHMMSS>',
             var_desc='Time flag'.ljust(80)
         )
     ).expand_dims(VAR=nv).transpose('TSTEP', 'VAR', 'DATE-TIME')
     ods.attrs['SDATE'] = int(ods['TFLAG'][0, 0, 0])
     ods.attrs['STIME'] = int(ods['TFLAG'][0, 0, 1])
-    ods.attrs['TSTEP'] = int(f'{dth:.0f}{dtm:02.0f}{dts:02.0f}')
+    ods.attrs['TSTEP'] = int(tstepstr)
 
     for dk in outkeys:
         ok = dk[:16]
-        ods[ok] = ds[dk].copy()
+        ods[ok] = ds[dk].astype('f')
         vprops = ods[ok].attrs
         vprops['long_name'] = vprops.get('long_name', ok)[:16].ljust(16)
         vprops['var_desc'] = vprops.get('var_desc', ok)[:80].ljust(80)
         vprops['units'] = vprops.get('units', 'unknown')[:16].ljust(16)
+        ods[ok].encoding.update(ds[dk].encoding)
 
     now = pd.to_datetime('now', utc=True)
     props['CDATE'] = props['WDATE'] = int(now.strftime('%Y%j'))
     props['CTIME'] = props['WTIME'] = int(now.strftime('%H%M%S'))
-    props['NCOLS'], props['NROWS'] = ds.dims['COL'], ds.dims['ROW']
-    props['NLAYS'], props['NVARS'] = ds.dims['LAY'], ods.dims['VAR']
+    props['NCOLS'], props['NROWS'] = ds.sizes['COL'], ds.sizes['ROW']
+    props['NLAYS'], props['NVARS'] = ds.sizes['LAY'], ods.sizes['VAR']
     props['XORIG'] = float(props['XORIG'] + ds.COL.min() - 0.5)
     props['YORIG'] = float(props['YORIG'] + ds.COL.min() - 0.5)
-    s = [1]
+    s = [1.]
     for i, sm in enumerate(ods.LAY):
         s.append(2 * sm - s[-1])
 
     props['VAR-LIST'] = varlist
     props['VGLVLS'] = np.array(s, dtype='f')
     props['UPNAM'] = f'pyrsig {__version__}'.ljust(16)
     defprops = {
+        'EXECUTION_ID': '????'.ljust(80),
         'IOAPI_VERSION': 'not applicable'.ljust(16), 'EXEC_ID': '?'.ljust(80),
         'FTYPE': 1, 'NTHIK': 1, 'GDTYP': 2, 'P_ALP': 33.0, 'P_BET': 45.0,
         'P_GAM': -97.0, 'XCENT': -97.0, 'YCENT': 40.0,
         'VGTYP': -9999, 'VGTOP': np.float32(5000.0),
-        'GDNAM': f'{"UNKNOWN":16s}'.ljust(16), 'metadata': ''
+        'GDNAM': f'{"UNKNOWN":16s}'.ljust(16), 'metadata': '',
+        'FILEDESC': ''.ljust(80 * 60), 'UPNAM': 'pyrsig'.ljust(16),
+        'HISTORY': 'pyrsig.cmaq.save_ioapi'.ljust(80 * 60)
     }
-
+    ods.attrs.update(props)
     for pk, pdef in defprops.items():
         ods.attrs.setdefault(pk, pdef)
 
-    return ods.to_netcdf(path, format=format, **kwds)
+    coords = list(ods.coords)
+    odds = ods.drop_indexes(coords).reset_coords(coords, drop=True)
+    return odds.to_netcdf(path, format=format, **kwds)
 
 
 def open_ioapi(path, metapath=None, earth_radius=6370000.):
     """
     Open an IOAPI file, add coordinate data, and optionally add RSIG metadata.
 
     Arguments
```

### Comparing `pyrsig-0.8.2/pyrsig/cmaq/pair.py` & `pyrsig-0.8.4/pyrsig/cmaq/pair.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/pyrsig/tests/test_api.py` & `pyrsig-0.8.4/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/pyrsig/tests/test_coards.py` & `pyrsig-0.8.4/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/pyrsig/tests/test_dataframes.py` & `pyrsig-0.8.4/pyrsig/tests/test_dataframes.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,25 @@
         )
         ds = rsigapi.to_dataframe(
             'pandora.L2_rnvh3p1_8.tropospheric_nitrogen_dioxide'
         )
         print(ds.shape)
 
 
+def test_hmssmoke():
+    from .. import RsigApi
+    import tempfile
+
+    with tempfile.TemporaryDirectory() as td:
+        bbox = (-80, 30, -60, 50)
+        rsigapi = RsigApi(bdate='2023-03-01', bbox=bbox, workdir=td)
+        ds = rsigapi.to_dataframe('hms.smoke')
+        print(ds.shape)
+
+
 def test_viirsnoaa():
     from .. import RsigApi
     import tempfile
 
     with tempfile.TemporaryDirectory() as td:
         rsigapi = RsigApi(
             bdate='2022-03-01', bbox=(-85, 30, -70, 45), workdir=td
```

### Comparing `pyrsig-0.8.2/pyrsig/tests/test_gui.py` & `pyrsig-0.8.4/pyrsig/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/pyrsig/tests/test_ioapi.py` & `pyrsig-0.8.4/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.8.2/pyrsig/xdr.py` & `pyrsig-0.8.4/pyrsig/xdr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 __all__ = ['from_xdrfile', 'from_xdr']
 
 
-def from_xdrfile(path, na_values=None, decompress=None):
+def from_xdrfile(path, na_values=None, decompress=None, as_dataframe=True):
     """
     Currently supports profile, site and swath (v2.0). Each is in XDR format
     with a custom set of header rows in text format. The text header rows also
     describe the binary portion of the file.
 
     Arguments
     ---------
     path : str
         Path to file in XDR format with RSIG headers
     decompress : bool
         If None, use decompress if path ends in .gz
         If True, decompress buffer.
         If False, buffer is already decompressed (or was never compressed)
+    as_dataframe : bool
+        If True (default), return data as a pandas.Dataframe.
+        If False, return a xarray.Dataset. Only subset and grid support
+        as_dataframe.
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
     """
     if decompress is None:
         decompress = path.endswith('.gz')
     with open(path, 'rb') as inf:
         buf = inf.read()
-        return from_xdr(buf, decompress=decompress, na_values=na_values)
+        return from_xdr(
+            buf, decompress=decompress, na_values=na_values,
+            as_dataframe=as_dataframe
+        )
 
 
-def from_xdr(buffer, na_values=None, decompress=False):
+def from_xdr(buffer, na_values=None, decompress=False, as_dataframe=True):
     """
     Currently supports profile, site and swath (v2.0). Each is in XDR format
     with a custom set of header rows in text format. The text header rows also
     describe the binary portion of the file.
 
     Infers RSIG format using first 40 characters.
 
@@ -40,17 +47,23 @@
     * Profile 2.0: from_profile
     * Swath 2.0: from_swath
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
+    na_values : scalar
+        Used to remove known missing values.
     decompress : bool
         If True, decompress buffer.
         If False, buffer is already decompressed (or was never compressed)
+    as_dataframe : bool
+        If True (default), return data as a pandas.Dataframe.
+        If False, return a xarray.Dataset. Only subset and grid support
+        as_dataframe.
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
     """
     import gzip
@@ -65,35 +78,90 @@
         df = from_site(buffer)
     elif defspec.startswith('point'):
         df = from_point(buffer)
     elif defspec.startswith('swath'):
         df = from_swath(buffer)
     elif defspec.startswith('calipso'):
         df = from_calipso(buffer)
+    elif defspec.startswith('polygon'):
+        df = from_polygon(buffer)
+    elif defspec.startswith('grid'):
+        df = from_grid(buffer, as_dataframe=as_dataframe)
+    elif defspec.startswith('subset'):
+        df = from_subset(buffer, as_dataframe=as_dataframe)
     else:
-        raise IOError('{defspec} not in profile, site, swath')
+        raise IOError(f'{defspec} not in profile, site, swath')
 
     if na_values is not None:
         df = df.replace(na_values, np.nan)
 
     return df
 
 
+def from_polygon(buffer):
+    """
+    Currently supports Polygon (v1.0) which has 10 header rows in text format.
+    The text header rows also describe the binary portion of the file, which
+    includes three segments of data corresponding to shx, shp, and dbf files
+    embeded within the buffer.
+
+    Arguments
+    ---------
+    buffer : bytes
+        Data buffer in XDR format with RSIG headers
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Dataframe with XDR content
+    """
+    import io
+    import tempfile
+    import geopandas as gpd
+
+    bf = io.BytesIO(buffer)
+    for i in range(10):
+        _l = bf.readline().decode().strip()
+        if i == 0:
+            assert (_l.lower() == 'polygon 1.0')
+        if i == 2:
+            dates, datee = _l.replace(':', '').replace('-0000', 'Z').split()
+        elif i == 9:
+            prefix, shxn, shpn, dbfn = _l.split()
+            shxn = int(shxn)
+            shpn = int(shpn)
+            dbfn = int(dbfn)
+    shxs = bf.tell()
+    shxe = shxs + shxn
+    shps = shxe
+    shpe = shps + shpn
+    dbfs = shpe
+    dbfe = dbfs + dbfn
+    with tempfile.TemporaryDirectory() as td:
+        filestem = f'{td}/{prefix}_{dates}_{datee}'
+        with open(filestem + '.shx', 'wb') as shxf:
+            shxf.write(buffer[shxs:shxe])
+        with open(filestem + '.shp', 'wb') as shpf:
+            shpf.write(buffer[shps:shpe])
+        with open(filestem + '.dbf', 'wb') as dbff:
+            dbff.write(buffer[dbfs:dbfe])
+        outdf = gpd.read_file(filestem + '.shp')
+
+    return outdf
+
+
 def from_profile(buffer):
     """
     Currently supports Profile (v2.0) which has 14 header rows in text format.
     The text header rows also describe the binary portion of the file.
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
-    decompress : bool
-        If True, decompress buffer.
-        If False, buffer is already decompressed (or was never compressed)
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
 
     Notes
@@ -184,17 +252,14 @@
     Currently supports Swath (v2.0) which has 14 header rows in text format.
     The text header rows also describe the binary portion of the file.
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
-    decompress : bool
-        If True, decompress buffer.
-        If False, buffer is already decompressed (or was never compressed)
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
 
     Notes
@@ -284,17 +349,14 @@
     Currently supports Site (v2.0) which has 14 header rows in text format.
     The text header rows also describe the binary portion of the file.
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
-    decompress : bool
-        If True, decompress buffer.
-        If False, buffer is already decompressed (or was never compressed)
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
 
     Notes
@@ -401,17 +463,14 @@
     Currently supports Point (v1.0) which has 12 header rows in text format.
     The text header rows also describe the binary portion of the file.
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
-    decompress : bool
-        If True, decompress buffer.
-        If False, buffer is already decompressed (or was never compressed)
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
 
     Notes
@@ -491,17 +550,14 @@
     Currently supports Calipso (v1.0) which has 15 header rows in text format.
     The text header rows also describe the binary portion of the file.
 
     Arguments
     ---------
     buffer : bytes
         Data buffer in XDR format with RSIG headers
-    decompress : bool
-        If True, decompress buffer.
-        If False, buffer is already decompressed (or was never compressed)
 
     Returns
     -------
     df : pd.DataFrame
         Dataframe with XDR content
 
     Notes
@@ -610,14 +666,297 @@
         + pd.to_timedelta(df['Profile_UTC_Time'] % 1, unit='d')
     ).dt.round('1s')
     df = df[['Timestamp(UTC)'] + varkeys[1:-1] + varkeys[:1] + varkeys[-1:]]
     df.rename(columns=renamer, inplace=True)
     return df
 
 
+def from_grid(buffer, as_dataframe=True):
+    """
+    Currently supports Grid (v1.0) which has 12 header rows in text format.
+    The text header rows also describe the binary portion of the file.
+
+    Arguments
+    ---------
+    buffer : bytes
+        Data buffer in XDR format with RSIG headers
+    as_dataframe : bool
+        If True (default), return data as a pandas.Dataframe.
+        If False, return a xarray.Dataset.
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Dataframe with XDR content
+
+    Notes
+    -----
+    xdrdump master_hrrr_wind_2020-02-17.xdr
+    Grid 1.0
+    http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/,HRRRSubset
+    2020-02-17T00:00:00-0000
+    # Dimensions: timesteps variables rows columns:
+    24 2 85 73
+    # Variable names:
+    wind_u wind_v
+    # Variable units:
+    m/s m/s
+    # IEEE-754 64-bit reals longitudes[rows][columns] and
+    # IEEE-754 64-bit reals latitudes[rows][columns] and
+    # IEEE-754 64-bit reals data[timesteps][variables][rows][columns]:
+    -7.8518169999999998e+01
+    -7.8484610000000004e+01
+    -7.8451070000000001e+01
+    ...
+    """
+    import numpy as np
+    import pandas as pd
+    import io
+    import xarray as xr
+
+    bf = io.BytesIO(buffer)
+    headerlines = []
+    for i in range(12):
+        _l = bf.readline().decode().strip()
+        headerlines.append(_l)
+        if i == 0:
+            assert (_l.lower() == 'grid 1.0')
+        elif i == 1:
+            rsig_program = _l
+        elif i == 2:
+            stime = pd.to_datetime(_l)
+        elif i == 4:
+            ntime, nvar, nrow, ncol = np.array(_l.split(), dtype='i')
+        elif i == 6:
+            varkeys = _l.split()
+        elif i == 8:
+            units = _l.split()
+        elif i == 10:
+            # bbox = [float(d) for d in _l.strip().split()]
+            pass  # not loading time because it is duplicative
+
+    sdn = bf.tell()
+    # [rows][columns]:
+    slon = sdn
+    elon = slon + nrow * ncol * 8
+    # [rows][columns]:
+    slat = elon
+    elat = slat + nrow * ncol * 8
+    # [timesteps][variables][rows][columns]:
+    svar = elat
+    evar = svar + ntime * nvar * nrow * ncol * 8
+    lon = np.frombuffer(buffer[slon:elon], dtype='>d').reshape(nrow, ncol)
+    lat = np.frombuffer(buffer[slat:elat], dtype='>d').reshape(nrow, ncol)
+    data = np.frombuffer(buffer[svar:evar], dtype='>d').reshape(
+        ntime, nvar, nrow, ncol
+    )
+    ds = xr.Dataset()
+    ds.attrs['rsig_program'] = rsig_program
+    dt = pd.to_timedelta('3600s')
+    reftime = '1970-01-01T00:00:00+0000'
+    attrs = dict(units=f'seconds since {reftime}', long_name='time')
+    ds.coords['time'] = ('time',), stime + np.arange(ntime) * dt, attrs
+    attrs = dict(units='index', long_name='x_center')
+    ds.coords['x'] = ('x',), np.arange(ncol, dtype='d') + 0.5
+    attrs = dict(units='index', long_name='y_center')
+    ds.coords['y'] = ('y',), np.arange(nrow, dtype='d') + 0.5
+    attrs = dict(units='degrees_north', long_name='latitude')
+    ds['lat'] = ('y', 'x'), lat, attrs
+    attrs = dict(units='degrees_east', long_name='longitude')
+    ds['lon'] = ('y', 'x'), lon, attrs
+    for vi, varkey in enumerate(varkeys):
+        attrs = dict(long_name=varkey, units=units[vi])
+        ds[varkey] = ('time', 'y', 'x'), data[:, vi, :, :], attrs
+
+    if as_dataframe:
+        df = ds.to_dataframe().astype('d')
+        time = df.index.get_level_values('time')
+        df['Timestamp(UTC)'] = time.strftime('%Y-%m-%dT%H:%M:%S+0000')
+        keepcols = ['Timestamp(UTC)', 'lon', 'lat'] + varkeys
+        renamer = {vk: f'{vk}({vu})' for vk, vu in zip(varkeys, units)}
+        renamer['lon'] = 'LONGITUDE(deg)'
+        renamer['lat'] = 'LATITUDE(deg)'
+        df = df[keepcols].rename(columns=renamer)
+        return df
+    else:
+        return ds
+
+
+def from_subset(buffer, as_dataframe=True):
+    """
+    Currently supports Subset (v9.0) which has 17 header rows in text format.
+    The text header rows also describe the binary portion of the file. This
+    data can be very large for high resolution continental data. For example,
+    CMAQ EQUATES CONUS for one 4D variable requires 4GB of memory as a
+    dataframe whereas the same data from CMAQ EQUATES HEMI is just 0.065GB.
+    Both are much smaller as a Dataset where coordinate data is not repeated.
+
+    Arguments
+    ---------
+    buffer : bytes
+        Data buffer in XDR format with RSIG headers
+    as_dataframe : bool
+        If True (default), return data as a pandas.Dataframe.
+        If False, return a xarray.Dataset.
+
+    Returns
+    -------
+    df : pd.DataFrame
+        Dataframe with XDR content
+
+    Notes
+    -----
+    /xdrdump master_cmaq_amad_hemi_ext_2006-08-28.xdr |m
+    SUBSET 9.0 CMAQ
+    108NHEMI1
+    http://www.epa.gov/ttn/scram/,CMAQSubset
+    2006-08-28T00:00:00-0000
+    # data dimensions: timesteps variables layers rows columns:
+    1 4 35 187 187
+    # subset indices (0-based time, 1-based layer/row/column): first-timestep
+      ... last-timestep first-layer last-layer first-row last-row first-column
+      ... last-column:
+     0 0 1 35 1 187 1 187
+    # Variable names:
+    LONGITUDE LATITUDE ELEVATION EXT_Recon
+    # Variable units:
+    deg deg m 1/km
+    # stereographic projection: lat_0 lon_0 lat_sec major_semiaxis
+      ... minor_semiaxis
+    90 -98 45 6.37e+06 6.37e+06
+    # Grid: ncols nrows xorig yorig xcell ycell vgtyp vgtop vglvls[36]:
+    187 187 -1.0098e+07 -1.0098e+07 108000 108000 7 5000 1 0.9975 0.995 ...
+    # IEEE-754 32-bit reals data[variables][timesteps][layers][rows][columns]:
+    -1.4300000000000000e+02
+    -1.4269029235839844e+02
+    ...
+    """
+    import numpy as np
+    import pandas as pd
+    import io
+    import xarray as xr
+    from .utils import get_proj4
+    import pyproj
+
+    bf = io.BytesIO(buffer)
+    headerlines = []
+    for i in range(17):
+        _l = bf.readline().decode().strip()
+        headerlines.append(_l)
+        if i == 0:
+            assert (_l.lower() == 'subset 9.0 cmaq')
+        elif i == 1:
+            gdnam = _l
+        elif i == 2:
+            rsig_program = _l
+        elif i == 3:
+            stime = pd.to_datetime(_l)
+        elif i == 5:
+            ntime, nvar, nlay, nrow, ncol = np.array(_l.split(), dtype='i')
+        elif i == 7:
+            ftime, ltime, flay, llay, frow, lrow, fcol, lcol = np.array(
+                _l.split(), dtype='i'
+            )
+        elif i == 9:
+            varkeys = _l.split()
+        elif i == 11:
+            units = _l.split()
+        elif i == 12:
+            crshdr = _l.lower()
+        elif i == 13:
+            crsparts = np.array(_l.split(), dtype='d')
+        elif i == 15:
+            projparts = np.array(_l.split(), dtype='d')
+            vgparts = np.array(projparts[-nlay - 3:], dtype='f')
+            gridparts = projparts[:-len(vgparts)]
+
+    vgprops = {}
+    vgprops['VGTYP'] = np.int32(vgparts[0])
+    vgprops['VGTOP'] = np.float32(vgparts[1])
+    vglvls = vgprops['VGLVLS'] = np.array(vgparts[2:], dtype='f')
+    gridkeys = ['NCOLS', 'NROWS', 'XORIG', 'YORIG', 'XCELL', 'YCELL']
+    gridprops = dict(zip(gridkeys, gridparts))
+    projattrs = {'GDNAM': gdnam}
+    projattrs.update(gridprops)
+    crskeys = crshdr.split(': ')[-1].split()
+    crsprops = dict(zip(crskeys, crsparts))
+    earth_radius = crsprops['major_semiaxis']
+    if 'stereographic' in crshdr:
+        projattrs['GDTYP'] = 6
+        projattrs['P_ALP'] = crsprops['lat_0'] / 90
+        projattrs['XCENT'] = projattrs['P_BET'] = crsprops['lon_0']
+        projattrs['YCENT'] = crsprops['lat_0']
+        projattrs['P_GAM'] = crsprops['lat_sec']
+    elif 'lcc' in crshdr:
+        projattrs['GDTYP'] = 2
+        projattrs['P_ALP'] = crsprops['lat_1']
+        projattrs['P_BET'] = crsprops['lat_2']
+        projattrs['P_GAM'] = crsprops['lon_0']
+        projattrs['XCENT'] = crsprops['lon_0']
+        projattrs['YCENT'] = crsprops['lat_0']
+    else:
+        raise KeyError(f'Need implement {crshdr}')
+        # projattrs['GDTYP'] = 7 # merc
+        # projattrs['GDTYP'] = 1 # lonlat
+
+    proj4 = get_proj4(projattrs, earth_radius=earth_radius)
+    proj = pyproj.Proj(proj4)
+    sdn = bf.tell()
+    data = np.frombuffer(buffer[sdn:], dtype='>f').reshape(
+        nvar, ntime, nlay, nrow, ncol
+    )
+    ds = xr.Dataset()
+    ds.attrs.update(**projattrs)
+    ds.attrs.update(**vgprops)
+    ds.attrs['UPNAM'] = rsig_program.ljust(16)
+    dt = pd.to_timedelta('3600s')
+    t = stime + np.arange(ntime) * dt
+    reftime = '1970-01-01T00:00:00+0000'
+    attrs = dict(long_name='TSTEP', units=f'seconds since {reftime}')
+    ds.coords['TSTEP'] = t
+    z = ((vglvls[1:] + vglvls[:-1]) / 2)[flay - 1:llay]
+    attrs = dict(long_name='LAY', units='layer_center')
+    ds.coords['LAY'] = ('LAY',), z, attrs
+    y = np.arange(nrow) + frow - 0.5
+    attrs = dict(long_name='ROW', units='cell_center')
+    ds.coords['ROW'] = ('ROW',), y, attrs
+    x = np.arange(ncol) + fcol - 0.5
+    attrs = dict(long_name='COL', units='cell_center')
+    ds.coords['COL'] = ('COL',), x, attrs
+    Y, X = xr.broadcast(ds['ROW'], ds['COL'])
+    LON, LAT = proj(X.values, Y.values, inverse=True)
+    attrs = dict(long_name='LONGITUDE'.ljust(16), units='degrees_east    ')
+    attrs['var_desc'] = attrs['long_name'].ljust(80)
+    ds['LONGITUDE'] = ('ROW', 'COL'), LON.astype('f'), attrs
+    attrs = dict(long_name='LATITUDE'.ljust(16), units='degrees_north   ')
+    attrs['var_desc'] = attrs['long_name'].ljust(80)
+    ds['LATITUDE'] = ('ROW', 'COL'), LAT.astype('f'), attrs
+    dims = ('TSTEP', 'LAY', 'ROW', 'COL')
+    for vi, vk in enumerate(varkeys):
+        attrs = dict(
+            units=units[vi].ljust(16), long_name=vk.ljust(16),
+            var_desc=vk.ljust(80)
+        )
+        vals = data[vi]
+        ds[vk] = dims, vals, attrs
+
+    if as_dataframe:
+        df = ds.astype('f').to_dataframe()
+        time = df.index.get_level_values('TSTEP')
+        df['Timestamp(UTC)'] = time.strftime('%Y-%m-%dT%H:%M:%S+0000')
+        keepcols = ['Timestamp(UTC)', 'LONGITUDE', 'LATITUDE'] + varkeys
+        renamer = {vk: f'{vk}({vu})' for vk, vu in zip(varkeys, units)}
+        renamer['LONGITUDE'] = 'LONGITUDE(deg)'
+        renamer['LATITUDE'] = 'LATITUDE(deg)'
+        df = df[keepcols].rename(columns=renamer)
+        return df
+    else:
+        return ds
+
+
 if __name__ == '__main__':
     import pyrsig
 
     baseurl = (
         'https://ofmpub.epa.gov/rsig/rsigserver?SERVICE=wcs&VERSION=1.0.0'
         + '&REQUEST=GetCoverage&FORMAT=xdr'
     )
```

### Comparing `pyrsig-0.8.2/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.8.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.8.2
+Version: 0.8.4
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
@@ -105,14 +105,19 @@
 # 3875
 ```
 
 ## Change Log
 
 Not all changes are listed, but notable changes are itemized for ease of review.
 
+* v0.8.4: Added support for Subset 9.0 CMAQ and Grid 1.0 xdr formats.
+          Updated keys to rely on descriptions (via DescribeCoverage).
+          Added utilites for basic polygon/cmaq intersections for HMS.
+* v0.8.3: Added xdr Polygon 1.0 format capability, added package
+          DescribeCoverage in data module and restructured utilities.
 * v0.8.2: Added xdr CALIPSO 1.0 format capability.
 * v0.8.1: Added xdr Point 1.0 format capability.
 * v0.8.0: Restructuring module code and adding CMAQ pairing.
 * v0.7.0: Added offline descriptions for review of space/time coverage.
 * v0.7.0: Added TEMPO options for screening
 * v0.6.0: Added latitude longitude grid pass thru support.
 * v0.5.1: Added convenience function for opening many IOAPI files at once.
```

### Comparing `pyrsig-0.8.2/setup.py` & `pyrsig-0.8.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,8 +27,10 @@
         "Development Status :: 4 - Beta",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         "pandas", "xarray", "requests"
     ],
+    include_package_data=True,
+    zip_safe=False
 )
```

