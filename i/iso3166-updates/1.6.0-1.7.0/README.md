# Comparing `tmp/iso3166-updates-1.6.0.tar.gz` & `tmp/iso3166_updates-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.6.0.tar", last modified: Tue Dec 12 16:56:10 2023, max compression
+gzip compressed data, was "iso3166_updates-1.7.0.tar", max compression
```

## Comparing `iso3166-updates-1.6.0.tar` & `iso3166_updates-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:56:10.668697 iso3166-updates-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26257 2023-12-12 16:56:10.668697 iso3166-updates-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:56:10.668697 iso3166-updates-1.6.0/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/iso3166_updates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   380278 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/iso3166_updates/iso3166-updates.json
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:56:10.668697 iso3166-updates-1.6.0/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26257 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-12 16:56:10.000000 iso3166-updates-1.6.0/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-12-12 16:56:10.668697 iso3166-updates-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2023-12-12 16:55:57.000000 iso3166-updates-1.6.0/setup.py
+-rw-r--r--   0        0        0     1059 2024-04-18 21:29:13.496417 iso3166_updates-1.7.0/LICENSE
+-rw-r--r--   0        0        0    26210 2024-04-18 21:29:13.496417 iso3166_updates-1.7.0/README.md
+-rw-r--r--   0        0        0     2794 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/README.md
+-rw-r--r--   0        0        0      803 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/__init__.py
+-rw-r--r--   0        0        0   369134 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/iso3166-updates.json
+-rw-r--r--   0        0        0    25216 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/iso3166_updates/iso3166_updates.py
+-rw-r--r--   0        0        0     1873 2024-04-18 21:29:13.500417 iso3166_updates-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    27994 1970-01-01 00:00:00.000000 iso3166_updates-1.7.0/PKG-INFO
```

### Comparing `iso3166-updates-1.6.0/PKG-INFO` & `iso3166_updates-1.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,252 +1,281 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.6.0
-Summary: ('A Python package that pulls the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest.',)
-Home-page: https://github.com/amckenna41/iso3166-updates
-Author: AJ McKenna, https://github.com/amckenna41
-Author-email: amckenna41@qub.ac.uk
-Maintainer: AJ McKenna
+Version: 1.7.0
+Summary: Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest.
 License: MIT
-Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
 Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,subdivisions,iso3166-1,alpha-2,alpha-3,selenium,chromedriver
