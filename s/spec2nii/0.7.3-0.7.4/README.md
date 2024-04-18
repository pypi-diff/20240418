# Comparing `tmp/spec2nii-0.7.3.tar.gz` & `tmp/spec2nii-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec2nii-0.7.3.tar", last modified: Tue Mar 12 15:15:29 2024, max compression
+gzip compressed data, was "spec2nii-0.7.4.tar", last modified: Thu Apr 18 15:27:27 2024, max compression
```

## Comparing `spec2nii-0.7.3.tar` & `spec2nii-0.7.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.210717 spec2nii-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-03-12 15:15:22.000000 spec2nii-0.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-12 15:15:22.000000 spec2nii-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-12 15:15:22.000000 spec2nii-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-03-12 15:15:29.210717 spec2nii-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-03-12 15:15:22.000000 spec2nii-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-12 15:15:22.000000 spec2nii-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 15:15:22.000000 spec2nii-0.7.3/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-12 15:15:29.210717 spec2nii-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-12 15:15:22.000000 spec2nii-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.202716 spec2nii-0.7.3/spec2nii/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.206717 spec2nii-0.7.3/spec2nii/GE/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GE/VESPA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   161099 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GE/ge_hdr_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GE/ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    48030 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GE/ge_read_pfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.206717 spec2nii-0.7.3/spec2nii/GSL/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GSL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/GSL/gslfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.206717 spec2nii-0.7.3/spec2nii/Philips/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Philips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Philips/philips.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Philips/philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Philips/philips_dcm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.206717 spec2nii-0.7.3/spec2nii/Siemens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Siemens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Siemens/dicomfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Siemens/rda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Siemens/twix_special_case.py
--rw-r--r--   0 runner    (1001) docker     (127)    45998 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/Siemens/twixfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-12 15:15:29.214717 spec2nii-0.7.3/spec2nii/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/anonymise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/bruker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/bruker_fid_override.json
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/bruker_properties.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.206717 spec2nii-0.7.3/spec2nii/dcm2niiOrientation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/dcm2niiOrientation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/dcm2niiOrientation/orientationFuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/due.py
--rw-r--r--   0 runner    (1001) docker     (127)    23327 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/fileiobase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/jmrui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/nifti_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/other_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    33039 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/spec2nii.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/uih.py
--rw-r--r--   0 runner    (1001) docker     (127)    64350 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/varian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-03-12 15:15:22.000000 spec2nii-0.7.3/spec2nii/varian_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.210717 spec2nii-0.7.3/spec2nii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 15:15:29.000000 spec2nii-0.7.3/spec2nii.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:15:29.210717 spec2nii-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_anon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_bruker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_ge_pfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_ge_pfile_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_jmrui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_nifti_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_other_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_dicom_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_orientation_dcm_spar_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_sdat_spar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_philips_sdat_spar_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_mrsi_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_rda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_special_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_svs_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_siemens_twix.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_spectralwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_uih.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_uih_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-12 15:15:22.000000 spec2nii-0.7.3/tests/test_varian.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-03-12 15:15:22.000000 spec2nii-0.7.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.945872 spec2nii-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-18 15:27:21.000000 spec2nii-0.7.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-18 15:27:21.000000 spec2nii-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 15:27:21.000000 spec2nii-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-18 15:27:27.945872 spec2nii-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-04-18 15:27:21.000000 spec2nii-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 15:27:21.000000 spec2nii-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 15:27:21.000000 spec2nii-0.7.4/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-18 15:27:27.945872 spec2nii-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-18 15:27:21.000000 spec2nii-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.937872 spec2nii-0.7.4/spec2nii/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.937872 spec2nii-0.7.4/spec2nii/GE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GE/VESPA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162242 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GE/ge_hdr_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GE/ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50075 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GE/ge_read_pfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.937872 spec2nii-0.7.4/spec2nii/GSL/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GSL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/GSL/gslfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.941872 spec2nii-0.7.4/spec2nii/Philips/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Philips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Philips/philips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Philips/philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Philips/philips_dcm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.941872 spec2nii-0.7.4/spec2nii/Siemens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Siemens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32079 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Siemens/dicomfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Siemens/rda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Siemens/twix_special_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47076 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/Siemens/twixfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 15:27:27.945872 spec2nii-0.7.4/spec2nii/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/anonymise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/bruker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/bruker_fid_override.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/bruker_properties.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.941872 spec2nii-0.7.4/spec2nii/dcm2niiOrientation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/dcm2niiOrientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/dcm2niiOrientation/orientationFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/due.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23327 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/fileiobase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/nifti_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/other_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33093 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/spec2nii.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/uih.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64350 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/varian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-18 15:27:21.000000 spec2nii-0.7.4/spec2nii/varian_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.945872 spec2nii-0.7.4/spec2nii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 15:27:27.000000 spec2nii-0.7.4/spec2nii.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:27.945872 spec2nii-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_anon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_ge_pfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_ge_pfile_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_jmrui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_nifti_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_other_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_dicom_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_orientation_dcm_spar_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_sdat_spar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_philips_sdat_spar_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_mrsi_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_rda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_special_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_svs_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_siemens_twix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_spectralwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_uih.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_uih_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-18 15:27:21.000000 spec2nii-0.7.4/tests/test_varian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-18 15:27:21.000000 spec2nii-0.7.4/versioneer.py
```

### Comparing `spec2nii-0.7.3/CHANGELOG.md` & `spec2nii-0.7.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 This document contains the Spec2nii release history in reverse chronological order.
 
+0.7.4 (Thursday 18th April 2024)
+--------------------------------
+- Refinements and improvements to the GE SVS pipeline from Mark Mikkelsen.
+- Add support for older jMRUI text formats which have a slightly different syntax. With thanks to Donnie Cameron.
+- Handle odd case of XA like .twix headers in a VX baseline scan
+- Improved (and validated) handling of Dinesh Deelchand's slaser sequences with integrated references (`svs_slaser(voi)_dkd(2)`)
+
 0.7.3 (Tuesday 12th March 2024)
 -------------------------------
 - Siemens .rda format now had corrected and validated orientations (tested on VE11 baseline).
 - Siemens .rda format now handles MRSI/CSI data and matches DICOM output. Validated on VE11 baseline data.
 - Fixes in Siemens Twix special case for universal editing sequence (HERMES conditions).
 - Added handling of custom Bruker sequences `mt_sLASER`, `mt_MEGA_sLASER_V35` and `cl_STELASER_PA360_b`.
 - Philips vendor MEGA-PRESS handled through DICOM pathway. Thanks to Sandeep Ganji and Yansong Zhao for their help.
```

### Comparing `spec2nii-0.7.3/LICENSE` & `spec2nii-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/PKG-INFO` & `spec2nii-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.7.3
+Version: 0.7.4
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `spec2nii-0.7.3/README.md` & `spec2nii-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/setup.cfg` & `spec2nii-0.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/setup.py` & `spec2nii-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/GE/VESPA_LICENSE` & `spec2nii-0.7.4/spec2nii/GE/VESPA_LICENSE`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/GE/ge_hdr_fields.py` & `spec2nii-0.7.4/spec2nii/GE/ge_hdr_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''List of GE p-file offsets.
+"""List of GE p-file offsets.
 
 This code is taken from the VESPA project https://scion.duhs.duke.edu/vespa/project.
 I therefore include their BSD statement here.
 
     Copyright (c) 2010, Duke University. All rights reserved.
 
     Redistribution and use in source and binary forms, with or without
@@ -56,15 +56,15 @@
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
     ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
     (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
     LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
     ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
     (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
     SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-'''
+"""
 
 import ctypes as ct
 import numpy as np
 
 
 class UnknownPfileHdr(RuntimeError):
     pass