-Platform: UNKNOWN
+Author: AJ Mckenna
+Author-email: amckenna41@qub.ac.uk
+Maintainer: AJ McKenna
+Maintainer-email: amckenna41@qub.ac.uk
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free For Educational Use
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Dist: iso3166 (>=2.1.1,<3.0.0)
+Project-URL: documentation, https://iso3166-updates.readthedocs.io/en/latest/
+Project-URL: homepage, https://iso3166-updates.com/api/
+Project-URL: repository, https://github.com/amckenna41/iso3166-updates
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
 
 # iso3166-updates 🌎
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/amckenna41/iso3166-updates/tree/main.svg?style=svg&circle-token=9b0c0a9f6cc032f255dc28842c95600401aa4426)](https://dl.circleci.com/status-badge/redirect/gh/amckenna41/iso3166-updates/tree/main)
 [![PythonV](https://img.shields.io/pypi/pyversions/iso3166-updates?logo=2)](https://pypi.org/project/iso3166-updates/)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+[![Documentation Status](https://readthedocs.org/projects/iso3166-updates/badge/?version=latest)](https://iso3166-updates.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
 <!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates) -->
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 <!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 
-<div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
-  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
-  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
+<div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
+  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
+  <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
 > Software and API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
 
-* The front-end <b>API</b> is available [here][api].
 * A <b>demo</b> of the software and API is available [here][demo_iso3166_updates].
 * A <b>demo</b> of the script used to pull and export all the latest updates is available [here][demo_get_all_iso3166_updates].
 * A <b>Medium</b> article that dives deeper into `iso3166-updates` is available [here][medium].
+* The front-end <b>API</b> is available [here][api].
+* The **documentation** for the software is available [here](https://iso3166-updates.readthedocs.io/en/latest/).
 
 Table of Contents
 -----------------
-  * [Introduction](#introduction)
-  * [API](#api)
-  * [Staying up to date](#staying-up-to-date)
-  * [Requirements](#requirements)
-  * [Installation](#installation)
-  * [Usage (iso3166-updates-Python-package)](#usage-iso3166-updates-Python-package)
-  * [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
-  * [Directories](#Directories)
-  * [Issues](#Issues)
-  * [Contact](#contact)
-  * [References](#references)
+- [Introduction](#introduction)
+- [API](#api)
+- [Documentation](#documentation)
+- [Staying up to date](#staying-up-to-date)
+- [Requirements](#requirements)
+- [Installation](#installation)
+- [Usage (iso3166-updates)](#usage-iso3166-updates-Python-package)
+- [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
+- [Directories](#Directories)
+- [Issues](#Issues)
+- [Contact](#contact)
+- [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a software and accompanying API that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui).
 
-The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
+The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these chantes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (up to $300) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API make it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free; with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2023-11-29. </strong>
-
 ### Intended Audience:
 
-This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 Last Updated
 ------------
-The list of ISO 3166 updates was last updated on <strong>Nov 2023</strong>. A log of the latest ISO 3166 updates can be seen in the [UPDATES.md][updates_md].
+The list of ISO 3166 updates was last updated on **March 2024**, with over **~950** individual published updates. A log of the latest ISO 3166 updates can be seen in the [UPDATES.md][updates_md]. 
+
+<!-- <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2024-02-29. </strong> -->
 
 API
 ---
 The main API endpoint is:
 
 > https://iso3166-updates.com/api
 
 The other endpoints available in the API are:
 * https://iso3166-updates.com/api/all
-* https://iso3166-updates.com/api/alpha2/<input_alpha2>
+* https://iso3166-updates.com/api/alpha/<input_alpha>
 * https://iso3166-updates.com/api/name/<input_name>
 * https://iso3166-updates.com/api/year/<input_year>
-* https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
+* https://iso3166-updates.com/api/alpha/<input_alpha>/year/<input_year>
 * https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
 * https://iso3166-updates.com/api/months/<input_month>
+* https://iso3166-updates.com/api/months/<input_month>/alpha/<input_alpha>
 
-The paths/endpoints available in the API are - `/api/all`, `/api/alpha2`, `/api/name`, `/api/year` and `/api/months`. 
+The paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
 
-* The `/api/all` path/endpoint returns all of the ISO 3166 updates/changes data for all countries.
+* `/api/all`: get all of the ISO 3166 updates/changes data for all countries.
 
-* The 2 letter alpha-2 country code can be appended to the **alpha2** path/endpoint e.g. <i>/api/alpha2/JP</i>. A single alpha-2 code or a list of them can be passed to the API e.g. <i>/api/alpha2/FR,DE,HU,ID,MA</i>. For redundancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be appened to the path e.g. <i>/api/alpha2/FRA,DEU,HUN,IDN,MAR</i>. The **alpha2** endpoint can be used in conjunction with the **year** endpoint to get the country updates for a specific country and year, in the format `api/alpha2/<input_alpha2>/year/<input_year>` or `api/year/<input_year>/alpha2/<input_alpha2>`. If an invalid alpha-2 code is input then an error will be returned.
+* `/api/alpha`: get all the ISO 3166 updates/changes data for one or more countries according to their ISO 3166-1 alpha-2, alpha-3 or numeric country codes. A single alpha code or a list of them can be passed to the API e.g. `/api/alpha/AL`, `/api/alpha/BW`, `/api/alpha/FR,DE,HUN,IDN,504`. If an invalid alpha code is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **month** endpoints to get the country updates for a specific country and year, and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/alpha/<input_alpha>/year/<input_year>` and `/api/alpha/<input_alpha>/months/<input_month>`, respectively.
 
-* The <b>name</b> parameter can be a country name as it is most commonly known in English, according to the ISO 3166-1. The name can similarly be appended to the **name** path/endpoint e.g. <i>/api/name/Denmark</i>. A single country name or list of them can be passed into the API e.g. <i>/name/France,Moldova,Benin</i>. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is <i>/api/name/Swede</i>. The **name** endpoint can be used in conjunction with the **year** endpoint to get the country updates for a specific country name and year, in the format `api/name/<input_name>/year/<input_year>`. If no country is found from the closeness function or an invalid name is input then an error will be returned.
+* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed into the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
 
-* The **year** parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year. The year value can be appended to the **year** path/endpoint e.g. <i>/api/year/2017, /api/year/2010-2015, /api/year/<2009, /api/year/>2002</i>. The **year** endpoint can be used in conjunction with the **alpha2** and **name** endpoints to get the country updates for a specific country and year, in the format `api/alpha2/<input_alpha2>/year/<input_year>` and `api/name/<input_name>/year/<input_year>`, respectively. If an invalid year is input then an error will be returned. 
+* `/api/year`: get all the ISO 3166 updates/changes data for one or more countries according to a specific year, year range, or a cut-off year to get updates less than/more than a year, e.g. `/api/year/2017`, `/api/year/2010-2015`, `/api/year/<2009`, `/api/year/>2002`. If an invalid year is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country and year. This will be in in the format `/api/alpha/<input_alpha>/year/<input_year>` and `/api/name/<input_name>/year/<input_year>`, respectively. 
 
-* The **months** parameter will gather all updates for 1 or more countries from an input number of months from the present day. The month value can be appended to the **months** path/endpoint e.g. <i>/api/months/12, /api/months/24</i>. If an invalid month value is input then an error will be returned.
+* `/api/months`: get all the ISO 3166 updates/changes data for one or more countries from an input number of months from the present day, e.g. `/api/months/12`, `/api/months/24`, `/api/months/50`. A month range can also be input to get the updates published within a specified range of months, with the start and end month separated by a '-' e.g. `/api/months/12-24`, `/api/months/36-50`. If an invalid month value is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country over the past number of months using their ISO 3166-1 alpha code or country name, respectively. This will be in the format: `/api/months/<input_month>/alpha/<input_alpha>` and `/api/months/<input_month>/name/<input_name>`, respectively.
 
-* The main API endpoint (`/` or `/api`) will return the homepage and API documentation.
+* `/api`: main homepage and API documentation.
 
 The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The full list of attributes available for each country are:
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 * Date Issued: date that the change was communicated.
 * Code/Subdivision change: overall summary of change/update made.
-* Description of change in newsletter: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Description of change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
 
-The API documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of the software and API are available [here][demo_iso3166_updates].
+Documentation
+-------------
+Documentation for the software and accompanying API is available on the software's [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/) page. Additionally the API's documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of both is also available [here][demo_iso3166_updates].
 
 <!-- <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png?raw=true" alt="gcp_arch" height="500" width="750"/>
 </p> -->
 
 Staying up to date
 ------------------
-The list of ISO 3166 updates was last updated on <strong>Nov 2023</strong>.
+The list of ISO 3166 updates was last updated on <strong>March 2024</strong>.
 
-The object storing all updates, both locally (iso3166-updates.json) for the software pacakge and on the API in GCP Storage bucket, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application.
+The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
 
 Additionally, a GitHub Issue in the custom-built [`iso3166-updates`](https://github.com/amckenna41/iso3166-updates), [`iso3166-2`](https://github.com/amckenna41/iso3166-2) and [`iso3166-flag-icons`](https://github.com/amckenna41/iso3166-flag-icons) repositories will be automatically created that formats and tabulates all updates/changes that need to be implemented into the JSONs on the aforementioned repos.
 
-Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest and most accurate ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the most latest, accurate and reliable ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.8
 * [iso3166][iso3166] >= 2.1.1 
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
 ```
 
-Installation from source:
-```bash
-git clone -b master https://github.com/amckenna41/iso3166-updates.git
-cd iso3166_updates
-python3 setup.py install
-```
-
 Usage (iso3166-updates Python package)
 --------------------------------------
 Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
-import iso3166_updates as iso
+from iso3166_updates import *
+```
+
+**Create instance of ISO3166_Updates() class**
+```python
+iso = ISO3166_Updates()
 ```
 
 **Get all listed changes/updates for all countries and years:**
 ```python
-iso.updates.all
+iso.all
 ```
 
 **Get all listed ISO 3166 changes/updates for Andorra (AD):**
 ```python
-iso.updates["AD"]
+iso["AD"]
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY:**
 ```python
-iso.updates["BA","DE","FR","HU","PY"]
+iso["BA","DE","FRA","HUN","600"]
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
+```python
+iso.year("2002, 2003, 2004")
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
+```python
+iso.year("2013-2016")
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
+```python
+iso.year(">2017")
+```
+
+**Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021:**
+```python
+iso.year("2012-2021").IE
 ```
 
-**Get any listed ISO 3166 changes/updates for Ireland, between the years 2012 and 2021:**
+**Get any listed ISO 3166 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
-iso.updates.year("2012-2021").IE
+iso.year(">2015").TA
 ```
 
-**Get any listed ISO 3166 changes/updates for Tanzania, with year >= 2015:**
+**Get any listed ISO 3166 changes/updates for Romania, with updates with year < 2007:**
 ```python
-iso.updates.year(">2015").TA
+iso.year("<2007").RO
 ```
 
-**Get any listed ISO 3166 changes/updates for Romania, with year < 2007:**
+**Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010:**
 ```python
-iso.updates.year("<2007").RO
+iso.year("<2010")["YE"]
 ```
 
-**Get any listed ISO 3166 changes/updates for Yemen, with year < 2010:**
+**Get any listed ISO 3166 changes/updates published over the past 12 months:**
 ```python
-iso.updates.year("<2010")["YE"]
+iso.months("12")
+```
+
+**Get any listed ISO 3166 changes/updates published over the past 36-48 months:**
+```python
+iso.months("36-48")
 ```
 
 Usage (get_all_iso3166_updates.py script)
 -----------------------------------------
 Below are some examples of using the `get_all_iso3166_updates.py` script which is used to pull all the ISO 3166 updates
 from the various data sources.
 
 **Requirements:**
 * [python][python] >= 3.8
 * [iso3166-updates][iso3166-updates] >= 1.3.0
 * [pandas][pandas] >= 1.4.4
-* [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 * [selenium][selenium] >= 4.10.0
 * [flask][flask] >= 2.3.2
 * [tqdm][tqdm] >= 4.64.0
 
 **Input parameters to get_updates function:**
 ```python
-  # -alpha2_codes ALPHA2_CODES, --alpha2_codes ALPHA2_CODES
-  #                       Alpha-2 code/s of the ISO 3166 countries to get updates from (default=[]-meaning use all country codes).
+  # -alpha_codes ALPHA_CODES, --alpha_codes ALPHA_CODES
+  #                       ISO 3166-1 alpha-2, alpha-3 or numeric code/s of the ISO 3166 countries to get updates from (default=[]-meaning use all country codes).
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
   #                       than or less than specified year (default=[]).
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files (default="iso3166-updates").
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO 3166 files (default="iso3166-updates-output").
   # -concat_updates CONCAT_UPDATES, --concat_updates CONCAT_UPDATES
-  #                       Whether to concatenate updates of individual countries into the same json file or seperate
-  #                       into seperate files (default=True).
+  #                       Whether to concatenate updates of individual countries into the same json file or separate
+  #                       into separate files (default=True).
   # -export_json EXPORT_JSON, --export_json EXPORT_JSON
   #                       Whether to export all found updates to json in export folder (default=True).
   # -export_csv EXPORT_CSV, --export_csv EXPORT_CSV
   #                       Whether to export all found updates to csv files in export folder (default=True).
   # -verbose VERBOSE, --verbose VERBOSE
   #                       Set to 1 to print out progress of updates function, 0 will not print progress (default=True).
   # -use_selenium USE_SELENIUM, --use_selenium USE_SELENIUM
@@ -271,15 +300,15 @@
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
 iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
-**Get any listed ISO 3166 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into seperate JSON files (concat_updates=False):**
+**Get any listed ISO 3166 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and separate updates into separate JSON files (concat_updates=False):**
 ```python
 iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
 #exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
 **Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
@@ -296,61 +325,60 @@
 **Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ``` -->
 
 The output files from the <i>get_all_iso3166_updates.py</i> script for the updates/changes to an ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change in Newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 * Date Issued: date that the change was communicated.
 * Code/Subdivision Change: overall summary of change/update made.
-* Description of change in newsletter: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
-| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change in Newsletter |   
+| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
 | Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
 | Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   "AD": [
       {
           "Date Issued": "2015-11-27",
           "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
-          "Code/Subdivision Change": "",
-          "Description of Change in Newsletter": "Update List Source."
+          "Code/Subdivision Change": "Update List Source.",
+          "Description of Change": ""
       },
       {
           "Date Issued": "2014-11-03",
           "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
-          "Code/Subdivision Change": "",
-          "Description of Change in Newsletter": "Update List Source."
+          "Code/Subdivision Change": "Update List Source.",
+          "Description of Change": ""
       },
       {
           "Date Issued": "2007-04-17",
           "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf).",
           "Code/Subdivision Change": "Subdivisions added: 7 parishes.",
-          "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements."
+          "Description of Change": "Addition of the administrative subdivisions and of their code elements."
       }
   ]
 }
 ```
 
-Directories 📁
---------------
-* `/docs` - documentation for `iso3166-updates` Python package.
+Directories 
+-----------
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
-* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file (Update: API moved to serverless app on Vercel platform to save on resources).
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all ISO 3166 countries, ensuring the API and jsons are reliable, accurate and up-to-date.
+* `/docs` - documentation for `iso3166-updates`, available on [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/).
 * `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
 * `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
 * `UPDATES.md` - log of all the latest updates from 2022 onwards. 
 
 Issues
 ------
@@ -375,19 +403,18 @@
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo_iso3166_updates]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [demo_get_all_iso3166_updates]: https://colab.research.google.com/drive/161aclDjGkWQJhis7KxBO1e6H_ghQOPRG?usp=sharing
 [api]: https://www.iso3166-updates.com/api
-[medium]: https://github.com/amckenna41/iso3166_updates
+[medium]: https://medium.com/@ajmckenna69/iso3166-updates-d06b817af3a7
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
-[numpy]: https://numpy.org/
 [tqdm]: https://github.com/tqdm/tqdm
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
 [google-cloud-storage]: https://cloud.google.com/python/docs/reference
 [google-api-python-client]: https://cloud.google.com/python/docs/reference
 [flask]: https://flask.palletsprojects.com/en/2.3.x/
@@ -396,8 +423,7 @@
 [selenium]: https://selenium-python.readthedocs.io/index.html
 [webdriver-manager]: https://pypi.org/project/webdriver-manager/
 [lxml]: https://lxml.de/
 [updates_md]: https://github.com/amckenna41/iso3166-updates/blob/main/UPDATES.md
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
 [Issues]: https://github.com/amckenna41/iso3166-updates/issues
-
```

### Comparing `iso3166-updates-1.6.0/README.md` & `iso3166_updates-1.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,217 +1,245 @@
 # iso3166-updates 🌎
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/amckenna41/iso3166-updates/tree/main.svg?style=svg&circle-token=9b0c0a9f6cc032f255dc28842c95600401aa4426)](https://dl.circleci.com/status-badge/redirect/gh/amckenna41/iso3166-updates/tree/main)
 [![PythonV](https://img.shields.io/pypi/pyversions/iso3166-updates?logo=2)](https://pypi.org/project/iso3166-updates/)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+[![Documentation Status](https://readthedocs.org/projects/iso3166-updates/badge/?version=latest)](https://iso3166-updates.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
 <!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates) -->
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 <!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 
-<div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
-  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
-  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
+<div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
+  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
+  <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
 > Software and API that checks for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package as well as an API. 
 
-* The front-end <b>API</b> is available [here][api].
 * A <b>demo</b> of the software and API is available [here][demo_iso3166_updates].
 * A <b>demo</b> of the script used to pull and export all the latest updates is available [here][demo_get_all_iso3166_updates].
 * A <b>Medium</b> article that dives deeper into `iso3166-updates` is available [here][medium].
+* The front-end <b>API</b> is available [here][api].
+* The **documentation** for the software is available [here](https://iso3166-updates.readthedocs.io/en/latest/).
 
 Table of Contents
 -----------------
-  * [Introduction](#introduction)
-  * [API](#api)
-  * [Staying up to date](#staying-up-to-date)
-  * [Requirements](#requirements)
-  * [Installation](#installation)
-  * [Usage (iso3166-updates-Python-package)](#usage-iso3166-updates-Python-package)
-  * [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
-  * [Directories](#Directories)
-  * [Issues](#Issues)
-  * [Contact](#contact)
-  * [References](#references)
+- [Introduction](#introduction)
+- [API](#api)
+- [Documentation](#documentation)
+- [Staying up to date](#staying-up-to-date)
+- [Requirements](#requirements)
+- [Installation](#installation)
+- [Usage (iso3166-updates)](#usage-iso3166-updates-Python-package)
+- [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
+- [Directories](#Directories)
+- [Issues](#Issues)
+- [Contact](#contact)
+- [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a software and accompanying API that consists of a series of scripts that check for any updates/changes to the ISO 3166 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui).
 
-The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
+The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations 🇺🇳 [[1]](#references). The ISO 3166-2 was first published in 1998 and as of November 2023 there are 5,039 codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these chantes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with and track these changes. These changes can occur for a variety of geopolitical and administrative reasons. Previously these changes were communicated via newsletters; but as of July 2013 these changes are now communicated via their online catalogue/Online Browsing Platform (OBP), or via a database, which usually costs money to subscribe to (up to $300) [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API make it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free; with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2023-11-29. </strong>
-
 ### Intended Audience:
 
-This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 Last Updated
 ------------
-The list of ISO 3166 updates was last updated on <strong>Nov 2023</strong>. A log of the latest ISO 3166 updates can be seen in the [UPDATES.md][updates_md].
+The list of ISO 3166 updates was last updated on **March 2024**, with over **~950** individual published updates. A log of the latest ISO 3166 updates can be seen in the [UPDATES.md][updates_md]. 
+
+<!-- <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2024-02-29. </strong> -->
 
 API
 ---
 The main API endpoint is:
 
 > https://iso3166-updates.com/api
 
 The other endpoints available in the API are:
 * https://iso3166-updates.com/api/all
-* https://iso3166-updates.com/api/alpha2/<input_alpha2>
+* https://iso3166-updates.com/api/alpha/<input_alpha>
 * https://iso3166-updates.com/api/name/<input_name>
 * https://iso3166-updates.com/api/year/<input_year>
-* https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
+* https://iso3166-updates.com/api/alpha/<input_alpha>/year/<input_year>
 * https://iso3166-updates.com/api/name/<input_name>/year/<input_year>
 * https://iso3166-updates.com/api/months/<input_month>
+* https://iso3166-updates.com/api/months/<input_month>/alpha/<input_alpha>
 
-The paths/endpoints available in the API are - `/api/all`, `/api/alpha2`, `/api/name`, `/api/year` and `/api/months`. 
+The paths/endpoints available in the API are - `/api/all`, `/api/alpha`, `/api/name`, `/api/year` and `/api/months`. 
 
-* The `/api/all` path/endpoint returns all of the ISO 3166 updates/changes data for all countries.
+* `/api/all`: get all of the ISO 3166 updates/changes data for all countries.
 
-* The 2 letter alpha-2 country code can be appended to the **alpha2** path/endpoint e.g. <i>/api/alpha2/JP</i>. A single alpha-2 code or a list of them can be passed to the API e.g. <i>/api/alpha2/FR,DE,HU,ID,MA</i>. For redundancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be appened to the path e.g. <i>/api/alpha2/FRA,DEU,HUN,IDN,MAR</i>. The **alpha2** endpoint can be used in conjunction with the **year** endpoint to get the country updates for a specific country and year, in the format `api/alpha2/<input_alpha2>/year/<input_year>` or `api/year/<input_year>/alpha2/<input_alpha2>`. If an invalid alpha-2 code is input then an error will be returned.
+* `/api/alpha`: get all the ISO 3166 updates/changes data for one or more countries according to their ISO 3166-1 alpha-2, alpha-3 or numeric country codes. A single alpha code or a list of them can be passed to the API e.g. `/api/alpha/AL`, `/api/alpha/BW`, `/api/alpha/FR,DE,HUN,IDN,504`. If an invalid alpha code is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **month** endpoints to get the country updates for a specific country and year, and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/alpha/<input_alpha>/year/<input_year>` and `/api/alpha/<input_alpha>/months/<input_month>`, respectively.
 
-* The <b>name</b> parameter can be a country name as it is most commonly known in English, according to the ISO 3166-1. The name can similarly be appended to the **name** path/endpoint e.g. <i>/api/name/Denmark</i>. A single country name or list of them can be passed into the API e.g. <i>/name/France,Moldova,Benin</i>. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is <i>/api/name/Swede</i>. The **name** endpoint can be used in conjunction with the **year** endpoint to get the country updates for a specific country name and year, in the format `api/name/<input_name>/year/<input_year>`. If no country is found from the closeness function or an invalid name is input then an error will be returned.
+* `/api/name`: get all the ISO 3166 updates/changes data for one or more countries according to their country name, as listed in the ISO 3166-1. A single country name or list of them can be passed into the API e.g. `/api/name/Brazil`, `/api/name/Colombia`, `/api/name/Benin,France,Moldova`. A closeness function is used to get the most approximate available country from the one input, e.g. Sweden will be used if the input is `/api/name/Swede`. If no matching country is found from the closeness function or an invalid name is input then an error will be returned. This endpoint can be used in conjunction with the **year** and **months** endpoint to get the country updates for a specific country name and year and the country updates for a specific country over the past number of months, respectively. This will be in the format: `/api/name/<input_name>/year/<input_year>` and `/api/name/<input_name>/months/<input_month>`, respectively. 
 
-* The **year** parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year. The year value can be appended to the **year** path/endpoint e.g. <i>/api/year/2017, /api/year/2010-2015, /api/year/<2009, /api/year/>2002</i>. The **year** endpoint can be used in conjunction with the **alpha2** and **name** endpoints to get the country updates for a specific country and year, in the format `api/alpha2/<input_alpha2>/year/<input_year>` and `api/name/<input_name>/year/<input_year>`, respectively. If an invalid year is input then an error will be returned. 
+* `/api/year`: get all the ISO 3166 updates/changes data for one or more countries according to a specific year, year range, or a cut-off year to get updates less than/more than a year, e.g. `/api/year/2017`, `/api/year/2010-2015`, `/api/year/<2009`, `/api/year/>2002`. If an invalid year is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country and year. This will be in in the format `/api/alpha/<input_alpha>/year/<input_year>` and `/api/name/<input_name>/year/<input_year>`, respectively. 
 
-* The **months** parameter will gather all updates for 1 or more countries from an input number of months from the present day. The month value can be appended to the **months** path/endpoint e.g. <i>/api/months/12, /api/months/24</i>. If an invalid month value is input then an error will be returned.
+* `/api/months`: get all the ISO 3166 updates/changes data for one or more countries from an input number of months from the present day, e.g. `/api/months/12`, `/api/months/24`, `/api/months/50`. A month range can also be input to get the updates published within a specified range of months, with the start and end month separated by a '-' e.g. `/api/months/12-24`, `/api/months/36-50`. If an invalid month value is input then an error will be returned. This endpoint can be used in conjunction with the **alpha** and **name** endpoints to get the country updates for a specific country over the past number of months using their ISO 3166-1 alpha code or country name, respectively. This will be in the format: `/api/months/<input_month>/alpha/<input_alpha>` and `/api/months/<input_month>/name/<input_name>`, respectively.
 
-* The main API endpoint (`/` or `/api`) will return the homepage and API documentation.
+* `/api`: main homepage and API documentation.
 
 The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The full list of attributes available for each country are:
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 * Date Issued: date that the change was communicated.
 * Code/Subdivision change: overall summary of change/update made.
-* Description of change in newsletter: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Description of change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
 
-The API documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of the software and API are available [here][demo_iso3166_updates].
+Documentation
+-------------
+Documentation for the software and accompanying API is available on the software's [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/) page. Additionally the API's documentation is available on the API [homepage](https://iso3166-updates.com/api). A demo of both is also available [here][demo_iso3166_updates].
 
 <!-- <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png?raw=true" alt="gcp_arch" height="500" width="750"/>
 </p> -->
 
 Staying up to date
 ------------------
-The list of ISO 3166 updates was last updated on <strong>Nov 2023</strong>.
+The list of ISO 3166 updates was last updated on <strong>March 2024</strong>.
 
-The object storing all updates, both locally (iso3166-updates.json) for the software pacakge and on the API in GCP Storage bucket, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application.
+The object storing all updates - iso3166-updates.json - for the software package is consistently checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes from the various data sources, to check for the latest updates within a certain period e.g. the past 6-12 months (this month range is used as the ISO usually publishes their updates at the end of the year with occasional mid-year updates). The app compares the generated output with that of the updates JSON currently in the software package and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to call the application on the aforementioned schedule. 
 
 Additionally, a GitHub Issue in the custom-built [`iso3166-updates`](https://github.com/amckenna41/iso3166-updates), [`iso3166-2`](https://github.com/amckenna41/iso3166-2) and [`iso3166-flag-icons`](https://github.com/amckenna41/iso3166-flag-icons) repositories will be automatically created that formats and tabulates all updates/changes that need to be implemented into the JSONs on the aforementioned repos.
 
-Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest and most accurate ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and associated APIs are up-to-date with the most latest, accurate and reliable ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.8
 * [iso3166][iso3166] >= 2.1.1 
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
 ```
 
-Installation from source:
-```bash
-git clone -b master https://github.com/amckenna41/iso3166-updates.git
-cd iso3166_updates
-python3 setup.py install
-```
-
 Usage (iso3166-updates Python package)
 --------------------------------------
 Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
-import iso3166_updates as iso
+from iso3166_updates import *
+```
+
+**Create instance of ISO3166_Updates() class**
+```python
+iso = ISO3166_Updates()
 ```
 
 **Get all listed changes/updates for all countries and years:**
 ```python
-iso.updates.all
+iso.all
 ```
 
 **Get all listed ISO 3166 changes/updates for Andorra (AD):**
 ```python
-iso.updates["AD"]
+iso["AD"]
 ```
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY:**
 ```python
-iso.updates["BA","DE","FR","HU","PY"]
+iso["BA","DE","FRA","HUN","600"]
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
+```python
+iso.year("2002, 2003, 2004")
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
+```python
+iso.year("2013-2016")
+```
+
+**Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
+```python
+iso.year(">2017")
+```
+
+**Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021:**
+```python
+iso.year("2012-2021").IE
+```
+
+**Get any listed ISO 3166 changes/updates for Tanzania, with updates with year >= 2015:**
+```python
+iso.year(">2015").TA
 ```
 
-**Get any listed ISO 3166 changes/updates for Ireland, between the years 2012 and 2021:**
+**Get any listed ISO 3166 changes/updates for Romania, with updates with year < 2007:**
 ```python
-iso.updates.year("2012-2021").IE
+iso.year("<2007").RO
 ```
 
-**Get any listed ISO 3166 changes/updates for Tanzania, with year >= 2015:**
+**Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010:**
 ```python
-iso.updates.year(">2015").TA
+iso.year("<2010")["YE"]
 ```
 
-**Get any listed ISO 3166 changes/updates for Romania, with year < 2007:**
+**Get any listed ISO 3166 changes/updates published over the past 12 months:**
 ```python
-iso.updates.year("<2007").RO
+iso.months("12")
 ```
 
-**Get any listed ISO 3166 changes/updates for Yemen, with year < 2010:**
+**Get any listed ISO 3166 changes/updates published over the past 36-48 months:**
 ```python
-iso.updates.year("<2010")["YE"]
+iso.months("36-48")
 ```
 
 Usage (get_all_iso3166_updates.py script)
 -----------------------------------------
 Below are some examples of using the `get_all_iso3166_updates.py` script which is used to pull all the ISO 3166 updates
 from the various data sources.
 
 **Requirements:**
 * [python][python] >= 3.8
 * [iso3166-updates][iso3166-updates] >= 1.3.0
 * [pandas][pandas] >= 1.4.4
-* [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 * [selenium][selenium] >= 4.10.0
 * [flask][flask] >= 2.3.2
 * [tqdm][tqdm] >= 4.64.0
 
 **Input parameters to get_updates function:**
 ```python
-  # -alpha2_codes ALPHA2_CODES, --alpha2_codes ALPHA2_CODES
-  #                       Alpha-2 code/s of the ISO 3166 countries to get updates from (default=[]-meaning use all country codes).
+  # -alpha_codes ALPHA_CODES, --alpha_codes ALPHA_CODES
+  #                       ISO 3166-1 alpha-2, alpha-3 or numeric code/s of the ISO 3166 countries to get updates from (default=[]-meaning use all country codes).
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
   #                       than or less than specified year (default=[]).
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files (default="iso3166-updates").
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO 3166 files (default="iso3166-updates-output").
   # -concat_updates CONCAT_UPDATES, --concat_updates CONCAT_UPDATES
-  #                       Whether to concatenate updates of individual countries into the same json file or seperate
-  #                       into seperate files (default=True).
+  #                       Whether to concatenate updates of individual countries into the same json file or separate
+  #                       into separate files (default=True).
   # -export_json EXPORT_JSON, --export_json EXPORT_JSON
   #                       Whether to export all found updates to json in export folder (default=True).
   # -export_csv EXPORT_CSV, --export_csv EXPORT_CSV
   #                       Whether to export all found updates to csv files in export folder (default=True).
   # -verbose VERBOSE, --verbose VERBOSE
   #                       Set to 1 to print out progress of updates function, 0 will not print progress (default=True).
   # -use_selenium USE_SELENIUM, --use_selenium USE_SELENIUM
@@ -236,15 +264,15 @@
 
 **Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
 iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
-**Get any listed ISO 3166 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into seperate JSON files (concat_updates=False):**
+**Get any listed ISO 3166 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and separate updates into separate JSON files (concat_updates=False):**
 ```python
 iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
 #exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
 **Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
@@ -261,61 +289,60 @@
 **Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ``` -->
 
 The output files from the <i>get_all_iso3166_updates.py</i> script for the updates/changes to an ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change in Newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision Change</b> and <b>Description of Change.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
 * Date Issued: date that the change was communicated.
 * Code/Subdivision Change: overall summary of change/update made.
-* Description of change in newsletter: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
-| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change in Newsletter |   
+| Edition/Newsletter | Date Issued | Code/Subdivision Change | Description of Change |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
 | Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
 | Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   "AD": [
       {
           "Date Issued": "2015-11-27",
           "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
-          "Code/Subdivision Change": "",
-          "Description of Change in Newsletter": "Update List Source."
+          "Code/Subdivision Change": "Update List Source.",
+          "Description of Change": ""
       },
       {
           "Date Issued": "2014-11-03",
           "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD).",
-          "Code/Subdivision Change": "",
-          "Description of Change in Newsletter": "Update List Source."
+          "Code/Subdivision Change": "Update List Source.",
+          "Description of Change": ""
       },
       {
           "Date Issued": "2007-04-17",
           "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf).",
           "Code/Subdivision Change": "Subdivisions added: 7 parishes.",
-          "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements."
+          "Description of Change": "Addition of the administrative subdivisions and of their code elements."
       }
   ]
 }
 ```
 
-Directories 📁
---------------
-* `/docs` - documentation for `iso3166-updates` Python package.
+Directories 
+-----------
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
-* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file (Update: API moved to serverless app on Vercel platform to save on resources).
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all ISO 3166 countries, ensuring the API and jsons are reliable, accurate and up-to-date.
+* `/docs` - documentation for `iso3166-updates`, available on [readthedocs](https://iso3166-updates.readthedocs.io/en/latest/).
 * `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
 * `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
 * `UPDATES.md` - log of all the latest updates from 2022 onwards. 
 
 Issues
 ------
@@ -340,19 +367,18 @@
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo_iso3166_updates]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [demo_get_all_iso3166_updates]: https://colab.research.google.com/drive/161aclDjGkWQJhis7KxBO1e6H_ghQOPRG?usp=sharing
 [api]: https://www.iso3166-updates.com/api
-[medium]: https://github.com/amckenna41/iso3166_updates
+[medium]: https://medium.com/@ajmckenna69/iso3166-updates-d06b817af3a7
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
-[numpy]: https://numpy.org/
 [tqdm]: https://github.com/tqdm/tqdm
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
 [google-cloud-storage]: https://cloud.google.com/python/docs/reference
 [google-api-python-client]: https://cloud.google.com/python/docs/reference
 [flask]: https://flask.palletsprojects.com/en/2.3.x/
```

### Comparing `iso3166-updates-1.6.0/iso3166_updates/README.md` & `iso3166_updates-1.7.0/iso3166_updates/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,66 +9,66 @@
 
 Usage
 -----
 Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
-import iso3166_updates as iso
+from iso3166_updates import *
+```
+
+**Create instance of ISO3166_Updates() class**
+```python
+iso = ISO3166_Updates()
 ```
 
 **Get all listed changes/updates for all countries and years:**
 ```python
-iso.updates.all
+iso.all
 ```
 
 **Get all listed ISO 3166 changes/updates for Andorra (AD):**
 ```python
-iso.updates["AD"]
+iso["AD"]
 ```
 
-**Get all listed ISO 3166 changes/updates for BA, DE, FR, HU, PY:**
+**Get all listed ISO 3166 changes/updates for BA, DE, FRA, HUN, PY (600):**
 ```python
-iso.updates["BA","DE","FR","HU","PY"]
+iso["BA","DE","FRA","HUN","600"]
 ```
 
 **Get all listed ISO 3166 changes/updates for all countries, for years 2002, 2003 and 2004:**
 ```python
-iso.updates.year("2002, 2003, 2004")
+iso.year("2002, 2003, 2004")
 ```
 
 **Get all listed ISO 3166 changes/updates for all countries, for year range 2013-2016:**
 ```python
-iso.updates.year("2013-2016")
+iso.year("2013-2016")
 ```
 
 **Get all listed ISO 3166 changes/updates for all countries, for all years after 2017 inclusive:**
 ```python
-iso.updates.year(">2017")
-```
-
-**Get any listed ISO 3166 changes/updates for Ireland, between years 2012 and 2021:**
-```python
-iso.updates.year("2012-2021").IE
+iso.year(">2017")
 ```
 
-**Get any listed ISO 3166 changes/updates for Tanzania, with updates with year >= 2015:**
+**Get all listed ISO 3166 changes/updates for all countries, for all years before 2010:**
 ```python
-iso.updates.year(">2015").TA
+iso.year("<2010")
 ```
 
-**Get any listed ISO 3166 changes/updates for Romania, with updates with year < 2007:**
+**Get all listed ISO 3166 changes/updates published from the past 12 months:**
 ```python
-iso.updates.year("<2007").RO
+iso.months("12")
 ```
 
-**Get any listed ISO 3166 changes/updates for Yemen, with updates with year < 2010:**
+**Get all listed ISO 3166 changes/updates published from the past 36-48 months:**
 ```python
-iso.updates.year("<2010")["YE"]
+iso.months("36-48")
 ```
 
 The output to the above functions for the updates/changes to an ISO 3166 country returns 4 attributes: 
 
-* Edition/Newsletter: Name and or edition of newsletter that the ISO 3166 change/update was communicated in.
-* Date Issued: Date that the change was communicated.
-* Code/Subdivision change: Overall summary of change/update made.
-* Description of change in newsletter: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
+* Edition/Newsletter: name and or edition of newsletter that the ISO 3166 change/update was communicated in (pre 2013), or the link to the country's ISO Online Browsing Platform page.
+* Date Issued: date that the change was communicated.
+* Code/Subdivision change: overall summary of change/update made.
+* Description of Change: more in-depth info about the change/update that was made, including any remarks listed on the official ISO page.
```

### Comparing `iso3166-updates-1.6.0/iso3166_updates/__init__.py` & `iso3166_updates-1.7.0/iso3166_updates/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .iso3166_updates import *
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.6.0"
-__description__ = "A Python package that pulls the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest."
+__version__ = "1.7.0"
+__description__ = "Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Production'
 __maintainer__ = "AJ McKenna"
```

### Comparing `iso3166-updates-1.6.0/iso3166_updates/iso3166-updates.json` & `iso3166_updates-1.7.0/iso3166_updates/iso3166-updates.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7649457252921112%*

 * *Differences: {"'AD'": "{0: {'Code/Subdivision Change': 'Update List Source.', 'Description of Change': '', "*

 * *         "delete: ['Description of Change in Newsletter']}, 1: {'Code/Subdivision Change': 'Update "*

 * *         "List Source.', 'Description of Change': '', delete: ['Description of Change in "*

 * *         "Newsletter']}, 2: {'Description of Change': 'Addition of the administrative subdivisions "*

 * *         "and of their code elements.', delete: ['Description of Change in Newsletter']}}",*

 * * "'AE'": "{0: {'Code/Subdivisio […]*

```diff
@@ -1,6016 +1,6046 @@
 {
     "AD": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 7 parishes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "AE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of AE-AJ, AE-RK; addition of local variation of AE-FK, AE-RK, AE-UQ; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of AE-AJ, AE-RK; addition of local variation of AE-FK, AE-RK, AE-UQ; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Spelling correction in AE-AZ.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Error correction: Spelling correction in AE-AZ.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in AE-RK.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling correction in AE-RK.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "AF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the local short name; change romanization system; change of spelling of categories of pus and fas; change of spelling of AF-KNR; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Correction of the local short name; change romanization system; change of spelling of categories of pus and fas; change of spelling of AF-KNR; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AF)."
         },
         {
             "Code/Subdivision Change": "Codes: AF-LOW Lowgar -> AF-LOG L\u014dgar AF-ORU Or\u016bzg\u0101n -> AF-URU Uruzg\u0101n.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Language corrections, administrative name corrections, alphabetical re-ordering and source list update.",
+            "Description of Change": "Language corrections, administrative name corrections, alphabetical re-ordering and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: AF-DAY D\u0101ykond\u012b AF-PAN Panjsh\u012br.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Addition of 2 provinces. Update of list source.",
+            "Description of Change": "Addition of 2 provinces. Update of list source.",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: AF-KHO Khowst AF-NUR N\u016brest\u0101n.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Addition of 2 provinces. Update of list source.",
+            "Description of Change": "Addition of 2 provinces. Update of list source.",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20081218103224/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         }
     ],
     "AG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change spelling of AG-04.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change spelling of AG-04.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AG)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: AG-11 Redonda.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 6 parishes, 1 dependency.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "AI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AI)."
         }
     ],
     "AL": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from pr\u00e9fecture to comt\u00e9 in French; deletion of all districts; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision category from pr\u00e9fecture to comt\u00e9 in French ; deletion of all districts ; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Separation of the variant local short names by semi-colon.",
             "Date Issued": "2014-04-03",
-            "Description of Change in Newsletter": "Separation of the variant local short names by semi-colon.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AL)."
         },
         {
             "Code/Subdivision Change": "Codes: format changed (leading digit 0 added).",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "Addition of the country code prefix as the first code element.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of generic term for administrative divisions. New list source.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Change of generic term for administrative divisions. New list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20081218103224/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 12 prefectures (now called counties) Codes: AL-LA La\u00e7 -> AL-KB Kurbin.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Introduction of 12 prefectures with their code elements. One district name and its code element changed. One district name corrected. Attribution of the prefecture code element to each district.",
+            "Description of Change": "Introduction of 12 prefectures with their code elements. One district name and its code element changed. One district name corrected. Attribution of the prefecture code element to each district.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "AM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AM)."
         }
     ],
     "AO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of AO-CCU, AO-CNO, AO-CUS, AO-LNO, AO-LSU; Addition of local variation for AO-CCU, AO-CNO, AO-CUS; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of AO-CCU, AO-CNO, AO-CUS, AO-LNO, AO-LSU; Addition of local variation for AO-CCU, AO-CNO, AO-CUS; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling of AO-CCU.",
             "Date Issued": "2015-02-12",
-            "Description of Change in Newsletter": "Correct spelling of AO-CCU.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling of AO-CNO and AO-CUS.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Correct spelling of AO-CNO and AO-CUS.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change spelling of AO-CNO, AO-CUS, and AO-CCU; update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change spelling of AO-CNO, AO-CUS, and AO-CCU; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in AO-ZAI.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling correction in AO-ZAI.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "AQ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AQ)."
         }
     ],
     "AR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of a name and update of the list and code sources.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Typographical correction of a name and update of the list and code sources.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "AS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-AS)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-AS)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AS)."
         }
     ],
     "AT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from federal L\u00e4nder to state; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision category from federal L\u00e4nder to state; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AT)."
         }
     ],
     "AU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source; update Code Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Update List Source; update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AU)."
         },
         {
             "Code/Subdivision Change": "Codes: New South Wales: AU-NS -> AU-NSW Queensland: AU-QL -> AU-QLD Tasmania: AU-TS -> AU-TAS Victoria: AU-VI -> AU-VIC Australian Capital Territory: AU-CT -> AU-ACT.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Change of subdivision code in accordance with Australian Standard AS 4212-1994.",
+            "Description of Change": "Change of subdivision code in accordance with Australian Standard AS 4212-1994.",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20081218103224/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         }
     ],
     "AW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-AW)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-AW)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the alpha 3 administrative language code pap.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of the alpha 3 administrative language code pap.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "AX": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct administrative languages.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Correct administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct administrative languages.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Correct administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AX)."
         }
     ],
     "AZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the romanization system; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of the romanization system; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:AZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: AZ-KAN K\u01ddng\u01ddrli AZ-NV Nax\u00e7\u0131van (municipality) Subdivisions deleted: AZ-SS \u015eu\u015fa Codes: AZ-AB \u018fli Bayraml\u0131 -> AZ-SR \u015eirvan AZ-DAV D\u0259v\u0259\u00e7i -> AZ-SBN \u015eabran AZ-XAN Xanlar -> AZ-GYG G\u00f6yg\u00f6l.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering, name change of administrative places, first level prefix addition and source list update.",
+            "Description of Change": "Alphabetical re-ordering, name change of administrative places, first level prefix addition and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: Nax\u00e7\u0131van: AZ-MM -> AZ-NX.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Correction of one code and four spelling errors. Notification of the rayons belonging to the autonomous republic.",
+            "Description of Change": "Correction of one code and four spelling errors. Notification of the rayons belonging to the autonomous republic.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "BA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-22",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of all cantons BA-01 to BA-10.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of all cantons BA-01 to BA-10.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct typographic error for the language code for Croatian.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Correct typographic error for the language code for Croatian.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BA)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BA-BRC Br\u010dko distrikt.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 10 cantons.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-2).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-2).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "BB": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BB)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 11 parishes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "BD": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of BD-03, BD-06, BD-08, BD-10, BD-22, BD-A, BD-B; Addition of local variation for BD-10, BD-B; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of BD-03, BD-06, BD-08, BD-10, BD-22, BD-A, BD-B; Addition of local variation for BD-10, BD-B; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of BD-24, BD-25, BD-29, BD-45; change of parent subdivision of BD-21, BD-34, BD-41, BD-55, BD-57; addition of parent subdivision BD-H; addition of an asterisk to divisions; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of BD-24, BD-25, BD-29, BD-45; change of parent subdivision of BD-21, BD-34, BD-41, BD-55, BD-57; addition of parent subdivision BD-H; addition of an asterisk to divisions; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct local short name and align with ISO 3166-2.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Correct local short name and align with ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BD-F Rangpur (division) Codes: Barisal (division) : BD-1 -> BD-A Chittagong (division) : BD-2 -> BD-B Dhaka (division) : BD-3 -> BD-C Khulna (division) : BD-4 -> BD-D Rajshahi (division) : BD-5 -> BD-E Sylhet (division) : BD-6 -> BD-G.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Country name romanization adjustment, first level prefix addition, deletion of generic terms, addition of administrative division and source list update.",
+            "Description of Change": "Country name romanization adjustment, first level prefix addition, deletion of generic terms, addition of administrative division and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BD-6 Sylhet bibhag Subdivisions deleted: 21 regions (see below).",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "New list source. One division added. 31 regions cancelled. Allocation of districts to divisions instead of regions. Correction of one spelling error.",
+            "Description of Change": "New list source. One division added. 31 regions cancelled. Allocation of districts to divisions instead of regions. Correction of one spelling error.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "BE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the parent subdivisions.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of the parent subdivisions.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "First level prefix addition, change of administrative languages and list source update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "First level prefix addition, change of administrative languages and list source update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "BF": [
         {
             "Code/Subdivision Change": "Spelling change: BF-TUI Tui -> Tuy.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of BF-TUI; update list source.",
+            "Description of Change": "Change of spelling of BF-TUI; update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the short name lowercase in French.",
             "Date Issued": "2014-04-15",
-            "Description of Change in Newsletter": "Correction of the short name lowercase in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BF)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 13 regions.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "BG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from region to district in eng and fra; update List Source.",
             "Date Issued": "2018-04-20",
-            "Description of Change in Newsletter": "Change of subdivision category from region to district in eng and fra; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of romanization system.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of romanization system.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment with ISO 3166-2 of the local short name Alignment with ISO 3166-2 of the local short name.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Alignment with ISO 3166-2 of the local short name Alignment with ISO 3166-2 of the local short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Local country name romanization system adjustment and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Local country name romanization system adjustment and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add the second romanized local name for Bulgaria.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Add the second romanized local name for Bulgaria.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add the second romanized local name for Bulgaria.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Add the second romanized local name for Bulgaria.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Application of the romanization system 26 October 2006.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Application of the romanization system 26 October 2006.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 9 regions (see below) -> 28 regions.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "New subdivision layout: Nine regions with former names (two remaining with former code). Ten regions with new names. New references for list source, code source and romanization system.",
+            "Description of Change": "New subdivision layout: Nine regions with former names (two remaining with former code). Ten regions with new names. New references for list source, code source and romanization system.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20081218103157/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "BH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name for BH-13; deletion of a governorate BH-16; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision name for BH-13; deletion of a governorate BH-16; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BH)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 12 regions (see below) -> 5 governorates.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "BI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BI)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: BI-RM Rumonge.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of one province BI-RM; update List Source.",
+            "Description of Change": "Addition of one province BI-RM; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BI)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BI-BM Bujumbura Mairie BI-BL Bujumbura Rural Subdivisions deleted: BI-BJ Bujumbura.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BI-MW Mwaro.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one province.",
+            "Description of Change": "Addition of one province.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "BJ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of BJ-AK, BJ-KO; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of BJ-AK, BJ-KO; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BJ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BJ-AL Alibori BJ-CO Collines BJ-DO Donga BJ-KO Kouffo BJ-LI Littoral BJ-PL Plateau.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "New subdivision layout: 12 departments. Six with previous names and six with new names.",
+            "Description of Change": "New subdivision layout: 12 departments. Six with previous names and six with new names.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "BL": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-BL)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-BL)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Barth\u00e9lemy\u201d in the French name field for Territory.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Barth\u00e9lemy\u201d in the French name field for Territory.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction to Newsletter VI-1.",
             "Date Issued": "2008-04-08",
-            "Description of Change in Newsletter": "Correction to Newsletter VI-1.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of new entry (in accordance with ISO 3166-1 Newsletter VI-1).",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of new entry (in accordance with ISO 3166-1 Newsletter VI-1).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add new entry.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Add new entry.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BL)."
         }
     ],
     "BM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BM)."
         }
     ],
     "BN": [
         {
             "Code/Subdivision Change": "Spelling change: BN-BM Brunei-Muara -> Brunei dan Muara (ms).",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Change of subdivision name of BN-BM; Update List Source.",
+            "Description of Change": "Change of subdivision name of BN-BM; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of subdivision category name in Malay; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of subdivision category name in Malay; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BN)."
         }
     ],
     "BO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a coma.",
+            "Date Issued": "2024-02-29",
+            "Description of Change": "",
+            "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BO)."
+        },
+        {
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short form country name in accordance with ISO 3166-1, NL VI-6 (2009-05-08).",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Change of short form country name in accordance with ISO 3166-1, NL VI-6 (2009-05-08).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short form country name in accordance with ISO 3166-1, NL VI-6 (2009-05-08).",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Change of short form country name in accordance with ISO 3166-1, NL VI-6 (2009-05-08).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short and full names.",
             "Date Issued": "2009-05-08",
-            "Description of Change in Newsletter": "Change of short and full names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BO)."
         }
     ],
     "BQ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of subdivision name of BQ-BO in pap (deleted leading space).",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Typographical correction of subdivision name of BQ-BO in pap (deleted leading space).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change in lower case the local short name.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change in lower case the local short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct local short name and align with ISO 3166-2.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Correct local short name and align with ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of code to align ISO 3166-1 and ISO 3166-2, addition of two divisions and update of the number of divisions.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of code to align ISO 3166-1 and ISO 3166-2, addition of two divisions and update of the number of divisions.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the English name to Sint Eustatius in alignment with United Nations Terminology and Reference Section (UNTERM).",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Correct the English name to Sint Eustatius in alignment with United Nations Terminology and Reference Section (UNTERM).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the English name to Sint Eustatius in alignment with United Nations Terminology and Reference Section (UNTERM).",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Correct the English name to Sint Eustatius in alignment with United Nations Terminology and Reference Section (UNTERM).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add new entry.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Add new entry.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BQ)."
         }
     ],
     "BR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of asterisk from state BR-TO; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Deletion of asterisk from state BR-TO; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BR)."
         }
     ],
     "BS": [
         {
             "Code/Subdivision Change": "Subdivision added: BS-NP New Providence.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of island BS-NP; Addition of Remark; Update List Source.",
+            "Description of Change": "Addition of island BS-NP; Addition of Remark; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BS)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: BS-GT Green Turtle Cay.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Correction of NL II-2 for toponyms and typographical errors, one deletion and source list update.",
+            "Description of Change": "Correction of NL II-2 for toponyms and typographical errors, one deletion and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 21 districts (see below) -> 32 districts (mistakenly listed as 31 districts in newsletter).",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "BT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of BT-43; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of BT-43; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of BT-13, BT-45; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of BT-13, BT-45; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BT)."
         }
     ],
     "BV": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BV)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct administrative language code from nbo to nob.",
             "Date Issued": "2014-04-03",
-            "Description of Change in Newsletter": "Correct administrative language code from nbo to nob.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BV)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add local short names.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Add local short names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BV)."
         }
     ],
     "BW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BW)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BW-CH Chobe BW-FR Francistown BW-GA \tGaborone BW-JW Jwaneng BW-LO Lobatse BW-SP Selibe Phikwe BW-ST Sowa Town Spelling changes: BW-NE North-East -> North East BW-NW North-West -> North West BW-SE South-East -> South East.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Add 1 district BW-CH, 2 cities BW-FR and BW-GA, 4 towns BW-JW, BW-LO, BW-SP, BW-ST; remove hyphens from BW-NE, BW-NW, and BW-SE; update List Source.",
+            "Description of Change": "Add 1 district BW-CH, 2 cities BW-FR and BW-GA, 4 towns BW-JW, BW-LO, BW-SP, BW-ST; remove hyphens from BW-NE, BW-NW, and BW-SE; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BW)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: BW-CH Chobe Codes: BW-NG Ngamiland -> BW-NW North-West.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Deletion of Chobe district which is incorporated into (new) BW-NW. Change of code element of North-West District to BW-NW. Deletion of alternative names. Update of list source.",
+            "Description of Change": "Deletion of Chobe district which is incorporated into (new) BW-NW. Change of code element of North-West District to BW-NW. Deletion of alternative names. Update of list source.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "BY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of spelling for BY-HR of BGN/PCGN 1979.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of spelling for BY-HR of BGN/PCGN 1979.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change romanization system from \"GOST 1983\" to \"Belarusian Lacinka\" of bel; change romanization system of BY-HM* of bel and rus.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change romanization system from \"GOST 1983\" to \"Belarusian Lacinka\" of bel; change romanization system of BY-HM* of bel and rus.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BY)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: BY-HM Horad Minsk.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of spelling mistakes and language code elements.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Correction of spelling mistakes and language code elements.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "BZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:BZ)."
         }
     ],
     "CA": [
         {
             "Code/Subdivision Change": "Name change: CA-YT Yukon Territory -> Yukon.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change spelling of CA-YT; update List Source.",
+            "Description of Change": "Change spelling of CA-YT; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CA)."
         },
         {
             "Code/Subdivision Change": "Codes: CA-NF Newfoundland -> CA-NL Newfoundland and Labrador.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Change of code element of Newfoundland and Labrador.",
+            "Description of Change": "Change of code element of Newfoundland and Labrador.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: CA-NF Newfoundland -> CA-NL Newfoundland and Labrador.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Correction of name form of CA-NF.",
+            "Description of Change": "Correction of name form of CA-NF.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CA-NU Nunavut.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Addition of 1 new territory.",
+            "Description of Change": "Addition of 1 new territory.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "CC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CC)."
         }
     ],
     "CD": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CD)."
         },
         {
             "Code/Subdivision Change": "Names changed: CD-BC, CD-KE Subdivisions deleted: CD-BN, CD-KA, CD-KW, CD-OR Subdivisions added: CD-BU, CD-HK, CD-HL, CD-HU, CD-IT, CD-KC, CD-KG, CD-KL, CD-KS, CD-LO, CD-LU, CD-MN, CD-MO, CD-NU, CD-SA, CD-SU, CD-TA, CD-TO, CD-TU.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision name of CD-BC, CD-KE; deletion of provinces CD-BN, CD-KA, CD-KW, CD-OR; addition of provinces CD-BU, CD-HK, CD-HL, CD-HU, CD-IT, CD-KC, CD-KG, CD-KL, CD-KS, CD-LO, CD-LU, CD-MN, CD-MO, CD-NU, CD-SA, CD-SU, CD-TA, CD-TO, CD-TU; update List Source.",
+            "Description of Change": "Change of subdivision name of CD-BC, CD-KE; deletion of provinces CD-BN, CD-KA, CD-KW, CD-OR; addition of provinces CD-BU, CD-HK, CD-HL, CD-HU, CD-IT, CD-KC, CD-KG, CD-KL, CD-KS, CD-LO, CD-LU, CD-MN, CD-MO, CD-NU, CD-SA, CD-SU, CD-TA, CD-TO, CD-TU; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CD)."
         },
         {
             "Code/Subdivision Change": "Codes: CD-HC Haut-Congo -> CD-OR Orientale.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "One subdivision name changed. Generic name of subdivisions changed. New reference in the list source.",
+            "Description of Change": "One subdivision name changed. Generic name of subdivisions changed. New reference in the list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "CF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct French full name and local short name to align with ISO 3166-2.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Correct French full name and local short name to align with ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of administrative language Sango (sg, sag).",
             "Date Issued": "2009-01-07",
-            "Description of Change in Newsletter": "Addition of administrative language Sango (sg, sag).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CF)."
         }
     ],
     "CG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the OBP entry error as follows: change of the font character from a dash to a hyphen in the name for Pointe-Noire.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the OBP entry error as follows: change of the font character from a dash to a hyphen in the name for Pointe-Noire.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 department CG-16.",
             "Date Issued": "2015-02-12",
-            "Description of Change in Newsletter": "Add 1 department CG-16.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change Subdivision category \u2018region\u2019 to \u2018department\u2019; change \u2018capital\u2019 to \u2018department\u2019; update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change Subdivision category \u2018region\u2019 to \u2018department\u2019; change \u2018capital\u2019 to \u2018department\u2019; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CG)."
         }
     ],
     "CH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of canton CH-GR in fra; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of canton CH-GR in fra; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction of CH-AI and CH-AR. New list source.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Spelling correction of CH-AI and CH-AR. New list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "CI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the French full name.",
             "Date Issued": "2022-09-02",
-            "Description of Change in Newsletter": "Correction of the French full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update Code Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of all regions CI-01 to CI-19; addition of districts CI-BS, CI-CM, CI-DN, CI-GD, CI-LC, CI-LG, CI-MG, CI-SM, CI-SV, CI-VB, CI-WR, CI-ZZ; addition of autonomous districts CI-AB, CI-YM; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of all regions CI-01 to CI-19; addition of districts CI-BS, CI-CM, CI-DN, CI-GD, CI-LC, CI-LG, CI-MG, CI-SM, CI-SV, CI-VB, CI-WR, CI-ZZ; addition of autonomous districts CI-AB, CI-YM; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CI)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CI-17 Bafing CI-18 Fromager CI-19 Moyen-Cavally.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "CK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CK)."
         }
     ],
     "CL": [
         {
             "Code/Subdivision Change": "Subdivisions added: CL-NB \u00d1uble.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of region CL-NB; Update List Source.",
+            "Description of Change": "Addition of region CL-NB; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CL)."
         },
         {
             "Code/Subdivision Change": "Spelling changes: CL-AI, CL-AR.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of CL-AR, CL-AI; addition of local variation of CL-AI, CL-LI; update list source.",
+            "Description of Change": "Change of spelling of CL-AR, CL-AI; addition of local variation of CL-AI, CL-LI; update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CL)."
         },
         {
             "Code/Subdivision Change": "Spelling changes: CL-AI, CL-BI.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change spelling of CL-AI and CL-BI; update List Source.",
+            "Description of Change": "Change spelling of CL-AI and CL-BI; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CL)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CL-AP Arica y Parinacota CL-LR Los R\u00edos.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "CM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CM)."
         }
     ],
     "CN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of CN-NX; Update List Source.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of spelling of CN-NX; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change language from mon to zho for CN-NM.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Change language from mon to zho for CN-NM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CN)."
         },
         {
             "Code/Subdivision Change": "Change of subdivision code: CN-11 -> CN-BJ CN-12 -> CN-TJ CN-13 -> CN-HE CN-14 -> CN-SX CN-15 -> CN-NM CN-21 -> CN-LN CN-22 -> CN-JL CN-23 -> CN-HL CN-31 -> CN-SH CN-32 -> CN-JS CN-33 -> CN-ZJ CN-34 -> CN-AH CN-35 -> CN-FJ CN-36 -> CN-JX CN-37 -> CN-SD CN-41 -> CN-HA CN-42 -> CN-HB CN-43 -> CN-HN CN-44 -> CN-GD CN-45 -> CN-GX CN-46 -> CN-HI CN-50 -> CN-CQ CN-51 -> CN-SC CN-52 -> CN-GZ CN-53 -> CN-YN CN-54 -> CN-XZ CN-61 -> CN-SN CN-62 -> CN-GS CN-63 -> CN-QH CN-64 -> CN-NX CN-65 -> CN-XJ CN-71 -> CN-TW CN-91 -> CN-HK CN-92 -> CN-MO.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of subdivision codes change of subdivision name of CN-NM, CN-GX, CN-XZ, CN-NX, CN-XJ, CN-BJ, CN-TJ, CN-SH, CN-CQ, CN-HE, CN-SX, CN-LN, CN-JL, CN-HL CN-JS, CN-ZJ, CN-AH, CN-FJ, CN-JX, CN-SD, CN-HA, CN-HB, CN-HN, CN-GD, CN-HI, CN-SC, CN-GZ, CN-YN, CN-SN, CN-GS, CN-QH, CN-TW, CN-HK, CN-MO addition of remark in parentheses to subdivision name for CN-HK, CN-MO in English addition of region CN-MO in Portuguese update code source update list source.",
+            "Description of Change": "Change of subdivision codes change of subdivision name of CN-NM, CN-GX, CN-XZ, CN-NX, CN-XJ, CN-BJ, CN-TJ, CN-SH, CN-CQ, CN-HE, CN-SX, CN-LN, CN-JL, CN-HL CN-JS, CN-ZJ, CN-AH, CN-FJ, CN-JX, CN-SD, CN-HA, CN-HB, CN-HN, CN-GD, CN-HI, CN-SC, CN-GZ, CN-YN, CN-SN, CN-GS, CN-QH, CN-TW, CN-HK, CN-MO addition of remark in parentheses to subdivision name for CN-HK, CN-MO in English addition of region CN-MO in Portuguese update code source update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of one name form in CN-15.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Deletion of one name form in CN-15.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20081218103224/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CN-92 Macau.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of one new entity. Precise specification and correction of Pinyin names. List source updated.",
+            "Description of Change": "Addition of one new entity. Precise specification and correction of Pinyin names. List source updated.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "CO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local variation of CO-DC, CO-SAP, CO-VAC; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of local variation of CO-DC, CO-SAP, CO-VAC; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of name of CO-DC.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Change of name of CO-DC.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         }
     ],
     "CR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CR)."
         }
     ],
     "CU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 2 provinces CU-15 and CU-16; delete CU-02; change name of CU-03; update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Add 2 provinces CU-15 and CU-16; delete CU-02; change name of CU-03; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CU)."
         }
     ],
     "CV": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CV)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the French remark.",
             "Date Issued": "2014-03-03",
-            "Description of Change in Newsletter": "Modification of the French remark.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CV)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "UN notification of name change for both short and full names.",
             "Date Issued": "2013-11-26",
-            "Description of Change in Newsletter": "UN notification of name change for both short and full names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CV)."
         },
         {
             "Code/Subdivision Change": "Codes: S\u00e3o Louren\u00e7o dos \u00d3rg\u00e3os CV-SL -> CV-SO.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Correction of NL II-2 for toponyms and typographical errors and source list update.",
+            "Description of Change": "Correction of NL II-2 for toponyms and typographical errors and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CV-RB Ribeira Brava CV-RS Ribeira Grande de Santiago CV-CF Santa Catarina do Fogo CV-SL S\u00e3o Louren\u00e7o dos \u00d3rg\u00e3os CV-SS S\u00e3o Salvador do Mundo CV-TS Tarrafal de S\u00e3o Nicolau Subdivisions deleted: CV-SN S\u00e3o Nicolau Codes: CV-CS Calheta de S\u00e3o Miguel -> CV-SM S\u00e3o Miguel.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, update of the administrative structure and of the list source.",
+            "Description of Change": "Addition of the country code prefix as the first code element, update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: CV-CS Calheta de S\u00e3o Miguel CV-MO Mosteiros CV-SF S\u00e3o Filipe.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Subdivision layout partially revised: Three new municipalities. New reference for list source.",
+            "Description of Change": "Subdivision layout partially revised: Three new municipalities. New reference for list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "CW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-CW)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-CW)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add new entry.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Add new entry.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CW)."
         }
     ],
     "CX": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CX)."
         }
     ],
     "CY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update Code Source; update List Source.",
             "Date Issued": "2018-04-20",
-            "Description of Change in Newsletter": "Update Code Source; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source; change of spelling of CY-02, CY-04 (tur).",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Update List Source; change of spelling of CY-02, CY-04 (tur).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CY)."
         }
     ],
     "CZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
             "Code/Subdivision Change": "Change of subdivision name: CZ-10 Praha, Hlavn\u00ed me\u0161to -> Praha, Hlavn\u00ed m\u011bsto CZ-802 Fr\u00fddek M\u00edstek -> Fr\u00fddek-M\u00edstek.",
             "Date Issued": "2020-03-02",
-            "Description of Change in Newsletter": "Typographical correction of subdivision name of CZ-10, CZ-802; Typographical correction of subdivision category name in Czech.",
+            "Description of Change": "Typographical correction of subdivision name of CZ-10, CZ-802; Typographical correction of subdivision category name in Czech.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
             "Code/Subdivision Change": "Deletion of subdivision code: CZ-101 CZ-102 CZ-103 CZ-104 CZ-105 CZ-106 CZ-107 CZ-108 CZ-109 CZ-110 CZ-111 CZ-112 CZ-113 CZ-114 CZ-115 CZ-116 CZ-117 CZ-118 CZ-119 CZ-120 CZ-121 CZ-122.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Deletion of districts CZ-101, CZ-102, CZ-103, CZ-104, CZ-105, CZ-106, CZ-107, CZ-108, CZ-109, CZ-110, CZ-111, CZ-112, CZ-113, CZ-114, CZ-115, CZ-116, CZ-117, CZ-118, CZ-119, CZ-120, CZ-121, CZ-122 ; Update List Source.",
+            "Description of Change": "Deletion of districts CZ-101, CZ-102, CZ-103, CZ-104, CZ-105, CZ-106, CZ-107, CZ-108, CZ-109, CZ-110, CZ-111, CZ-112, CZ-113, CZ-114, CZ-115, CZ-116, CZ-117, CZ-118, CZ-119, CZ-120, CZ-121, CZ-122; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
             "Code/Subdivision Change": "Change of subdivision code: CZ-621 -> CZ-641 CZ-624 -> CZ-644 CZ-622 -> CZ-642 CZ-623 -> CZ-643 CZ-611 -> CZ-631 CZ-612 -> CZ-632 CZ-613 -> CZ-633 CZ-10A -> CZ-110 CZ-10B -> CZ-111 CZ-10C -> CZ-112 CZ-10D -> CZ-113 CZ-0E -> CZ-114 CZ-10F -> CZ-115 CZ-614 -> CZ-634 CZ-626 -> CZ-646 CZ-615 -> CZ-635 CZ-627 -> CZ-647 CZ-PR -> CZ-10.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of category name of \u201ccapital city\u201d in eng, fra, ces; change of subdivision category of CZ-10 from region to capital city; change of spelling of CZ-802, CZ-806, CZ-63; typographical correction of CZ-615; addition of districts CZ-116 to CZ-122; change of parent subdivision from CZ-JC to CZ-31, CZ-JM to CZ-64, CZ-KA to CZ-41, CZ-KR to CZ-52, CZ-LI to CZ-51, Z-O to CZ-80, CZ-OL to CZ-71, CZ-PA to CZ-53, CZ-PL to CZ-32, CZ-ST to CZ-20, CZ-US to CZ-42, CZ-VY to CZ-63, CZ-ZL to CZ-72; change of subdivision code from CZ-621 to CZ 641, CZ-624 to CZ 644; CZ-622 to CZ 642, CZ-623 to CZ 643, CZ-611 to CZ 631, CZ-612 to CZ 632, CZ-613 to CZ 633, CZ-10A to CZ 110, CZ-10B to CZ 111, CZ-10C to CZ 112, CZ-10D to CZ 113, CZ-0E to CZ 114, CZ-10F to CZ 115, CZ-614 to CZ 634, CZ-626 to CZ 646, CZ-615 to CZ 635, CZ-627 to CZ 647, CZ-PR to CZ-10; update List Source.",
+            "Description of Change": "Addition of category name of \u201ccapital city\u201d in eng, fra, ces; change of subdivision category of CZ-10 from region to capital city; change of spelling of CZ-802, CZ-806, CZ-63; typographical correction of CZ-615; addition of districts CZ-116 to CZ-122; change of parent subdivision from CZ-JC to CZ-31, CZ-JM to CZ-64, CZ-KA to CZ-41, CZ-KR to CZ-52, CZ-LI to CZ-51, Z-O to CZ-80, CZ-OL to CZ-71, CZ-PA to CZ-53, CZ-PL to CZ-32, CZ-ST to CZ-20, CZ-US to CZ-42, CZ-VY to CZ-63, CZ-ZL to CZ-72; change of subdivision code from CZ-621 to CZ 641, CZ-624 to CZ 644; CZ-622 to CZ 642, CZ-623 to CZ 643, CZ-611 to CZ 631, CZ-612 to CZ 632, CZ-613 to CZ 633, CZ-10A to CZ 110, CZ-10B to CZ 111, CZ-10C to CZ 112, CZ-10D to CZ 113, CZ-0E to CZ 114, CZ-10F to CZ 115, CZ-614 to CZ 634, CZ-626 to CZ 646, CZ-615 to CZ 635, CZ-627 to CZ 647, CZ-PR to CZ-10; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the short name.",
             "Date Issued": "2016-09-28",
-            "Description of Change in Newsletter": "Change of the short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:CZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 91 districts.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in CZ-PR and adjustment of name form in CZ-VY.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Spelling correction in CZ-PR and adjustment of name form in CZ-VY.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Spelling correction and correction of word order in CZ-VY. List of subdivision names resorted.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Error correction: Spelling correction and correction of word order in CZ-VY. List of subdivision names resorted.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 1 city, 7 regions (see below) -> 14 regions.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Completely new subdivision layout. New reference for the list source.",
+            "Description of Change": "Completely new subdivision layout. New reference for the list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "DE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of category name in eng.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of category name in eng.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Reinstate the remarks in Column 7 concerning the use of the code 280 which is transitionally reserved until 2040-10.",
             "Date Issued": "2013-07-02",
-            "Description of Change in Newsletter": "Reinstate the remarks in Column 7 concerning the use of the code 280 which is transitionally reserved until 2040-10.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Reinstate the remarks in Column 7 concerning the use of the code 280 provisionally until 2013-11-03.",
             "Date Issued": "2012-08-02",
-            "Description of Change in Newsletter": "Reinstate the remarks in Column 7 concerning the use of the code 280 provisionally until 2013-11-03.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete the remarks in Column 7 concerning the use of the code 280.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Delete the remarks in Column 7 concerning the use of the code 280.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DE)."
         }
     ],
     "DJ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of DJ-OB in ara.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of DJ-OB in ara.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add romanization system for Arabic; typographical correction of DJ-AS; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Add romanization system for Arabic; typographical correction of DJ-AS; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Language adjustment and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Language adjustment and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: DJ-AR Arta.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Change of generic term for administrative divisions. Addition of new region \"Arta\". New list source and code source.",
+            "Description of Change": "Change of generic term for administrative divisions. Addition of new region \"Arta\". New list source and code source.",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         }
     ],
     "DK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Local generic term is changed to singular, alphabetical re-ordering by generic term suppression and source list update.",
             "Date Issued": "2011-12-13",
-            "Description of Change in Newsletter": "Local generic term is changed to singular, alphabetical re-ordering by generic term suppression and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DK)."
         }
     ],
     "DM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DM)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 10 parishes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "DO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of DO-07; update List Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision name of DO-07; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Assign parent subdivision to DO-01.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Assign parent subdivision to DO-01.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add regi\u00f3n (region) as top-level of subdivisions; add 10 regions DO-33 to DO-42; change subdivision name of DO-03, DO-08 and DO-19; update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Add regi\u00f3n (region) as top-level of subdivisions; add 10 regions DO-33 to DO-42; change subdivision name of DO-03, DO-08 and DO-19; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DO)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: DO-31 San Jos\u00e9 de Ocoa DO-32 Santo Domingo.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-2).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         },
         {
             "Code/Subdivision Change": "Codes: format changed (see below).",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Introduction of new subdivision code elements taken from the Dominican Statistics Code. Correction of alphabetic sorting of subdivision names. Addition of 1 alternative name form.",
+            "Description of Change": "Introduction of new subdivision code elements taken from the Dominican Statistics Code. Correction of alphabetic sorting of subdivision names. Addition of 1 alternative name form.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "DZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of province DZ-49, DZ-50, DZ-51, DZ-52, DZ-53, DZ-54, DZ-55, DZ-56, DZ-57, DZ-58; Update list source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Addition of province DZ-49, DZ-50, DZ-51, DZ-52, DZ-53, DZ-54, DZ-55, DZ-56, DZ-57, DZ-58; Update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of DZ-28; Update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of DZ-28; Update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision name of DZ-11; Update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Change subdivision name of DZ-11; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:DZ)."
         }
     ],
     "EC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of EC-S, EC-Z; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of EC-S, EC-Z; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EC)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: EC-SE Santa Elena EC-SD Santo Domingo de los Ts\u00e1chilas.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: EC-D Orellana.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one province.",
+            "Description of Change": "Addition of one province.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "EE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of category urban municipality, rural municipality; Addition of urban municipality EE-184, EE-296, EE-321, EE-424, EE-446, EE-511, EE-514, EE-567, EE-624, EE-663, EE-735, EE-784, EE-793, EE-897, EE-919; Addition of rural municipality EE-130, EE-141, EE-142, EE-171, EE-191, EE-198, EE-205, EE-214, EE-245, EE-247, EE-251, EE-255, EE-272, EE-283, EE-284, EE-291, EE-293, EE-303, EE-305, EE-317, EE-338, EE-353, EE-430, EE-431, EE-432, EE-441, EE-442, EE-478, EE-480, EE-486, EE-503, EE-528, EE-557, EE-586, EE-615, EE-618, EE-622, EE-638, EE-651, EE-653, EE-661, EE-668, EE-689, EE-698, EE-708, EE-712, EE-714, EE-719, EE-726, EE-732, EE-792, EE-796, EE-803, EE-809, EE-824, EE-834, EE-855, EE-890, EE-899, EE-901, EE-903, EE-907, EE-917, EE-928; Change of subdivision code from EE-44 to EE-45, EE-49 to EE-50, EE-51 to EE-52, EE-57 to EE-56, EE-59 to EE-60, EE-65 to EE-64, EE-67 to EE-68, EE-70 to EE-71, EE-78 to EE-79, EE-82 to EE-81, EE-86 to EE-87; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of category urban municipality, rural municipality; Addition of urban municipality EE-184, EE-296, EE-321, EE-424, EE-446, EE-511, EE-514, EE-567, EE-624, EE-663, EE-735, EE-784, EE-793, EE-897, EE-919; Addition of rural municipality EE-130, EE-141, EE-142, EE-171, EE-191, EE-198, EE-205, EE-214, EE-245, EE-247, EE-251, EE-255, EE-272, EE-283, EE-284, EE-291, EE-293, EE-303, EE-305, EE-317, EE-338, EE-353, EE-430, EE-431, EE-432, EE-441, EE-442, EE-478, EE-480, EE-486, EE-503, EE-528, EE-557, EE-586, EE-615, EE-618, EE-622, EE-638, EE-651, EE-653, EE-661, EE-668, EE-689, EE-698, EE-708, EE-712, EE-714, EE-719, EE-726, EE-732, EE-792, EE-796, EE-803, EE-809, EE-824, EE-834, EE-855, EE-890, EE-899, EE-901, EE-903, EE-907, EE-917, EE-928; Change of subdivision code from EE-44 to EE-45, EE-49 to EE-50, EE-51 to EE-52, EE-57 to EE-56, EE-59 to EE-60, EE-65 to EE-64, EE-67 to EE-68, EE-70 to EE-71, EE-78 to EE-79, EE-82 to EE-81, EE-86 to EE-87; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EE)."
         }
     ],
     "EG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of conventional/anglicised names as local variation to EG-BA, EG-ALX, EG-GZ, EG-C, EG-LX, EG-WAD, EG-SUZ, EG-PTS, EG-DT, EG-JS, EG-SIN, EG-SHG.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of conventional/anglicised names as local variation to EG-BA, EG-ALX, EG-GZ, EG-C, EG-LX, EG-WAD, EG-SUZ, EG-PTS, EG-DT, EG-JS, EG-SIN, EG-SHG.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete EG-HU and EG-SU; update List Source.",
             "Date Issued": "2014-10-29",
-            "Description of Change in Newsletter": "Delete EG-HU and EG-SU; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EG)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: EG-SU As S\u0101dis min Ukt\u016bbar EG-HU \u1e28ulw\u0101n.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: EG-LX Al Uq\u015fur.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-3).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-3).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "EH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:EH)."
         }
     ],
     "ER": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ER)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add romanization system for Arabic; change of subdivision category name in Arabic from iql\u012bm to min\u0163aqah; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Add romanization system for Arabic; change of subdivision category name in Arabic from iql\u012bm to min\u0163aqah; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ER)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ER)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change the full name.",
             "Date Issued": "2012-08-02",
-            "Description of Change in Newsletter": "Change the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ER)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct local short name and align with ISO 3166-2.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Correct local short name and align with ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ER)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Country name romanization adjustment, language adjustment, alphabetical re-ordering and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Country name romanization adjustment, language adjustment, alphabetical re-ordering and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 10 provinces (see below) -> 6 provinces.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Introduction of a completely new subdivision layout.",
+            "Description of Change": "Introduction of a completely new subdivision layout.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "ES": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of ES-PM; Update List Source; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of ES-PM; Update List Source; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (remark: In the autonomous communities of Galicia, Catalonia and the Balearics, the respective regional languages are the sole official languages of toponymy. Castilian language forms are given in square brackets for information. For the autonomous communities of Navarra, Valencia and the Basque Country, with the exception of the province names Bizkaia and Gipuzkoa, the regional language has co-official status with Castilian (regional language forms are marked with an asterisk)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (remark: In the autonomous communities of Galicia, Catalonia and the Balearics, the respective regional languages are the sole official languages of toponymy. Castilian language forms are given in square brackets for information. For the autonomous communities of Navarra, Valencia and the Basque Country, with the exception of the province names Bizkaia and Gipuzkoa, the regional language has co-official status with Castilian (regional language forms are marked with an asterisk)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the English remark part 2; deletion of asterisk ES-BI, ES-SS.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Modification of the English remark part 2; deletion of asterisk ES-BI, ES-SS.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete ES-SS Guip\u00fazcoa spa and ES-BI Vizcaya spa; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Delete ES-SS Guip\u00fazcoa spa and ES-BI Vizcaya spa; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, update of the administrative structure, addition of names in administrative languages.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, update of the administrative structure, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ES)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use) Asturias, Principado de: ES-O -> ES-AS Cantabria (autonomous community): ES-S -> ES-CB La Rioja: (autonomous community): ES-LO -> ES-RI Madrid, Comunidad de: ES-M -> ES-MD Murcia, Regi\u00f3n de: ES-MU -> ES-MC Navarra, Comunidad Foral de: ES-NA -> ES-NC.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, update of the administrative structure, addition of names in administrative languages.",
+            "Description of Change": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, update of the administrative structure, addition of names in administrative languages.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Regional subdivision indicator corrected in ES-PM.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Error correction: Regional subdivision indicator corrected in ES-PM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: Illes Balears: ES-PM -> ES-IB (to correct duplicate use) ES-GE Gerona -> ES-GI Girona.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling correction and update in header information. Four corrections in spellings of subdivisions.",
+            "Description of Change": "Spelling correction and update in header information. Four corrections in spellings of subdivisions.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Code elements for autonomous communities withdrawn to correct the erroneous duplicate coding of the whole Spanish territory (see 4.1.1 of ISO 3166-2). Introduction of a third column stating a regional level of subdivision which is not coded (see 4.4. c) of ISO 3166-2). Introduction of 2 alternative name forms. Correction of 1 spelling error.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Code elements for autonomous communities withdrawn to correct the erroneous duplicate coding of the whole Spanish territory (see 4.1.1 of ISO 3166-2). Introduction of a third column stating a regional level of subdivision which is not coded (see 4.4. c) of ISO 3166-2). Introduction of 2 alternative name forms. Correction of 1 spelling error.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "ET": [
         {
             "Code/Subdivision Change": "Subdivisions added: ET-SW Southwest Ethiopia Peoples.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Addition of regional state ET-SW; Update List Source.",
+            "Description of Change": "Addition of regional state ET-SW; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ET-SI Sidama.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Addition of regional state ET-SI; Update List Source.",
+            "Description of Change": "Addition of regional state ET-SI; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
             "Code/Subdivision Change": "Category change: state -> regional state.",
             "Date Issued": "2019-04-09",
-            "Description of Change in Newsletter": "Change of eng subdivision category from state to regional state; Update List Source.",
+            "Description of Change": "Change of eng subdivision category from state to regional state; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the romanization system for subdivisions in eng; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of the romanization system for subdivisions in eng; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ET)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ET-DD Dire Dawa.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Change of generic name of one subdivision category to administration. Addition of an administration. Update of list sources.",
+            "Description of Change": "Change of generic name of one subdivision category to administration. Addition of an administration. Update of list sources.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "FI": [
         {
             "Code/Subdivision Change": "Name change: Satakunda -> Satakunta.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of spelling of FI-17; Update List Source.",
+            "Description of Change": "Change of spelling of FI-17; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update Code Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FI)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 6 provinces (see below) -> 19 regions.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative re-organization, deletion of useless information and the region names in English and French, source list and source code update.",
+            "Description of Change": "Administrative re-organization, deletion of useless information and the region names in English and French, source list and source code update.",
             "Edition/Newsletter": "Newsletter II-3[1]."
         }
     ],
     "FJ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Reinstatement of provinces deleted due to a technical glitch.",
             "Date Issued": "2016-11-22",
-            "Description of Change in Newsletter": "Reinstatement of provinces deleted due to a technical glitch.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Assign parent subdivision to FJ-01, FJ-02, FJ-03, FJ-04, FJ-05, FJ-06, FJ-07, FJ-08, FJ-09, FJ-10, FJ-11, FJ-12, FJ-13, FJ-14.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Assign parent subdivision to FJ-01, FJ-02, FJ-03, FJ-04, FJ-05, FJ-06, FJ-07, FJ-08, FJ-09, FJ-10, FJ-11, FJ-12, FJ-13, FJ-14.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add provinces FJ-01 to FJ 14; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Add provinces FJ-01 to FJ 14; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Official name change of long name.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Official name change of long name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Official name change of long name.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Official name change of long name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FJ)."
         }
     ],
     "FK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FK)."
         }
     ],
     "FM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a coma and correct the remark in English of the entry of Micronesia Federate states (removing duplicated text).",
+            "Date Issued": "2024-02-29",
+            "Description of Change": "",
+            "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FM)."
+        },
+        {
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FM)."
         }
     ],
     "FO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FO)."
         }
     ],
     "FR": [
         {
             "Code/Subdivision Change": "Codes added: FR-6AE Alsace FR-69M M\u00e9tropole de Lyon Codes changed: FR-75 Paris (metropolitan department) -> FR-75C Paris (metropolitan collectivity with special status) Codes removed: FR-GF Guyane (fran\u00e7aise) FR-GP Guadeloupe FR-MQ Martinique FR-RE La R\u00e9union FR-YT Mayotte Category changes: FR-971 overseas department -> overseas departmental collectivity FR-972 overseas department -> overseas unique territorial collectivity FR-973 overseas department -> overseas unique territorial collectivity FR-974 overseas department -> overseas departmental collectivity FR-976 overseas department -> overseas departmental collectivity Parent changes: FR-67 FR-GES -> FR-6AE FR-68 FR-GES -> FR-6AE.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Addition of category European collectivity in eng & fra; Addition of European collectivity FR-6AE; Addition of metropolitan collectivity with special status FR-69M; Change of category name from metropolitan department to metropolitan collectivity with special status for FR-75; Change of subdivision code from FR-75 to FR-75C; Addition of category overseas departmental collectivity in English & French; Change of category name from overseas department to overseas departmental collectivity for FR-971, FR-974, FR-976; Addition of category overseas unique territorial collectivity in eng & fra; Change of category name from overseas department to overseas unique territorial collectivity for FR-972, FR-973; Deletion of category name overseas department; Deletion of overseas region FR-GF, FR-GP, FR-MQ, FR-RE, FR-YT; Deletion of category name overseas region; Change of parent subdivision of FR-67, FR-68; Deletion of parent subdivision of FR-971, FR-972, FR-973, FR-974, FR-976; Modification of Remark part 2; Update List Source and Code Source.",
+            "Description of Change": "Addition of category European collectivity in eng & fra; Addition of European collectivity FR-6AE; Addition of metropolitan collectivity with special status FR-69M; Change of category name from metropolitan department to metropolitan collectivity with special status for FR-75; Change of subdivision code from FR-75 to FR-75C; Addition of category overseas departmental collectivity in English & French; Change of category name from overseas department to overseas departmental collectivity for FR-971, FR-974, FR-976; Addition of category overseas unique territorial collectivity in eng & fra; Change of category name from overseas department to overseas unique territorial collectivity for FR-972, FR-973; Deletion of category name overseas department; Deletion of overseas region FR-GF, FR-GP, FR-MQ, FR-RE, FR-YT; Deletion of category name overseas region; Change of parent subdivision of FR-67, FR-68; Deletion of parent subdivision of FR-971, FR-972, FR-973, FR-974, FR-976; Modification of Remark part 2; Update List Source and Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of category name from collectivity to metropolitan collectivity with special status for FR-COR; Change of category name from overseas department to overseas region for FR-GP, FR-RE, FR-YT; Deletion of parent subdivision of FR-GP, FR-RE, FR-YT; Change of category name from overseas region to overseas department for FR-GUA, FR-LRE, FR-MAY; Change of subdivision code from FR-COR to FR-20R, FR-GUA to FR-971, FR-LRE to FR-974, FR-MAY to FR-976; Assign parent subdivision to FR-971, FR-974, FR-976; Change of parent subdivision of FR-972, FR-973; Change of category name from overseas territorial collectivity to overseas collectivity for FR-BL, FR-MF, FR-PF, FR-PM, FR-WF; Addition of category overseas territory with specific status, overseas territory; Change of category name from overseas territorial collectivity to overseas collectivity with special status for FR-NC; Change of category name from overseas territorial collectivity to overseas territory for FR-TF; Update List Source and Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of category name from collectivity to metropolitan collectivity with special status for FR-COR; Change of category name from overseas department to overseas region for FR-GP, FR-RE, FR-YT; Deletion of parent subdivision of FR-GP, FR-RE, FR-YT; Change of category name from overseas region to overseas department for FR-GUA, FR-LRE, FR-MAY; Change of subdivision code from FR-COR to FR-20R, FR-GUA to FR-971, FR-LRE to FR-974, FR-MAY to FR-976; Assign parent subdivision to FR-971, FR-974, FR-976; Change of parent subdivision of FR-972, FR-973; Change of category name from overseas territorial collectivity to overseas collectivity for FR-BL, FR-MF, FR-PF, FR-PM, FR-WF; Addition of category overseas territory with specific status, overseas territory; Change of category name from overseas territorial collectivity to overseas collectivity with special status for FR-NC; Change of category name from overseas territorial collectivity to overseas territory for FR-TF; Update List Source and Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
             "Code/Subdivision Change": "Category change: FR-COR metropolitan region -> collectivity.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of category name \"collectivity\" in eng/fra; Change of category name from metropolitan region to collectivity for FR-COR; Update List Source.",
+            "Description of Change": "Addition of category name \"collectivity\" in eng/fra; Change of category name from metropolitan region to collectivity for FR-COR; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
             "Code/Subdivision Change": "Parent changes: FR-02 FR-PDL -> FR-HDF FR-60 FR-PDL -> FR-HDF FR-80 FR-PDL -> FR-HDF.",
             "Date Issued": "2016-12-07",
-            "Description of Change in Newsletter": "Correction of parent subdivision of FR-02, FR-60, FR-80 from FR-PDL to FR-HDF.",
+            "Description of Change": "Correction of parent subdivision of FR-02, FR-60, FR-80 from FR-PDL to FR-HDF.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: FR-GUA Guadeloupe FR-LRE La R\u00e9union FR-MAY Mayotte Category change: FR-GR overseas department -> overseas territorial collectivity FR-MQ overseas department -> overseas territorial collectivity.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of the delimitation of the regions, reducing their number from 22 to 13 in metropolitan France, change of parent subdivision of metropolitan departments; addition of overseas regions FR-GUA, FR-LRE, FR-MAY; change of subdivision category from overseas department to overseas territorial collectivity for FR-GR, FR-MQ; update List Source.",
+            "Description of Change": "Change of the delimitation of the regions, reducing their number from 22 to 13 in metropolitan France, change of parent subdivision of metropolitan departments; addition of overseas regions FR-GUA, FR-LRE, FR-MAY; change of subdivision category from overseas department to overseas territorial collectivity for FR-GR, FR-MQ; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
             "Code/Subdivision Change": "Category change: FR-YT Mayotte overseas territorial collectivity -> overseas department.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "NL II-2 correction for ultramarine administrative organisation change and alphabetical re-ordering.",
+            "Description of Change": "NL II-2 correction for ultramarine administrative organisation change and alphabetical re-ordering.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: FR-CP Clipperton FR-BL Saint-Barth\u00e9lemy FR-MF Saint-Martin.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add Saint Barth\u00e9lemy, Saint Martin and the Clipperton Island.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Add Saint Barth\u00e9lemy, Saint Martin and the Clipperton Island.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:FR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Metropolitan region code in FR-79.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Correction of the Metropolitan region code in FR-79.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "GA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GA)."
         }
     ],
     "GB": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of two-tier county GB-NTH; Addition of unitary authority GB-NNH, GB-WNH; Change of category name from two-tier county to unitary authority for GB-BKM; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Deletion of two-tier county GB-NTH; Addition of unitary authority GB-NNH, GB-WNH; Change of category name from two-tier county to unitary authority for GB-BKM; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of parent subdivision of GB-PEM.",
             "Date Issued": "2022-03-03",
-            "Description of Change in Newsletter": "Correction of parent subdivision of GB-PEM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of subdivision categories country and province in eng & fra; Modification of remark part 2; Addition of country GB-ENG, GB-WLS, GB-SCT; Addition of province GB-NIR; Addition of parent subdivisions (bS 6879 gives alternative name forms in Welsh (cy) for some of the Welsh unitary authorities (together with alternative code elements). Since this part of ISO 3166 does not allow for duplicate coding of identical subdivisions, such alternative names in Welsh and code elements are shown for information purposes only in square brackets after the English name of the subdivision. BS 6879 has been superseded but remains the original source of the codes. Included for completeness: EAW England and Wales; GBN Great Britain; UKM United Kingdom).",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Addition of subdivision categories country and province in eng & fra; Modification of remark part 2; Addition of country GB-ENG, GB-WLS, GB-SCT; Addition of province GB-NIR; Addition of parent subdivisions (bS 6879 gives alternative name forms in Welsh (cy) for some of the Welsh unitary authorities (together with alternative code elements). Since this part of ISO 3166 does not allow for duplicate coding of identical subdivisions, such alternative names in Welsh and code elements are shown for information purposes only in square brackets after the English name of the subdivision. BS 6879 has been superseded but remains the original source of the codes. Included for completeness: EAW England and Wales; GBN Great Britain; UKM United Kingdom).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of GB-BMH, GB-POL; Addition of GB-BCP; Correction of spelling for GB-BFS, GB-DRS, GB-DUR, GB-MUL, GB-RCT, GB-SCB; Modification of remark, part 2; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of GB-BMH, GB-POL; Addition of GB-BCP; Correction of spelling for GB-BFS, GB-DRS, GB-DUR, GB-MUL, GB-RCT, GB-SCB; Modification of remark, part 2; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of GB-ABC, GB-DRS; Modification of remark part 2; Update List Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Change of subdivision name of GB-ABC, GB-DRS; Modification of remark part 2; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of Northern Ireland district council areas GB-ANT, GB-ARD, GB-ARM, GB-BLA, GB-BLY, GB-BNB, GB-CKF, GB-CSR, GB-CLR, GB-CKT, GB-CGV, GB-DRY, GB-DOW, GB-DGN, GB-FER, GB-LRN, GB-LMV, GB-LSB, GB-MFT, GB-MYL, GB-NYM, GB-NTA, GB-NDN, GB-OMH, GB-STB; change of subdivision category from district council area to district GB-BFS; addition of Northern Ireland districts GB-ANN, GB-AND, GB-ABC, GB-CCG, GB-DRS, GB-FMO, GB-LBC, GB-MEA, GB-MUL, GB-NMD; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of Northern Ireland district council areas GB-ANT, GB-ARD, GB-ARM, GB-BLA, GB-BLY, GB-BNB, GB-CKF, GB-CSR, GB-CLR, GB-CKT, GB-CGV, GB-DRY, GB-DOW, GB-DGN, GB-FER, GB-LRN, GB-LMV, GB-LSB, GB-MFT, GB-MYL, GB-NYM, GB-NTA, GB-NDN, GB-OMH, GB-STB; change of subdivision category from district council area to district GB-BFS; addition of Northern Ireland districts GB-ANN, GB-AND, GB-ABC, GB-CCG, GB-DRS, GB-FMO, GB-LBC, GB-MEA, GB-MUL, GB-NMD; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add GB-IOS.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Add GB-IOS.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
             "Code/Subdivision Change": "Status change: WLS Wales principality -> country.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "NL II-2 correction for administrative name changes.",
+            "Description of Change": "NL II-2 correction for administrative name changes.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update and reorganization of the subdivision data and update of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update and reorganization of the subdivision data and update of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of administrative structure.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Modification of administrative structure.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: GB-CHA Channel Islands GB-IOM Isle of Man (see ISO 3166-2:IM) GB-GSY Guernsey (see ISO 3166-2:GG) GB-JSY Jersey (see ISO 3166-2:JE).",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Various corrections of name forms i.e. deletion of name adjuncts.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Various corrections of name forms i.e. deletion of name adjuncts.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "GD": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local variation of GD-10; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of local variation of GD-10; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 6 parishes, 1 dependency.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "GE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of diacritical signs.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of diacritical signs.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Introduction of third subdivision category.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Introduction of third subdivision category.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 2 autonomous republics, 13 cities, 63 rayons (see below) -> 2 autonomous republics, 10 regions.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "New subdivision layout. City level cancelled. Spelling of autonomous republics' names changed. One generic subdivision name changed.",
+            "Description of Change": "New subdivision layout. City level cancelled. Spelling of autonomous republics' names changed. One generic subdivision name changed.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "GF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-973)).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-973)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GF)."
         }
     ],
     "GG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction.",
             "Date Issued": "2009-03-03",
-            "Description of Change in Newsletter": "Typographical correction.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of remark and administrative language French (fr, fra); Addition of the islands mentioned in the Remarks column (Column 7).",
             "Date Issued": "2008-09-09",
-            "Description of Change in Newsletter": "Addition of remark and administrative language French (fr, fra); Addition of the islands mentioned in the Remarks column (Column 7).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "GH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of region GH-BA; Addition of regions GH-AF, GH-BE, GH-BO, GH-NE, GH-OT, GH-SV, GH-WN; Update List Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Deletion of region GH-BA; Addition of regions GH-AF, GH-BE, GH-BO, GH-NE, GH-OT, GH-SV, GH-WN; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GH)."
         }
     ],
     "GI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GI)."
         }
     ],
     "GL": [
         {
             "Code/Subdivision Change": "Subdivision deleted: GL-QA Qaasuitsup Kommunia Subdivisions added: GL-AV Avannaata Kommunia GL-QT Kommune Qeqertalik.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Deletion of municipality GL-QA; Addition of municipality GL-AV, GL-QT; Update List Source.",
+            "Description of Change": "Deletion of municipality GL-QA; Addition of municipality GL-AV, GL-QT; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GL)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: GL-KU Kommune Kujalleq GL-QA Qaasuitsup Kommunia GL-QE Qeqqata Kommunia GL-SM Kommuneqarfik Sermersooq.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition and update of the administrative structure and of the list and code sources.",
+            "Description of Change": "Addition and update of the administrative structure and of the list and code sources.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of administrative language from Inuktitut (iu, iku) to Greenlandic or Kalaallit (kl, kal).",
             "Date Issued": "2008-09-09",
-            "Description of Change in Newsletter": "Correction of administrative language from Inuktitut (iu, iku) to Greenlandic or Kalaallit (kl, kal).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GL)."
         }
     ],
     "GM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2017-03-17",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2016-03-31",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name lower case and the English full name with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name lower case and the English full name with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GM)."
         }
     ],
     "GN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change Subdivision category special zone to governorate (GN-C); change governorates to administrative regions; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Change Subdivision category special zone to governorate (GN-C); change governorates to administrative regions; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, deletion of the generic term in subdivision names.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, deletion of the generic term in subdivision names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, deletion of the generic term in subdivision names.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, deletion of the generic term in subdivision names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use) Koundara: GN-KD -> GN-KN.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "One governorate changed into a city (new subdivision level). One code corrected.",
+            "Description of Change": "One governorate changed into a city (new subdivision level). One code corrected.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "GP": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-971)).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-971)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete Saint Barth\u00e9lemy and Saint Martin.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Delete Saint Barth\u00e9lemy and Saint Martin.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GP)."
         }
     ],
     "GQ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of province GQ-DJ; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of province GQ-DJ; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add the local short name and align with ISO 3166-2.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Add the local short name and align with ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Language adjustment, typo correction, first level prefix addition and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Language adjustment, typo correction, first level prefix addition and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "GR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of subdivision name of GR-J.",
             "Date Issued": "2020-03-02",
-            "Description of Change in Newsletter": "Typographical correction of subdivision name of GR-J.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Grammar corrrection of GR-J, GR-K, GR-L.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Grammar corrrection of GR-J, GR-K, GR-L.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of GR-M; deletion of subdivision category department; deletion of departments GR-01, GR-11, GR-12, GR-31, GR-A1, GR-64, GR-94, GR-85, GR-81, GR-52, GR-71, GR-05, GR-04, GR-63, GR-07, GR-06, GR-51, GR-14, GR-53, GR-33, GR-91, GR-41, GR-56, GR-55, GR-23, GR-22, GR-57, GR-15, GR-58, GR-82, GR-16, GR-42, GR-92, GR-24, GR-83, GR-43, GR-07, GR-59, GR-61, GR-34, GR-93, GR-73, GR-84, GR-62, GR-32, GR-54, GR-44, GR-03, GR-72, GR-21; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of GR-M; deletion of subdivision category department; deletion of departments GR-01, GR-11, GR-12, GR-31, GR-A1, GR-64, GR-94, GR-85, GR-81, GR-52,GR-71, GR-05, GR-04, GR-63, GR-07, GR-06, GR-51, GR-14, GR-53, GR-33, GR-91, GR-41, GR-56, GR-55, GR-23, GR-22, GR-57, GR-15, GR-58, GR-82, GR-16, GR-42, GR-92, GR-24, GR-83, GR-43, GR-07, GR-59, GR-61, GR-34, GR-93, GR-73, GR-84, GR-62, GR-32, GR-54, GR-44, GR-03, GR-72, GR-21; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the local short name.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of the local short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling of GR-01, GR-81, GR-23, GR-93, GR-69; correct diacritic marks; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Correct spelling of GR-01, GR-81, GR-23, GR-93, GR-69; correct diacritic marks; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, addition of names in administrative languages.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GR)."
         },
         {
             "Code/Subdivision Change": "Codes: format changed (see below).",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, addition of names in administrative languages.",
+            "Description of Change": "Addition of the country code prefix as the first code element, reallocation of 3166-2 alpha-2 codes to avoid duplication, addition of names in administrative languages.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         }
     ],
     "GS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GS)."
         }
     ],
     "GT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision code from GT-AV to GT-16, GT-BV to GT-15, GT-CM to GT-04, GT-CQ to GT-20, GT-ES to GT-05, GT-GU to GT-01, GT-HU to GT-13, GT-IZ to GT-18, GT-JA to GT-21, GT-JU to GT-22, GT-PE to GT-17, GT-PR to GT-02, GT-QC to GT-14, GT-QZ to GT-09, GT-RE to GT-11, GT-SA to GT-03, GT-SM to GT-12, GT-SO to GT-07, GT-SR to GT-06, GT-SU to GT-10, GT-TO to GT-08, GT-ZA to GT-19; Update Code Source.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of subdivision code from GT-AV to GT-16, GT-BV to GT-15, GT-CM to GT-04, GT-CQ to GT-20, GT-ES to GT-05, GT-GU to GT-01, GT-HU to GT-13, GT-IZ to GT-18, GT-JA to GT-21, GT-JU to GT-22, GT-PE to GT-17, GT-PR to GT-02, GT-QC to GT-14, GT-QZ to GT-09, GT-RE to GT-11, GT-SA to GT-03, GT-SM to GT-12, GT-SO to GT-07, GT-SR to GT-06, GT-SU to GT-10, GT-TO to GT-08, GT-ZA to GT-19; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in GT-QZ.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling correction in GT-QZ.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "GU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of the United States (US-GU)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of the United States (US-GU)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GU)."
         }
     ],
     "GW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of GW-BL; Addition of local variation of GW-BS; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of GW-BL; Addition of local variation of GW-BS; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         }
     ],
     "GY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2018-11-06",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:GY)."
         }
     ],
     "HK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of China (CN-HK)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of China (CN-HK)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HK)."
         }
     ],
     "HM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HM)."
         }
     ],
     "HN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Comment taken into account and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Comment taken into account and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "HR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct typographic error for the language code for Croatian.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Correct typographic error for the language code for Croatian.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HR)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: HR-21 Grad Zagreb.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of one city subdivision. Three spelling corrections.",
+            "Description of Change": "Addition of one city subdivision. Three spelling corrections.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "HT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of HT-GA; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of HT-GA; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Language adjustment.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Language adjustment.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: HT-NI Nippes.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-2).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "HU": [
         {
             "Code/Subdivision Change": "Subdivision renamed: HU-CS Csongr\u00e1d -> Csongr\u00e1d-Csan\u00e1d.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of name of HU-CS; Update List Source.",
+            "Description of Change": "Change of name of HU-CS; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of category name in eng; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of category name in eng; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change the full name.",
             "Date Issued": "2012-02-15",
-            "Description of Change in Newsletter": "Change the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:HU)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: HU-ER \u00c9rd.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "ID": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of province ID-PD; Update List Source.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Addition of province ID-PD; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of provinces ID-PE, ID-PS and ID-PT; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Addition of provinces ID-PE, ID-PS and ID-PT; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of category name in eng/fra from special district to capital district (ID-JK); change of category name from autonomous province to province for ID-AC; deletion of category autonomous province (eng) / province autonome (fra) / nanggroe (ind); update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of category name in eng/fra from special district to capital district (ID-JK); change of category name from autonomous province to province for ID-AC; deletion of category autonomous province (eng) / province autonome (fra) / nanggroe (ind); update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local variation of ID-JK, ID-YO; change of spelling of ID-BB, update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of local variation of ID-JK, ID-YO; change of spelling of ID-BB, update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add province ID-KU; change code for Papua formely ID-IJ; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Add province ID-KU; change code for Papua formely ID-IJ; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
             "Code/Subdivision Change": "Codes: Maluku (geographical unit) ID-MA -> ID-ML.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Removal of duplicate code.",
+            "Description of Change": "Removal of duplicate code.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering, administrative update.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering, administrative update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ID)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ID-PB Papua Barat.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, alphabetical re-ordering, administrative update.",
+            "Description of Change": "Addition of the country code prefix as the first code element, alphabetical re-ordering, administrative update.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ID-SR Sulawesi Barat.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Addition of a new province \"Sulawesi Barat\".",
+            "Description of Change": "Addition of a new province \"Sulawesi Barat\".",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ID-KR Kepulauan Riau.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Move \"Aceh\" to a new category of \"autonomous province\". Addition of a new province \"Kepulauan Riau\".",
+            "Description of Change": "Move \"Aceh\" to a new category of \"autonomous province\". Addition of a new province \"Kepulauan Riau\".",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of name of one geographical unit.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Change of name of one geographical unit.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: ID-BB Bangka Belitung ID-BT Banten ID-GO Gorontalo ID-MU Maluku Utara Subdivisions deleted: ID-TT Timor Timur (see ISO 3166-2:TL) Codes: (to correct duplicate use) ID-IJ Irian Jaya (province) -> ID-PA Papua.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of four new provinces and deletion of one (ID-TT). Inclusion of one alternative name form and one changed province name (ID-PA, formerly ID-IJ).",
+            "Description of Change": "Addition of four new provinces and deletion of one (ID-TT). Inclusion of one alternative name form and one changed province name (ID-PA, formerly ID-IJ).",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "IE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IE)."
         },
         {
             "Code/Subdivision Change": "Codes: Cork IE-C -> IE-CO.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Removal of duplicate code.",
+            "Description of Change": "Removal of duplicate code.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         }
     ],
     "IL": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the local variation of IL-Z.",
             "Date Issued": "2018-04-20",
-            "Description of Change in Newsletter": "Correction of the local variation of IL-Z.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change romanization system from \"BGN/PCGN (ara)\" to \"BGN/PCGN 1956\"; change romanization system from \"Israeli national romanization 1957, updated to 2006 (he)\" to \" Israeli national romanization 1957, updated to 2006\"; addition of local variation of IL-JM, IL-M, IL-D, IL-Z, IL-HA, IL-TA; change of spelling of IL-M, IL-D, IL-Z, IL-HA, IL-TA in heb.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change romanization system from \"BGN/PCGN (ara)\" to \"BGN/PCGN 1956\"; change romanization system from \"Israeli national romanization 1957, updated to 2006 (he)\" to \" Israeli national romanization 1957, updated to 2006\"; addition of local variation of IL-JM, IL-M, IL-D, IL-Z, IL-HA, IL-TA; change of spelling of IL-M, IL-D, IL-Z, IL-HA, IL-TA in heb.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IL)."
         }
     ],
     "IM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "IN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision code from IN-OR to IN-OD, from IN-CT to IN-CG, from IN-TG to IN-TS, from IN-UT to IN-UK; Deletion of the asterisk from IN-JH; Update Code Source.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Change of subdivision code from IN-OR to IN-OD, from IN-CT to IN-CG, from IN-TG to IN-TS, from IN-UT to IN-UK; Deletion of the asterisk from IN-JH; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of Union territory IN-DD, IN-DN; Addition of Union territory IN-DH; Correction of spelling for IN-AR, IN-BR, IN-CH, IN-CT, IN-DH, IN-GJ, IN-HP, IN-HR, IN-JH, IN-JK, IN-KA, IN-LA, IN-MH, IN-ML, IN-NL, IN-RJ, IN-TG, IN-TN, IN-UT; Addition of romanization system \"Indian System of Transliteration\"; Update List Source; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of Union territory IN-DD, IN-DN; Addition of Union territory IN-DH; Correction of spelling for IN-AR, IN-BR, IN-CH, IN-CT, IN-DH, IN-GJ, IN-HP, IN-HR, IN-JH, IN-JK, IN-KA, IN-LA, IN-MH, IN-ML, IN-NL, IN-RJ, IN-TG, IN-TN, IN-UT; Addition of romanization system \"Indian System of Transliteration\"; Update List Source; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from state to Union territory for IN-JK; Addition of Union territory IN-LA; Update List Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Change of subdivision category from state to Union territory for IN-JK; Addition of Union territory IN-LA; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 state IN-TG; change spelling of IN-OR; update List Source and Code Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Add 1 state IN-TG; change spelling of IN-OR; update List Source and Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IN)."
         },
         {
             "Code/Subdivision Change": "Codes: IN-UL Uttaranchal -> IN-UT Uttarakhand.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of local generic administrative terms, update of the official languages according to ISO 3166-2, addition of a comment and source list update.",
+            "Description of Change": "Addition of local generic administrative terms, update of the official languages according to ISO 3166-2, addition of a comment and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Reintroduction of old name form in IN-WB.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Error correction: Reintroduction of old name form in IN-WB.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use) Chhattisgarh: IN-CH -> IN-CT.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Error correction: Duplicate use of IN-CH corrected. Spelling correction.",
+            "Description of Change": "Error correction: Duplicate use of IN-CH corrected. Spelling correction.",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: IN-CH Chhattisgarh IN-JH Jharkhand IN-UL Uttaranchal.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Partial reorganization of subdivision layout: Three new states. Addition of an alternative name for one state. New list source.",
+            "Description of Change": "Partial reorganization of subdivision layout: Three new states. Addition of an alternative name for one state. New list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "IO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IO)."
         }
     ],
     "IQ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of category region in eng, fra, ara, kur; Addition of region IQ-KR; Assign parent subdivision to IQ-AR, IQ-DA, IQ-SU; Update List and Code Source.",
             "Date Issued": "2022-03-03",
-            "Description of Change in Newsletter": "Addition of category region in eng, fra, ara, kur; Addition of region IQ-KR; Assign parent subdivision to IQ-AR, IQ-DA, IQ-SU; Update List and Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the alpha 2 and alpha 3 administrative language codes ku, kur.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of the alpha 2 and alpha 3 administrative language codes ku, kur.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of IQ-KA; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Typographical correction of IQ-KA; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision code from IQ-TS to IQ-KI; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Change subdivision code from IQ-TS to IQ-KI; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IQ)."
         }
     ],
     "IR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a coma.",
+            "Date Issued": "2024-02-29",
+            "Description of Change": "",
+            "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
+        },
+        {
+            "Code/Subdivision Change": "Change of subdivision code from IR-01 to IR-03, IR-02 to IR-04, IR-03 to IR-24, IR-04 to IR-10, IR-05 to IR-16, IR-06 to IR-18, IR-07 to IR-23, IR-08 to IR-14, IR-10 to IR-06, IR-11 to IR-19, IR-12 to IR-20, IR-13 to IR-11, IR-14 to IR-07, IR-15 to IR-08, IR-16 to IR-12, IR-17 to IR-05, IR-18 to IR-17, IR-19 to IR-01, IR-20 to IR-15, IR-21 to IR-02, IR-22 to IR-00, IR-23 to IR-22, IR-24 to IR-13, IR-25 to IR-21, IR-26 to IR-25, IR-28 to IR-26, IR-30 to IR-09, IR-31 to IR-28, IR-32 to IR-30; Update Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision code from IR-01 to IR-03, IR-02 to IR-04, IR-03 to IR-24, IR-04 to IR-10, IR-05 to IR-16, IR-06 to IR-18, IR-07 to IR-23, IR-08 to IR-14, IR-10 to IR-06, IR-11 to IR-19, IR-12 to IR-20, IR-13 to IR-11, IR-14 to IR-07, IR-15 to IR-08, IR-16 to IR-12, IR-17 to IR-05, IR-18 to IR-17, IR-19 to IR-01, IR-20 to IR-15, IR-21 to IR-02, IR-22 to IR-00, IR-23 to IR-22, IR-24 to IR-13, IR-25 to IR-21, IR-26 to IR-25, IR-28 to IR-26, IR-30 to IR-09, IR-31 to IR-28, IR-32 to IR-30 ; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name for IR-08, IR-18, IR-29, IR-30, IR-31; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision name for IR-08, IR-18, IR-29, IR-30, IR-31; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name upper and lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name upper and lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 province IR-32; update List Source.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Add 1 province IR-32; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IR)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: IR-29 Khor\u0101s\u0101n-e Jan\u016bb\u012b IR-30 Khor\u0101s\u0101n-e Razav\u012b IR-31 Khor\u0101s\u0101n-e Shem\u0101l\u012b Subdivisions deleted: IR-09 Khor\u0101s\u0101n.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: IR-27 Golest\u0101n IR-28 Qazv\u012bn.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Partial reorganization of subdivision layout. Two new provinces. Two name corrections (IR-17 and IR-18). New reference for the list source.",
+            "Description of Change": "Partial reorganization of subdivision layout. Two new provinces. Two name corrections (IR-17 and IR-18). New reference for the list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "IS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of municipality IS-AKH, IS-BLO, IS-HEL, IS-HUT, IS-SBH, IS-SKU, IS-SSF; Addition of municipality IS-HUG, IS-SKR.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Deletion of municipality IS-AKH, IS-BLO, IS-HEL, IS-HUT, IS-SBH, IS-SKU, IS-SSF; Addition of municipality IS-HUG, IS-SKR.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2022-11-21",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of municipality IS-BFJ, IS-DJU, IS-FLD, IS-SEY; Addition of municipality IS-MUL; Update List Source.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Deletion of municipality IS-BFJ, IS-DJU, IS-FLD, IS-SEY; Addition of municipality IS-MUL; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of category municipality; Addition of municipality IS-AKH, IS-AKN, IS-AKU, IS-ARN, IS-ASA, IS-BFJ, IS-BLA, IS-BLO, IS-BOG, IS-BOL, IS-DAB, IS-DAV, IS-DJU, IS-EOM, IS-EYF, IS-FJD, IS-FJL, IS-FLA, IS-FLD, IS-FLR, IS-GAR, IS-GOG, IS-GRN, IS-GRU, IS-GRY, IS-HAF, IS-HEL, IS-HRG, IS-HRU, IS-HUT, IS-HUV, IS-HVA, IS-HVE, IS-ISA, IS-KAL, IS-KJO, IS-KOP, IS-LAN, IS-MOS, IS-MYR, IS-NOR, IS-RGE, IS-RGY, IS-RHH, IS-RHN, IS-RKV, IS-SBH, IS-SBT, IS-SDN, IS-SDV, IS-SEL, IS-SEY, IS-SFA, IS-SHF, IS-SKF, IS-SKG, IS-SKO, IS-SKU, IS-SNF, IS-SOG, IS-SOL, IS-SSF, IS-SSS, IS-STR, IS-STY, IS-SVG, IS-TAL, IS-THG, IS-TJO, IS-VEM, IS-VER, IS-VOP; Update List Source; Update Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of category municipality; Addition of municipality IS-AKH, IS-AKN, IS-AKU, IS-ARN, IS-ASA, IS-BFJ, IS-BLA, IS-BLO, IS-BOG, IS-BOL, IS-DAB, IS-DAV, IS-DJU, IS-EOM, IS-EYF, IS-FJD, IS-FJL, IS-FLA, IS-FLD, IS-FLR, IS-GAR, IS-GOG, IS-GRN, IS-GRU, IS-GRY, IS-HAF, IS-HEL, IS-HRG, IS-HRU, IS-HUT, IS-HUV, IS-HVA, IS-HVE, IS-ISA, IS-KAL, IS-KJO, IS-KOP, IS-LAN, IS-MOS, IS-MYR, IS-NOR, IS-RGE, IS-RGY, IS-RHH, IS-RHN, IS-RKV, IS-SBH, IS-SBT, IS-SDN, IS-SDV, IS-SEL, IS-SEY, IS-SFA, IS-SHF, IS-SKF, IS-SKG, IS-SKO, IS-SKU, IS-SNF, IS-SOG, IS-SOL, IS-SSF, IS-SSS, IS-STR, IS-STY, IS-SVG, IS-TAL, IS-THG, IS-TJO, IS-VEM, IS-VER, IS-VOP; Update List Source; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of IS-1; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of IS-1; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of region IS-0.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of region IS-0.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IS)."
         }
     ],
     "IT": [
         {
             "Code/Subdivision Change": "Code changes: IT-SD -> IT-SU Sud Sardegna Subdivisions added: IT-GO Gorizia IT-PN Pordenone IT-TS Trieste IT-UD Udine.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of subdivision code from IT-SD to IT-SU; Addition of category decentralized regional entity; addition of decentralized regional entity IT-GO, IT-PN, IT-TS, IT-UD; Update List Source.",
+            "Description of Change": "Correction of subdivision code from IT-SD to IT-SU; Addition of category decentralized regional entity; addition of decentralized regional entity IT-GO, IT-PN, IT-TS, IT-UD; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IT)."
         },
         {
             "Code/Subdivision Change": "Name changes: IT-36 Friuli-Venezia Giulia -> Friuli Venezia Giulia free communal consortia -> free municipal consortium Subdivisions deleted: IT-AO Aosta Category changes: IT-23, IT-32, IT-36, IT-82, IT-88: region -> autonomous region IT-BZ, IT-TN: province -> autonomous province.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Change of spelling of IT-36; Deletion of province IT-AO; Change of spelling of category name in eng from free communal consortia to free municipal consortium; Change of spelling of category name in ita from libero consorzion communale [sic] to libero consorzio comunale ; Change of spelling of category name in ita from citt\u00e0 metropolitan to citt\u00e0 metropolitana; Addition of category name autonomous region and autonomous province; Change of category name from region to autonomous region for IT-23, IT-32, IT-36, IT-82, IT-88; Change of category name from province to autonomous province for IT-BZ, IT-TN; Update List Source.",
+            "Description of Change": "Change of spelling of IT-36; Deletion of province IT-AO; Change of spelling of category name in eng from free communal consortia to free municipal consortium; Change of spelling of category name in ita from libero consorzion communale [sic] to libero consorzio comunale; Change of spelling of category name in ita from citt\u00e0 metropolitan to citt\u00e0 metropolitana; Addition of category name autonomous region and autonomous province; Change of category name from region to autonomous region for IT-23, IT-32, IT-36, IT-82, IT-88; Change of category name from province to autonomous province for IT-BZ, IT-TN; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IT)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: 8 provinces ()see below) Subdivisions added: IT-SD Sud Sardegna Category changes: IT-AG, IT-CL, IT-EN, IT-RG, IT-SR, IT-TP: province -> free communal consortia IT-BA, IT-BO, IT-CA, IT-CT, IT-FI, IT-GE, IT-ME, IT-MI, IT-NA, IT-PA, IT-RC, IT-RM, IT-TO, IT-VE: province -> metropolitan city.",
             "Date Issued": "2019-04-09",
-            "Description of Change in Newsletter": "Addition of province IT-SD; Addition of category names free communal consortia and metropolitan cities in eng,fra and ita; Change of category name from province to free communal consortia for IT-AG, IT-CL, IT-EN, IT-RG, IT-SR, IT-TP; Change of category name from province to metropolitan city for IT-BA, IT-BO, IT-CA, IT-CT, IT-FI, IT-GE, IT-ME, IT-MI, IT-NA, IT-PA, IT-RC, IT-RM, IT-TO, IT-VE; Deletion of provinces IT-CI, IT-GO, IT-OG, IT-OT, IT-PN, IT-TS, IT-UD, IT-VS; Update List Source.",
+            "Description of Change": "Addition of province IT-SD; Addition of category names free communal consortia and metropolitan cities in eng, fra and ita; Change of category name from province to free communal consortia for IT-AG, IT-CL, IT-EN, IT-RG, IT-SR, IT-TP; Change of category name from province to metropolitan city for IT-BA, IT-BO, IT-CA, IT-CT, IT-FI, IT-GE, IT-ME, IT-MI, IT-NA, IT-PA, IT-RC, IT-RM, IT-TO, IT-VE; Deletion of provinces IT-CI, IT-GO, IT-OG, IT-OT, IT-PN, IT-TS, IT-UD, IT-VS; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IT)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct inconsistencies between newsletters) Medio Campidano: IT-MA -> IT-VS Olbia-Tempio IT-OL -> IT-OT Pesaro e Urbino IT-PS -> IT-PU.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Corrections from Newsletters I-1 and I-8.",
+            "Description of Change": "Corrections from Newsletters I-1 and I-8.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, administrative update.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:IT)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: IT-BT Barletta-Andria-Trani IT-FM Fermo IT-MB Monza e Brianza Codes: IT-FO Forl\u00ec -> IT-FC Forl\u00ec-Cesena.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update.",
+            "Description of Change": "Addition of the country code prefix as the first code element, administrative update.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: IT-CI Carbonia-Iglesias IT-VS Medio Campidano IT-OG Ogliastra IT-OT Olbia-Tempio.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of spelling mistakes of names of 2 provinces.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Correction of spelling mistakes of names of 2 provinces.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "JE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add local short names.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Add local short names.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of a new entry (in accordance with ISO 3166-1 Newsletter V-11).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "JM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JM)."
         }
     ],
     "JO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name for JO-AM, JO-AJ, JO-AQ, JO-BA, JO-AZ, JO-MN; addition of local variations JO-AM, JO-AQ; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision name for JO-AM, JO-AJ, JO-AQ, JO-BA, JO-AZ, JO-MN; addition of local variations JO-AM, JO-AQ; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering, administrative names precision and evolution and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering, administrative names precision and evolution and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "JP": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delation of the romanization system for subdivisions in eng.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Delation of the romanization system for subdivisions in eng.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:JP)."
         }
     ],
     "KE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update Code Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KE)."
         },
         {
             "Code/Subdivision Change": "Deleted codes: KE-110, KE-200, KE-300, KE-400, KE-500, KE-600, KE-700, KE-800 Added codes: KE-01 through KE-47.",
             "Date Issued": "2014-10-30",
-            "Description of Change in Newsletter": "Delete provinces; add 47 counties; update List Source.",
+            "Description of Change": "Delete provinces; add 47 counties; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: Western: KE-900 -> KE-800.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "KG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of subdivision category in kir replacing oblast with oblus; Correction of subdivision names KG-GB, KG-GO in kir; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of subdivision category in kir replacing oblast with oblus; Correction of subdivision names KG-GB, KG-GO in kir; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of KG-C.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of KG-C.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 city KG-GO; update List Source.",
             "Date Issued": "2014-10-31",
-            "Description of Change in Newsletter": "Add 1 city KG-GO; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KG)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KG-GB Bishkek KG-B Batken.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one region and one city. One spelling correction.",
+            "Description of Change": "Addition of one region and one city. One spelling correction.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "KH": [
         {
             "Code/Subdivision Change": "Name changes: KH-1.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of spelling of KH-1.",
+            "Description of Change": "Change of spelling of KH-1.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
             "Code/Subdivision Change": "Name changes: KH-1, KH-18, KH-22.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of spelling of KH-22, KH-1, KH-18.",
+            "Description of Change": "Correction of spelling of KH-22, KH-1, KH-18.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
             "Code/Subdivision Change": "Name changes: KH-18, KH-23, KH-24 Local variations added: KH-01, KH-02, KH-03, KH-05, KH-06, KH-08, KH-09, KH-10, KH-11, KH-14, KH-15, KH-16, KH-17, KH-18, KH-19, KH-20, KH-21, KH-22, KH-23.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of subdivision name of KH-18, KH-23, KH24; Correction of the romanization system label; Addition of local variation of KH-01, KH-02, KH-03, KH-05, KH-06, KH-08, KH-09, KH-10, KH-11, KH-14, KH-15, KH-16, KH-17, KH-18, KH-19, KH-20, KH-21, KH-22, KH-23.",
+            "Description of Change": "Change of subdivision name of KH-18, KH-23, KH24; Correction of the romanization system label; Addition of local variation of KH-01, KH-02, KH-03, KH-05, KH-06, KH-08, KH-09, KH-10, KH-11, KH-14, KH-15, KH-16, KH-17, KH-18, KH-19, KH-20, KH-21, KH-22, KH-23.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of KH-25.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of KH-25.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
             "Code/Subdivision Change": "Category changes: KH-18, KH-23, KH-24 autonomous municipality -> province Subdivision added: KH-25.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision category from autonomous municipalities to provinces for KH-18, KH-23, KH-24; addition of province KH-25, update List Source.",
+            "Description of Change": "Change of subdivision category from autonomous municipalities to provinces for KH-18, KH-23, KH-24; addition of province KH-25, update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KH)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KH-24 Krong Pailin.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one autonomous municipality.",
+            "Description of Change": "Addition of one autonomous municipality.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "KI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of administrative language Gilbertese (-, gil).",
             "Date Issued": "2009-03-03",
-            "Description of Change in Newsletter": "Addition of administrative language Gilbertese (-, gil).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KI)."
         }
     ],
     "KM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of subdivision category in ara replacing jaz\u0101\u2019ir (plural) with jaz\u012brah (singular).",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of subdivision category in ara replacing jaz\u0101\u2019ir (plural) with jaz\u012brah (singular).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of quotation marks in the remark.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Correction of quotation marks in the remark.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Remarks to Parts 1 and 2 concerning the language code \u201c002\u201d to read \u201cThe language code \"002\" refers to the administrative language \u201cShikomor\u201d that has not been assigned an ISO 639 language code.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the Remarks to Parts 1 and 2 concerning the language code \u201c002\u201d to read \u201cThe language code \"002\" refers to the administrative language \u201cShikomor\u201d that has not been assigned an ISO 639 language code.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of administrative language Shikomor (-,-).",
             "Date Issued": "2009-01-07",
-            "Description of Change in Newsletter": "Addition of administrative language Shikomor (-,-).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KM)."
         }
     ],
     "KN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 2 states, 14 parishes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "KP": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name upper case in eng: replace the parentheses with a coma.",
+            "Date Issued": "2024-02-29",
+            "Description of Change": "",
+            "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
+        },
+        {
+            "Code/Subdivision Change": "Addition of metropolitan city KP-15; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Addition of metropolitan city KP-15; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of KP-10, KP-13 (McCune-Reischauer, 1939); addition of metropolitan city KP-14; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of KP-10, KP-13 (McCune-Reischauer, 1939); addition of metropolitan city KP-14; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the space between \"de\" and the parenthesis in the short French name lower case.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Deletion of the space between \"de\" and the parenthesis in the short French name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Administrative update, replacement of alphabetical characters with numeric characters in second code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Administrative update, replacement of alphabetical characters with numeric characters in second code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KP)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: KP-KAE Kaesong-si KP-NAM Nampo-si Codes: format changed (see below).",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Administrative update, replacement of alphabetical characters with numeric characters in second code element.",
+            "Description of Change": "Administrative update, replacement of alphabetical characters with numeric characters in second code element.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in header of list source.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Spelling correction in header of list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KP-NAJ Najin Sonbong-si.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one special city. Subdivision categories in header re-sorted.",
+            "Description of Change": "Addition of one special city. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "KR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of category name from province to special self-governing province for KR-42; Update List Source.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Change of category name from province to special self-governing province for KR-42; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the romanization systems \"ISO/TR 11941\" and \"Ministry of Home Affairs, Republic of Korea 1984\"; move the short or contracted forms of subdivision names to local variation; deletion of the remark part 2.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Deletion of the romanization systems \"ISO/TR 11941\" and \"Ministry of Home Affairs, Republic of Korea 1984\"; move the short or contracted forms of subdivision names to local variation; deletion of the remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change to national romanization system and add short forms in brackets; add one special self-governing city; update List Source.",
             "Date Issued": "2014-10-31",
-            "Description of Change in Newsletter": "Change to national romanization system and add short forms in brackets; add one special self-governing city; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of 1 spelling mistake. Update of the source information.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Correction of 1 spelling mistake. Update of the source information.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "KW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Swap subdivision name with local variation of KW-KU.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Swap subdivision name with local variation of KW-KU.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Administrative name update and list source update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative name update and list source update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KW-MU Mub\u0101rak al Kab\u012br.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-3).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "KY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KY)."
         }
     ],
     "KZ": [
         {
             "Code/Subdivision Change": "Codes changed: KZ-ALA -> KZ-75 KZ-AST -> KZ-71 KZ-SHY -> KZ-79 KZ-ALM -> KZ-19 KZ-AKM -> KZ-11 KZ-AKT -> KZ-15 KZ-ATY -> KZ-23 KZ-VOS -> KZ-63 KZ-MAN -> KZ-47 KZ-SEV -> KZ-59 KZ-YUZ -> KZ-61 KZ-PAV -> KZ-55 KZ-KAR -> KZ-35 KZ-KUS -> KZ-39 KZ-KZY -> KZ-43 KZ-ZAP -> KZ-27 KZ-ZHA -> KZ-31 Subdivisions added: KZ-10, KZ-33, and KZ-62 Name change: KZ-71 Nur-Sultan -> Astana.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of subdivision code from KZ-ALA to KZ-75, KZ-AST to KZ-71, KZ-SHY to KZ-79, KZ-ALM to KZ-19, KZ-AKM to KZ-11, KZ-AKT to KZ-15, KZ-ATY to KZ-23, KZ-VOS to KZ-63, KZ-MAN to KZ-47, KZ-SEV to KZ-59, KZ-YUZ to KZ-61, KZ-PAV to KZ-55, KZ-KAR to KZ-35, KZ-KUS to KZ-39, KZ-KZY to KZ-43, KZ-ZAP to KZ-27, KZ-ZHA to KZ-31; Addition of region KZ-10, KZ-33, KZ-62; Change of subdivision name for KZ-71 in kaz and rus; Update List Source; Update Code Source.",
+            "Description of Change": "Change of subdivision code from KZ-ALA to KZ-75, KZ-AST to KZ-71, KZ-SHY to KZ-79, KZ-ALM to KZ-19, KZ-AKM to KZ-11, KZ-AKT to KZ-15, KZ-ATY to KZ-23, KZ-VOS to KZ-63, KZ-MAN to KZ-47, KZ-SEV to KZ-59, KZ-YUZ to KZ-61, KZ-PAV to KZ-55, KZ-KAR to KZ-35, KZ-KUS to KZ-39, KZ-KZY to KZ-43, KZ-ZAP to KZ-27, KZ-ZHA to KZ-31; Addition of region KZ-10, KZ-33, KZ-62; Change of subdivision name for KZ-71 in kaz and rus; Update List Source; Update Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KZ)."
         },
         {
             "Code/Subdivision Change": "Subdivision deleted: KZ-BAY Bayqongyr Name change: KZ-AST Astana -> Nur-Sultan.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of city KZ-BAY; Change of subdivision name of KZ\u2010AST; Correction of the Code Source; Update List Source.",
+            "Description of Change": "Deletion of city KZ-BAY; Change of subdivision name of KZ\u2010AST; Correction of the Code Source; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KZ)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: KZ-SHY Name change: KZ-YUZ Ongt\u00fcstik Qazaqstan oblysy (kk), Yuzhno-Kazakhstankaya oblast' (ru BGN/PCGN), Ju\u017eno-Kazahstankaja oblast' (ru GOST) -> T\u00fcrkistan oblysy (kk), Turkestankaya oblast' (ru BGN/PCGN), Turkestanskaja oblast' (ru GOST).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label; Addition of city KZ-SHY; Change of subdivision name of KZ-YUZ; Update List Source.",
+            "Description of Change": "Correction of the romanization system label; Addition of city KZ-SHY; Change of subdivision name of KZ-YUZ; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KZ-BAY.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of city KZ-BAY; update List Source.",
+            "Description of Change": "Addition of city KZ-BAY; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:KZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: KZ-BAY Bayqongyr.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Removal of one city from the list (Bayqongyr).",
+            "Description of Change": "Removal of one city from the list (Bayqongyr).",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Various spelling corrections.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Error correction: Various spelling corrections.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: KZ-AST Astana.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of one city. Nine name spellings corrected. List source updated.",
+            "Description of Change": "Addition of one city. Nine name spellings corrected. List source updated.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "LA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the French short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local variation of LA-AT, LA-BL, LA-CH, LA-HO, LA-KH, LA-LM, LA-LP, LA-OU, LA-PH, LA-SL, LA-SV, LA-XA, LA-XE, LA-XI, LA-XS; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Addition of local variation of LA-AT, LA-BL, LA-CH, LA-HO, LA-KH, LA-LM, LA-LP, LA-OU, LA-PH, LA-SL, LA-SV, LA-XA, LA-XE, LA-XI, LA-XS; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the romanization system \"Taken from old French maps still in use in the Lao People's Democratic Republic\"; addition of romanization system \u201cLao Commission Nationale de Toponymie (CNT)\u201d; change of spelling of LA-VT, LA-VI; addition of local variation of LA-VT, LA-VI; change of the romanization system of LA-VT, LA-AT, LA-BK, LA-BL, LA-CH, LA-O, A-KH, LA-LM, LA-LP, LA-OU, LA-PH, LA-SL, LA-SV, LA-VI, LA-XA, LA-XS, LA-XE, LA-XI, LA-XI.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Deletion of the romanization system \"Taken from old French maps still in use in the Lao People's Democratic Republic\"; addition of romanization system \u201cLao Commission Nationale de Toponymie (CNT)\u201d; change of spelling of LA-VT, LA-VI; addition of local variation of LA-VT, LA-VI; change of the romanization system of LA-VT, LA-AT, LA-BK, LA-BL, LA-CH, LA-O, A-KH, LA-LM, LA-LP, LA-OU, LA-PH, LA-SL, LA-SV, LA-VI, LA-XA, LA-XS, LA-XE, LA-XI, LA-XI.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of special zone LA-XN; addition of province LA-XS; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of special zone LA-XN; addition of province LA-XS; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change spelling of LA-XI; update List Source.",
             "Date Issued": "2014-10-31",
-            "Description of Change in Newsletter": "Change spelling of LA-XI; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Generic name of one subdivision changed to \"special zone\".",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Error correction: Generic name of one subdivision changed to \"special zone\".",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: LA-XN Xais\u00f4mboun.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "One new province added. One new reference for the list source. One code source cancelled. Information on romanization system updated. Origin of names in brackets given.",
+            "Description of Change": "One new province added. One new reference for the list source. One code source cancelled. Information on romanization system updated. Origin of names in brackets given.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "LB": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LB)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: LB-AK Aakk\u00e2r LB-BH Baalbek-Hermel.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         }
     ],
     "LC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision category to district; add 1 district LC-12; delete 2 districts LC-04 and LC-09; update List Source.",
             "Date Issued": "2014-10-31",
-            "Description of Change in Newsletter": "Change subdivision category to district; add 1 district LC-12; delete 2 districts LC-04 and LC-09; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LC)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 11 quarters.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "LI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LI)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 11 communes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "LK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of parent subdivision of LK-11, LK-12, LK-13, LK-21, LK-22, LK-23, LK-31, LK-32, LK-41, LK-43, LK-44, LK-45, LK-51, LK-52, LK-53, LK-61, LK-62, LK-71, LK-81, LK-82, LK-91, LK-92; Update List Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Correction of parent subdivision of LK-11, LK-12, LK-13, LK-21, LK-22, LK-23, LK-31, LK-32, LK-41, LK-43, LK-44, LK-45, LK-51, LK-52, LK-53, LK-61, LK-62, LK-71, LK-81, LK-82, LK-91, LK-92; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add administrative language.",
             "Date Issued": "2012-08-02",
-            "Description of Change in Newsletter": "Add administrative language.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         }
     ],
     "LR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling and addition of local variation of LR-RI; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling and addition of local variation of LR-RI; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LR)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: LR-GP Gbarpolu LR-RG River Gee.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         }
     ],
     "LS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of LS-B; Addition of local variation of LS-B; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of LS-B; Addition of local variation of LS-B; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local generic administrative term, update of the official languages according to ISO 3166-2 and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of local generic administrative term, update of the official languages according to ISO 3166-2 and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "LT": [
         {
             "Code/Subdivision Change": "Subdivisions renamed: LT-05 Bir\u0161tono -> Bir\u0161tonas LT-14 Kalvarijos -> Kalvarija LT-39 Rietavo -> Rietavas.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of spelling of LT-05, LT-14, LT-39; Assign parent subdivision to LT-01 through LT-60; Update List Source.",
+            "Description of Change": "Change of spelling of LT-05, LT-14, LT-39; Assign parent subdivision to LT-01 through LT-60; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of 7 city municipalities, 44 district municipalities, and 9 municipalities.",
             "Date Issued": "2014-10-31",
-            "Description of Change in Newsletter": "Addition of 7 city municipalities, 44 district municipalities, and 9 municipalities.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LT)."
         }
     ],
     "LU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of cantons LU-CA, LU-CL, LU-DI, LU-EC, LU-ES, LU-GR, LU-LU, LU-ME, LU-RD, LU-RM, LU-VD, LU-WI; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of cantons LU-CA, LU-CL, LU-DI, LU-EC, LU-ES, LU-GR, LU-LU, LU-ME, LU-RD, LU-RM, LU-VD, LU-WI; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LU)."
         }
     ],
     "LV": [
         {
             "Code/Subdivision Change": "Subdivisions added: LV-111 Aug\u0161daugavas novads LV-112 Dienvidkurzemes Novads LV-113 Valmieras Novads Subdivisions deleted: LV-JKB J\u0113kabpils LV-VMR Valmiera LV-001 Aglonas novads LV-003 Aizputes novads LV-004 Akn\u012bstes novads LV-005 Alojas novads LV-006 Alsungas novads LV-008 Amatas novads LV-009 Apes novads LV-010 Auces novads LV-012 Bab\u012btes novads LV-013 Baldones novads LV-014 Baltinavas novads LV-017 Bever\u012bnas novads LV-018 Broc\u0113nu novads LV-019 Burtnieku novads LV-020 Carnikavas novads LV-021 Cesvaines novads LV-023 Ciblas novads LV-024 Dagdas novads LV-025 Daugavpils novads LV-027 Dundagas novads LV-028 Durbes novads LV-029 Engures novads LV-030 \u0112rg\u013cu novads LV-031 Garkalnes novads LV-032 Grobi\u0146as novads LV-034 Iecavas novads LV-035 Ik\u0161\u0137iles novads LV-036 Il\u016bkstes novads LV-037 In\u010dukalna novads LV-038 Jaunjelgavas novads LV-039 Jaunpiebalgas novads LV-040 Jaunpils novads LV-043 Kandavas novads LV-044 K\u0101rsavas novads LV-045 Koc\u0113nu novads LV-046 Kokneses novads LV-048 Krimuldas novads LV-049 Krustpils novads LV-051 \u0136eguma novads LV-053 Lielv\u0101rdes novads LV-055 L\u012bgatnes novads LV-057 Lub\u0101nas novads LV-060 Mazsalacas novads LV-061 M\u0101lpils novads LV-063 M\u0113rsraga novads LV-064 Nauk\u0161\u0113nu novads LV-065 Neretas novads LV-066 N\u012bcas novads LV-069 Ozolnieku novads LV-070 P\u0101rgaujas novads LV-071 P\u0101vilostas novads LV-072 P\u013cavi\u0146u novads LV-074 Priekules novads LV-075 Prieku\u013cu novads LV-076 Raunas novads LV-078 Riebi\u0146u novads LV-079 Rojas novads LV-081 Rucavas novads LV-082 Rug\u0101ju novads LV-083 Rund\u0101les novads LV-084 R\u016bjienas novads LV-085 Salas novads LV-086 Salacgr\u012bvas novads LV-090 S\u0113jas novads LV-092 Skr\u012bveru novads LV-093 Skrundas novads LV-095 Stopi\u0146u novads LV-096 Stren\u010du novads LV-098 T\u0113rvetes novads LV-100 Vai\u0146odes novads LV-103 V\u0101rkavas novads LV-104 Vecpiebalgas novads LV-105 Vecumnieku novads LV-107 Vies\u012btes novads LV-108 Vi\u013cakas novads LV-109 Vi\u013c\u0101nu novads LV-110 Zilupes novads.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Deletion of republican city LV-JKB, LV-VMR; Deletion of municipality LV-001, LV-003, LV-004, LV-005, LV-006, LV-008, LV-009, LV-010, LV-012, LV-013, LV-014, LV-017, LV-018, LV-019, LV-020, LV-021, LV-023, LV-024, LV-025, LV-027, LV-028, LV-029, LV-030, LV-031, LV-032, LV-034, LV-035, LV-036, LV-037, LV-038, LV-039, LV-040, LV-043, LV-044, LV-045, LV-046, LV-048, LV-049, LV-051, LV-053, LV-055, LV-057, LV-060, LV-061, LV-063, LV-064, LV-065, LV-066, LV-069, LV-070, LV-071, LV-072, LV-074, LV-075, LV-076, LV-078, LV-079, LV-081, LV-082, LV-083, LV-084, LV-085, LV-086, LV-090, LV-092, LV-093, LV-095, LV-096, LV-098, LV-100, LV-103, LV-104, LV-105, LV-107, LV-108, LV-109, LV-110; Change of category name from republican city to state city for LV-DGV, LV-JEL, LV-JUR, LV-LPX, LV-REZ, LV-RIX, LV-VEN; Addition of municipality LV-111, LV-112, LV-113; Update List Source.",
+            "Description of Change": "Deletion of republican city LV-JKB, LV-VMR; Deletion of municipality LV-001, LV-003, LV-004, LV-005, LV-006, LV-008, LV-009, LV-010, LV-012, LV-013, LV-014, LV-017, LV-018, LV-019, LV-020, LV-021, LV-023, LV-024, LV-025, LV-027, LV-028, LV-029, LV-030, LV-031, LV-032, LV-034, LV-035, LV-036, LV-037, LV-038, LV-039, LV-040, LV-043, LV-044, LV-045, LV-046, LV-048, LV-049, LV-051, LV-053, LV-055, LV-057, LV-060, LV-061, LV-063, LV-064, LV-065, LV-066, LV-069, LV-070, LV-071, LV-072, LV-074, LV-075, LV-076, LV-078, LV-079, LV-081, LV-082, LV-083, LV-084, LV-085, LV-086, LV-090, LV-092, LV-093, LV-095, LV-096, LV-098, LV-100, LV-103, LV-104, LV-105, LV-107, LV-108, LV-109, LV-110; Change of category name from republican city to state city for LV-DGV, LV-JEL, LV-JUR, LV-LPX, LV-REZ, LV-RIX, LV-VEN; Addition of municipality LV-111, LV-112, LV-113; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LV)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 26 districts ()see below) -> 110 municipalities Subdivisions added: (republican cities) LV-JKB J\u0113kabpils LV-VMR Valmiera.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative re-organization and source list update.",
+            "Description of Change": "Administrative re-organization and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "LY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2; Correction of the Code Source (the subdivision category sha\u2018b\u012byah (popularate) is no longer used since the fall of Gaddafi. The word Mu\u1e29\u0101faz\u0327ah governorate is now sometimes used instead for these subdivisions of Libya, which are those pre-2011. The unrest in Libya means that there is no recognised current administrative structure).",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Modification of remark part 2; Correction of the Code Source (the subdivision category sha\u2018b\u012byah (popularate) is no longer used since the fall of Gaddafi. The word Mu\u1e29\u0101faz\u0327ah governorate is now sometimes used instead for these subdivisions of Libya, which are those pre-2011. The unrest in Libya means that there is no recognised current administrative structure).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2018-02-05",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of LY-JI.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of LY-JI.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Name change.",
             "Date Issued": "2011-11-08",
-            "Description of Change in Newsletter": "Name change.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:LY)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 34 municipalities (see below) -> 22 popularates.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 13 municipalities (see below) -> 34 municipalities.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Revision of subdivision layout. Revision of header information.",
+            "Description of Change": "Revision of subdivision layout. Revision of header information.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "MA": [
         {
             "Code/Subdivision Change": "Spelling change: MA-KHE Khemisset -> Kh\u00e9misset MA-KHN Khenifra -> Kh\u00e9nifra MA-TAR Taroudant -> Taroudannt.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of MA-KHE, MA-KHN, MA-TAR; Deletion of an asterisk of the local variation of MA-CAS; Update List Source.",
+            "Description of Change": "Change of spelling of MA-KHE, MA-KHN, MA-TAR; Deletion of an asterisk of the local variation of MA-CAS; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
             "Code/Subdivision Change": "Parent changes: MA-CAS MA-08 -> MA-06 MA-SET MA-08 -> MA-06 MA-SIK MA-06 -> MA-04 Spelling change: MA-03 F\u00e8s- Mekn\u00e8s -> F\u00e8s-Mekn\u00e8s.",
             "Date Issued": "2019-04-09",
-            "Description of Change in Newsletter": "Correction of parent subdivision of MA-CAS, MA-SET, MA-SIK; Typographical correction of MA-03.",
+            "Description of Change": "Correction of parent subdivision of MA-CAS, MA-SET, MA-SIK; Typographical correction of MA-03.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
             "Code/Subdivision Change": "Spelling change: MA-05 B\u00e9ni-Mellal-Kh\u00e9nifra -> B\u00e9ni Mellal-Kh\u00e9nifra Location change: MA-ESM Es-Semara (EH) -> Es-Semara (EH-partial).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of spelling of MA-05; Change of (EH) to (EH-partial) for MA-ESM; Correction of the romanization system label.",
+            "Description of Change": "Change of spelling of MA-05; Change of (EH) to (EH-partial) for MA-ESM; Correction of the romanization system label.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: MA-01 - MA-16 MA-MDF MA-MMD MA-MMN MA-SYB Subdivisions added: MA-01 - MA-12 MA-BRR MA-DRI MA-FQH MA-GUF MA-MAR MA-MID MA-OUZ MA-REH MA-SIB MA-SIF MA-SIL MA-TAF MA-TIN MA-YUS Category changes: MA-AOU prefecture -> province MA-FAH prefecture -> province MA-TET prefecture -> province Parent changes: MA-AGD MA-13 -> MA-09 MA-AOU MA-16 -> MA-12 MA-ASZ MA-14 -> MA-10 MA-AZI MA-12 -> MA-05 MA-BEM MA-12 -> MA-05 MA-BER MA-04 -> MA-02 MA-BES MA-09 -> MA-06 MA-BOD MA-15 -> MA-11 MA-BOM MA-05 -> MA-03 MA-CHI MA-11 -> MA-07 MA-CHT MA-13 -> MA-06 MA-ERR MA-06 -> MA-08 MA-ESI MA-11 -> MA-07 MA-ESM MA-14 -> MA-11 MA-FES MA-05 -> MA-03 MA-FIG MA-04 -> MA-02 MA-GUE MA-14 -> MA-10 MA-HAJ MA-06 -> MA-03 MA-HAO MA-11 -> MA-07 MA-HOC MA-03 -> MA-01 MA-IFR MA-06 -> MA-03 MA-INE MA-13 -> MA-09 MA-JDI MA-10 -> MA-06 MA-JRA MA-04 -> MA-02 MA-KEN MA-02 -> MA-04 MA-KES MA-11 -> MA-07 MA-KHE MA-07 -> MA-04 MA-KHN MA-06 -> MA-05 MA-KHO MA-09 -> MA-05 MA-LAA MA-15 -> MA-11 MA-MED MA-08 -> MA-06 MA-MEK MA-06 -> MA-03 MA-MOH MA-08 -> MA-06 MA-MOU MA-05 -> MA-03 MA-NAD MA-04 -> MA-02 MA-NOU MA-08 -> MA-04 MA-OUA MA-13 -> MA-08 MA-OUD MA-16 -> MA-12 MA-OUJ MA-04 -> MA-02 MA-RAB MA-07 -> MA-04 MA-SAF MA-10 -> MA-07 MA-SAL MA-07 -> MA-04 MA-SEF MA-05 -> MA-03 MA-SET MA-09 -> MA-08 MA-SIK MA-02 -> MA-06 MA-SKH MA-07 -> MA-04 MA-TAI MA-04 -> MA-02 MA-TAR MA-13 -> MA-09 MA-TAT MA-14 -> MA-09 MA-TIZ MA-13 -> MA-09 MA-TNT MA-14 -> MA-10 MA-ZAG MA-13 -> MA-08.",
             "Date Issued": "2018-04-20",
-            "Description of Change in Newsletter": "Modification of remark part 2; deletion of regions MA-01 to MA-16; addition of new regions MA-01 to MA-12; change of spelling of MA-AGD, MA-BES, MA-ESM, MA-FAH, MA-FES, MA-JRA, MA-KES, MA-OUD; change of category name from prefecture to province for MA-AOU, MA-FAH, MA-TET; addition of prefectures MA-MAR, MA-MDF; deletion of prefectures, MA-MMD, MA-MMN, MA-SYB; addition of provinces MA-BRR, MA-DRI, MA-FQH, MA-GUF, MA-MID, MA-OUZ, MA-REH, MA-SIF, MA-SIL, MA-SIB, MA-TAF, MA-TIN, MA-YUS; change of parent subdivision for MA-AGD, MA-AOU, MA-FES, MA-INE, MA-MEK, MA-MOH, MA-OUJ, MA-RAB, MA-SAL, MA-SKH, MA-ASZ, MA-AZI, MA-BEM, MA-BER, MA-BES, MA-BOD, MA-BOM, MA-CHI, MA-CHT, MA-ERR, MA-ESI, MA-ESM, MA-FIG, MA-GUE, MA-HAJ, MA-HAO, MA-HOC, MA-IFR, MA-JDI, MA-JRA, MA-KEN, MA-KES, MA-KHE, MA-KHN, MA-KHO, MA-LAA, MA-MED, MA-MOU, MA-NAD, MA-NOU, MA-OUA, MA-OUD, MA-SAF, MA-SEF, MA-SET, MA-SIK, MA-TAI, MA-TAR, MA-TAT, MA-TIZ, MA-TNT, MA-ZAG; addition of (EH) to MA-LAA; addition of (EH-partial) to MA-ASZ, MA-TNT; update List Source.",
+            "Description of Change": "Modification of remark part 2; deletion of regions MA-01 to MA-16; addition of new regions MA-01 to MA-12; change of spelling of MA-AGD, MA-BES, MA-ESM, MA-FAH, MA-FES, MA-JRA, MA-KES, MA-OUD; change of category name from prefecture to province for MA-AOU, MA-FAH, MA-TET; addition of prefectures MA-MAR, MA-MDF; deletion of prefectures, MA-MMD, MA-MMN, MA-SYB; addition of provinces MA-BRR, MA-DRI, MA-FQH, MA-GUF, MA-MID, MA-OUZ, MA-REH, MA-SIF, MA-SIL, MA-SIB, MA-TAF, MA-TIN, MA-YUS; change of parent subdivision for MA-AGD, MA-AOU, MA-FES, MA-INE, MA-MEK, MA-MOH, MA-OUJ, MA-RAB, MA-SAL, MA-SKH, MA-ASZ, MA-AZI, MA-BEM, MA-BER, MA-BES, MA-BOD, MA-BOM, MA-CHI, MA-CHT, MA-ERR, MA-ESI, MA-ESM, MA-FIG, MA-GUE, MA-HAJ, MA-HAO, MA-HOC, MA-IFR, MA-JDI, MA-JRA, MA-KEN, MA-KES, MA-KHE, MA-KHN, MA-KHO, MA-LAA, MA-MED, MA-MOU, MA-NAD, MA-NOU, MA-OUA, MA-OUD, MA-SAF, MA-SEF, MA-SET, MA-SIK, MA-TAI, MA-TAR, MA-TAT, MA-TIZ, MA-TNT, MA-ZAG; addition of (EH) to MA-LAA; addition of (EH-partial) to MA-ASZ, MA-TNT; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change spelling of MA-14; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change spelling of MA-14; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MA)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: MA-AOU Aousserd MA-FAH Fahs-Anjra MA-MED M\u00e9diouna MA-MMD Marrakech-Medina MA-MMN Marrakech-Menara MA-MOH Mohammadia MA-MOU Moulay Yacoub MA-NOU Nouaceur MA-RAB Rabat MA-SAL Sal\u00e9 MA-SKH Skhirate-T\u00e9mara MA-SYB Sidi Youssef Ben Ali MA-TAI Taourirt MA-ZAG Zagora Subdivisions deleted: MA-MAR Marrakech MA-RBA Rabat-Sal\u00e9 Code changes: MA-BAH A\u00eft Baha -> MA-CHT Chtouka-Ait Baha MA-MEL A\u00eft Melloul -> MA-INE Inezgane-Ait Melloul.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling for La\u00e2youne.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Change of spelling for La\u00e2youne.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 7 economic regions (see below) -> 16 economic regions (now called regions) Code changes: Jerada: MA-IRA -> MA-JRA.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "New subdivision layout at economic region level. List source updated. Addition of one reference in the code source. Two name spellings corrected. One code corrected.",
+            "Description of Change": "New subdivision layout at economic region level. List source updated. Addition of one reference in the code source. Two name spellings corrected. One code corrected.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "MC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Administrative subdivisions addition.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative subdivisions addition.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "MD": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the French short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the administrative language codes from mo, mol to ro, ron.",
             "Date Issued": "2015-08-04",
-            "Description of Change in Newsletter": "Correction of the administrative language codes from mo, mol to ro, ron.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision name of MD-BD.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change subdivision name of MD-BD.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages, and update of the administrative structure and of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name.",
             "Date Issued": "2009-01-07",
-            "Description of Change in Newsletter": "Change of short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of administrative language from Romanian (ro, ron) to Moldavian (mo, mol).",
             "Date Issued": "2008-09-09",
-            "Description of Change in Newsletter": "Correction of administrative language from Romanian (ro, ron) to Moldavian (mo, mol).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name.",
             "Date Issued": "2008-04-08",
-            "Description of Change in Newsletter": "Change of short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: MD-TA Taraclia.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one district. Subdivision categories in header re-sorted.",
+            "Description of Change": "Addition of one district. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Error correction: Header information on number of districts corrected.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Error correction: Header information on number of districts corrected.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 10 cities, 40 districts (see below) -> 1 autonomous territory, 1 city, 1 territorial unit, 9 districts.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Completely new subdivision layout.",
+            "Description of Change": "Completely new subdivision layout.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "ME": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of municipality ME-25; Update List Source.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Addition of municipality ME-25; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Update List Source; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of municipality ME-24; Update List Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Addition of municipality ME-24; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of remark part 2.",
             "Date Issued": "2018-03-26",
-            "Description of Change in Newsletter": "Deletion of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of quotation marks in the remark.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Correction of quotation marks in the remark.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Remarks to Parts 1 and 2 concerning the language code \"001\" to read \"The language code \"001\" refers to the administrative language \"Montenegrin\" that has not been assigned an ISO 639 language code.\".",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the Remarks to Parts 1 and 2 concerning the language code \"001\" to read \"The language code \"001\" refers to the administrative language \"Montenegrin\" that has not been assigned an ISO 639 language code.\".",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add two municipalities ME-22 and ME-23.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add two municipalities ME-22 and ME-23.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Local generic administrative term addition and suppression of the comment.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Local generic administrative term addition and suppression of the comment.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of full name.",
             "Date Issued": "2008-04-08",
-            "Description of Change in Newsletter": "Change of full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ME)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 21 municipalities.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of a new country (in accordance with ISO 3166-1 Newsletter V-12).",
+            "Description of Change": "Addition of a new country (in accordance with ISO 3166-1 Newsletter V-12).",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "MF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-MF)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-MF)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Martin, partie nord de\u201d in the French name field for Territory.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Martin, partie nord de\u201d in the French name field for Territory.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling error in the French remarks.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Correct spelling error in the French remarks.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of new entry (in accordance with ISO 3166-1 Newsletter VI-1).",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of new entry (in accordance with ISO 3166-1 Newsletter VI-1).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add new entry.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Add new entry.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MF)."
         }
     ],
     "MG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Inclusion of English as official language in Article 4 of the Constitution of Madagascar, April 2007.",
             "Date Issued": "2008-04-08",
-            "Description of Change in Newsletter": "Inclusion of English as official language in Article 4 of the Constitution of Madagascar, April 2007.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MG)."
         }
     ],
     "MH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the French short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of subdivision name in mah of MH\u2010ALK, MH\u2010ALL, MH\u2010ARN, MH\u2010EBO, MH\u2010JAB, MH\u2010JAL, MH\u2010KWA, MH\u2010LIB, MH\u2010MAJ, MH\u2010MAL, MH\u2010MEJ, MH\u2010MIL, MH\u2010NMK, MH\u2010NMU, MH\u2010RON, MH\u2010UTI, MH\u2010WTH, WTJ; in mah/eng of MH-ENI, MH-KIL; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of subdivision name in mah of MH\u2010ALK, MH\u2010ALL, MH\u2010ARN, MH\u2010EBO, MH\u2010JAB, MH\u2010JAL, MH\u2010KWA, MH\u2010LIB, MH\u2010MAJ, MH\u2010MAL, MH\u2010MEJ, MH\u2010MIL, MH\u2010NMK, MH\u2010NMU, MH\u2010RON, MH\u2010UTI, MH\u2010WTH, WTJ; in mah/eng of MH-ENI, MH-KIL; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling changes to MH-ENI, MH-KIL, MH-NMK and MH-UTI; update the List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Spelling changes to MH-ENI, MH-KIL, MH-NMK and MH-UTI; update the List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MH)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MH)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: MH-JAB Jabat Subdivisions deleted: MH-UJL Ujelang.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         }
     ],
     "MK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of municipality MK-85; Change of subdivision code from MK-02 to MK-802, MK-03 to MK-201, MK-04 to MK-501, MK-05 to MK-401, MK-06 to MK-601, MK-07 to MK-402, MK-08 to MK-602, MK-10 to MK-403, MK-11 to MK-404, MK-12 to MK-301, MK-13 to MK-101, MK-14 to MK-202, MK-16 to MK-603, MK-18 to MK-405, MK-19 to MK-604, MK-20 to MK-102, MK-21 to MK-303, MK-22 to MK-304, MK-23 to MK-203, MK-24 to MK-103, MK-25 to MK-502, MK-26 to MK-406, MK-27 to MK-503, MK-30 to MK-605, MK-32 to MK-806, MK-33 to MK-204, MK-34 to MK-807, MK-35 to MK-606, MK-36 to MK-104, MK-37 to MK-205, MK-40 to MK-307, MK-41 to MK-407, MK-42 to MK-206, MK-43 to MK-701, MK-44 to MK-702, MK-45 to MK-504, MK-46 to MK-505, MK-47 to MK-703, MK-48 to MK-704, MK-49 to MK-105, MK-50 to MK-607, MK-51 to MK-207, MK-52 to MK-308, MK-53 to MK-506, MK-54 to MK-106, MK-55 to MK-507, MK-56 to MK-408, MK-58 to MK-310, MK-59 to MK-810, MK-60 to MK-208, MK-61 to MK-311, MK-62 to MK-508, MK-63 to MK-209, MK-64 to MK-409, MK-65 to MK-705, MK-66 to MK-509, MK-67 to MK-107, MK-69 to MK-108, MK-70 to MK-812, MK-71 to MK-706, MK-72 to MK-312, MK-73 to MK-410, MK-74 to MK-813, MK-75 to MK-608, MK-76 to MK-609, MK-78 to MK-313, MK-80 to MK-109, MK-81 to MK-210, MK-82 to MK-816, MK-83 to MK-211; Typographical correction of subdivision name of MK-816, addition of municipality MK-801, MK-803, MK-804, MK-805, MK-808, MK-809, MK-811, MK-814, MK-815, MK-817; Update List Source; Update Code Source.",
             "Date Issued": "2020-03-02",
-            "Description of Change in Newsletter": "Deletion of municipality MK-85; Change of subdivision code from MK-02 to MK-802, MK-03 to MK-201, MK-04 to MK-501, MK-05 to MK-401, MK-06 to MK-601, MK-07 to MK-402, MK-08 to MK-602, MK-10 to MK-403, MK-11 to MK-404, MK-12 to MK-301, MK-13 to MK-101, MK-14 to MK-202, MK-16 to MK-603, MK-18 to MK-405, MK-19 to MK-604, MK-20 to MK-102, MK-21 to MK-303, MK-22 to MK-304, MK-23 to MK-203, MK-24 to MK-103, MK-25 to MK-502, MK-26 to MK-406, MK-27 to MK-503, MK-30 to MK-605, MK-32 to MK-806, MK-33 to MK-204, MK-34 to MK-807, MK-35 to MK-606, MK-36 to MK-104, MK-37 to MK-205, MK-40 to MK-307, MK-41 to MK-407, MK-42 to MK-206, MK-43 to MK-701, MK-44 to MK-702, MK-45 to MK-504, MK-46 to MK-505, MK-47 to MK-703, MK-48 to MK-704, MK-49 to MK-105, MK-50 to MK-607, MK-51 to MK-207, MK-52 to MK-308, MK-53 to MK-506, MK-54 to MK-106, MK-55 to MK-507, MK-56 to MK-408, MK-58 to MK-310, MK-59 to MK-810, MK-60 to MK-208, MK-61 to MK-311, MK-62 to MK-508, MK-63 to MK-209, MK-64 to MK-409, MK-65 to MK-705, MK-66 to MK-509, MK-67 to MK-107, MK-69 to MK-108, MK-70 to MK-812, MK-71 to MK-706, MK-72 to MK-312, MK-73 to MK-410, MK-74 to MK-813, MK-75 to MK-608, MK-76 to MK-609, MK-78 to MK-313, MK-80 to MK-109, MK-81 to MK-210, MK-82 to MK-816, MK-83 to MK-211; Typographical correction of subdivision name of MK-816, addition of municipality MK-801, MK-803, MK-804, MK-805, MK-808, MK-809, MK-811, MK-814, MK-815, MK-817; Update List Source; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the short and full name: Macedonia (the former Yugoslav Republic of) -> North Macedonia; the former Yugoslav Republic of Macedonia -> Republic of North Macedonia.",
             "Date Issued": "2019-03-13",
-            "Description of Change in Newsletter": "Change of the short and full name: Macedonia (the former Yugoslav Republic of) -> North Macedonia; the former Yugoslav Republic of Macedonia -> Republic of North Macedonia.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of municipalities MK-01, MK-09, MK-15, MK-17, MK-28, MK-29, MK-31, MK-38, MK-39, MK-57, MK-68, MK-77, MK-79, MK-84; deletion of remark; change romanization system; addition of municipality MK-85; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of municipalities MK-01, MK-09, MK-15, MK-17, MK-28, MK-29, MK-31, MK-38, MK-39, MK-57, MK-68, MK-77, MK-79, MK-84; deletion of remark; change romanization system; addition of municipality MK-85; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: format changed (see below).",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of numeric code elements.",
+            "Description of Change": "Addition of numeric code elements.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 84 municipalities.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "ML": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of regions ML-9, ML-10; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Addition of regions ML-9, ML-10; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ML)."
         }
     ],
     "MM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of MM-07, MM-05; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of MM-07, MM-05; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision category divisions to regions; change spellings of MM-05 and MM-07; add one union territory MM-18.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change subdivision category divisions to regions; change spellings of MM-05 and MM-07; add one union territory MM-18.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local generic administrative terms, source list update and addition of a comment.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of local generic administrative terms, source list update and addition of a comment.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Official name change of long name.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Official name change of long name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Official name change of long name.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Official name change of long name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MM)."
         }
     ],
     "MN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MN)."
         }
     ],
     "MO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (subdivision in 2 districts, distrito (pt), which is not relevant for this part of ISO 3166. Included also as a subdivision of China (CN-MO)).",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Modification of remark part 2 (subdivision in 2 districts, distrito (pt), which is not relevant for this part of ISO 3166. Included also as a subdivision of China (CN-MO)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the English country name. In accordance with ISO 3166-1 Newsletter V-4.",
             "Date Issued": "2002-05-20",
-            "Description of Change in Newsletter": "Change of the English country name. In accordance with ISO 3166-1 Newsletter V-4.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         }
     ],
     "MP": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-MP)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-MP)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MP)."
         }
     ],
     "MQ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-972)).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-972)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MQ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MQ)."
         }
     ],
     "MR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the romanization system for MR-13, MR-14, MR-15 in fra.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Deletion of the romanization system for MR-13, MR-14, MR-15 in fra.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of regions MR-13, MR-14, MR-15; deletion of district MR-NKC; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of regions MR-13, MR-14, MR-15; deletion of district MR-NKC; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MR)."
         }
     ],
     "MS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MS)."
         }
     ],
     "MT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of subdivision category in mlt.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of subdivision category in mlt.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of quotation marks in the List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Correction of quotation marks in the List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MT)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 68 local councils.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         }
     ],
     "MU": [
         {
             "Code/Subdivision Change": "Deleted: MU-BR ()Beau Bassin-Rose Hill), MU-CU ()Curepipe), MU-PU ()Port Louis), MU-QB ()Quatre Bornes), MU-VP ()Vacoas-Phoenix).",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of city MU-BR, MU-CU, MU-PU, MU-QB, MU-VP; Update List Source; Correction of the Code Source.",
+            "Description of Change": "Deletion of city MU-BR, MU-CU, MU-PU, MU-QB, MU-VP; Update List Source; Correction of the Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MU)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use) Port Louis (city): MU-PL -> MU-PU.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Error correction: Duplicate use of one code element corrected. Subdivision categories in header re-sorted.",
+            "Description of Change": "Error correction: Duplicate use of one code element corrected. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "MV": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MV)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: MV-CE Central MV-NC North Central MV-NO North MV-SC South Central MV-SU South MV-UN Upper North MV-US Upper South Category changes: MV-MLE capital -> city MV-01 administrative atoll -> city Spelling changes (dv): MV-00 Ari Atholhu Dhekunuburi -> Ariatholhu Dhekunuburi MV-02 Ari Atholhu Uthuruburi -> Ariatholhu Uthuruburi MV-04 Ari Atholhu Uthuruburi -> Felidheatholhu MV-14 Ari Atholhu Uthuruburi -> Nilandheatholhu Uthuruburi MV-17 Nilandhe Atholhu Dhekunuburi -> Nilandheatholhu Dhekunuburi MV-26 Maale Atholhu -> MV-27 -> Maaleatholhu MV-28 Huvadhu Atholhu Dhekunuburi -> Huvadhuatholhu Dhekunuburi Spelling changes (en): MV-00 Alifu Dhaalu -> South Ari Atoll MV-01 Seenu -> Addu City MV-02 Alifu Alifu -> North Ari Atoll MV-03 Lhaviyani -> Faadhippolhu MV-04 Vaavu -> Felidhu Atoll MV-05 Laamu -> Felidhu Atoll MV-07 Haa Alifu -> North Thiladhunmathi MV-08 Thaa -> Kolhumadulu MV-12 Meemu -> Mulaku Atoll MV-13 Raa -> Mulaku Atoll MV-14 Faafu -> North Nilandhe Atoll MV-17 Dhaalu -> South Nilandhe Atoll MV-20 Baa -> South Nilandhe Atoll MV-23 Haa Dhaalu -> South Thiladhunmathi MV-24 Shaviyani -> North Miladhunmadulu MV-25 Noonu -> South Miladhunmadulu MV-26 Kaafu -> South Miladhunmadulu MV-27 Gaafu Alifu -> North Huvadhu Atoll MV-28 Gaafu Dhaalu -> North Huvadhu Atoll MV-29 Gnaviyani -> Fuvammulah Local variants added: all subdivisions.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of spelling in div of MV-00, MV-02, MV-04, MV-14, MV-17, MV-26, MV-27, MV-28; Change of spelling in eng of MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Addition of local variation of MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Change of category name from capital to city for MV-MLE; Change of category name from administrative atoll to city for MV-01; Removal of parent subdivision of MV-MLE, MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Deletion of provinces MV-CE, MV-NC, MV-NO, MV-SC, MV-SU, MV-UN and MV-US; Update List Source.",
+            "Description of Change": "Change of spelling in div of MV-00, MV-02, MV-04, MV-14, MV-17, MV-26, MV-27, MV-28; Change of spelling in eng of MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Addition of local variation of MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Change of category name from capital to city for MV-MLE; Change of category name from administrative atoll to city for MV-01; Removal of parent subdivision of MV-MLE, MV-00, MV-01, MV-02, MV-03, MV-04, MV-05, MV-07, MV-08, MV-12, MV-13, MV-14, MV-17, MV-20, MV-23, MV-24, MV-25, MV-26, MV-27, MV-28, MV-29; Deletion of provinces MV-CE, MV-NC, MV-NO, MV-SC, MV-SU, MV-UN and MV-US; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MV)."
         },
         {
             "Code/Subdivision Change": "Spelling change: MV-05.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of MV-05.",
+            "Description of Change": "Change of spelling of MV-05.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MV)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 7 provinces MV-00 Alifu Dhaalu.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative re-organization, addition of local generic administrative terms, language adjustment and source list update.",
+            "Description of Change": "Administrative re-organization, addition of local generic administrative terms, language adjustment and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "MW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MW)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: MW-NE Neno.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages, typographical error correction, update of the administrative structure and of the list source.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages, typographical error correction, update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: MW-BA Balaka MW-LK Likoma Island MW-PH Phalombe.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of three districts. List source updated.",
+            "Description of Change": "Addition of three districts. List source updated.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "MX": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from federal district to federal entity; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of subdivision category from federal district to federal entity; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of MX-CMX; update List source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Typographical correction of MX-CMX; update List source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision code from MX-DIF to MX-CMX; change of name of MX-CMX, MX-COA, MX-MIC, MX-VER; addition of local variation of MX-COA, MX-MIC, MX-VER; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision code from MX-DIF to MX-CMX; change of name of MX-CMX, MX-COA, MX-MIC, MX-VER; addition of local variation of MX-COA, MX-MIC, MX-VER; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-04",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:MX)."
         }
     ],
     "MY": [
         {
             "Code/Subdivision Change": "Subdivisions added: MY-16 Wilayah Persekutuan Putrajaya Codes: format changed (see below).",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Addition of one federal territory. Inclusion of new codes. List source updated. Code source updated.",
+            "Description of Change": "Addition of one federal territory. Inclusion of new codes. List source updated. Code source updated.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "MZ": {},
     "NA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of NA-KA; Change of local variation of NA-KA; Addition of local variation of NA-KA; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of NA-KA; Change of local variation of NA-KA; Addition of local variation of NA-KA; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of local variation of NA-KA; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Addition of local variation of NA-KA; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete 1 region NA-OK; add two regions NA-KE and NA-KW; change subdivision name of NA-CA.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Delete 1 region NA-OK; add two regions NA-KE and NA-KW; change subdivision name of NA-CA.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NA)."
         }
     ],
     "NC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-NC)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-NC)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NC)."
         }
     ],
     "NE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision category from department to region; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change subdivision category from department to region; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NE)."
         }
     ],
     "NF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NF)."
         }
     ],
     "NG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change spelling of NG-NA; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change spelling of NG-NA; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Consistency between ISO 3166-1 and ISO 3166-2, addition of names in administrative languages.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of French (fr, fra) as an administrative language.",
             "Date Issued": "2008-09-09",
-            "Description of Change in Newsletter": "Deletion of French (fr, fra) as an administrative language.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NG)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: NG-BY Bayelsa NG-EB Ebonyi NG-EK Ekiti NG-GO Gombe NG-NA Nassarawa NG-ZA Zamfara.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Addition of 6 new states.",
+            "Description of Change": "Addition of 6 new states.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "NI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NI)."
         },
         {
             "Code/Subdivision Change": "Name change: NI-AN Atl\u00e1ntico Norte -> Costa Caribe Norte NI-AS Atl\u00e1ntico Sur -> Costa Caribe Sur.",
             "Date Issued": "2018-04-20",
-            "Description of Change in Newsletter": "Change of subdivision name of NI-AN, NI-AS; update List Source.",
+            "Description of Change": "Change of subdivision name of NI-AN, NI-AS; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NI)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: NI-AN Atl\u00e1ntico Norte NI-AS Atl\u00e1ntico Sur Subdivisions deleted: NI-ZE Zelaya.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Deletion of one department. Addition of two autonomous regions. New list source.",
+            "Description of Change": "Deletion of one department. Addition of two autonomous regions. New list source.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "NL": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the short name.",
             "Date Issued": "2023-04-04",
-            "Description of Change in Newsletter": "Change of the short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NL)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 3 countries 3 special municipalities.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Update resulting from the addition of the administrative readjustment and source list update.",
+            "Description of Change": "Update resulting from the addition of the administrative readjustment and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the English name to Sint Eustatius in alignment with UNTERM.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Correct the English name to Sint Eustatius in alignment with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the English name to Sint Eustatius in alignment with UNTERM.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Correct the English name to Sint Eustatius in alignment with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add Bonaire, Saint Eustatius and Saba Islands.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Add Bonaire, Saint Eustatius and Saba Islands.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NL)."
         }
     ],
     "NO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Subdivisions deleted: NO-01 \u00d8stfold NO-02 Akershus NO-04 Hedmark NO-05 Oppland NO-06 Buskerud NO-07 Vestfold NO-08 Telemark NO-09 Aust-Agder NO-10 Vest-Agder NO-12 Hordaland NO-14 Sogn og Fjordane NO-19 Troms NO-20 Finnmark Subdivisions added: NO-30 Viken NO-34 Innlandet NO-38 Vestfold og Telemark NO-42 Agder NO-46 Vestland NO-54 Troms og Finnmark.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Subdivisions deleted: NO-01 \u00d8stfold NO-02 Akershus NO-04 Hedmark NO-05 Oppland NO-06 Buskerud NO-07 Vestfold NO-08 Telemark NO-09 Aust-Agder NO-10 Vest-Agder NO-12 Hordaland NO-14 Sogn og Fjordane NO-19 Troms NO-20 Finnmark Subdivisions added: NO-30 Viken NO-34 Innlandet NO-38 Vestfold og Telemark NO-42 Agder NO-46 Vestland NO-54 Troms og Finnmark.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Code change: Tr\u00f8ndelag: NO-23 -> NO-50.",
             "Date Issued": "2019-04-09",
-            "Description of Change in Newsletter": "Code change: Tr\u00f8ndelag: NO-23 -> NO-50.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Subdivisions deleted: NO-16 S\u00f8r-Tr\u00f8ndelag NO-17 Nord-Tr\u00f8ndelag Subdivisions added: NO-23 Tr\u00f8ndelag.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Subdivisions deleted: NO-16 S\u00f8r-Tr\u00f8ndelag NO-17 Nord-Tr\u00f8ndelag Subdivisions added: NO-23 Tr\u00f8ndelag.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NO)."
         }
     ],
     "NP": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of NP-P1; Update List Source.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Change of subdivision name of NP-P1; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of development regions NP-1, NP-2, NP-3, NP-4, NP-5; Change of subdivision name of NP-P4, NP-P6 in nep; Change of subdivision name of NP-P2, NP-P7 in eng and nep; Change of subdivision name of NP-P3 in eng; Addition of location variation for NP-2 in eng and nep; Modification of local variation for NP-P7 in eng and nep; Deletion of zones NP-BA, NP-BH, NP-DH, NP-GA, NP-JA, NP-KA, NP-KO, NP-LU, NP-MA, NP-ME, NP-NA, NP-RA, NP-SA, NP-SE: Update List Source; Modification of remark part 2 (in September 2015 Nepal created a new federal structure consisting of seven numbered provinces. Six of these provinces have now been named. The remaining province is identified by number only. These provinces have replaced the zones and development regions).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Deletion of development regions NP-1, NP-2, NP-3, NP-4, NP-5; Change of subdivision name of NP-P4, NP-P6 in nep; Change of subdivision name of NP-P2, NP-P7 in eng and nep; Change of subdivision name of NP-P3 in eng; Addition of location variation for NP-2 in eng and nep; Modification of local variation for NP-P7 in eng and nep; Deletion of zones NP-BA, NP-BH, NP-DH, NP-GA, NP-JA, NP-KA, NP-KO, NP-LU, NP-MA, NP-ME, NP-NA, NP-RA, NP-SA, NP-SE: Update List Source; Modification of remark part 2 (in September 2015 Nepal created a new federal structure consisting of seven numbered provinces. Six of these provinces have now been named. The remaining province is identified by number only. These provinces have replaced the zones and development regions).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of NP-P5; Modification of remark part 2; Update List Source.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Change of spelling of NP-P5; Modification of remark part 2; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the full name.",
             "Date Issued": "2021-01-20",
-            "Description of Change in Newsletter": "Change of the full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of NP-P3, NP-P7; Addition of local variation of NP-P3, NP-P7; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of NP-P3, NP-P7; Addition of local variation of NP-P3, NP-P7; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update Code Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label; Addition of provinces NP-P1, NP-P2, NP-P3, NP-P4, NP-P5, NP-P6, NP-P7; Addition of local variation for NP-P4 and NP-P6; Update List Source; Addition of remark.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label; Addition of provinces NP-P1, NP-P2, NP-P3, NP-P4, NP-P5, NP-P6, NP-P7; Addition of local variation for NP-P4 and NP-P6; Update List Source; Addition of remark.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "First level prefix addition, language adjustment, comment addition, deletion of the romanization system and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "First level prefix addition, language adjustment, comment addition, deletion of the romanization system and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the formal name.",
             "Date Issued": "2008-09-09",
-            "Description of Change in Newsletter": "Modification of the formal name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NP)."
         }
     ],
     "NR": [
         {
             "Code/Subdivision Change": "Name changed: NR-05 Baiti -> Baitsi.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of subdivision name of NR-05; addition of local variation of NR-05, update List Source.",
+            "Description of Change": "Change of subdivision name of NR-05; addition of local variation of NR-05, update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Local generic administrative term addition.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Local generic administrative term addition.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 14 districts.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20081218103230/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "NU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the long name which was incorrect.",
             "Date Issued": "2011-07-14",
-            "Description of Change in Newsletter": "Correct the long name which was incorrect.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the long name which was incorrect.",
             "Date Issued": "2011-06-12",
-            "Description of Change in Newsletter": "Correct the long name which was incorrect.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NU)."
         }
     ],
     "NZ": [
         {
             "Code/Subdivision Change": "Subdivision changed: NZ-AUK.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Deletion of the space before the dash of NZ-AUK in mri.",
+            "Description of Change": "Deletion of the space before the dash of NZ-AUK in mri.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NZ)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of subdivision name of NZ-AUK, NZ-BOP, NZ-STL, NZ-GIS, NZ-HKB, NZ-NTL, NZ-WTC in mri; Change of subdivision name of NZ-WGN, NZ-MWT in eng and mri; Addition of subdivision name for NZ-WKO in eng; Addition of subdivision name for NZ-TAS in mri; Update List Source.",
+            "Description of Change": "Change of subdivision name of NZ-AUK, NZ-BOP, NZ-STL, NZ-GIS, NZ-HKB, NZ-NTL, NZ-WTC in mri; Change of subdivision name of NZ-WGN, NZ-MWT in eng and mri; Addition of subdivision name for NZ-WKO in eng; Addition of subdivision name for NZ-TAS in mri; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NZ)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of all unitary authorities; deletion of islands NZ-N, NZ-S; Change of subdivision name of NZ-GIS, NZ-MBH, NZ-NSN, NZ-TAS, change of subdivision category from regional council to region; update List Source.",
+            "Description of Change": "Deletion of all unitary authorities; deletion of islands NZ-N, NZ-S; Change of subdivision name of NZ-GIS, NZ-MBH, NZ-NSN, NZ-TAS, change of subdivision category from regional council to region; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NZ)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change subdivision category of NZ-AUK.",
+            "Description of Change": "Change subdivision category of NZ-AUK.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:NZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: NZ-CIT Chatham Islands Territory.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "OM": [
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision category from region to governate for OM-BA, OM-DA, OM-SH, OM-WU, OM-ZA; change of subdivision code from OM-BA to OM-BJ, from OM-SH to OM-SJ; change of spelling of OM-BJ, OM-SJ; addition of governorates OM-BS, OM-SS; addition of local variations of OM-MA, OM-ZU; update List Source.",
+            "Description of Change": "Change of subdivision category from region to governate for OM-BA, OM-DA, OM-SH, OM-WU, OM-ZA; change of subdivision code from OM-BA to OM-BJ, from OM-SH to OM-SJ; change of spelling of OM-BJ, OM-SJ; addition of governorates OM-BS, OM-SS; addition of local variations of OM-MA, OM-ZU; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:OM)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: OM-BU Al Buraym\u012b Codes: OM-JA Al Jan\u016bb\u012byah -> OM-ZU Z\u0327uf\u0101r.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "PA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of subdivision name of PA-NB; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of spelling of subdivision name of PA-NB; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of indigenous region PA-NT; Update List Source.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Addition of indigenous region PA-NT; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision name of PA-KY; addition of local variation of PA-KY, update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of subdivision name of PA-KY; addition of local variation of PA-KY, update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 province PA-10; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 1 province PA-10; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PA)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: PA-EM Ember\u00e1 PA-NB Ng\u00f6be-Bugl\u00e9 Codes: PA-0 Comarca de San Blas -> PA-KY Kuna Yala.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "PE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change Subdivision categories from department and constitutional province to region; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change Subdivision categories from department and constitutional province to region; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PE)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: PE-LMA Municipalidad Metropolitana de Lima.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and languages and update of the list source.",
+            "Description of Change": "Update of the administrative structure and languages and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         }
     ],
     "PF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-PF)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-PF)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete the Clipperton Island.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Delete the Clipperton Island.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PF)."
         }
     ],
     "PG": [
         {
             "Code/Subdivision Change": "Subdivisions added: PG-HLA Hela PG-JWK Jiwaka Name changed: PG-SAN Sandaun [West Sepik] -> West Sepik.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add two provinces PG-HLA and PG-JWK; change subdivision name of PG-SAN; update List Source.",
+            "Description of Change": "Add two provinces PG-HLA and PG-JWK; change subdivision name of PG-SAN; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add \"the\" before the English full name.",
             "Date Issued": "2014-03-03",
-            "Description of Change in Newsletter": "Add \"the\" before the English full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "UN notification of full name.",
             "Date Issued": "2013-05-10",
-            "Description of Change in Newsletter": "UN notification of full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PG)."
         },
         {
             "Code/Subdivision Change": "Codes: PG-NSA North Solomons (province) -> PG-NSB Bougainville (autonomous region).",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative readjustment, local generic administrative term addition and source list and source code update.",
+            "Description of Change": "Administrative readjustment, local generic administrative term addition and source list and source code update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "PH": [
         {
             "Code/Subdivision Change": "Subdivision deleted: PH-MAG Maguindanao Subdivisions added: PH-MGN Maguindanao del Norte PH-MGS Maguindanao del Sur.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Deletion of province PH-MAG; Addition of province PH-MGN, PH-MGS.",
+            "Description of Change": "Deletion of province PH-MAG; Addition of province PH-MGN, PH-MGS.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PH)."
         },
         {
             "Code/Subdivision Change": "Subdivisions renamed: PH-COM Compostela Valley -> Davao de Oro.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of PH-COM in eng; Deletion of subdivision name of PH-COM in tgl; Update List Source ; Correction of the Code Source.",
+            "Description of Change": "Change of subdivision name of PH-COM in eng; Deletion of subdivision name of PH-COM in tgl; Update List Source; Correction of the Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PH)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: PH-DVO Davao Occidental.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of province PH-DVO.",
+            "Description of Change": "Addition of province PH-DVO.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PH)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: PH-40 Calabarzon PH-41 Mimaropa PH-DIN Dinagat Islands Subdivisions deleted: PH-04 Southern Tagalog.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
+            "Description of Change": "Addition of the country code prefix as the first code element, addition of names in administrative languages, update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: PH-13 Caraga PH-APA Apayao PH-BIL Biliran PH-COM Compostela Valley PH-GUI Guimaras PH-SAR Sarangani PH-ZSI Zamboanga Sibugay Codes: Cordillera Administrative Region: PH-13 -> PH-15.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of one region and six provinces. New list source and code source. Precise specification of and minor corrections to the spelling of names.",
+            "Description of Change": "Addition of one region and six provinces. New list source and code source. Precise specification of and minor corrections to the spelling of names.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "PK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PK)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Deletion of territory PK-TA; Update List Source.",
+            "Description of Change": "Deletion of territory PK-TA; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PK)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of category name from ilaqa to \u2018al\u0101qahilaqa, from suba to s\u016bbah, from wafaqi dar-ul-hakumat ka ilaqa to waf\u0101q\u012b d\u0101r al \u1e29ik\u016bmat \u2018al\u0101qah; change of subdivision name of PK-JK (eng & urd); addition of local variation of PK-JK in eng; update List Source.",
+            "Description of Change": "Change of spelling of category name from ilaqa to \u2018al\u0101qahilaqa, from suba to s\u016bbah, from wafaqi dar-ul-hakumat ka ilaqa to waf\u0101q\u012b d\u0101r al \u1e29ik\u016bmat \u2018al\u0101qah; change of subdivision name of PK-JK (eng & urd); addition of local variation of PK-JK in eng; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of romanization system for urd.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of romanization system for urd.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PK)."
         },
         {
             "Code/Subdivision Change": "Codes: PK-NW North-West Frontier -> PK-KP Khyber Pakhtunkhwa PK-NA Northern Areas -> PK-GB Gilgit-Baltistan.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Name change, language readjustment and source list update.",
+            "Description of Change": "Name change, language readjustment and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "PL": [
         {
             "Code/Subdivision Change": "Name changes: 04 Kujawsko-pomorskie -> Kujawsko-Pomorskie 28 Warmi\u0144sko-mazurskie -> Warmi\u0144sko-Mazurskie.",
             "Date Issued": "2023-11-23",
-            "Description of Change in Newsletter": "Change of spelling of PL-04, PL-28; Update Code Source and List Source.",
+            "Description of Change": "Change of spelling of PL-04, PL-28; Update Code Source and List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PL)."
         },
         {
             "Code/Subdivision Change": "Category change: province -> voivodship Code changes: DS -> 02 KP -> 04 LB -> 08 LD -> 10 LU -> 06 MA -> 12 MZ -> 14 OP -> 16 PD -> 20 PK -> 18 PM -> 22 SK -> 26 SL -> 24 WN -> 28 WP -> 30 ZP -> 32.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of category name from province to voivodship in eng and from r\u00e9gion to vo\u00efvodie in fra; Change of subdivision code from PL-DS to PL-02, PL-KP to PL-04, PL-LB to PL-08, PL-LD to PL-10, PL-LU to PL-06, PL-MA to PL-12, PL-MZ to PL-14, PL-OP to PL-16, PL-PD to PL-20, PL-PK to PL-18, PL-PM to PL-22, PL-SK to PL-26, PL-SL to PL-24, PL-WN to PL-28, PL-WP to PL-30 and PL-ZP to PL-32; Update List Source; Update Code Source.",
+            "Description of Change": "Change of category name from province to voivodship in eng and from r\u00e9gion to vo\u00efvodie in fra; Change of subdivision code from PL-DS to PL-02, PL-KP to PL-04, PL-LB to PL-08, PL-LD to PL-10, PL-LU to PL-06, PL-MA to PL-12, PL-MZ to PL-14, PL-OP to PL-16, PL-PD to PL-20, PL-PK to PL-18, PL-PM to PL-22, PL-SK to PL-26, PL-SL to PL-24, PL-WN to PL-28, PL-WP to PL-30 and PL-ZP to PL-32; Update List Source; Update Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 49 provinces (see below) -> 16 provinces.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Introduction of a completely new subdivision layout.",
+            "Description of Change": "Introduction of a completely new subdivision layout.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "PM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-PM)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-PM)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PM)."
         }
     ],
     "PN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PN)."
         }
     ],
     "PR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-PR)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-PR)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PR)."
         }
     ],
     "PS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of romanization system for ara; change of spelling of category name in ara; change of spelling of PS-QQA, PS-JRH, PS-RBH; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of romanization system for ara; change of spelling of category name in ara; change of spelling of PS-QQA, PS-JRH, PS-RBH; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "UN notification of full name[1][2] (#cite_note-2).",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "UN notification of full name[1][2] (#cite_note-1).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PS)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 16 governorates.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative division taken into account.",
+            "Description of Change": "Administrative division taken into account.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of local name.",
             "Date Issued": "2008-04-08",
-            "Description of Change in Newsletter": "Correction of local name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PS)."
         },
         {
             "Code/Subdivision Change": "New entry (no codes).",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Insertion of a new entry between PUERTO RICO and PORTUGAL; in accordance with ISO 3166-1 Newsletter V-2.",
+            "Description of Change": "Insertion of a new entry between PUERTO RICO and PORTUGAL; in accordance with ISO 3166-1 Newsletter V-2.",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         }
     ],
     "PT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PT)."
         }
     ],
     "PW": [
         {
             "Code/Subdivision Change": "Name changed: PW-050 Hatobohei -> Hatohobei.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of PW-050 in eng, pau; update list source.",
+            "Description of Change": "Change of spelling of PW-050 in eng, pau; update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:PW)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 16 states.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "PY": {},
     "QA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of municipality QA-SH.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Addition of municipality QA-SH.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:QA)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: QA-ZA Az\u0327 Za\u0327`\u0101yin Subdivisions deleted: QA-GH Al Ghuwayr\u012byah QA-JU Al Jumayl\u012byah QA-JB Jar\u012by\u0101n al B\u0101\u0163nah.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Update resulting from the addition of names in administrative languages, and update of the administrative structure and of the list source.",
+            "Description of Change": "Update resulting from the addition of names in administrative languages, and update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "RE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-974)).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-974)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Delete the French scattered Indian Ocean Islands.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Delete the French scattered Indian Ocean Islands.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RE)."
         }
     ],
     "RO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RO)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: RO-IF Ilfov.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one department. Subdivision categories in header re-sorted.",
+            "Description of Change": "Addition of one department. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of spelling mistake of subdivision category in header.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Correction of spelling mistake of subdivision category in header.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "RS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of an asterisk to RS-KM, RS-VO; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of an asterisk to RS-KM, RS-VO; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, administrative update.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, administrative update.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 1 city, 2 autonomous republics, 29 districts.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of a new country (in accordance with ISO 3166-1 Newsletter V-12).",
+            "Description of Change": "Addition of a new country (in accordance with ISO 3166-1 Newsletter V-12).",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "RU": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of language from 'urd' to 'rus' for RU-PSK, RU-ROS, RU-PRI.",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Correction of language from 'urd' to 'rus' for RU-PSK, RU-ROS, RU-PRI.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RU)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RU)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: RU-ZAB Zabaykal'skiy kray Subdivisions deleted: RU-CHI Chitinskaya oblast' RU-AGB Aginskiy Buryatskiy avtonomnyy okrug RU-UOB Ust'-Ordynskiy Buryatskiy avtonomnyy okrug.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and of the list source.",
+            "Description of Change": "Update of the administrative structure and of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: RU-KAM Kamchatskiy kray Subdivisions deleted: RU-KAM Kamchatskaya oblast' RU-EVE Evenkiyskiy avtonomnyy okrug RU-KOR Koryakskiy avtonomnyy okrug RU-TAY Taymyrskiy avtonomnyy okrug.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Update and use of long forms of country names as given in Draft NL I-8 538, 22-02-2007 and formation of Permskiy kray after amalgamation.",
+            "Description of Change": "Update and use of long forms of country names as given in Draft NL I-8 538, 22-02-2007 and formation of Permskiy kray after amalgamation.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: RU-PER Permskiy kray Subdivisions deleted: RU-PER Permskaya oblast' RU-KOP Komi-Permyatskiy avtonomnyy okrug.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add local language name to the title Khanty-Mansiyskiy avtonomnyy okrug. Update of list source.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Add local language name to the title Khanty-Mansiyskiy avtonomnyy okrug. Update of list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Introduction of alternative name forms for 2 republics. Correction of a spelling mistake in the name of 1 autonomous district.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Introduction of alternative name forms for 2 republics. Correction of a spelling mistake in the name of 1 autonomous district.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "RW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from town council to city; change of spelling of category name in kin.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision category from town council to city; change of spelling of category name in kin.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of RW-01, RW-02, RW-03, RW-04, RW-05; addition of category name in kin; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of RW-01, RW-02, RW-03, RW-04, RW-05; addition of category name in kin; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:RW)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 12 prefectures (see below) -> 1 town council, 4 provinces.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "SA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from province to region.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of subdivision category from province to region.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change subdivision names of SA-02, SA-03 and SA-09; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Change subdivision names of SA-02, SA-03 and SA-09; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alphabetical re-ordering.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "SB": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the French short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SB)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SB)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: SB-CH Choiseul SB-RB Rennell and Bellona.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "SC": [
         {
             "Code/Subdivision Change": "Subdivisions added: SC-26 Ile Perseverance I SC-27 Ile Perseverance II.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of district SC-26, SC-27; Update List Source.",
+            "Description of Change": "Addition of district SC-26, SC-27; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct the local language code for the local short name.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Correct the local language code for the local short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SC)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: SC-24 Les Mamelles SC-25 Roche Caiman.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and languages and update of the list source.",
+            "Description of Change": "Update of the administrative structure and languages and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 23 districts.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "SD": [
         {
             "Code/Subdivision Change": "Spelling changes: SD-DC Wasa\u0163 D\u0101rf\u016br Z\u0101linjay -> Wasa\u0163 D\u0101rf\u016br SD-KN Shiam\u0101l Kurduf\u0101n -> Sham\u0101l Kurduf\u0101n.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Typographical correction of subdivision name of SD-KN, SD-DC; Addition of local variation of SD-DC.",
+            "Description of Change": "Typographical correction of subdivision name of SD-KN, SD-DC; Addition of local variation of SD-DC.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SD)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SD)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: SD-GK Gharb Kurduf\u0101n (ar), West Kordofan (en) Spelling changes: SD-DC Zalingei -> Wasa\u0163 D\u0101rf\u016br Z\u0101linjay SD-DN ? -> Sham\u0101l D\u0101rf\u016br SD-KN Sham\u0101l Kurduf\u0101n -> Shiam\u0101l Kurduf\u0101n SD-NO ? -> Ash Sham\u0101l\u012byah SD-NR An N\u012bl -> Nahr an N\u012bl.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Additions of state SD-GK; change spelling of SD-NR, SD-NO, SD-DN, SD-KN, SD-DC; update List Source.",
+            "Description of Change": "Additions of state SD-GK; change spelling of SD-NR, SD-NO, SD-DN, SD-KN, SD-DC; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SD)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 25 states (see below) -> 17 states Subdivisions deleted: 10 states ()SD-14 \u2013 SD-23) seceded to create South Sudan (SS) Subdivisions added: SD-DE Sharq D\u0101rf\u016br SD-DC Zalingei.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative adjustment and update.",
+            "Description of Change": "Administrative adjustment and update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct numeric code after split.",
             "Date Issued": "2011-08-09",
-            "Description of Change in Newsletter": "Correct numeric code after split.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions deleted: SD-10 Gharb Kurduf\u0101n.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Modification of administrative structure.",
+            "Description of Change": "Modification of administrative structure.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         }
     ],
     "SE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Name precision of the administrative division, Alphabetical re-ordering and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Name precision of the administrative division, Alphabetical re-ordering and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         }
     ],
     "SG": [
         {
             "Code/Subdivision Change": "Subdivisions added: 5 districts.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative divisions and their codes.",
+            "Description of Change": "Addition of administrative divisions and their codes.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         }
     ],
     "SH": [
         {
             "Code/Subdivision Change": "Subdivisions added: 3 geographical entities.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative subdivisions addition.",
+            "Description of Change": "Administrative subdivisions addition.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Consistency between ISO 3166-1 and ISO 3166-2 for change of name (in accordance with ISO 3166-1 Newsletter VI-7).",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Consistency between ISO 3166-1 and ISO 3166-2 for change of name (in accordance with ISO 3166-1 Newsletter VI-7).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of name; Addition of islands given in Clauses 9 and 10.",
             "Date Issued": "2010-02-22",
-            "Description of Change in Newsletter": "Change of name; Addition of islands given in Clauses 9 and 10.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SH)."
         }
     ],
     "SI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of SI-044, SI-197; Addition of category urban municipality; Change of category name from municipality to urban municipality for SI-011, SI-050, SI-052, SI-054, SI-061, SI-070, SI-080, SI-084, SI-085, SI-096, SI-112, SI-133; Update List Source.",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Change of spelling of SI-044, SI-197; Addition of category urban municipality; Change of category name from municipality to urban municipality for SI-011, SI-050, SI-052, SI-054, SI-061, SI-070, SI-080, SI-084, SI-085, SI-096, SI-112, SI-133; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of remark part 2 (the Italian and Hungarian languages are locally official in those municipalities where Italian or Hungarian national communities reside. For these municipalities the Hungarian or Italian subdivision name is provided under \u2018local variation\u2019).",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Addition of remark part 2 (the Italian and Hungarian languages are locally official in those municipalities where Italian or Hungarian national communities reside. For these municipalities the Hungarian or Italian subdivision name is provided under \u2018local variation\u2019).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of spelling for SI-065, SI-116, SI-169, SI-182, SI-204, SI-210; Deletion of asterisk from SI-212; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of spelling for SI-065, SI-116, SI-169, SI-182, SI-204, SI-210; Deletion of asterisk from SI-212; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from commune to municipality; addition of municipality SI-213.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision category from commune to municipality; addition of municipality SI-213.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 commune SI-212; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 1 commune SI-212; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update of the administrative structure and languages and update of the list source.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and languages and update of the list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SI)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of official language names for some municipalities.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Addition of official language names for some municipalities.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 12 statistical regions (see below) -> 193 municipalities.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Replacement of statistical regions with 193 municipalities.",
+            "Description of Change": "Replacement of statistical regions with 193 municipalities.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "SJ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of Norway (NO-21, NO-22)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of Norway (NO-21, NO-22)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SJ)."
         }
     ],
     "SK": {},
     "SL": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of an asterisk to SL-NW; Update Code Source.",
             "Date Issued": "2019-11-22",
-            "Description of Change in Newsletter": "Addition of an asterisk to SL-NW; Update Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SL)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of province SL-NW; Update List Source.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of province SL-NW; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SL)."
         }
     ],
     "SM": [
         {
             "Code/Subdivision Change": "Subdivisions renamed: SM-07 San Marino -> Citt\u00e0 di San Marino.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of SM-07; Addition of local variation for SM-07; Update List Source.",
+            "Description of Change": "Change of spelling of SM-07; Addition of local variation for SM-07; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SM)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 9 municipalities.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "SN": [
         {
             "Code/Subdivision Change": "Subdivisions added: SN-KA Kaffrine SN-KE K\u00e9dougou SN-SE S\u00e9dhiou.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and languages and update of the list source.",
+            "Description of Change": "Update of the administrative structure and languages and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: SN-MT Matam.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Addition of one new region. List source updated.",
+            "Description of Change": "Addition of one new region. List source updated.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "SO": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add \"the\" before the English full name.",
             "Date Issued": "2014-03-03",
-            "Description of Change in Newsletter": "Add \"the\" before the English full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SO)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "UN notification of full name.",
             "Date Issued": "2013-07-11",
-            "Description of Change in Newsletter": "UN notification of full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SO)."
         }
     ],
     "SR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SR)."
         }
     ],
     "SS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Typographical correction of SS-BW (deletion of the extra space between el and Ghazal).",
             "Date Issued": "2021-11-25",
-            "Description of Change in Newsletter": "Typographical correction of SS-BW (deletion of the extra space between el and Ghazal).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of the space after the short English name lower case.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Deletion of the space after the short English name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SS)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 10 states.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative subdivisions addition.",
+            "Description of Change": "Administrative subdivisions addition.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Assign code elements.",
             "Date Issued": "2011-08-09",
-            "Description of Change in Newsletter": "Assign code elements.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SS)."
         }
     ],
     "ST": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of province ST-S; Change of subdivision category from province to autonomous region for ST-P; Addition of district ST-01, ST-02, ST-03, ST-04, ST-05, ST-06; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Deletion of province ST-S; Change of subdivision category from province to autonomous region for ST-P; Addition of district ST-01, ST-02, ST-03, ST-04, ST-05, ST-06; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ST)."
         }
     ],
     "SV": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SV)."
         }
     ],
     "SX": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-SX)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of Netherlands (NL-SX)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Martin, partie sud de\u201d in the French name field for Territory.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the OBP entry error as follows: deletion of \u201cSaint-Martin, partie sud de\u201d in the French name field for Territory.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling error in the French remarks.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Correct spelling error in the French remarks.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SX)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Addition of code to align ISO 3166-1 and ISO 3166-2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add new entry.",
             "Date Issued": "2010-12-15",
-            "Description of Change in Newsletter": "Add new entry.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SX)."
         }
     ],
     "SY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the English short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the English short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SY)."
         }
     ],
     "SZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category from district to region; Update List Source.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of subdivision category from district to region; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the short name, full name and local short name in eng.",
             "Date Issued": "2018-07-16",
-            "Description of Change in Newsletter": "Change of the short name, full name and local short name in eng.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:SZ)."
         }
     ],
     "TC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the OBP entry error as follows: addition of \u201cCaicos Islands\u201d to the English name field for Territory and \u201c\u00celes Caicos\u201d to the French name fields for Territory.",
             "Date Issued": "2015-02-26",
-            "Description of Change in Newsletter": "Correction of the OBP entry error as follows: addition of \u201cCaicos Islands\u201d to the English name field for Territory and \u201c\u00celes Caicos\u201d to the French name fields for Territory.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TC)."
         }
     ],
     "TD": [
         {
             "Code/Subdivision Change": "Spelling changes: TD-BA Al Ba\u0163\u1e29ah (ar) -> Al Ba\u0163\u1e29\u0101\u2019 TD-LO L\u016bq\u016bn al Gharb\u012b (ar) -> L\u016bgh\u016bn al Gharb\u012b TD-LR L\u016bq\u016bn ash Sharq\u012b (ar) -> L\u016bgh\u016bn ash Sharq\u012b TD-TA T\u0101njil\u012b (ar) -> T\u0101nj\u012bl\u012b TD-WF W\u0101d\u012b F\u012br\u0101 (ar) -> W\u0101d\u012b F\u012br\u0101\u2019.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision category region to province; Modification of spelling for TD-BA, TD-LO, TD-LR, TD-TA, TD-WF in ara; Addition of local variation for TD-BG in fra; Addition of subdivision name of TD-EE, TD-OE in ara; Update List Source.",
+            "Description of Change": "Change of subdivision category region to province; Modification of spelling for TD-BA, TD-LO, TD-LR, TD-TA, TD-WF in ara; Addition of local variation for TD-BG in fra; Addition of subdivision name of TD-EE, TD-OE in ara; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TD-EE Ennedi-Est (fr) TD-EO Ennedi-Ouest (fr) Subdivision deleted: TD-EN Inn\u012bd\u012b (ar), Ennedi (fr) Spelling change: TD-BA Al Ba\u1e6d\u1e29ah (ar) -> Al Ba\u0163\u1e29ah.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add two regions TD-EE and TD-EO; correct spelling of TD-BA; delete TD-EN; update List Source.",
+            "Description of Change": "Add two regions TD-EE and TD-EO; correct spelling of TD-BA; delete TD-EN; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TD)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TD-BG Bahr el Gazel TD-BO Borkou TD-EN Ennedi TD-SI Sila TD-TI Tibesti Subdivisions deleted: TD-BET Borkou-Ennedi-Tibesti.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and languages and update of the list source.",
+            "Description of Change": "Update of the administrative structure and languages and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 14 prefectures (see below) -> 18 regions.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Modification of the administrative structure.",
+            "Description of Change": "Modification of the administrative structure.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "TF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-TF)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as subdivision of France (FR-TF)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add the French scattered Indian Ocean Islands.",
             "Date Issued": "2007-09-21",
-            "Description of Change in Newsletter": "Add the French scattered Indian Ocean Islands.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TF)."
         }
     ],
     "TG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of TG-S; update List Source.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of spelling of TG-S; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of TG-C; update list source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of TG-C; update list source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TG)."
         }
     ],
     "TH": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TH)."
         }
     ],
     "TJ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
             "Code/Subdivision Change": "Spelling change: TJ-RA Nohiyahoi Tobei Jumhur\u00ed -> nohiyahoi tobei jumhur\u00ed.",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Change of subdivision name of TJ-RA; change of spelling of category name in eng, tgk; update List Source; modification of the English remark part 2.",
+            "Description of Change": "Change of subdivision name of TJ-RA; change of spelling of category name in eng, tgk; update List Source; modification of the English remark part 2.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: TJ-RA Nohiyahoi Tobei Jumhur\u00ed.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Modification of the remark part 2; addition of category name Districts Under Republic Administration in eng, fra, tgk; addition of Districts Under Republic Administration TJ-RA; update list source.",
+            "Description of Change": "Modification of the remark part 2; addition of category name Districts Under Republic Administration in eng, fra, tgk; addition of Districts Under Republic Administration TJ-RA; update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Removed the reference to Dushanbe in remark part 2; correct spelling of DU.",
             "Date Issued": "2015-02-12",
-            "Description of Change in Newsletter": "Removed the reference to Dushanbe in remark part 2; correct spelling of DU.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: TJ-DU.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 1 capital territory TJ-DU.",
+            "Description of Change": "Add 1 capital territory TJ-DU.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TJ)."
         },
         {
             "Code/Subdivision Change": "Subdivision deleted: TJ-KR Karategin Codes: TJ-LN Leninabad -> TJ-SU Sughd.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Change of name of one region. Deletion of one region. Introduction of one Tajik name form. Subdivision categories in header re-sorted.",
+            "Description of Change": "Change of name of one region. Deletion of one region. Introduction of one Tajik name form. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "TK": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TK)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the alpha 3 administrative language code tkl.",
             "Date Issued": "2016-07-25",
-            "Description of Change in Newsletter": "Addition of the alpha 3 administrative language code tkl.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TK)."
         }
     ],
     "TL": [
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Change of subdivision category name from district to municipality; Addition of category name in tet; Change of category name from district to special administrative region for TL-OE; Change of spelling in por of TL-OE; Change of spelling of TL-LA; Addition of local variation of TL-OE; Update List Source.",
+            "Description of Change": "Change of subdivision category name from district to municipality; Addition of category name in tet; Change of category name from district to special administrative region for TL-OE; Change of spelling in por of TL-OE; Change of spelling of TL-LA; Addition of local variation of TL-OE; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TL)."
         },
         {
             "Code/Subdivision Change": "Spelling change TL-DI Dili -> D\u00edli.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Update of the language adjustment and source list update.",
+            "Description of Change": "Update of the language adjustment and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Change of country name in accordance with ISO 3166-1 Newsletter V-6 (East Timor renamed Timor-Leste in English and French). Spelling correction in TL-LI.",
+            "Description of Change": "Change of country name in accordance with ISO 3166-1 Newsletter V-6 (East Timor renamed Timor-Leste in English and French). Spelling correction in TL-LI.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 13 districts.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Change of the ISO 3166-1 alpha-2 code element to TL. Insertion of 13 districts. In accordance with ISO 3166-1 Newsletter V-5.",
+            "Description of Change": "Change of the ISO 3166-1 alpha-2 code element to TL. Insertion of 13 districts. In accordance with ISO 3166-1 Newsletter V-5.",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         }
     ],
     "TM": [
         {
             "Code/Subdivision Change": "Subdivisions added: TM-S A\u015fgabat.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and update of the list source.",
+            "Description of Change": "Update of the administrative structure and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "One spelling correction. Correction of header information.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "One spelling correction. Correction of header information.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "TN": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the local short name; change of spelling of TN-12, TN-73, TN-82; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Correction of the local short name; change of spelling of TN-12, TN-73, TN-82; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Toponym evolution, alphabetical re-ordering and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Toponym evolution, alphabetical re-ordering and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Adjustment of name form in TN-14. List source updated.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Adjustment of name form in TN-14. List source updated.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TN-14 Manouba.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Addition of one new governorate. List source updated. Code source updated.",
+            "Description of Change": "Addition of one new governorate. List source updated. Code source updated.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "TO": [
         {
             "Code/Subdivision Change": "Subdivisions added: 5 divisions.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "TR": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of the short and full name.",
             "Date Issued": "2022-07-11",
-            "Description of Change in Newsletter": "Change of the short and full name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TR)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Toponym evolution and source list update.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Toponym evolution and source list update.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TR-81 D\u00fczce.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Addition of one province. Update of list source information.",
+            "Description of Change": "Addition of one province. Update of list source information.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TR-80 Osmaniye.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Addition of 1 new province. Correction of 2 spelling errors.",
+            "Description of Change": "Addition of 1 new province. Correction of 2 spelling errors.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "TT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of category name from municipality to borough for TT-ARI, TT-CHA, TT-PTF; Change of subdivision category name from municipality to city for TT-POS, TT-SFO; Update List Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of category name from municipality to borough for TT-ARI, TT-CHA, TT-PTF; Change of subdivision category name from municipality to city for TT-POS, TT-SFO; Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Deletion of regions TT-ETO, TT-RCM, TT-WTO; addition of region TT-MRC; addition of one ward TT-TOB; update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Deletion of regions TT-ETO, TT-RCM, TT-WTO; addition of region TT-MRC; addition of one ward TT-TOB; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TT)."
         }
     ],
     "TV": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of TV-NMG; update List Source.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of TV-NMG; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TV)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of administrative language Tuvaluan (-, tvl).",
             "Date Issued": "2009-03-03",
-            "Description of Change in Newsletter": "Addition of administrative language Tuvaluan (-, tvl).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TV)."
         },
         {
             "Code/Subdivision Change": "Codes: Nui: TV-NIU -> TV-NUI.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 1 town council, 7 island councils.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "TW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TW)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TW)."
         },
         {
             "Code/Subdivision Change": "(each) district -> county(each) municipality -> city.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of subdivision category from municipality to city and district to county; update List Source.",
+            "Description of Change": "Change of subdivision category from municipality to city and district to county; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TW)."
         },
         {
             "Code/Subdivision Change": "Subdivision added:Kinmen (district): TW-KINLienchiang (district): TW-LIENew Taipei (special municipality): TW-NWTSubdivision deleted:Kaohsiung (district): TW-KHQTainan (district): TW-TNQTaipei (district): TW-TPQTaichung (district): TW-TXQSubdivision category changed:Taoyuan (TW-TAO): district -> special municipalityTainan (TW-TNN): municipality -> special municipalityTaichung (TW-TXG): municipality -> special municipality.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of category name for special municipality in zho; change of spelling of TW-ILA; deletion of districts TW-KHQ, TW-TNQ, TW-TPQ, TW-TXQ; addition of districts TW-KIN, TW-LIE and special municipality TW-NWT; change of subdivision category from municipalities to special municipalities for TW-TXG, TW-TNN; change of subdivision category from district to special municipality for TW-TAO; update List Source.",
+            "Description of Change": "Addition of category name for special municipality in zho; change of spelling of TW-ILA; deletion of districts TW-KHQ, TW-TNQ, TW-TPQ, TW-TXQ; addition of districts TW-KIN, TW-LIE and special municipality TW-NWT; change of subdivision category from municipalities to special municipalities for TW-TXG, TW-TNN; change of subdivision category from district to special municipality for TW-TAO; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TW)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use)Chiayi (district): TW-CYI -> TW-CYQHsinchu (district): TW-HSZ -> TW-HSQKaohsiung (district): TW-KHH -> TW-KHQTaichung (district): TW-TXG -> TW-TXQTainan (district): TW-TNN -> TW-TNQTaipei (district): TW-TPE -> TW-TPQ.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Error correction: Duplicate use of six code elements corrected. Subdivision categories in header re-sorted.",
+            "Description of Change": "Error correction: Duplicate use of six code elements corrected. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "TZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the English and French short name lower case.",
             "Date Issued": "2019-02-15",
-            "Description of Change in Newsletter": "Modification of the English and French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TZ)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of the English and French short name lower case.",
             "Date Issued": "2019-02-14",
-            "Description of Change in Newsletter": "Modification of the English and French short name lower case.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TZ)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: TZ-31 Songwe (sw), Songwe (en).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of region TZ-31; Update List Source.",
+            "Description of Change": "Addition of region TZ-31; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: TZ-27 Geita (sw) TZ-28 Katavi (sw) TZ-29 Njombe (sw) TZ-30 Simiyu (sw).",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 4 regions TZ-27 to TZ-30; update List Source.",
+            "Description of Change": "Add 4 regions TZ-27 to TZ-30; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:TZ)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: TZ-26 Manyara (sw).",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Addition of one new region. One spelling correction. List source updated. Code source updated.",
+            "Description of Change": "Addition of one new region. One spelling correction. List source updated. Code source updated.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         }
     ],
     "UA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the romanization system label.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Correction of the romanization system label.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update subdivision name of UA-43; update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update subdivision name of UA-43; update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UA)."
         }
     ],
     "UG": [
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of district UG-237, UG-335, UG-336, UG-337, UG-433, UG-434, UG-435; Change of spelling of UG-220; Removal of an asterisk from UG-125, UG-126, UG-233, UG-234, UG-235, UG-236, UG-331, UG-332, UG-333, UG-334, UG-427, UG-428, UG-429, UG-430, UG-431, UG-432.",
+            "Description of Change": "Addition of district UG-237, UG-335, UG-336, UG-337, UG-433, UG-434, UG-435; Change of spelling of UG-220; Removal of an asterisk from UG-125, UG-126, UG-233, UG-234, UG-235, UG-236, UG-331, UG-332, UG-333, UG-334, UG-427, UG-428, UG-429, UG-430, UG-431, UG-432.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Addition of districts UG-126, UG-235, UG-236, UG-333, UG-334, UG-432; Update List Source.",
+            "Description of Change": "Addition of districts UG-126, UG-235, UG-236, UG-333, UG-334, UG-432; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2017-11-23",
-            "Description of Change in Newsletter": "Addition of districts UG-125, UG-233, UG-234, UG-331, UG-332, UG-427, UG-428, UG-429, UG-430, UG-431; update List Source.",
+            "Description of Change": "Addition of districts UG-125, UG-233, UG-234, UG-331, UG-332, UG-427, UG-428, UG-429, UG-430, UG-431; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Update Code Source; update List Source; change of parent subdivision of UG-325; deletion of asterisks from districts; change of subdivision code from UG-114 to UG-115, UG-115 to UG-116, UG-116 to UG-114, UG-218 to UG-220, UG-219 to UG-221, UG-220 to UG-222, UG-221 to UG-223, UG-222 to UG-224, UG-223 to UG-218, UG-224 to UG-219, UG-314 to UG-315, UG-315 to UG-318, UG-316 to UG-319, UG-317 to UG-314, UG-318 to UG-317, UG-319 to UG-316, UG-325 to UG-420, UG-326 to UG-325, UG-327 to UG-326, UG-328 to UG-327, UG-329 to UG-328, UG-330 to UG-329, UG-331 to UG-330, UG-416 to UG-417, UG-417 to UG-418, UG-418 to UG-419, UG-419 to UG-416, UG-420 to UG-421, UG-421 to UG-422, UG-422 to UG-423, UG-423 to UG-424, UG-424 to UG-425, UG-425 to UG-426.",
+            "Description of Change": "Update Code Source; update List Source; change of parent subdivision of UG-325; deletion of asterisks from districts; change of subdivision code from UG-114 to UG-115, UG-115 to UG-116, UG-116 to UG-114, UG-218 to UG-220, UG-219 to UG-221, UG-220 to UG-222, UG-221 to UG-223, UG-222 to UG-224, UG-223 to UG-218, UG-224 to UG-219, UG-314 to UG-315, UG-315 to UG-318, UG-316 to UG-319, UG-317 to UG-314, UG-318 to UG-317, UG-319 to UG-316, UG-325 to UG-420, UG-326 to UG-325, UG-327 to UG-326, UG-328 to UG-327, UG-329 to UG-328, UG-330 to UG-329, UG-331 to UG-330, UG-416 to UG-417, UG-417 to UG-418, UG-418 to UG-419, UG-419 to UG-416, UG-420 to UG-421, UG-421 to UG-422, UG-422 to UG-423, UG-423 to UG-424, UG-424 to UG-425, UG-425 to UG-426.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
             "Code/Subdivision Change": "(TBD).",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 32 districts UG-117 to UG- 124, UG-225 to UG-232, UG-322 to UG-331 and UG-420 to UG-425; change subdivision category from district to city for UG-102.",
+            "Description of Change": "Add 32 districts UG-117 to UG- 124, UG-225 to UG-232, UG-322 to UG-331 and UG-420 to UG-425; change subdivision category from district to city for UG-102.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of the country code prefix as the first code element, administrative update, alphabetical re-ordering.",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update, alphabetical re-ordering.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UG)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: UG-223 Bududa UG-224 Bukedea UG-116 Lyantonde.",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Addition of the country code prefix as the first code element, administrative update, alphabetical re-ordering.",
+            "Description of Change": "Addition of the country code prefix as the first code element, administrative update, alphabetical re-ordering.",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: UG-317 Abim UG-314 Amolatar UG-216 Amuria UG-319 Amuru UG-217 Budaka UG-218 Bukwo UG-419 Bulisa UG-219 Butaleja UG-318 Dokolo UG-416 Ibanda UG-417 Isingiro UG-315 Kaabong UG-220 Kaliro UG-418 Kiruhura UG-316 Koboko UG-221 Manafwa UG-320 Maracha UG-114 Mityana UG-115 Nakaseke UG-222 Namutumba UG-321 Oyam.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative divisions and their codes.",
+            "Description of Change": "Addition of administrative divisions and their codes.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: UG-213 Kaberamaido UG-413 Kamwenge UG-414 Kanungu UG-112 Kayunga UG-415 Kyenjojo UG-214 Mayuge UG-311 Nakapiripirit UG-312 Pader UG-215 Sironko UG-113 Wakiso UG-313 Yumbe Codes: format changed (see below).",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Addition of 11 new districts. List source updated. Code source updated.",
+            "Description of Change": "Addition of 11 new districts. List source updated. Code source updated.",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: UG-AJM Adjumani UG-BUG Bugiri UG-BUA Busia UG-KAT Katakwi UG-NAK Nakasongola UG-SEM Sembabule.",
             "Date Issued": "2002-08-20",
-            "Description of Change in Newsletter": "Addition of 6 new districts.",
+            "Description of Change": "Addition of 6 new districts.",
             "Edition/Newsletter": "Newsletter I-3 (https://web.archive.org/web/20081218103236/http://www.iso.org/iso/iso_3166-2_newsletter_i-3_en.pdf)."
         }
     ],
     "UM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UM)."
         }
     ],
     "US": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:US)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:US)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:US)."
         }
     ],
     "UY": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UY)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UY)."
         }
     ],
     "UZ": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of an asterisk to region UZ-XO; Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of an asterisk to region UZ-XO; Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:UZ)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: UZ-TK Toshkent (city).",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Introduction of third subdivision category. Addition of one city. Subdivision categories in header re-sorted.",
+            "Description of Change": "Introduction of third subdivision category. Addition of one city. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: UZ-KH Khorazm -> UZ-XO Xorazm.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling corrections in accordance with the newly adopted Roman alphabet.",
+            "Description of Change": "Spelling corrections in accordance with the newly adopted Roman alphabet.",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         }
     ],
     "VA": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VA)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Short and full names of Vatican City changed from Vatican City State (Holy See) to Holy See (Vatican City State).[2] (#cite_note-2).",
             "Date Issued": "1996-04-03",
-            "Description of Change in Newsletter": "Short and full names of Vatican City changed from Vatican City State (Holy See) to Holy See (Vatican City State).[2] (#cite_note-2).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter IV-1."
         }
     ],
     "VC": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VC)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VC)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: 6 parishes.",
             "Date Issued": "2007-04-17",
-            "Description of Change in Newsletter": "Addition of the administrative subdivisions and of their code elements.",
+            "Description of Change": "Addition of the administrative subdivisions and of their code elements.",
             "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)."
         }
     ],
     "VE": [
         {
+            "Code/Subdivision Change": "Change of short name upper case: replace the parentheses with a coma.",
+            "Date Issued": "2024-02-29",
+            "Description of Change": "",
+            "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
+        },
+        {
             "Code/Subdivision Change": "Subdivisions renamed: VE-X Vargas -> La Guaira.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of subdivision name of VE-X; Update List Source; Correction of the Code Source.",
+            "Description of Change": "Change of subdivision name of VE-X; Update List Source; Correction of the Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of spelling of category name in fra and spa.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of spelling of category name in fra and spa.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the English and French short names upper and lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short form country name in accordance with ISO 3166-1 NL VI-5 (2009-03-03).",
             "Date Issued": "2010-02-19",
-            "Description of Change in Newsletter": "Change of short form country name in accordance with ISO 3166-1 NL VI-5 (2009-03-03).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short form country name in accordance with ISO 3166-1 NL VI-5 (2009-03-03).",
             "Date Issued": "2010-02-03 (corrected 2010-02-19)",
-            "Description of Change in Newsletter": "Change of short form country name in accordance with ISO 3166-1 NL VI-5 (2009-03-03).",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter II-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-1_corrected_2010-02-19.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of short name.",
             "Date Issued": "2009-03-03",
-            "Description of Change in Newsletter": "Change of short name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VE)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Change of subdivision category of two Federal territories to States. List source updated.",
             "Date Issued": "2003-09-05",
-            "Description of Change in Newsletter": "Change of subdivision category of two Federal territories to States. List source updated.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-5 (https://web.archive.org/web/20081218103244/http://www.iso.org/iso/iso_3166-2_newsletter_i-5_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: VE-X Vargas.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of one state. Subdivision categories in header re-sorted.",
+            "Description of Change": "Addition of one state. Subdivision categories in header re-sorted.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "VG": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VG)."
         }
     ],
     "VI": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-VI)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of the United States (US-VI)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VI)."
         }
     ],
     "VN": [
         {
             "Code/Subdivision Change": "Subdivision renamed: VN-CT Can Tho -> C\u1ea7n Th\u01a1 VN-DN Da Nang -> \u0110\u00e0 N\u1eb5ng VN-HN Ha Noi -> H\u00e0 N\u1ed9i VN-HP Hai Phong -> H\u1ea3i Ph\u00f2ng VN-SG Ho Chi Minh -> H\u1ed3 Ch\u00ed Minh.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Change of spelling of VN-CT, VN-DN, VN-HN, VN-HP, VN-SG; Update List Source.",
+            "Description of Change": "Change of spelling of VN-CT, VN-DN, VN-HN, VN-HP, VN-SG; Update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VN)."
         },
         {
             "Code/Subdivision Change": "Subdivision deleted: VN-15 Ha Tay (Merged into VN-HN in 2008).",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Delete subdivision VN-15; change spelling for all the provinces except for VN-28, VN-30, VN-41 and VN-44; update List Source.",
+            "Description of Change": "Delete subdivision VN-15; change spelling for all the provinces except for VN-28, VN-30, VN-41 and VN-44; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VN)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correct spelling error in French long name.",
             "Date Issued": "2013-02-06",
-            "Description of Change in Newsletter": "Correct spelling error in French long name.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:VN)."
         },
         {
             "Code/Subdivision Change": "Subdivision layout: 5 provinces -> 5 municipalities.",
             "Date Issued": "2011-12-13 (corrected 2011-12-15)",
-            "Description of Change in Newsletter": "Administrative adjustment update, typo corrections and source list update.",
+            "Description of Change": "Administrative adjustment update, typo corrections and source list update.",
             "Edition/Newsletter": "Newsletter II-3 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-3_2011-12-13.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: VN-72 \u0110\u1eafk N\u00f4ng VN-71 \u0110i\u1ec7n Bi\u00ean VN-73 H\u1eadu Giang.",
             "Date Issued": "2005-09-13",
-            "Description of Change in Newsletter": "Addition of 3 provinces. Update of list source.",
+            "Description of Change": "Addition of 3 provinces. Update of list source.",
             "Edition/Newsletter": "Newsletter I-7 (https://web.archive.org/web/20081218103217/http://www.iso.org/iso/iso_3166-2_newsletter_i-7_en.pdf)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Spelling correction in VN-65.",
             "Date Issued": "2002-05-21",
-            "Description of Change in Newsletter": "Spelling correction in VN-65.",
+            "Description of Change": "",
             "Edition/Newsletter": "Newsletter I-2 (https://web.archive.org/web/20120131102127/http://www.iso.org/iso/iso_3166-2_newsletter_i-2_en.pdf)."
         },
         {
             "Code/Subdivision Change": "Codes: (to correct duplicate use) Qu\u1ea3ng Ninh: VN-24 -> VN-13.",
             "Date Issued": "2000-06-21",
-            "Description of Change in Newsletter": "Duplicate assignment of VN-24 corrected. Correction of 1 subdivision name. Correction of alphabetic sorting of subdivision names.",
+            "Description of Change": "Duplicate assignment of VN-24 corrected. Correction of 1 subdivision name. Correction of alphabetic sorting of subdivision names.",
             "Edition/Newsletter": "Newsletter I-1 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_i-1_en.pdf)."
         }
     ],
     "VU": {},
     "WF": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (included also as a subdivision of France (FR-WF)).",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2 (included also as a subdivision of France (FR-WF)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:WF)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of administrative precinct WF-AL, WF-SG, WF-UV; update List Source code source and categories.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Addition of administrative precinct WF-AL, WF-SG, WF-UV; update List Source code source and categories.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:WF)."
         }
     ],
     "WS": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:WS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
             "Date Issued": "2014-12-18",