@@ -750,18 +750,24 @@
         plist.append(('rhr_rh_file_contents',     ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_data_collect_type', ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 6))
         plist.append(('rhr_rh_npasses',           ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 2))
         plist.append(('rhr_rh_nslices',           ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 10))
+        plist.append(('rhr_rh_nechoes',           ct.c_short))
+        plist.append(('rhr_rh_navs',              ct.c_short))
+        plist.append(('rhr_rh_nframes',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 4))
         plist.append(('rhr_rh_frame_size',        ct.c_ushort))
         plist.append(('rhr_rh_point_size',        ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 32))
+        plist.append(('pad_xx',                   ct.c_char * 18))
+        plist.append(('rhr_rh_da_xres',           ct.c_short))
+        plist.append(('rhr_rh_da_yres',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_raw_pass_size',     ct.c_uint))
         plist.append(('pad_xx',                   ct.c_char * 80))
         plist.append(('rhr_rh_dab[0]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[0]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[1]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[1]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[2]_start_rcv',  ct.c_short))
@@ -974,18 +980,24 @@
         plist.append(('rhr_rh_file_contents',     ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_data_collect_type', ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 6))
         plist.append(('rhr_rh_npasses',           ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 2))
         plist.append(('rhr_rh_nslices',           ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 10))
+        plist.append(('rhr_rh_nechoes',           ct.c_short))
+        plist.append(('rhr_rh_navs',              ct.c_short))
+        plist.append(('rhr_rh_nframes',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 4))
         plist.append(('rhr_rh_frame_size',        ct.c_ushort))
         plist.append(('rhr_rh_point_size',        ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 32))
+        plist.append(('pad_xx',                   ct.c_char * 18))
+        plist.append(('rhr_rh_da_xres',           ct.c_short))
+        plist.append(('rhr_rh_da_yres',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_raw_pass_size',     ct.c_uint))
         plist.append(('pad_xx',                   ct.c_char * 80))
         plist.append(('rhr_rh_dab[0]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[0]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[1]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[1]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[2]_start_rcv',  ct.c_short))
@@ -1198,18 +1210,24 @@
         plist.append(('rhr_rh_file_contents',     ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_data_collect_type', ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 6))
         plist.append(('rhr_rh_npasses',           ct.c_short))
         plist.append(('pad_xx',                   ct.c_char * 2))
         plist.append(('rhr_rh_nslices',           ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 10))
+        plist.append(('rhr_rh_nechoes',           ct.c_short))
+        plist.append(('rhr_rh_navs',              ct.c_short))
+        plist.append(('rhr_rh_nframes',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 4))
         plist.append(('rhr_rh_frame_size',        ct.c_ushort))
         plist.append(('rhr_rh_point_size',        ct.c_short))
-        plist.append(('pad_xx',                   ct.c_char * 32))
+        plist.append(('pad_xx',                   ct.c_char * 18))
+        plist.append(('rhr_rh_da_xres',           ct.c_short))
+        plist.append(('rhr_rh_da_yres',           ct.c_short))
+        plist.append(('pad_xx',                   ct.c_char * 10))
         plist.append(('rhr_rh_raw_pass_size',     ct.c_uint))
         plist.append(('pad_xx',                   ct.c_char * 80))
         plist.append(('rhr_rh_dab[0]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[0]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[1]_start_rcv',  ct.c_short))
         plist.append(('rhr_rh_dab[1]_stop_rcv',   ct.c_short))
         plist.append(('rhr_rh_dab[2]_start_rcv',  ct.c_short))
```

### Comparing `spec2nii-0.7.3/spec2nii/GE/ge_pfile.py` & `spec2nii-0.7.4/spec2nii/GE/ge_pfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''spec2nii module containing functions specific to interpreting the GE pfile format
+"""spec2nii module containing functions specific to interpreting the GE pfile format
 
 Author: William Clarke <william.clarke@ndcn.ox.ac.uk>
 Copyright (C) 2020 University of Oxford
 
 This code is adapted from the VESPA project https://scion.duhs.duke.edu/vespa/project.
 I therefore include their BSD statement here.
 
@@ -29,15 +29,15 @@
     CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
     LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
     OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
     DAMAGE.
 
     For portions of this code, copyright and license information differs from
     the above. In these cases, copyright and/or license information is inline.
-'''
+"""
 
 # Python modules
 from datetime import datetime
 from os.path import basename
 from warnings import warn
 
 # 3rd party modules
@@ -79,53 +79,57 @@
         else:
             fnames.append(fname_out + fns)
 
     return data, fnames
 
 
 def _process_svs_pfile(pfile):
-    '''Handle SVS data
+    """Handle SVS data
 
     :param Pfile pfile: Pfile object
     :return: List of NIFTI MRS data objects
     :return: List of file name suffixes
-    '''
+    """
     psd = pfile.hdr.rhi_psdname.decode('utf-8').lower()
 
-    if psd in ('probe-p', 'probe-s'):
+    # MM: Some 'gaba' psd strings contain full path names, so truncate to the end of the path
+    if psd.endswith('gaba'):
+        psd = 'gaba'
+
+    numecho = pfile.hdr.rhi_numecho
+
+    if psd in ('probe-p', 'probe-s', 'probe-p_ach'):
         data, meta, dwelltime, fname_suffix = _process_probe_p(pfile)
-    elif psd in ('oslaser', 'slaser_cni'):
+    elif psd in ('oslaser', 'slaser_cni') and numecho == 1:  # MM: If non-edited data, use _process_oslaser
         data, meta, dwelltime, fname_suffix = _process_oslaser(pfile)
+    elif psd == 'oslaser' and numecho > 1:  # MM: If edited data, use _process_gaba
+        data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     elif psd == 'slaser':
         data, meta, dwelltime, fname_suffix = _process_slaser(pfile)
-    elif psd in ('gaba', 'hbcd'):
-        data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
-    elif 'jpress_ac' in psd:  # Bergen patch
-        data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
-    elif psd == 'jpress':
+    elif psd in ('jpress', 'jpress_ac', 'gaba', 'hbcd', 'probe-p-mega_rml', 'repress7'):
         data, meta, dwelltime, fname_suffix = _process_gaba(pfile)
     else:
         raise UnsupportedPulseSequenceError(f'Unrecognised sequence {psd}.')
 
     orientation = NIFTIOrient(_calculate_affine(pfile))
 
     out_nmrs = []
     for dd, mm in zip(data, meta):
         out_nmrs.append(gen_nifti_mrs_hdr_ext(dd, dwelltime, mm, orientation.Q44, no_conj=True))
 
     return out_nmrs, fname_suffix
 
 
 def _process_probe_p(pfile):
-    '''Extract metabolite and reference data from a prob_p format pfile
+    """Extract metabolite and reference data from a prob_p format pfile
 
     :param Pfile pfile: Pfile object
     :return: List numpy data arrays
     :return: List of file name suffixes
-    '''
+    """
 
     metab = pfile.map.raw_suppressed                    # typically (1,1,1,navg,ncoil,npts)
     metab = np.transpose(metab, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
     water = pfile.map.raw_unsuppressed                  # typically (1,1,1,navg,ncoil,npts)
     water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
@@ -140,23 +144,23 @@
     meta_ref.set_dim_info(0, 'DIM_COIL')
     meta_ref.set_dim_info(1, 'DIM_DYN')
 
     return [metab, water], [meta, meta_ref], dwelltime, ['', '_ref']
 
 
 def _process_oslaser(pfile):
-    '''Extract metabolite and reference data from a oslaser format pfile
+    """Extract metabolite and reference data from a oslaser format pfile
 
     I think this is like the CMRR sLASER sequence with 2 ecc and 2 water scaling
     scans at the start and end of each acquisition.
 
     :param Pfile pfile: Pfile object
     :return: List numpy data arrays
     :return: List of file name suffixes
-    '''
+    """
 
     water = pfile.map.raw_unsuppressed                  # typically (1,1,1,navg,ncoil,npts)
     metab = pfile.map.raw_suppressed
     metab = np.transpose(metab, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
     water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
     data = []
@@ -175,22 +179,22 @@
 
     dwelltime = 1 / pfile.hdr.rhr_spectral_width
 
     return data, meta, dwelltime, fname_suffix
 
 
 def _process_slaser(pfile):
-    '''Extract metabolite and reference data from a slaser format pfile
+    """Extract metabolite and reference data from a slaser format pfile
 
     This seems to be like a standard probe-p. Maybe slaser is the canonical vendor implementation.
 
     :param Pfile pfile: Pfile object
     :return: List numpy data arrays
     :return: List of file name suffixes
-    '''
+    """
 
     metab = pfile.map.raw_suppressed                    # typically (1,1,1,navg,ncoil,npts)
     metab = np.transpose(metab, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
     water = pfile.map.raw_unsuppressed                  # typically (1,1,1,navg,ncoil,npts)
     water = np.transpose(water, [0, 1, 2, 5, 4, 3])     # swap to (1,1,1,npts,ncoil,navg)
 
@@ -198,49 +202,86 @@
 
     meta = _populate_metadata(pfile, water_suppressed=True, data_dimensions=metab.ndim)
     meta_ref = _populate_metadata(pfile, water_suppressed=False, data_dimensions=water.ndim)
 
     return [metab, water], [meta, meta_ref], dwelltime, ['', '_ref']
 
 
+def _add_editing_info(pfile, meta, data):
+    """Add editing information to dimension tags and headers
+
+    :param pfile: p-file object
+    :type pfile: Pfile
+    :param meta: Header extension object
+    :type meta: Hdr_Ext
+    :param data: Shaped complex data
+    :type data: np.ndarray
+    """
+    edit_rf_waveform = pfile.hdr.rhi_user19
+    # edit_rf_waveform == 19.0 is used by HERMES and HERCULES
+    if data.shape[-1] == 2 and not edit_rf_waveform == 19.0:
+        edit_rf_freq_off1 = pfile.hdr.rhi_user20
+        edit_rf_freq_off2 = pfile.hdr.rhi_user21
+        edit_rf_ppm_off1 = edit_rf_freq_off1 / float(pfile.hdr.rhr_rh_ps_mps_freq * 1E-7)
+        edit_rf_ppm_off2 = edit_rf_freq_off2 / float(pfile.hdr.rhr_rh_ps_mps_freq  * 1E-7)
+        edit_rf_dur = pfile.hdr.rhi_user22
+        # check for default value (-1) of pulse length
+        if edit_rf_dur <= 0:
+            edit_rf_dur = 16000
+        dim_info = "MEGA-EDITED j-difference editing, two conditions"
+        dim_header = {"EditCondition": ["ON", "OFF"]}
+        edit_pulse_val = {
+            "ON": {"PulseOffset": edit_rf_ppm_off1, "PulseDuration": edit_rf_dur / 1E6},
+            "OFF": {"PulseOffset": edit_rf_ppm_off2, "PulseDuration": edit_rf_dur / 1E6}}
+
+        meta.set_dim_info(2, 'DIM_EDIT', hdr=dim_header, info=dim_info)
+        meta.set_standard_def("EditPulse", edit_pulse_val)
+    else:
+        meta.set_dim_info(2, 'DIM_EDIT')
+
+
 def _process_gaba(pfile):
-    '''Extract metabolite and reference data from a gaba (MPRESS) format pfile
+    """Extract metabolite and reference data from a gaba (MPRESS) format pfile
 
     :param Pfile pfile: Pfile object
     :return: List numpy data arrays
     :return: List of file name suffixes
-    '''
+    """
 
     # Note that custom mapper sorts dimensions already
     metab = pfile.map.raw_suppressed
     water = pfile.map.raw_unsuppressed
 
     dwelltime = 1 / pfile.hdr.rhr_spectral_width
 
     meta = _populate_metadata(pfile, water_suppressed=True)
     meta_ref = _populate_metadata(pfile, water_suppressed=False)
 
     meta.set_dim_info(0, 'DIM_COIL')
     meta.set_dim_info(1, 'DIM_DYN')
-    meta.set_dim_info(2, 'DIM_EDIT')
+    # Only set an EDIT dim if there is an editing dimension
+    if metab.ndim == 7:
+        _add_editing_info(pfile, meta, metab)
 
     meta_ref.set_dim_info(0, 'DIM_COIL')
     meta_ref.set_dim_info(1, 'DIM_DYN')
-    meta_ref.set_dim_info(2, 'DIM_EDIT')
+    # Only set an EDIT dim if there is an editing dimension
+    if water.ndim == 7:
+        _add_editing_info(pfile, meta_ref, water)
 
     return [metab, water], [meta, meta_ref], dwelltime, ['', '_ref']
 
 
 def _process_mrsi_pfile(pfile):
-    '''Handle MRSI data
+    """Handle MRSI data
 
     :param Pfile pfile: Pfile object
     :return: List of NIFTI MRS data objects
     :return: List of file name suffixes
-    '''
+    """
     psd = pfile.hdr.rhi_psdname.decode('utf-8').lower()
 
     known_formats = ('probe-p', 'probe-sl', 'slaser_cni', 'presscsi')
     if psd not in known_formats:
         raise UnsupportedPulseSequenceError(
             f"Unrecognised sequence {psd}, psdname must be in: {','.join(known_formats)}.")
 
@@ -266,15 +307,15 @@
 
     orientation = NIFTIOrient(_calculate_affine_mrsi(pfile))
 
     return [gen_nifti_mrs_hdr_ext(data, dwelltime, meta, orientation.Q44, no_conj=True), ], ['', ]
 
 
 def _calculate_affine_mrsi(pfile):
-    '''Calculate the 4x4 affine matrix for mrsi'''
+    """Calculate the 4x4 affine matrix for mrsi"""
 
     dcos = pfile.map.get_dcos.T
     dcos[dcos == 0.0] = 0.0             # remove -0.0 values
 
     voxel_size = pfile.map.get_voxel_spacing
     voxel_size_eye = np.diag(voxel_size)
     voi_position = pfile.map.get_origin_from_center(pfile.map.get_select_box_center,
@@ -288,15 +329,15 @@
     affine[:3, 3] = voi_position
     affine[3, 3] = 1.0
 
     return affine
 
 
 def _calculate_affine(pfile):
-    '''Calculate the 4x4 affine matrix'''
+    """Calculate the 4x4 affine matrix"""
 
     dcos = pfile.map.get_dcos.T
     dcos[dcos == 0.0] = 0.0             # remove -0.0 values
 
     voxel_size = pfile.map.get_select_box_size
     voxel_size_eye = np.diag(voxel_size)
     voi_position = pfile.map.get_select_box_center
@@ -317,15 +358,15 @@
     (coil, dyn, indirect) will be included. Otherwise manually specify
     outside this function.
 
     :param pfile: pfile object
     :type pfile: pfile map object
     :param water_suppressed: Set water suppression header field, defaults to True
     :type water_suppressed: bool, optional
-    :param data_dimensions: If set to 5,6, or 7 will inlcude default dim tags for those diemnsions, defaults to None
+    :param data_dimensions: If set to 5,6, or 7 will include default dim tags for those dimensions, defaults to None
     :type data_dimensions: int, optional
     :return: Header extension object
     :rtype: nifti_mrs.hdr_ext
     """
     hdr = pfile.hdr
     spec_frequency = float(pfile.hdr.rhr_rh_ps_mps_freq) / 1e7
```

### Comparing `spec2nii-0.7.3/spec2nii/GE/ge_read_pfile.py` & `spec2nii-0.7.4/spec2nii/GE/ge_read_pfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Reader for GE p-files.
+"""Reader for GE p-files.
 
 This code is taken from the VESPA project https://scion.duhs.duke.edu/vespa/project.
 I therefore include their BSD statement here.
 
     Copyright (c) 2010, Duke University. All rights reserved.
 
     Redistribution and use in source and binary forms, with or without
@@ -56,15 +56,15 @@
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
     ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
     (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
     LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
     ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
     (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
     SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-'''
+"""
 # Python modules
 import math
 import sys
 import csv
 import ctypes
 import ctypes as ct
 from collections import namedtuple
@@ -174,50 +174,50 @@
     def get_mapper(self):
 
         if self.hdr is None:
             return None
 
         psd = self.hdr.rhi_psdname.decode('utf-8').lower()
 
-        if psd in ('probe-p', 'probe-s'):
+        # MM: Some 'gaba' psd strings contain full path names, so truncate to the end of the path
+        if psd.endswith('gaba'):
+            psd = 'gaba'
+
+        numecho = self.hdr.rhi_numecho
+
+        if psd in \
+                (
+                    'probe-p',
+                    'probe-s',
+                    'probe-p_ach',       # MM - added for Calgary PROBE-P sequence
+                    'presscsi',
+                    'fidcsi',            # bjs - added for Pom's fidcsi 13C data
+                    'ia/stable/fidcsi',  # bjs - added for Kearny's 13C data
+                    'presscsi_nfl',      # bjs - added for Govind's SVS data off v25
+                    'epsi_3d_24',        # bjs - added for soher check of MIDAS Browndyke data
+                    'fidall'             # WTC - added for JG's Hyperpolarised 13C data
+                ):
             mapper = PfileMapper
-        elif psd in ('oslaser', 'slaser_cni', 'slaser'):
-            mapper = PfileMapperSlaser
-        elif psd == 'presscsi':
-            mapper = PfileMapper
-        elif psd == 'fidcsi':
-            # bjs - added for Pom's fidcsi 13C data
-            mapper = PfileMapper
-        elif psd == 'ia/stable/fidcsi':
-            # bjs - added for Kearny's 13C data
-            mapper = PfileMapper
-        elif psd == 'presscsi_nfl':
-            # bjs - added for Govind's SVS data off v25
-            mapper = PfileMapper
-        elif psd == 'epsi_3d_24':
-            # bjs - added for soher check of MIDAS Browndyke data
-            mapper = PfileMapper
-        elif psd == 'gaba':
-            # wtc - added for Nottingham MEGA-PRESS sequence.
-            mapper = PfileMapperGaba
-        elif psd == 'hbcd':
-            # ATG - added HBCD - reuse GABA mapper
+        elif psd in ('oslaser', 'slaser_cni', 'slaser') and numecho == 1:
+            mapper = PfileMapperSlaser  # MM: If non-edited data, use PfileMapperSlaser
+        elif psd == 'oslaser' and numecho > 1:
+            mapper = PfileMapperGaba  # MM: If edited data, use PfileMapperGaba
+        elif psd in \
+                (
+                    'jpress',            # wtc - added for J-edited data.
+                    'jpress_ac',         # ARC - added for Bergen jpress patch
+                    'gaba',              # wtc - added for Nottingham MEGA-PRESS sequence
+                    'hbcd',              # ATG - added HBCD - reuse GABA mapper
+                    'probe-p-mega_rml',  # MM - added for Calgary MEGA-PRESS sequence
+                    'repress7'           # MM - added for old CUBRIC data
+                ):
             mapper = PfileMapperGaba
         elif psd == 'probe-sl':
-            # wtc - added for CSI sequence from Manchester.
+            # wtc - added for CSI sequence from Manchester
             mapper = PfileMapperProbeSL
-        elif 'jpress_ac' in psd:
-            # ARC : Added for Bergen jpress patch
-            mapper = PfileMapperGaba
-        elif psd == 'jpress':
-            # wtc - Added for HURCULES data.
-            mapper = PfileMapperGaba
-        elif psd == 'fidall':
-            # WTC - added for JG's Hyperpolarised 13C data
-            mapper = PfileMapper
         else:
             raise UnknownPfile("No Pfile mapper for pulse sequence = %s" % psd)
 
         return mapper
 
     def read_header(self):
 
@@ -307,15 +307,15 @@
 
         rev_little = rev_little.revision
         rev_big    = rev_big.revision
 
         known_revisions = \
             [
                 7, 8, 9, 10, 11,
-                14.0, 14.1, 14.2,
+                14.0, 14.1, 14.2, 14.3,
                 15.000, 15.001, 16.000,
                 20.001, 20.002, 20.003, 20.004, 20.005, 20.006, 20.007,
                 24.000,
                 25.001, 25.002, 25.003, 25.004,
                 26.000, 26.001, 26.002,
                 27.000, 27.001,
                 28.000, 28.002, 28.003,
@@ -707,15 +707,15 @@
         if (math.ceil(nex) * necho) <= 1:
             chop = True
 
         return chop
 
     @property
     def get_frequency_offset(self):
-        """ Returns the spectral frquency offset """
+        """ Returns the spectral frequency offset """
         if self.version > 9:
             return 0.0
         else:
             return self.hdr.rhr_rh_user13
 
     @property
     def get_center_from_raw_file(self):
@@ -821,16 +821,16 @@
 
         return int(nvox[0] * nvox[1] * nvox[2])
 
     @property
     def get_num_kspace_points(self):
         """
         Determine the number of sampled k-space points in the data set.
-        This may differ from the number of voxels in the rectalinear grid,
-        for example if elliptical or another non rectangular acquisition
+        This may differ from the number of voxels in the rectilinear grid,
+        for example if elliptical or another non-rectangular acquisition
         sampling strategy was employed.  GE product sequences pad the
         reduced k-space data with zeros so the number of k-space points
         is the same as the number of voxels, but that may not be true for
         custom sequences.
 
         """
         return int(self.get_num_voxels_in_vol)
@@ -1075,15 +1075,15 @@
                         pFileOffset += numPtsPerSpectrum
 
         filelike.close()
 
         self.raw_data = data
 
         #  Modify the data loading behavior.  For single voxel multi-acq data
-        #  this means return the averaged (suppresssed data, if applicable).
+        #  this means return the averaged (suppressed data, if applicable).
 
         numUnsuppressed = self.get_number_unsuppressed_acquisitions
         numSuppressed   = self.get_number_suppressed_acquisitions
 
         # bjs - changed numTimePoints to >= 1 below due to Pom's fidcsi 13C data
         # bjs - changed numSuppressed to >= 1 below due to oslaser dv26 data
 
@@ -1182,49 +1182,52 @@
         """
         MEGA-PRESS sequence.
         WTC first saw data from Nottingham but it seems general and appears in
         e.g. the Big GABA dataset.
 
         Without some more knowledgeable input I can't currently square the logic
         of BJS's mapper classes with the logic from Gannet/Osprey etc.
-        Therefore this is really a hack that uses the PfileMapper orientation logic
+        Therefore, this is really a hack that uses the PfileMapper orientation logic
         but otherwise uses the logic from Gannet/Osprey.
 
-        Thus most work is done in the overloaded read_data method and functions like
+        Thus, most work is done in the overloaded read_data method and functions like
         get_num_voxels_in_vol are currently meaningless. I would like to square both
         methods in the future.
         """
         PfileMapper.__init__(self, file_name, hdr, version, endian)
 
     def read_data(self):
         """Function that contains all the data loading logic for the 'gaba'
         sequence.
 
-        This is currently  a reimplementation of the Gannert/Osprey GELoad.m
-        function. Therefore the logic is unlike the other mappers.
+        This is currently a reimplementation of the Gannet/Osprey GELoad.m
+        function. Therefore, the logic is unlike the other mappers.
         The suppressed and unsuppressed data can be fetched from the raw_suppressed
         and raw_unsuppressed property.
         """
 
         nechoes = self.hdr.rhr_rh_nechoes
         nex = self.hdr.rhr_rh_navs
         nframes = self.hdr.rhr_rh_nframes
         npoints = self.hdr.rhr_rh_da_xres
         nrows = self.hdr.rhr_rh_da_yres
 
-        dataframes = self.hdr.rhi_user4 / nex
-        refframes = self.hdr.rhi_user19
+        dataframes = self.hdr.rhr_rh_user4 / nex
+        refframes = int(self.hdr.rhr_rh_user19)
 
         nreceivers = self.get_num_coils
-        dataWordSize    = self.hdr.rhr_rh_point_size
+        dataWordSize = self.hdr.rhr_rh_point_size
+
+        # MM: CV24 is a control variable (CV) that defines several advanced options not stored in the other CVs
+        cv24 = self.hdr.rhi_user24
 
         # Check if single voxel
         numVoxels = self.get_num_voxels
         self.is_svs = False
-        if (numVoxels[0] * numVoxels[1] * numVoxels[2] == 1):
+        if numVoxels[0] * numVoxels[1] * numVoxels[2] == 1:
             self.is_svs = True
 
         # Data loading
         # Compute size (in bytes) of data
         data_elements = npoints * 2
         totalframes = nrows * nechoes
         data_elements = data_elements * totalframes * nreceivers
@@ -1242,75 +1245,100 @@
         if self.endian != 'little':
             tempData.byteswap(True)     # swap in-place
 
         tempData = tempData.astype(np.float32)
         tempData = tempData.view(np.complex64)
 
         if nechoes == 1:
-            tempData = tempData.reshape((1, 1, 1, nreceivers, totalframes, npoints))
-            self.raw_data = np.swapaxes(tempData, -1, -3)
-
-            if (dataframes + refframes) != nframes:
+            if int(dataframes + refframes) != nframes:
                 mult = 1
                 dataframes *= nex
                 refframes = int(nframes - dataframes)
             else:
-                mult = 1.0 / nex
+                mult = 1 / nex
 
-            self.raw_unsuppressed = self.raw_data[:, :, :, :, 1:(refframes + 1), :]
-            self.raw_suppressed   = self.raw_data[:, :, :, :, (refframes + 1):, :]
+            tempData = tempData.reshape((1, 1, 1, nreceivers, totalframes, npoints))
+            self.raw_data = np.swapaxes(tempData, -1, -3)
+            self.raw_unsuppressed = self.raw_data[:, :, :, :, 1:(refframes + 1), :] * mult
+            self.raw_suppressed = self.raw_data[:, :, :, :, (refframes + 1):, :] * mult / 2
 
         else:
             if int(dataframes + refframes) != nframes:
                 mult = nex / 2
                 multw = nex
                 noadd = 1
                 dataframes *= nex
                 refframes = nframes - dataframes
             else:
-                mult = nex / 2
+                # MM: Change mult to match latest code in Gannet (2020)
+                # Previous factors:
+                #   mult: 1 (RTN 2017), nex / 2 (RTN 2016)
+                #   multw: 1 / nex (RTN 2017), 1 (RTN 2016)
+                mult = 1 / nex
                 multw = 1
                 noadd = 0
 
             if totalframes != (dataframes + refframes + 1) * nechoes:
                 raise ValueError('# of totalframes not same as (dataframes + refframes + 1) * nechoes')
 
             tempData = tempData.reshape((1, 1, 1, nreceivers, totalframes, npoints))
             self.raw_data = np.swapaxes(tempData, -1, -3)
 
             # Marked as MM (180404) in GELoad.m
             X1, X2 = np.meshgrid(np.arange(refframes), np.arange(nechoes))
             X1 = X1.T.ravel()
             X2 = X2.T.ravel()
-            Y1 = (-1)**(noadd * X1)
+            # Do not apply any phase cycling correction if the receiver phase toggle in sLASER was set
+            if cv24 >= 16384:
+                Y1 = np.ones_like(X1)
+            else:
+                Y1 = (-1) ** (noadd * X1)
             Y1 = np.moveaxis(np.broadcast_to(Y1, (1, 1, 1, npoints, nreceivers, Y1.size)), -1, -2)
             Y2 = (1 + (totalframes / nechoes) * X2 + X1).astype(int)
 
             self.raw_unsuppressed = self.raw_data[:, :, :, :, Y2, :] * Y1 * multw
 
             X1, X2 = np.meshgrid(np.arange(dataframes), np.arange(nechoes))
             X1 = X1.T.ravel()
             X2 = X2.T.ravel()
-            Y1 = (-1)**(noadd * X1)
+            # Do not apply any phase cycling correction if the receiver phase toggle in sLASER was set
+            if cv24 >= 16384:
+                Y1 = np.ones_like(X1)
+            else:
+                Y1 = (-1) ** (noadd * X1)
             Y1 = np.moveaxis(np.broadcast_to(Y1, (1, 1, 1, npoints, nreceivers, Y1.size)), -1, -2)
             Y2 = (1 + refframes + (totalframes / nechoes) * X2 + X1).astype(int)
 
             self.raw_suppressed = self.raw_data[:, :, :, :, Y2, :] * Y1 * mult
 
+        # Test if this is the case of the jpress like sequence being used for a non-editing condition
+        edit_waveform = self.hdr.rhi_user19
+        if nechoes == 1 and edit_waveform == 0:
+            # Editing conditions = 1 and there is no editing waveform
+            self.raw_suppressed[:, :, :, :, 0::2, :] *= np.exp(1j * np.pi)
+            self.raw_unsuppressed[:, :, :, :, 0::2, :] *= np.exp(1j * np.pi)
+
+            # Rearrange axes to (x, y, z, t, coils, dynamics)
+            self.raw_suppressed = np.moveaxis(self.raw_suppressed, (4, 5), (5, 4))
+            self.raw_unsuppressed = np.moveaxis(self.raw_unsuppressed, (4, 5), (5, 4))
+        else:
+            # Editing condition, update nechoes if needed for special cases like probe-p-mega_rml
+            if nechoes == 1:
+                nechoes = 2
+
             # Up to this point we have simply replicated the logic of the GELoad function.
-            # Now reorganise dimensions to give a editing dimension.
+            # Now reorganise dimensions to give an editing dimension.
             # This means that this is done in a not particularly clear order, but it enables testing against
             # the matlab code.
-
             reorg_suppressed = []
             reorg_unsuppressed = []
             for ne in range(nechoes):
                 reorg_suppressed.append(self.raw_suppressed[:, :, :, :, ne::nechoes, :])
                 reorg_unsuppressed.append(self.raw_unsuppressed[:, :, :, :, ne::nechoes, :])
 
             reorg_suppressed = np.stack(reorg_suppressed, axis=-1)
-            # Rearange axes to (x, y, z, t, coils, dynamics, edit)
+            # Rearrange axes to (x, y, z, t, coils, dynamics, edit)
             self.raw_suppressed = np.moveaxis(reorg_suppressed, (4, 5), (5, 4))
 
             reorg_unsuppressed = np.stack(reorg_unsuppressed, axis=-1)
-            # Rearange axes to (x, y, z, t, coils, dynamics, edit)
+            # Rearrange axes to (x, y, z, t, coils, dynamics, edit)
             self.raw_unsuppressed = np.moveaxis(reorg_unsuppressed, (4, 5), (5, 4))
```

### Comparing `spec2nii-0.7.3/spec2nii/GSL/gslfunctions.py` & `spec2nii-0.7.4/spec2nii/GSL/gslfunctions.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/Philips/philips.py` & `spec2nii-0.7.4/spec2nii/Philips/philips.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/Philips/philips_data_list.py` & `spec2nii-0.7.4/spec2nii/Philips/philips_data_list.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/Philips/philips_dcm.py` & `spec2nii-0.7.4/spec2nii/Philips/philips_dcm.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/Siemens/dicomfunctions.py` & `spec2nii-0.7.4/spec2nii/Siemens/dicomfunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -715,29 +715,61 @@
 
     fullcsa = csar.get_csa_header(img.dcm_data, csa_type='series')
     xprot = parse_buffer(fullcsa['tags']['MrPhoenixProtocol']['items'][0])
 
     # Handle CMRR DKD sequence
     # https://www.cmrr.umn.edu/spectro/
     # SEMI-LASER (MRM 2011, NMB 2019) Release 2016-12
+    # Three cases as explained by DKD.
+    '''
+    dkd_slaserVOI_dkd
+        ScanMode = 8
+        (NOTE DKD originally said 2, but from testing the sLASER_VE11C_Sept2016 version 8 is the only option
+        xprot[('sSpecPara', 'lAutoRefScanMode')] = 1 when set to 'off' and 8 when set to 'on')
+            4 water ref at start and 4 at the end where the first 2 water ref in
+            each are acquired with VAPOR RF off but OVS on while last 2 ref are with VAPOR and OVS completely off.
+
+    dkd_slaserVOI_dkd2
+        ScanMode =8
+            does the same as ScanMode =8 above
+
+        ScanMode =2 with ScanNo=2
+            this means 2 water ref at start and 2 at end;
+            this acq is done with VAPOR and OVS RF off, but all gradients still ON.
+    '''
     seq_file_name = xprot[('tSequenceFileName',)].strip('"').lower()
-    match = re.search(r'svs_slaservoi_dkd', seq_file_name)
-    if match and xprot[('sSpecPara', 'lAutoRefScanMode')] == 8.0:
+    if (re.search(r'svs_slaser(voi)?_dkd2$', seq_file_name)
+        and xprot[('sSpecPara', 'lAutoRefScanMode')] == 8.0)\
+        or (re.search(r'svs_slaser(voi)?_dkd$', seq_file_name)
+            and xprot[('sSpecPara', 'lAutoRefScanMode')] == 8.0):
         num_ref = int(xprot[('sSpecPara', 'lAutoRefScanNo')])
         num_dyn = int(xprot[('lAverages',)])
         total_dyn = num_dyn + (num_ref * 4)
         if inst_num <= num_ref:
             # First ecc calibration references
-            return 1, '_ecc'
+            return 1, '_rf_off'
         elif inst_num <= (num_ref * 2):
             # First quantitation calibration references
-            return 2, '_quant'
+            return 2, '_rf_grads_ovs_off'
         elif (total_dyn - (2 * num_ref)) < inst_num <= (total_dyn - num_ref):
             # Second ecc calibration references
-            return 1, '_ecc'
+            return 1, '_rf_off'
         elif (total_dyn - num_ref) < inst_num <= total_dyn:
             # Second quantitation calibration references
-            return 2, '_quant'
+            return 2, '_rf_grads_ovs_off'
+        else:
+            return 0, ''
+    elif (re.search(r'svs_slaser(voi)?_dkd2', seq_file_name)
+            and xprot[('sSpecPara', 'lAutoRefScanMode')] == 2.0):
+        num_ref = int(xprot[('sSpecPara', 'lAutoRefScanNo')])
+        num_dyn = int(xprot[('lAverages',)])
+        total_dyn = num_dyn + (num_ref * 2)
+        if inst_num < num_ref:
+            # First WS and OVS RF off
+            return 1, '_vapor_ovs_rfoff'
+        elif inst_num >= (total_dyn - num_ref):
+            # SecondWS and OVS RF off
+            return 1, '_vapor_ovs_rfoff'
         else:
             return 0, ''
     else:
         return 0, ''
```

### Comparing `spec2nii-0.7.3/spec2nii/Siemens/rda.py` & `spec2nii-0.7.4/spec2nii/Siemens/rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/Siemens/twixfunctions.py` & `spec2nii-0.7.4/spec2nii/Siemens/twixfunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -301,29 +301,29 @@
         xa_ref_scans = xa_ref_scans[:, ~xa_zero_index]\
             .reshape(xa_ref_scans.shape[0], xa_ref_scans.shape[1], -1)
     else:
         xa_ref_scans = None
 
     # AG 03/22/2023 Moved the NIFTI/Out lists and if statement up to work with new Hyper function below.
     # AG 03/22/2023 Create Lists for assembled data - Starts with XA reference..
-    nifit_mrs_out = []
+    nifti_mrs_out = []
     filename_out  = []
 
     if xa_ref_scans is not None:
         # Pad with three singleton dimensions (x,y,z)
         newshape = (1, 1, 1) + xa_ref_scans.shape
         if xa_ref_scans.ndim > 2:
             ref_tags = ['DIM_COIL', 'DIM_DYN', None]
         else:
             ref_tags = ['DIM_COIL', None, None]
 
         meta_obj_ref = extractTwixMetadata(twixObj['hdr'], basename(twixObj[dataKey].filename))
         meta_obj_ref.set_standard_def('WaterSuppressed', True)
 
-        nifit_mrs_out.append(
+        nifti_mrs_out.append(
             assemble_nifti_mrs(
                 xa_ref_scans.reshape(newshape),
                 dwellTime,
                 orientation,
                 meta_obj_ref,
                 dim_tags=ref_tags))
 
@@ -391,66 +391,84 @@
                                                                    meta_obj,
                                                                    dim_tags,
                                                                    subseq=ii,
                                                                    subseq_name=hyp_names[ii])
 
             if reord_data_.ndim <= 4:                                                       # 4 or less Dims
                 newshape  = (1, 1, 1) + reord_data_.shape                                   # Pad 3 singleton dims
-                nifit_mrs_out.append(assemble_nifti_mrs(reord_data_.reshape(newshape),
+                nifti_mrs_out.append(assemble_nifti_mrs(reord_data_.reshape(newshape),
                                                         dwellTime,
                                                         orientation,
                                                         meta_obj_))
                 filename_out.append(f'{mainStr}_{hyp_suffix[ii]}')
 
-        return nifit_mrs_out, filename_out
+        return nifti_mrs_out, filename_out
 
     # HERCULES Data
     elif (xa_or_vx(twixObj['hdr']) == 'xa' and 'smm_svs_herc' in twixObj['hdr']['Meas'][('tSequenceFileName')]):
         from spec2nii.Siemens.twix_special_case import mgs_svs_ed_twix
         reord_data, meta_obj, dim_tags = mgs_svs_ed_twix(twixObj, reord_data, meta_obj, dim_tags)
 
+    elif re.search(
+            r'svs_slaser(voi)?_dkd',
+            twixObj['hdr']['Meas'][('tSequenceFileName')],
+            re.IGNORECASE):
+        from spec2nii.Siemens.twix_special_case import slaser_dkd
+        for data, meta, name in slaser_dkd(twixObj, reord_data, meta_obj, dim_tags):
+
+            nifti_mrs_out.append(
+                gen_nifti_mrs_hdr_ext(
+                    data,
+                    dwellTime,
+                    meta,
+                    orientation.Q44,
+                    no_conj=True))
+
+            filename_out.append(f'{mainStr}{name}')
+
+        return nifti_mrs_out, filename_out
     else:
         # Set dim tags in meta now as no additional info
         for idx, dt in enumerate(dim_tags):
             meta_obj.set_dim_info(idx, dt)
 
     if reord_data.ndim <= 4:
         # Pad with three singleton dimensions (x,y,z)
         newshape = (1, 1, 1) + reord_data.shape
 
-        nifit_mrs_out.append(assemble_nifti_mrs(reord_data.reshape(newshape),
+        nifti_mrs_out.append(assemble_nifti_mrs(reord_data.reshape(newshape),
                                                 dwellTime,
                                                 orientation,
                                                 meta_obj))
 
         filename_out.append(mainStr)
 
     else:
         # loop over any dimensions over 4
         for index in np.ndindex(reord_data.shape[4:]):
             modIndex = (slice(None), slice(None), slice(None), slice(None)) + index
 
             # Pad with three singleton dimensions (x,y,z)
             newshape = (1, 1, 1) + reord_data[modIndex].shape
 
-            nifit_mrs_out.append(
+            nifti_mrs_out.append(
                 assemble_nifti_mrs(reord_data[modIndex].reshape(newshape),
                                    dwellTime,
                                    orientation,
                                    meta_obj))
 
             # Create strings
             out_name = f'{mainStr}'
             for idx, ii in enumerate(index):
                 indexStr = dim_order[3 + idx]
                 out_name += f'_{indexStr}{ii :03d}'
 
             filename_out.append(out_name)
 
-    return nifit_mrs_out, filename_out
+    return nifti_mrs_out, filename_out
 
 
 def process_fid(twixObj, base_name_out, name_in, dataKey, dim_overrides, remove_os, quiet=False, verbose=False):
     """Process a twix file into a NIfTI MRS file.
     Inputs:
         twixObj: object from mapVBVD.
         base_name_out: Core string of output file.
@@ -576,21 +594,21 @@
 
     # Permute the order of dimension in the data
     original = list(range(1, squeezedData.ndim))
     new = [twixObj[dataKey].sqzDims.index(dd) for dd in dim_order]
     reord_data = np.moveaxis(squeezedData, original, new)
 
     # Now assemble data
-    nifit_mrs_out = []
+    nifti_mrs_out = []
     filename_out = []
     if reord_data.ndim <= 4:
         # Pad with three singleton dimensions (x,y,z)
         newshape = (1, 1, 1) + reord_data.shape
 
-        nifit_mrs_out.append(assemble_nifti_mrs(reord_data.reshape(newshape),
+        nifti_mrs_out.append(assemble_nifti_mrs(reord_data.reshape(newshape),
                                                 dwellTime,
                                                 orientation,
                                                 meta_obj,
                                                 dim_tags))
 
         filename_out.append(mainStr)
 
@@ -598,15 +616,15 @@
         # loop over any dimensions over 4
         for index in np.ndindex(reord_data.shape[4:]):
             modIndex = (slice(None), slice(None), slice(None), slice(None)) + index
 
             # Pad with three singleton dimensions (x,y,z)
             newshape = (1, 1, 1) + reord_data[modIndex].shape
 
-            nifit_mrs_out.append(
+            nifti_mrs_out.append(
                 assemble_nifti_mrs(reord_data[modIndex].reshape(newshape),
                                    dwellTime,
                                    orientation,
                                    meta_obj,
                                    dim_tags))
 
             # Create strings
@@ -624,25 +642,25 @@
             ref_tags = ['DIM_COIL', 'DIM_DYN', None]
         else:
             ref_tags = ['DIM_COIL', None, None]
 
         meta_obj_ref = extractTwixMetadata(twixObj['hdr'], basename(twixObj[dataKey].filename))
         meta_obj_ref.set_standard_def('WaterSuppressed', True)
 
-        nifit_mrs_out.append(
+        nifti_mrs_out.append(
             assemble_nifti_mrs(
                 xa_ref_scans.reshape(newshape),
                 dwellTime,
                 orientation,
                 meta_obj_ref,
                 ref_tags))
 
         filename_out.append(mainStr + '_ref')
 
-    return nifit_mrs_out, filename_out
+    return nifti_mrs_out, filename_out
 
 
 def assemble_nifti_mrs(data, dwellTime, orientation, meta_obj, dim_tags=None):
 
     if dim_tags is not None:
         for idx, dt in zip(range(data.ndim - 4), dim_tags):
             meta_obj.set_dim_info(idx, dt)
@@ -876,15 +894,25 @@
         tmpSqzDims = ', '.join(twixObj[ev].sqzDims)
         print(f'{ev: <15}:\t{tmpSqzDims: <20}\t{tmpSqzSize}')
 
 
 def extractTwixMetadata(mapVBVDHdr, original_file):
     """Pass to appropriate extractTwixMetadata function for software version."""
     if xa_or_vx(mapVBVDHdr) == 'vx':
-        return extractTwixMetadata_vx(mapVBVDHdr, original_file)
+        try:
+            return extractTwixMetadata_vx(mapVBVDHdr, original_file)
+        except KeyError as original_err:
+            try:
+                print(f'VX-line scanner headers caused KeyError {original_err}.')
+                print('Trying XA interpreter. ')
+                return extractTwixMetadata_xa(mapVBVDHdr, original_file)
+            except Exception as backup_err:
+                print(f'XA interpreter failed with reason {backup_err}. Raising original error.')
+                raise original_err
+
     elif xa_or_vx(mapVBVDHdr) == 'xa':
         return extractTwixMetadata_xa(mapVBVDHdr, original_file)
 
 
 def extractTwixMetadata_xa(mapVBVDHdr, original_file):
     """ Extract information from the pymapVBVD header to insert into the json sidecar.
```

### Comparing `spec2nii-0.7.3/spec2nii/anonymise.py` & `spec2nii-0.7.4/spec2nii/anonymise.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/bruker.py` & `spec2nii-0.7.4/spec2nii/bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/bruker_fid_override.json` & `spec2nii-0.7.4/spec2nii/bruker_fid_override.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/bruker_properties.json` & `spec2nii-0.7.4/spec2nii/bruker_properties.json`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/dcm2niiOrientation/orientationFuncs.py` & `spec2nii-0.7.4/spec2nii/dcm2niiOrientation/orientationFuncs.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/due.py` & `spec2nii-0.7.4/spec2nii/due.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/fileiobase.py` & `spec2nii-0.7.4/spec2nii/fileiobase.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/jmrui.py` & `spec2nii-0.7.4/spec2nii/jmrui.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     -------
     array-like
         Complex data
     dict
         Header information
 
     """
-    signalRe = re.compile(r'Signal (\d{1,}) out of (\d{1,}) in file')
+    signalRe = re.compile(r'Signal (?:number: |)(\d{1,}) out of (\d{1,}) in file')
     headerRe = re.compile(r'(\w*):(.*)')
     header = {}
     data   = []
     recordData = False
     signal_index = 0
     with open(filename, 'r') as txtfile:
         for line in txtfile:
```

### Comparing `spec2nii-0.7.3/spec2nii/nifti_orientation.py` & `spec2nii-0.7.4/spec2nii/nifti_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/other.py` & `spec2nii-0.7.4/spec2nii/other.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/other_formats.py` & `spec2nii-0.7.4/spec2nii/other_formats.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/spec2nii.py` & `spec2nii-0.7.4/spec2nii/spec2nii.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,21 @@
         parser_twix.add_argument('--remove_os', action='store_true', help='Remove time-domain oversampling.')
         parser_twix = add_common_parameters(parser_twix)
         parser_twix.set_defaults(func=self.twix)
 
         # Handle dicom subcommand
         parser_dicom = subparsers.add_parser('dicom', help='Convert from Siemens DICOM format.')
         parser_dicom.add_argument('file', help='file or directory to convert', type=str)
-        parser_dicom.add_argument("-t", "--tag", type=str, help="Specify NIfTI MRS tag used for 5th "
-                                                                "dimension if multiple files are passed.")
+        parser_dicom.add_argument(
+            "-t",
+            "--tag",
+            type=str,
+            default='DIM_DYN',
+            help="Specify NIfTI MRS tag used for 5th dimension if multiple files are passed. "
+                 "Defaults to DIM_DYN.")
         parser_dicom.add_argument('--voi', action='store_true', help='Output VOI as single voxel NIfTI mask.')
         parser_dicom = add_common_parameters(parser_dicom)
         parser_dicom.set_defaults(func=self.dicom)
 
         # Handle rda subcommand
         parser_rda = subparsers.add_parser('rda', help='Convert from Siemens spectroscopy .rda format.')
         parser_rda.add_argument('file', help='file to convert', type=Path)
```

### Comparing `spec2nii-0.7.3/spec2nii/uih.py` & `spec2nii-0.7.4/spec2nii/uih.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/varian.py` & `spec2nii-0.7.4/spec2nii/varian.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii/varian_importer.py` & `spec2nii-0.7.4/spec2nii/varian_importer.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/spec2nii.egg-info/PKG-INFO` & `spec2nii-0.7.4/spec2nii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec2nii
-Version: 0.7.3
+Version: 0.7.4
 Summary: Multi-format in vivo MR spectroscopy conversion to NIFTI
 Home-page: https://github.com/wtclarke/spec2nii
 Author: Will Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `spec2nii-0.7.3/spec2nii.egg-info/SOURCES.txt` & `spec2nii-0.7.4/spec2nii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_anon.py` & `spec2nii-0.7.4/tests/test_anon.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_auto.py` & `spec2nii-0.7.4/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_bruker.py` & `spec2nii-0.7.4/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_ge_pfile.py` & `spec2nii-0.7.4/tests/test_uih.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,86 @@
-'''Tests for GE pfile format conversion.
+'''Tests for UIH dicom format conversion.
 
 Copyright William Clarke, University of Oxford 2021
 Subject to the BSD 3-Clause License.
 '''
 
 import subprocess
 from pathlib import Path
 import json
 
 import numpy as np
 
 from .io_for_tests import read_nifti_mrs
 
 # Data paths
-ge_path = Path(__file__).parent / 'spec2nii_test_data' / 'ge'
-svs_path = ge_path / 'pFiles' / 'svMRS' / 'P03072.7'
-mrsi_path = ge_path / 'pFiles' / 'MRSI' / 'P18432.7'
-mpress_path = ge_path / 'pFiles' / 'big_gaba' / 'S01_GABA_68.7'
+data_base = Path(__file__).parent / 'spec2nii_test_data' / 'UIH'
+
+data_paths = {'svs': data_base / 'mrs_data/dicom/svs_press_te144_SVS_801/00000001.dcm',
+              'csi_2d': data_base / 'mrs_data/dicom/csi_hise_te144_CSI_1201/00000000.dcm',
+              'csi_3d': data_base / 'mrs_3d/dicom/csi_hise_3d_te144_CSI_1301/00000000.dcm'}
 
 
 def test_svs(tmp_path):
 
-    subprocess.check_call(['spec2nii', 'ge',
+    subprocess.check_call(['spec2nii', 'uih',
                            '-f', 'svs',
                            '-o', tmp_path,
                            '-j',
-                           str(svs_path)])
-
-    img = read_nifti_mrs(tmp_path / 'svs.nii.gz')
-    img_ref = read_nifti_mrs(tmp_path / 'svs_ref.nii.gz')
+                           str(data_paths['svs'])])
 
-    assert img.shape == (1, 1, 1, 4096, 32, 2)
-    assert np.iscomplexobj(img.dataobj)
-    assert 1 / img.header['pixdim'][4] == 5000.0
+    img_t = read_nifti_mrs(tmp_path / 'svs.nii.gz')
 
-    assert img_ref.shape == (1, 1, 1, 4096, 32, 2)
-    assert np.iscomplexobj(img_ref.dataobj)
-    assert 1 / img_ref.header['pixdim'][4] == 5000.0
+    assert img_t.shape == (1, 1, 1, 2048)
+    assert np.iscomplexobj(img_t.dataobj)
+    assert 1 / img_t.header['pixdim'][4] == 2000.0
 
-    hdr_ext_codes = img.header.extensions.get_codes()
-    hdr_ext = json.loads(img.header.extensions[hdr_ext_codes.index(44)].get_content())
+    hdr_ext_codes = img_t.header.extensions.get_codes()
+    hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
 
-    assert hdr_ext['dim_5'] == 'DIM_COIL'
-    assert hdr_ext['dim_6'] == 'DIM_DYN'
-    assert hdr_ext['SpectrometerFrequency'][0] == 127.76365
+    assert hdr_ext['SpectrometerFrequency'][0] == 128.207081
     assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == svs_path.name
-
-    assert np.isclose(hdr_ext['EchoTime'], 0.27)
-    assert np.isclose(hdr_ext['RepetitionTime'], 2.0)
+    assert hdr_ext['OriginalFile'][0] == data_paths['svs'].name
 
 
-def test_mrsi(tmp_path):
+def test_2D(tmp_path):
 
-    subprocess.check_call(['spec2nii', 'ge',
-                           '-f', 'mrsi',
+    subprocess.check_call(['spec2nii', 'uih',
+                           '-f', 'csi_2d',
                            '-o', tmp_path,
                            '-j',
-                           str(mrsi_path)])
+                           str(data_paths['csi_2d'])])
 
-    img = read_nifti_mrs(tmp_path / 'mrsi.nii.gz')
+    img_t = read_nifti_mrs(tmp_path / 'csi_2d.nii.gz')
 
-    assert img.shape == (8, 8, 1, 1024, 32)
-    assert np.iscomplexobj(img.dataobj)
-    assert 1 / img.header['pixdim'][4] == 4000.0
+    assert img_t.shape == (16, 16, 1, 2048)
+    assert np.iscomplexobj(img_t.dataobj)
+    assert 1 / img_t.header['pixdim'][4] == 2000.0
 
-    hdr_ext_codes = img.header.extensions.get_codes()
-    hdr_ext = json.loads(img.header.extensions[hdr_ext_codes.index(44)].get_content())
+    hdr_ext_codes = img_t.header.extensions.get_codes()
+    hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
 
-    assert hdr_ext['SpectrometerFrequency'][0] == 127.763607
+    assert hdr_ext['SpectrometerFrequency'][0] == 128.207084
     assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == mrsi_path.name
+    assert hdr_ext['OriginalFile'][0] == data_paths['csi_2d'].name
 
 
-def test_mpress(tmp_path):
+def test_3D(tmp_path):
 
-    subprocess.check_call(['spec2nii', 'ge',
-                           '-f', 'mpress',
+    subprocess.check_call(['spec2nii', 'uih',
+                           '-f', 'csi_3d',
                            '-o', tmp_path,
                            '-j',
-                           str(mpress_path)])
+                           str(data_paths['csi_3d'])])
 
-    img = read_nifti_mrs(tmp_path / 'mpress.nii.gz')
-    img_ref = read_nifti_mrs(tmp_path / 'mpress_ref.nii.gz')
+    img_t = read_nifti_mrs(tmp_path / 'csi_3d.nii.gz')
 
-    assert img.shape == (1, 1, 1, 2048, 8, 160, 2)
-    assert np.iscomplexobj(img.dataobj)
-    assert 1 / img.header['pixdim'][4] == 2000.0
-
-    assert img_ref.shape == (1, 1, 1, 2048, 8, 8, 2)
-    assert np.iscomplexobj(img_ref.dataobj)
-    assert 1 / img_ref.header['pixdim'][4] == 2000.0
-
-    hdr_ext_codes = img.header.extensions.get_codes()
-    hdr_ext = json.loads(img.header.extensions[hdr_ext_codes.index(44)].get_content())
-
-    assert hdr_ext['dim_5'] == 'DIM_COIL'
-    assert hdr_ext['dim_6'] == 'DIM_DYN'
-    assert hdr_ext['dim_7'] == 'DIM_EDIT'
-    assert hdr_ext['SpectrometerFrequency'][0] == 127.758139
-    assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == mpress_path.name
+    assert img_t.shape == (8, 8, 8, 1024)
+    assert np.iscomplexobj(img_t.dataobj)
+    assert 1 / img_t.header['pixdim'][4] == 2000.0
+
+    hdr_ext_codes = img_t.header.extensions.get_codes()
+    hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
 
-    assert np.isclose(hdr_ext['EchoTime'], 0.068)
-    assert np.isclose(hdr_ext['RepetitionTime'], 2.0)
+    assert hdr_ext['SpectrometerFrequency'][0] == 128.207089
+    assert hdr_ext['ResonantNucleus'][0] == '1H'
+    assert hdr_ext['OriginalFile'][0] == data_paths['csi_3d'].name
```

### Comparing `spec2nii-0.7.3/tests/test_ge_pfile_orientation.py` & `spec2nii-0.7.4/tests/test_ge_pfile_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_jmrui.py` & `spec2nii-0.7.4/tests/test_jmrui.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import os.path as op
 import nibabel as nib
 
 file_path = Path(__file__).parent
 testdata = {'fida_single': file_path / 'spec2nii_test_data/jmrui/metab_jmrui.txt',
             'txt_multi': file_path / 'spec2nii_test_data/jmrui/basis_woTMS.txt',
             'mrui_single': file_path / 'spec2nii_test_data/jmrui/press2.mrui',
-            'mrui_multi': file_path / 'spec2nii_test_data/jmrui/ALLSIG.mrui'}
+            'mrui_multi': file_path / 'spec2nii_test_data/jmrui/ALLSIG.mrui',
+            'txt_old': file_path / 'spec2nii_test_data/jmrui/P31rest_proc_jmrui.txt'}
 
 
 @pytest.fixture
 def affine_file(tmp_path):
 
     affinepath = op.join(tmp_path, 'affine.txt')
 
@@ -102,7 +103,26 @@
 
     # Load the new nifti file
     converted = nib.load(tmp_path / 'mrui_multi.nii.gz')
 
     assert converted.shape == (1, 1, 1, 2048, 28)
     assert np.iscomplexobj(converted.dataobj)
     assert np.allclose(np.loadtxt(affine_file), converted.affine)
+
+
+def test_jmrui_old(affine_file, tmp_path):
+    """Test the 'jmrui' txt old format with different # signal syntax.
+    Namely, 'Signal number: ' rather than 'Signal')
+    """
+    # Run spec2nii on text
+    subprocess.call(['spec2nii', 'jmrui',
+                     '-f', 'txt_old',
+                     '-o', str(tmp_path),
+                     '-a', affine_file,
+                     '-j', testdata['txt_old']])
+
+    # Load the new nifti file
+    converted = nib.load(tmp_path / 'txt_old.nii.gz')
+
+    assert converted.shape == (1, 1, 1, 2048)
+    assert np.iscomplexobj(converted.dataobj)
+    assert np.allclose(np.loadtxt(affine_file), converted.affine)
```

### Comparing `spec2nii-0.7.3/tests/test_nifti_options.py` & `spec2nii-0.7.4/tests/test_nifti_options.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_other.py` & `spec2nii-0.7.4/tests/test_other.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_other_func.py` & `spec2nii-0.7.4/tests/test_other_func.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_data_list.py` & `spec2nii-0.7.4/tests/test_philips_data_list.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_dicom.py` & `spec2nii-0.7.4/tests/test_philips_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_dicom_orientation.py` & `spec2nii-0.7.4/tests/test_philips_dicom_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_orientation_dcm_spar_new.py` & `spec2nii-0.7.4/tests/test_philips_orientation_dcm_spar_new.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_sdat_spar.py` & `spec2nii-0.7.4/tests/test_philips_sdat_spar.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_philips_sdat_spar_orientation.py` & `spec2nii-0.7.4/tests/test_philips_sdat_spar_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_siemens_dicom.py` & `spec2nii-0.7.4/tests/test_siemens_dicom.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_siemens_mrsi_orientation.py` & `spec2nii-0.7.4/tests/test_siemens_mrsi_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_siemens_rda.py` & `spec2nii-0.7.4/tests/test_siemens_rda.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_siemens_svs_orientation.py` & `spec2nii-0.7.4/tests/test_siemens_svs_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_siemens_twix.py` & `spec2nii-0.7.4/tests/test_siemens_twix.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_spectralwidth.py` & `spec2nii-0.7.4/tests/test_spectralwidth.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/tests/test_uih.py` & `spec2nii-0.7.4/tests/test_varian.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,44 @@
-'''Tests for UIH dicom format conversion.
+'''Tests for Varian format conversion.
 
-Copyright William Clarke, University of Oxford 2021
+Copyright Jack Miller, University of Oxford and University of Aarhus, 2021
 Subject to the BSD 3-Clause License.
 '''
 
 import subprocess
 from pathlib import Path
 import json
 
 import numpy as np
 
 from .io_for_tests import read_nifti_mrs
 
 # Data paths
-data_base = Path(__file__).parent / 'spec2nii_test_data' / 'UIH'
-
-data_paths = {'svs': data_base / 'mrs_data/dicom/svs_press_te144_SVS_801/00000001.dcm',
-              'csi_2d': data_base / 'mrs_data/dicom/csi_hise_te144_CSI_1201/00000000.dcm',
-              'csi_3d': data_base / 'mrs_3d/dicom/csi_hise_3d_te144_CSI_1301/00000000.dcm'}
+varian_path = Path(__file__).parent / 'spec2nii_test_data' / 'varian'
+data_path = varian_path / '13C_spuls_01.fid'
 
 
 def test_svs(tmp_path):
 
-    subprocess.check_call(['spec2nii', 'uih',
+    subprocess.check_call(['spec2nii', 'varian',
                            '-f', 'svs',
                            '-o', tmp_path,
                            '-j',
-                           str(data_paths['svs'])])
+                           '-d',
+                           '-t', 'DIM_USER_0',
+                           str(data_path)])
 
     img_t = read_nifti_mrs(tmp_path / 'svs.nii.gz')
 
-    assert img_t.shape == (1, 1, 1, 2048)
-    assert np.iscomplexobj(img_t.dataobj)
-    assert 1 / img_t.header['pixdim'][4] == 2000.0
-
-    hdr_ext_codes = img_t.header.extensions.get_codes()
-    hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
-
-    assert hdr_ext['SpectrometerFrequency'][0] == 128.207081
-    assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == data_paths['svs'].name
-
-
-def test_2D(tmp_path):
-
-    subprocess.check_call(['spec2nii', 'uih',
-                           '-f', 'csi_2d',
-                           '-o', tmp_path,
-                           '-j',
-                           str(data_paths['csi_2d'])])
-
-    img_t = read_nifti_mrs(tmp_path / 'csi_2d.nii.gz')
-
-    assert img_t.shape == (16, 16, 1, 2048)
-    assert np.iscomplexobj(img_t.dataobj)
-    assert 1 / img_t.header['pixdim'][4] == 2000.0
-
-    hdr_ext_codes = img_t.header.extensions.get_codes()
-    hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
-
-    assert hdr_ext['SpectrometerFrequency'][0] == 128.207084
-    assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == data_paths['csi_2d'].name
-
-
-def test_3D(tmp_path):
-
-    subprocess.check_call(['spec2nii', 'uih',
-                           '-f', 'csi_3d',
-                           '-o', tmp_path,
-                           '-j',
-                           str(data_paths['csi_3d'])])
-
-    img_t = read_nifti_mrs(tmp_path / 'csi_3d.nii.gz')
-
-    assert img_t.shape == (8, 8, 8, 1024)
+    assert img_t.shape == (1, 1, 1, 2048, 1, 80)
     assert np.iscomplexobj(img_t.dataobj)
-    assert 1 / img_t.header['pixdim'][4] == 2000.0
+    assert np.isclose(1 / img_t.header['pixdim'][4], 40323, atol=2)
 
     hdr_ext_codes = img_t.header.extensions.get_codes()
     hdr_ext = json.loads(img_t.header.extensions[hdr_ext_codes.index(44)].get_content())
 
-    assert hdr_ext['SpectrometerFrequency'][0] == 128.207089
-    assert hdr_ext['ResonantNucleus'][0] == '1H'
-    assert hdr_ext['OriginalFile'][0] == data_paths['csi_3d'].name
+    assert hdr_ext['SpectrometerFrequency'][0] == 100.4451626
+    assert hdr_ext['ResonantNucleus'][0] == "13C"
+    assert hdr_ext['OriginalFile'][0] == data_path.name
+    assert 'VarianProcpar' in hdr_ext
+    assert hdr_ext['dim_5'] == 'DIM_COIL'
+    assert hdr_ext['dim_6'] == 'DIM_USER_0'
```

### Comparing `spec2nii-0.7.3/tests/test_uih_orientation.py` & `spec2nii-0.7.4/tests/test_uih_orientation.py`

 * *Files identical despite different names*

### Comparing `spec2nii-0.7.3/versioneer.py` & `spec2nii-0.7.4/versioneer.py`

 * *Files identical despite different names*