-            "Description of Change in Newsletter": "Alignment of the French short name lower case with UNTERM; update of the remarks in French.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:WS)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:WS)."
         }
     ],
     "YE": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Correction of the Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Correction of the Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YE)."
         },
         {
             "Code/Subdivision Change": "Spelling change: YE-AB Aby\u0101n -> Abyan.",
             "Date Issued": "2016-11-15",
-            "Description of Change in Newsletter": "Change of spelling of YE-AB; update list source.",
+            "Description of Change": "Change of spelling of YE-AB; update list source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YE)."
         },
         {
             "Code/Subdivision Change": "Subdivision added: YE-SU Arkhab\u012bl Suqu\u0163r\u00e1 Name changes: YE-AD YE-AM YE-BA YE-DA YE-MA.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Change of subdivision name of YE-DA, YE-AD, YE-BA, YE-AM, YE-MA; addition of governorate YE-SU; addition of romanisation system of YE-RA; update List Source.",
+            "Description of Change": "Change of subdivision name of YE-DA, YE-AD, YE-BA, YE-AM, YE-MA; addition of governorate YE-SU; addition of romanisation system of YE-RA; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YE)."
         },
         {
             "Code/Subdivision Change": "Spelling change: YE-SA \u015ean\u2018\u0101\u2019 [city] -> Am\u0101nat al \u2018\u0100\u015fimah [city].",
             "Date Issued": "2014-11-17",
-            "Description of Change in Newsletter": "Change spelling for YE-SA; update List Source.",
+            "Description of Change": "Change spelling for YE-SA; update List Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YE)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: YE-RA Raymah.",
             "Date Issued": "2010-06-30",
-            "Description of Change in Newsletter": "Update of the administrative structure and its alphabetical order and update of the list source.",
+            "Description of Change": "Update of the administrative structure and its alphabetical order and update of the list source.",
             "Edition/Newsletter": "Newsletter II-2 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/iso_3166-2_newsletter_ii-2_2010-06-30.pdf)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: YE-SA \u015ean\u2018\u0101' [city].",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-1).",
+            "Description of Change": "Second edition of ISO 3166-2 (this change was not announced in a newsletter)[1] (#cite_note-3).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         },
         {
             "Code/Subdivision Change": "Subdivisions added: YE-DA A\u1e11 \u1e10\u0101li' YE-AM 'Amr\u0101n.",
             "Date Issued": "2002-12-10",
-            "Description of Change in Newsletter": "Addition of two governorates.",
+            "Description of Change": "Addition of two governorates.",
             "Edition/Newsletter": "Newsletter I-4 (https://web.archive.org/web/20081218103210/http://www.iso.org/iso/iso_3166-2_newsletter_i-4_en.pdf)."
         }
     ],
     "YT": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-976)).",
             "Date Issued": "2022-11-29",
-            "Description of Change in Newsletter": "Modification of remark part 2 (no subdivisions relevant for this standard. Included also as a subdivision of France (FR-976)).",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YT)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Modification of remark part 2.",
             "Date Issued": "2018-11-26",
-            "Description of Change in Newsletter": "Modification of remark part 2.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:YT)."
         }
     ],
     "ZA": [
         {
-            "Code/Subdivision Change": "Change of subdivision code: ZA-GT -> ZA-GP ZA-NL -> ZA-KZN.",
+            "Code/Subdivision Change": "Codes: ZA-GT -> ZA-GP ZA-NL -> ZA-KZN.",
             "Date Issued": "2020-03-02",
-            "Description of Change in Newsletter": "Change of subdivision code from ZA-GT to ZA-GP, ZA-NL to ZA-KZN; Update Code Source.",
+            "Description of Change": "Change of subdivision code from ZA-GT to ZA-GP, ZA-NL to ZA-KZN; Update Code Source.",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ZA)."
         },
         {
             "Code/Subdivision Change": "Codes: Gauteng: ZA-GP -> ZA-GT KwaZulu-Natal: ZA-ZN -> ZA-NL.",
             "Date Issued": "2007-12-13",
-            "Description of Change in Newsletter": "Second edition of ISO 3166-2 (this change was not announced in a newsletter).",
+            "Description of Change": "Second edition of ISO 3166-2 (not announced in a newsletter).",
             "Edition/Newsletter": "ISO 3166-2:2007 (http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=39718)."
         },
         {
             "Code/Subdivision Change": "Codes: (not marked with red colour in newsletter) Gauteng: ZA-GT -> ZA-GP KwaZulu-Natal: ZA-NL -> ZA-ZN.",
             "Date Issued": "2007-11-28",
-            "Description of Change in Newsletter": "Addition of administrative divisions and their codes.",
+            "Description of Change": "Addition of administrative divisions and their codes.",
             "Edition/Newsletter": "Newsletter I-9 (https://www.iso.org/files/live/sites/isoorg/files/archive/pdf/en/newsletter_i-9.pdf)."
         },
         {
-            "Code/Subdivision Change": "Codes: ZA-NP Northern Province -> ZA-LP Limpopo.",
+            "Code/Subdivision Change": "Subdivision: ZA-NP Northern Province -> ZA-LP Limpopo.",
             "Date Issued": "2004-03-08",
-            "Description of Change in Newsletter": "Change of name of Northern Province to Limpopo.",
+            "Description of Change": "Change of name of Northern Province to Limpopo.",
             "Edition/Newsletter": "Newsletter I-6 (https://web.archive.org/web/20120112041245/http://www.iso.org/iso/iso_3166-2_newsletter_i-6_en.pdf)."
         }
     ],
     "ZM": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Addition of an asterisk to ZM-01 to ZM-10; Correction du Code Source.",
             "Date Issued": "2020-11-24",
-            "Description of Change in Newsletter": "Addition of an asterisk to ZM-01 to ZM-10; Correction du Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ZM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source and Code Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source and Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ZM)."
         },
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Add 1 province ZM-10; update List Source and Code Source.",
             "Date Issued": "2014-11-03",
-            "Description of Change in Newsletter": "Add 1 province ZM-10; update List Source and Code Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ZM)."
         }
     ],
     "ZW": [
         {
-            "Code/Subdivision Change": "",
+            "Code/Subdivision Change": "Update List Source.",
             "Date Issued": "2015-11-27",
-            "Description of Change in Newsletter": "Update List Source.",
+            "Description of Change": "",
             "Edition/Newsletter": "Online Browsing Platform (OBP) - (https://www.iso.org/obp/ui/#iso:code:3166:ZW)."
         }
     ]
 }
```

### Comparing `iso3166-updates-1.6.0/iso3166_updates/iso3166_updates.py` & `iso3166_updates-1.7.0/iso3166_updates/iso3166_updates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,282 @@
 import os
 import sys
 import json
 import re
 from datetime import datetime
+from dateutil import relativedelta
 import iso3166
+import platform
 
 class ISO3166_Updates():
     """
     This class is used to access all the ISO-3166 updates/changes data from its respective json
     created from the data sources used in the get_all_iso3166_updates.py script. All of the 
     keys and objects in the JSON are accessible via dot notation using the Map class. Each
     country has the attributes: Date Issued, Edition/Newsletter, Code/Subdivision Change and
-    Description of Change in Newsletter. 
+    Description of Change. 
     
-    Date Issued is the date at which the change was published by the ISO, the Edition/Newsletter
-    column is the name and or edition of newsletter that the ISO 3166 change/update was 
-    communicated in, Code/Subdivision Change column is the overall summary of change/update made
-    and "Description of Change in Newsletter" is more in-depth info about the change/update that 
-    was made.
+    "Date Issued" is the date at which the change was published by the ISO, the "Edition/Newsletter"
+    column is the name and or edition of newsletter that the ISO 3166 change/update was communicated 
+    in, "Code/Subdivision Change" column is the overall summary of change/update made and 
+    "Description of Change" is a more in-depth info about the change/update that was made.
 
-    Currently there are 250 country's listed in the updates json with updates dating from 2000 up
-    until the current year.
+    Currently there are 249 country's listed in the updates json with updates dating from 2000 up
+    to the present year, with ~500 individual published updates.
 
     Parameters
     ==========
-    None
+    :country_code: str (default="")
+        ISO 3166-1 alpha-2, alpha-3 or numeric country code to get subdivision data for. A list
+        of country codes can also be input. If the alpha-3 or numeric codes are input, they are
+        converted into their alpha-2 counterparts.
 
     Methods
     =======
     year(input_year):
         get all listed updates/changes in the updates json object for an input year, set of years,
         year range or greater than/less than year.
-    __getitem__(alpha2_code):
+    months(input_month):
+        get all listed updates/changes in the updates json that have been published within the past
+        number of months or within a specified month range.    
+    __getitem__(alpha_code):
         get all listed updates/changes in the updates json object for an input country/countries,
-        using the 2 letter alpha-2 ISO 3166-1 code by making the class subscriptable. For redundancy, 
-        a country's 3 letter alpha-3 ISO 3166-1 code can also be accepted.
+        by making the instance object subscriptable and updates accessible via their alpha-2, 
+        alpha-3 or numeric country codes.
+    convert_to_alpha2(alpha_code):
+        convert the inputted ISO 3166-1 alpha-3 or numeric country codes into their 2 letter 
+        alpha-2 counterpart.
 
     Usage
     =====
-    import iso3166_updates as iso
+    from iso3166_updates import *
 
-    #get ALL listed changes/updates for ALL countries 
-    iso.updates.all
+    #create instance of class
+    iso = ISO3166_Updates()
+
+    #get all listed changes/updates for ALL countries 
+    iso.all
 
     #get ALL listed country updates/changes data for Ireland, Colombia, Denmark and Finland
-    iso.updates['IE']
-    iso.updates['CO']
-    iso.updates['DK']
-    iso.updates['FI']
+    iso['IE']
+    iso['CO']
+    iso['DK']
+    iso['FI']
+
+    #get all listed country updates/changes data for France and Germany
+    iso["FR,DE"]
+
+    #get all listed country updates/changes data for Fiji, Guyana, Haiti and Hungary
+    iso["FJ,GY,HI,HU"]
 
-    #get ALL listed country updates/changes data for France and Germany
-    iso.updates["FR,DE"]
+    #get all listed country updates/changes data for 2016
+    iso.year("2016")
 
-    #get ALL listed country updates/changes data for Fiji, Guyana, Haiti and Hungary
-    iso.updates["FJ,GY,HI,HU"]
+    #get all listed country updates/changes data for 2002, 2009, 2023
+    iso.year("2002,2009,2023")
 
-    #get ALL listed country updates/changes data for year 2016
-    iso.updates.year("2016")
+    #get all listed country updates/changes data for years 2005 - 2010
+    iso.year("2005-2010")
 
-    #get ALL listed country updates/changes data for years 2005 - 2010
-    iso.updates.year("2005-2010")
+    #get all listed country updates/changes data with year <2009
+    iso.year("<2009")
 
-    #get ALL listed country updates/changes data with year <2009
-    iso.updates.year("<2009")
+    #get all listed country updates/changes data with years >2020, for France
+    iso.year(">2020").FR
 
-    #get ALL listed country updates/changes data with years >2020
-    iso.updates.year(">2020")
+    #get all listed country updates/changes data published over the previous 6 months
+    iso.months("6")
+
+    #get all listed country updates/changes data published over the previous 24-36 months
+    iso.months("24-36")
     """
-    def __init__(self):
+    def __init__(self, country_code: str="") -> None:
         
         self.iso3166_updates_json_filename = "iso3166-updates.json"
+        self.country_code = country_code
         
         #get module path to access the json object
         self.iso3166_updates_module_path = os.path.dirname(os.path.abspath(sys.modules[self.__module__].__file__))
         
-        #raise error if iso3166-upates json doesnt exist in folder
+        #raise error if iso3166-updates json doesn't exist in folder
         if not (os.path.isfile(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename))):
-            raise OSError("Issue finding iso3166-updates.json in dir: {}".format(
-                os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)))
+            raise OSError(f"Issue finding iso3166-updates.json in dir: {os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)}.")
 
-        #open iso3166-updates json file and load it into class variable
-        with open(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)) as iso3166_updates_json:
-            self.all = json.load(iso3166_updates_json)
+        #importing all updates data from JSON, open iso3166-updates json file and load it into class variable, loading in a JSON is different in Windows & Unix/Linux systems
+        if (platform.system() != "Windows"):
+            with open(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)) as iso3166_updates_json:
+                self.all = json.load(iso3166_updates_json)
+        else:
+            with open(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename), encoding="utf-8") as iso3166_updates_json:
+                self.all = json.loads(iso3166_updates_json.read())
 
         #make all updates object subscriptable using Map class
-        self.all = Map(self.all)
+        # self.all = Map(self.all)
+
+        #if input country code param set, iterate over data object and get updates data for specified input/inputs
+        if (self.country_code != ""):
+            temp_updates_data = {}
+            self.country_code = self.country_code.upper().replace(" ", "").split(',')
+            for code in range(0, len(self.country_code)):
+                #if 3 letter alpha-3 or numeric codes input then convert to corresponding alpha-2, if invalid code then raise error
+                if (len(self.country_code[code]) == 3):
+                    temp_alpha_code = self.convert_to_alpha2(self.country_code[code])
+                    if (temp_alpha_code is None and self.country_code[code].isdigit()):
+                        raise ValueError(f"Invalid ISO 3166-1 numeric country code input, cannot convert into corresponding alpha-2 code: {self.country_code[code]}.")
+                    if (temp_alpha_code is None):
+                        raise ValueError(f"Invalid ISO 3166-1 alpha-3 country code input, cannot convert into corresponding alpha-2 code: {self.country_code[code]}.")
+                    self.country_code[code] = temp_alpha_code
+
+                #raise error if invalid alpha-2 code input
+                if not (self.country_code[code] in sorted(list(iso3166.countries_by_alpha2.keys()))) or not (self.country_code[code] in list(self.all.keys())):
+                    raise ValueError(f"Invalid alpha-2 country code input: {self.country_code[code]}.")
+                
+                #create temporary updates data object
+                temp_updates_data[self.country_code[code]] = {}
+                temp_updates_data[self.country_code[code]] = self.all[self.country_code[code]]
+            
+            #delete existing 'all' class attribute that currently has all updates data for all countries, which aren't needed if input country is specified
+            del self.all
+
+            #set 'all' class attribute to the updates data from input country/countries
+            self.all = temp_updates_data
+        
+        #get list of all countries by their 2 letter alpha-2 code
+        # self.alpha2 = sorted(list(iso3166.countries_by_alpha2.keys()))
+
+    def __getitem__(self, alpha_code: str) -> dict:
+        """
+        Get all listed updates/changes in the updates json object for an input country/countries,
+        using the ISO 3166-1 alpha-2, alpha-3 or numeric country codes. This function uses the Map 
+        class to make the instance object of the class subscriptable. It can accept 1 or more alpha 
+        codes for countries and return the data for each. If the alpha-3 or numeric codes are input 
+        its converted into its alpha-2 counterpart.
+        
+        Parameters
+        ==========
+        :alpha_code: str
+            one or more ISO 3166-1 alpha-2, alpha-3 or numeric country codes for sought country/
+            territory updates e.g. AD, DE, EGT, 184. The alpha-3 or numeric codes will be 
+            converted into their alpha-3 counterparts. 
+
+        Returns
+        =======
+        :country_updates_dict: dict
+            dict object of country updates info for inputted code/codes.
 
-        #get list of all countries by their 2 letter alpha-3 code
-        self.alpha2 = sorted(list(iso3166.countries_by_alpha2.keys()))
+        Usage
+        -----
+        from iso3166_updates import *
         
-        #get list of all countries by their 3 letter alpha-3 code
-        self.alpha3 = sorted(list(iso3166.countries_by_alpha3.keys()))
+        #create instance of class
+        iso = ISO3166_Updates()
+
+        #get country ISO 3166 updates info for Ethiopia
+        iso["ET"] 
+        iso["ETH"] 
+        iso["231"] 
+ 
+        #get country ISO 3166 updates info for Gabon
+        iso["GA"] 
+        iso["GAB"] 
+        iso["266"] 
+
+        #get country ISO 3166 updates info for Rwanda, Tuvalu, Ukraine and Uruguay
+        iso["RW, TV, UA, UY"]
+        iso["RWA, TUV, UKR, URY"]
+        iso["646, 798, 804, 858"]
+        """
+        #raise type error if input isn't a string
+        if not (isinstance(alpha_code, str)):
+            raise TypeError('Input parameter {} is not of correct datatype string, got {}.'.format(alpha_code, type(alpha_code)))       
     
-    def year(self, input_year):
+        #stripping input of whitespace, uppercasing, separating multiple alpha codes, if applicable and sort list
+        alpha_code = alpha_code.strip().upper()
+        alpha_code = sorted(alpha_code.replace(' ', '').split(','))
+
+        #object to store country data, it is a dict if more than one country or list if only one country
+        country_updates_dict = {}
+
+        #iterate over all input alpha codes, appending all updates to country object, pass through Map class to access via dot notation
+        for code in range(0, len(alpha_code)):
+
+            #if 3 letter alpha-3 or numeric codes input then convert to corresponding alpha-2, else raise error
+            if (len(alpha_code[code]) == 3):
+                temp_alpha_code = self.convert_to_alpha2(alpha_code[code])
+                if (temp_alpha_code is None and alpha_code[code].isdigit()):
+                    raise ValueError(f"Invalid ISO 3166-1 numeric country code input, cannot convert into corresponding alpha-2 code: {alpha_code[code]}.")
+                if (temp_alpha_code is None):
+                    raise ValueError(f"Invalid ISO 3166-1 alpha-3 country code input, cannot convert into corresponding alpha-2 code: {alpha_code[code]}.")
+                alpha_code[code] = temp_alpha_code
+               
+            #raise error if invalid alpha-2 code input or country data not imported on object instantiation 
+            if not (alpha_code[code] in sorted(list(iso3166.countries_by_alpha2.keys()))):
+                raise ValueError(f"Invalid alpha-2 code input: {alpha_code[code]}.")
+            if not (alpha_code[code] in list(self.all.keys())):
+                raise ValueError(f"Valid alpha-2 code input {alpha_code[code]}, but country data not available as 'country_code' parameter was input on class instantiation,"
+                                " try creating another instance of the class with no initial input parameter value, e.g iso = ISO3166_Updates().")
+
+            #add each country update to country object
+            country_updates_dict[alpha_code[code]] = []
+            for update in range(0, len(self.all[alpha_code[code]])):
+                country_updates_dict[alpha_code[code]].append(Map(self.all[alpha_code[code]][update]))
+                #iterate over nested dicts, convert into instances of Map class so they can be accessed via dot notation
+                for key in country_updates_dict[alpha_code[code]][update].keys():
+                    if (isinstance(country_updates_dict[alpha_code[code]][update][key], dict)):
+                        country_updates_dict[alpha_code[code]][update][key] = Map(country_updates_dict[alpha_code[code]][update][key])
+            
+        #keys in updates dict needs sorted in the case of alpha-3 and or numeric codes being input
+        country_updates_dict = dict(sorted(country_updates_dict.items()))
+
+        #convert into instance of Map class so keys can be accessed via dot notation
+        country_updates_dict = Map(country_updates_dict)
+
+        return country_updates_dict 
+    
+    def year(self, input_year: str) -> dict:
         """
         Get all listed updates/changes in the updates json object for an input year, set of years,
-        year range or greater than/less than year. The json object will be iterated over and
-        any matching updates from the "Date Issued" column will be appended to the output dict.
+        year range or greater than/less than year. The json object will be iterated over and any
+        matching updates from the "Date Issued" column will be appended to the output dict.
 
         Parameters
         ==========
-        :input_year: str/list
-            single or list of multiple years. Can also accept a year range or a year to get updates
-            greater than or less than e.g "2015", "2009,2019", ">2022", "<2004", "2005-2012".
+        :input_year: str
+            single or comma separated list of multiple years. Can also accept a year range or a year 
+            to get updates greater than or less than e.g "2015", "2009,2019", ">2022", "<2004", "2005-2012".
 
         Returns
         =======
         :country_output_dict: dict
             output dictionary of sought ISO 3166 updates for input year/years.
         """
-        #if single str of 1 or more years input then convert to array, remove whitespace, seperate using comma
+        #if single str of 1 or more years input then convert to array, remove whitespace, separate using comma
         if (isinstance(input_year, str)):
             input_year = input_year.replace(' ', '').split(',')
         else:
             #raise error if invalid data type for year parameter
-            raise TypeError("Invalid data type for year parameter, expected str, got {}.".format(type(input_year)))
+            raise TypeError(f"Invalid data type for year parameter, expected str, got {type(input_year)}.")
         
         country_output_dict = {}
 
         year_range = False
         greater_than = False
         less_than = False
         
-        #a '-' seperating 2 years implies a year range of sought country updates, validate format of years in range
-        #a ',' seperating 2 years implies a list of years
+        #a '-' separating 2 years implies a year range of sought country updates
+        #a ',' separating 2 years implies a list of years
         #a '>' before year means get all country updates greater than or equal to specified year
         #a '<' before year means get all country updates less than specified year
         if (input_year != []):
             if ('-' in input_year[0]):
                 year_range = True
                 input_year = input_year[0].split('-')
+                #if year range years are wrong way around then swap them
+                if (input_year[0] > input_year[1]):
+                    input_year[0], input_year[1] = input_year[1], input_year[0]
                 #only 2 years should be included in input parameter
                 if (len(input_year) > 2):
                     input_year = []
                     year_range = False
             #parse array for using greater than symbol
             elif ('>' in input_year[0]):
                 input_year = list(input_year[0].rpartition(">")[1:])
@@ -155,15 +298,15 @@
                 input_year = input_year[0].split(',')
         #validate each year's format using regex
         for year_ in input_year:
             #skip to next iteration if < or > symbol
             if (year_ == '<' or year_ == '>' or year_ == '-'):
                 continue
             if not (bool(re.match(r"^1[0-9][0-9][0-9]$|^2[0-9][0-9][0-9]$", year_))):
-                raise ValueError("Invalid year input: {}.".format(year_))
+                raise ValueError(f"Invalid year input: {year_}.")
 
         #temp object to not override original updates object
         country_output_dict = {}
 
         #drop rows of dict where Date Issued column isn't same as year parameter, if greater_than, 
         #less_than or year_range bools set then drop any objects of dict that don't meet condition
         if (input_year != []): 
@@ -203,111 +346,132 @@
             country_output_dict = {i:j for i,j in country_output_dict.items() if j != []}
 
         #make updates object subscriptable using Map class
         country_output_dict = Map(country_output_dict)
 
         return country_output_dict
 
-    def __getitem__(self, alpha2_code):
+    def months(self, input_month: str) -> dict:
         """
-        Get all listed updates/changes in the updates json object for an input country/countries,
-        using the 2 letter ISO 3166-1 code. This function uses the Map class to make the clas
-        subscriptable. It can accept 1 or more 2 letter alpha-2 codes for countries. Also the
-        3 letter alpha-3 code for a country can be input which will be converted into its alpha-2 
-        counterpart.
-        
+        Get all listed updates/changes in the updates json object that have a published date
+        over the past number of months, inclusive, specified by the input parameter, e.g. 
+        all updates from the past 12, 24 or 36 months. You can also get those published within 
+        a month range e.g all updates from the past 6-12 months. The json object will be 
+        iterated over and any matching updates from the "Date Issued" column will be appended 
+        to the output dict.
+
         Parameters
         ==========
-        :alpha2_code: str
-            one or more 2 letter alpha-2 codes for sought country/territory e.g (AD, EG, DE). Can 
-            also accept 3 letter alpha-3 code e.g (AND, EGT, DEU), this will be converted into 
-            its alpha-2 counterpart.
+        :input_month: str
+            single month or month range from present day e.g "12", "24", "36-60".
 
         Returns
         =======
-        :country_updates_dict: dict
-            dict object of country updates info for inputted code/codes.
+        :country_output_dict: dict
+            output dictionary of sought ISO 3166 updates for input months/month range.
+        """
+        # #if no input month parameter specified then return error message
+        # if (input_month == ""):
+        #     raise ValueError("The month input parameter cannot be empty.")
 
-        Usage
-        -----
-        import iso3166_updates as iso
+        #add int functionality
 
-        #get country ISO 3166 updates info for Ethiopia
-        iso.updates["ET"] 
-        iso.updates["ETH"] 
-        iso.updates["et"] 
- 
-        #get country ISO 3166 updates info for Gabon
-        iso.updates["GA"] 
-        iso.updates["GAB"] 
-        iso.updates["ga"] 
+        #return error if invalid month value type input, skip if month range input
+        if not ('-' in input_month):
+            if not (str(input_month).isdigit()):
+                raise ValueError(f"Invalid month input: {''.join(input_month)}.")
 
-        #get country ISO 3166 updates info for Rwanda, Tuvalu, Ukraine and Uruguay
-        iso.updates["RW, TV, UA, UY"]
-        iso.updates["RWA, TUV, UKR, URY"]
-        iso.updates["rw, tv, ua, uy"]
-        """
-        #raise type error if input isn't a string
-        if not (isinstance(alpha2_code, str)):
-            raise TypeError('Input parameter {} is not of correct datatype string, got {}.'.format(alpha2_code, type(alpha2_code)))       
-        
-        #stripping input of whitespace, uppercasing, seperating multiple alpha-2 codes, if applicable and sort list
-        alpha2_code = alpha2_code.strip().upper()
-        alpha2_code = sorted(alpha2_code.replace(' ', '').split(','))
+        #get current datetime object
+        current_datetime = datetime.strptime(datetime.today().strftime('%Y-%m-%d'), "%Y-%m-%d")
 
-        #object to store country data, dict if more than one country or list if only one country
-        country_updates_dict = {}
+        #object to store country updates 
+        country_output_dict = {}
 
-        #iterate over all input alpha-2 codes, appending all updates to country object, pass through Map class to access via dot notation
-        for code in alpha2_code:
+        #get all alpha-2 codes from iso3166 and all updates data before filtering by month
+        input_alpha_codes = list(iso3166.countries_by_alpha2.keys())
 
-            #validate 2 letter alpha-2 code exists in ISO 3166-1, raise error if not found            
-            if (len(code) == 2):
-                if not (code in self.alpha2):      
-                    raise ValueError("Alpha-2 Code {} not found in list of ISO 3166-1 alpha-2 codes.".format(code))            
-
-            #if 3 letter alpha-3 code input, check it exists in ISO 3166-1, then convert into its 2 letter alpha-2 code, raise error if not found            
-            if (len(code) == 3):
-                if (code in self.alpha3):      
-                    code = iso3166.countries_by_alpha3[code].alpha2
+        #remove XK (Kosovo) from list, if applicable
+        if ("XK" in input_alpha_codes):
+            input_alpha_codes.remove("XK")
+
+        #filter out updates that are not within specified month range
+        for code in input_alpha_codes:
+            country_output_dict[code] = [] 
+            for update in range(0, len(self.all[code])):
+
+                #convert year in Date Issued column to date object, remove "corrected" date if applicable
+                if ("corrected" in self.all[code][update]["Date Issued"]):
+                    row_date = datetime.strptime(re.sub("[(].*[)]", "", self.all[code][update]["Date Issued"]).replace(' ', "").
+                                                        replace(".", '').replace('\n', ''), '%Y-%m-%d')
                 else:
-                    raise ValueError("Alpha-3 Code {} not found in list of ISO 3166-1 alpha-3 codes.".format(code))        
-
-            #raise error if alpha-2 code not found in list of available codes
-            if not (code in self.alpha2):
-                raise ValueError("Alpha-2 Code {} not found in list of ISO 3166-1 alpha-2 codes.".format(code))        
-
-            #if only one alpha-2 code input, convert country object to list and append all country update to it
-            if (len(alpha2_code) == 1):
-                country_updates_dict = []
-                for update in range(0, len(self.all[code])):
-                    country_updates_dict.append(Map(self.all[code][update]))
-                    #iterate over nested dicts, convert into instances of Map class so they can be accessed via dot notation
-                    for key in country_updates_dict[update].keys():
-                        if (isinstance(country_updates_dict[update][key], dict)):
-                            country_updates_dict[update][key] = Map(country_updates_dict[update][key])
-            #if multiple alpha-2 codes input, add update dict to country object
-            else:
-                country_updates_dict[code] = []
-                for update in range(0, len(self.all[code])):
-                    country_updates_dict[code].append(Map(self.all[code][update]))
-                    #iterate over nested dicts, convert into instances of Map class so they can be accessed via dot notation
-                    for key in country_updates_dict[code][update].keys():
-                        if (isinstance(country_updates_dict[code][update][key], dict)):
-                            country_updates_dict[code][update][key] = Map(country_updates_dict[code][update][key])
+                    row_date = datetime.strptime(self.all[code][update]["Date Issued"].replace('\n', ''), '%Y-%m-%d')
                 
-                #convert into instance of Map class so keys can be accessed via dot notation
-                country_updates_dict = Map(country_updates_dict)
+                #calculate difference in dates
+                date_diff = relativedelta.relativedelta(current_datetime, row_date)
 
-        return country_updates_dict 
+                #calculate months difference
+                diff_months = date_diff.months + (date_diff.years * 12)
+
+                #parse parameter to get range of months to get updates from
+                if ('-' in input_month):
+                    start_month, end_month = int(input_month.split('-')[0]), int(input_month.split('-')[1])
+                    #if months in month range input are wrong way around then swap them
+                    if (start_month > end_month):
+                        start_month, end_month = end_month, start_month
+                    #if current updates row is >= start month input param and <= end month then add to output object
+                    if ((diff_months >= start_month) and (diff_months <= end_month)):
+                        country_output_dict[code].append(self.all[code][update])
+                else:
+                    #if current updates row is <= month input param then add to output object
+                    if (diff_months <= int(input_month)):
+                        country_output_dict[code].append(self.all[code][update])
+
+            #if current alpha-2 has no rows for selected month range, remove from output object
+            if (country_output_dict[code] == []):
+                country_output_dict.pop(code, None)
+
+        #make updates object subscriptable using Map class
+        country_output_dict = Map(country_output_dict)
+
+        return country_output_dict
+        
+    def convert_to_alpha2(self, alpha_code: str) -> str:
+        """ 
+        Auxillary function that converts an ISO 3166 country's 3 letter alpha-3 
+        or numeric code into its 2 letter alpha-2 counterpart. 
+
+        Parameters 
+        ==========
+        :alpha_code: str
+            3 letter ISO 3166-1 alpha-3 or numeric country code.
+        
+        Returns
+        =======
+        :iso3166.countries_by_alpha3[alpha3_code].alpha2: str
+            2 letter ISO 3166 alpha-2 country code. 
+        """
+        if (alpha_code.isdigit()):
+            #return error if numeric code not found
+            if not (alpha_code in list(iso3166.countries_by_numeric.keys())):
+                return None
+            else:
+                #use iso3166 package to find corresponding alpha-2 code from its numeric code
+                return iso3166.countries_by_numeric[alpha_code].alpha2
+    
+        #return error if 3 letter alpha-3 code not found
+        if not (alpha_code in list(iso3166.countries_by_alpha3.keys())):
+            return None
+        else:
+            #use iso3166 package to find corresponding alpha-2 code from its alpha-3 code
+            return iso3166.countries_by_alpha3[alpha_code].alpha2
     
-    def __str__(self):
-        return "Instance of ISO Updates class."
+    def __str__(self) -> str:
+        return "Instance of ISO3166 Updates class."
 
-    def __sizeof__(self):
+    def __sizeof__(self) -> float:
         """ Return size of instance of ISO 3166 Updates class. """
         return self.__sizeof__()
 
 class Map(dict):
     """
     Class that accepts a dict and allows you to use dot notation to access
     members of the dictionary. 
@@ -360,11 +524,8 @@
         self.__dict__.update({key: value})
 
     def __delattr__(self, item):
         self.__delitem__(item)
 
     def __delitem__(self, key):
         super(Map, self).__delitem__(key)
-        del self.__dict__[key]
-
-#create instance of ISO3166_Updates class
-updates = ISO3166_Updates()
+        del self.__dict__[key]
```

### Comparing `iso3166-updates-1.6.0/setup.py` & `iso3166_updates-1.7.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,45 @@
-###############################################################################
-#####   Setup.py - installs all the required packages and dependancies    #####
-###############################################################################
+[tool.poetry]
+name = "iso3166-updates"
+version = "1.7.0"
+description = "Get the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest." 
+authors = ["AJ Mckenna <amckenna41@qub.ac.uk>"]
+maintainers = ["AJ McKenna <amckenna41@qub.ac.uk>"]
+license = "MIT"
+readme = "README.md"
+classifiers = [
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Information Technology",
+        "License :: OSI Approved :: MIT License",
+        "License :: Free For Educational Use",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",	
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Software Development :: Libraries :: Python Modules"
+]
+keywords = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv", "iso3166-2", "subdivisions", "iso3166-1", "alpha-2", "alpha-3", "selenium", "chromedriver"]
+packages = [{include = "iso3166_updates"}]
 
-import pathlib
-from setuptools import setup, find_packages
+[tool.poetry.dependencies]
+python = "^3.8"
+iso3166 = "^2.1.1"
 
-#software metadata
-__name__ = 'iso3166-updates'
-__version__ = "1.6.0"
-__description__ = "A Python package that pulls the latest updates & changes to all ISO 3166 listed countries, dependent territories, and special areas of geographical interest.", 
-__author__ = 'AJ McKenna, https://github.com/amckenna41'
-__authorEmail__ = 'amckenna41@qub.ac.uk'
-__license__ = 'MIT'
-__url__ = 'https://github.com/amckenna41/iso3166-updates'
-__download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
-__status__ = 'Production'
-__maintainer__ = "AJ McKenna"
-__keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv", \
-            "iso3166-2", "subdivisions", "iso3166-1", "alpha-2", "alpha-3", "selenium", "chromedriver"]
-__test_suite__ = "tests"
- 
-#get path to README file
-HERE = pathlib.Path(__file__).parent
-README = (HERE / 'README.md').read_text()
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.0.2"
 
-setup(name=__name__,
-      version=__version__,
-      description=__description__,
-      long_description = README,
-      long_description_content_type = "text/markdown",
-      author=__author__,
-      author_email=__authorEmail__,
-      maintainer=__maintainer__,
-      license=__license__,
-      url=__url__,
-      download_url=__download_url__,
-      keywords=__keywords__,
-      classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Information Technology',
-        'License :: OSI Approved :: MIT License',
-        'License :: Free For Educational Use',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',	
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Programming Language :: Python :: 3 :: Only',
-        'Topic :: Scientific/Engineering',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-    ],
-      install_requires=[
-          'iso3166'
-      ],
-     test_suite=__test_suite__,
-     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", 
-        "iso3166-updates-api", "iso3166-check-for-updates", ".github"]),
-     include_package_data=True,
-     zip_safe=False)
+[tool.poetry.urls]
+homepage = "https://iso3166-updates.com/api/"
+repository = "https://github.com/amckenna41/iso3166-updates"
+documentation = "https://iso3166-updates.readthedocs.io/en/latest/"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

