# Comparing `tmp/atlas-densities-0.2.3.tar.gz` & `tmp/atlas-densities-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-densities-0.2.3.tar", last modified: Thu Feb  8 07:49:28 2024, max compression
+gzip compressed data, was "atlas-densities-0.2.4.tar", last modified: Thu Apr 18 12:15:18 2024, max compression
```

## Comparing `atlas-densities-0.2.3.tar` & `atlas-densities-0.2.4.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.494844 atlas-densities-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.498844 atlas-densities-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.498844 atlas-densities-0.2.3/atlas_densities/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.502844 atlas-densities-0.2.3/atlas_densities/app/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43412 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.502844 atlas-densities-0.2.3/atlas_densities/app/data/
--rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.506844 atlas-densities-0.2.3/atlas_densities/app/data/markers/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/markers/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/markers/realigned_slices_bbp.json
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.506844 atlas-densities-0.2.3/atlas_densities/app/data/measurements/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/gaba_papers.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/homogenous_regions.csv
--rw-r--r--   0 runner    (1001) docker     (127)   839727 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/measurements.csv
--rw-r--r--   0 runner    (1001) docker     (127)   347207 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/mmc1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)   291827 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/mmc3.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/non_density_measurements.csv
--rw-r--r--   0 runner    (1001) docker     (127)   199258 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/measurements/std_cells.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.510844 atlas-densities-0.2.3/atlas_densities/app/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/ca1_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/group_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/isocortex_23_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/isocortex_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/metadata/thalamus_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.510844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.510844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/composition.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.510844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.510844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.514844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.514844 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/probability_map/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/probability_map/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)   930916 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.518844 atlas-densities-0.2.3/atlas_densities/combination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/combination/annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/combination/markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.522844 atlas-densities-0.2.3/atlas_densities/densities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/cell_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    26599 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    29885 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36094 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_composition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.522844 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/refined_inhibitory_neuron_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/atlas_densities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.502844 atlas-densities-0.2.3/atlas_densities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-08 07:49:28.000000 atlas-densities-0.2.3/atlas_densities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.522844 atlas-densities-0.2.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.522844 atlas-densities-0.2.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)   230179 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/bbpp82_628_linear_program.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/cell_densities.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/combination.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/mtype_densities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.522844 atlas-densities-0.2.3/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (127)    55115 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/doc/source/static/atlas-densities.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.526844 atlas-densities-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/1.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.526844 atlas-densities-0.2.3/tests/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/app/test_cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/app/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/app/test_mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/app/test_refined_inhibitory_neuron_densities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.526844 atlas-densities-0.2.3/tests/combination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/combination/test_annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/combination/test_markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/tests/densities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.498844 atlas-densities-0.2.3/tests/densities/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/tests/densities/data/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/meta/mapping.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/meta/mapping_exc_only.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:49:28.530844 atlas-densities-0.2.3/tests/densities/data/mtypes/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/BP.dat
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/data/mtypes/mtype-taxonomy.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_inhibitory_neuron_density_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_optimization_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_refined_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/densities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/markers_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/mocking_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-08 07:49:24.000000 atlas-densities-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.437560 atlas-densities-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22025 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43635 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.445560 atlas-densities-0.2.4/atlas_densities/app/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.445560 atlas-densities-0.2.4/atlas_densities/app/data/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_bbp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/gaba_papers.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/homogenous_regions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   839727 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   347207 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   291827 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/non_density_measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   199258 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/measurements/std_cells.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/ca1_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/group_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/isocortex_23_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/isocortex_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/metadata/thalamus_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/composition.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.449560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.453560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.457560 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   930916 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.457560 atlas-densities-0.2.4/atlas_densities/combination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/combination/markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/atlas_densities/densities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26599 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_composition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21589 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/atlas_densities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.441560 atlas-densities-0.2.4/atlas_densities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26437 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 12:15:18.000000 atlas-densities-0.2.4/atlas_densities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)   230179 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/bbpp82_628_linear_program.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/cell_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/combination.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/mtype_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.461560 atlas-densities-0.2.4/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    55115 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/doc/source/static/atlas-densities.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   637735 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15618 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15178 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/app/test_refined_inhibitory_neuron_densities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.465560 atlas-densities-0.2.4/tests/combination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/test_annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/combination/test_markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.437560 atlas-densities-0.2.4/tests/densities/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/data/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/meta/mapping_exc_only.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:18.469560 atlas-densities-0.2.4/tests/densities/data/mtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/data/mtypes/mtype-taxonomy.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25290 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_optimization_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_refined_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13839 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/densities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/markers_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/mocking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 12:15:14.000000 atlas-densities-0.2.4/tox.ini
```

### Comparing `atlas-densities-0.2.3/.github/workflows/publish-sdist.yml` & `atlas-densities-0.2.4/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/.github/workflows/run-tox.yml` & `atlas-densities-0.2.4/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/.pylintrc` & `atlas-densities-0.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/CHANGELOG.rst` & `atlas-densities-0.2.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/CONTRIBUTING.rst` & `atlas-densities-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/LICENSE.txt` & `atlas-densities-0.2.4/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2005-2023 Blue Brain Project/EPFL
+   Copyright (c) 2005-2024 Blue Brain Project/EPFL
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `atlas-densities-0.2.3/PKG-INFO` & `atlas-densities-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: |banner|
         
@@ -269,16 +269,19 @@
         We fit here transfer functions that describe the relation between mean ISH expression in regions of
         the mouse brain and literature regional density estimates (see `Rodarie et al. (2022)`_ for more
         details). This step leverages AIBS ISH marker datasets (in their expression form, see also
         `fit_average_densities_ccfv2_config.yaml`_) and the previously computed
         literature density values.
         These transfer functions are used to obtain first estimates of neuron densities in regions not
         covered by literature.
-        The result of the following command is a list of first density estimates for each neuron type and
-        for each region of the annotation volume.
+        
+        The results of the following command includes a csv file (`first_estimates.csv`) storing the list
+        of first density estimates for each neuron type and for each region of the annotation volume.
+        The `fitting.json` output file contains the coefficients fitted by the algorithm together with their
+        respective standard deviation and `coefficient of determination`_ (`r_square`).
         
         .. code-block:: bash
         
             # make output folder
             mkdir -p data/ccfv2/first_estimates
         
             atlas-densities cell-densities fit-average-densities                                            \
@@ -436,15 +439,15 @@
         
         The development of this software was supported by funding to the Blue Brain Project, a research
         center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board
         of the Swiss Federal Institutes of Technology.
         
         For license and authors, see LICENSE.txt and AUTHORS.txt respectively.
         
-        Copyright © 2022 Blue Brain Project/EPFL
+        Copyright (c) 2022-2024 Blue Brain Project/EPFL
         
         .. _`Allen Institute for Brain Science (AIBS)`: https://alleninstitute.org/what-we-do/brain-science/
         .. _`Eroe et al. (2018)`: https://www.frontiersin.org/articles/10.3389/fninf.2018.00084/full
         .. _`Kim et al. (2017)`: https://www.sciencedirect.com/science/article/pii/S0092867417310693
         .. _`Markram et al. (2015)`: https://www.cell.com/cell/fulltext/S0092-8674(15)01191-5
         .. _`Rodarie et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010739
         .. _`Roussel et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010058
@@ -453,14 +456,15 @@
         .. _`DeepAtlas`: https://github.com/BlueBrain/Deep-Atlas
         .. _`fit_average_densities_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
         .. _`combine_markers_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
         .. _`mmc1.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc1.xlsx
         .. _`mmc3.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc3.xlsx
         .. _`gaba_papers.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/gaba_papers.xlsx
         .. _`mtypes_probability_map_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+        .. _`coefficient of determination`: https://en.wikipedia.org/wiki/Coefficient_of_determination
         
         .. substitutions
         
         .. |banner| image:: doc/source/static/atlas-densities.jpg
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `atlas-densities-0.2.3/README.rst` & `atlas-densities-0.2.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -261,16 +261,19 @@
 We fit here transfer functions that describe the relation between mean ISH expression in regions of
 the mouse brain and literature regional density estimates (see `Rodarie et al. (2022)`_ for more
 details). This step leverages AIBS ISH marker datasets (in their expression form, see also
 `fit_average_densities_ccfv2_config.yaml`_) and the previously computed
 literature density values.
 These transfer functions are used to obtain first estimates of neuron densities in regions not
 covered by literature.
-The result of the following command is a list of first density estimates for each neuron type and
-for each region of the annotation volume.
+
+The results of the following command includes a csv file (`first_estimates.csv`) storing the list
+of first density estimates for each neuron type and for each region of the annotation volume.
+The `fitting.json` output file contains the coefficients fitted by the algorithm together with their
+respective standard deviation and `coefficient of determination`_ (`r_square`).
 
 .. code-block:: bash
 
     # make output folder
     mkdir -p data/ccfv2/first_estimates
 
     atlas-densities cell-densities fit-average-densities                                            \
@@ -428,15 +431,15 @@
 
 The development of this software was supported by funding to the Blue Brain Project, a research
 center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board
 of the Swiss Federal Institutes of Technology.
 
 For license and authors, see LICENSE.txt and AUTHORS.txt respectively.
 
-Copyright © 2022 Blue Brain Project/EPFL
+Copyright (c) 2022-2024 Blue Brain Project/EPFL
 
 .. _`Allen Institute for Brain Science (AIBS)`: https://alleninstitute.org/what-we-do/brain-science/
 .. _`Eroe et al. (2018)`: https://www.frontiersin.org/articles/10.3389/fninf.2018.00084/full
 .. _`Kim et al. (2017)`: https://www.sciencedirect.com/science/article/pii/S0092867417310693
 .. _`Markram et al. (2015)`: https://www.cell.com/cell/fulltext/S0092-8674(15)01191-5
 .. _`Rodarie et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010739
 .. _`Roussel et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010058
@@ -445,11 +448,12 @@
 .. _`DeepAtlas`: https://github.com/BlueBrain/Deep-Atlas
 .. _`fit_average_densities_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
 .. _`combine_markers_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
 .. _`mmc1.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc1.xlsx
 .. _`mmc3.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc3.xlsx
 .. _`gaba_papers.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/gaba_papers.xlsx
 .. _`mtypes_probability_map_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+.. _`coefficient of determination`: https://en.wikipedia.org/wiki/Coefficient_of_determination
 
 .. substitutions
 
 .. |banner| image:: doc/source/static/atlas-densities.jpg
```

### Comparing `atlas-densities-0.2.3/atlas_densities/app/cell_densities.py` & `atlas-densities-0.2.4/atlas_densities/app/cell_densities.py`

 * *Files 0% similar despite different names*

```diff
@@ -901,21 +901,26 @@
     cell_density_stddev = {
         # Use the AIBS name attribute as key (this is a unique identifier in 1.json)
         # (Ex: former key "|root|Basic cell groups and regions|Cerebrum" -> new key: "Cerebrum")
         name.split("|")[-1]: stddev
         for (name, stddev) in cell_density_stddev.items()
     }
 
-    gene_marker_volumes = {
-        gene: {
+    gene_marker_volumes = {}
+    for gene, gene_data in gene_voxeldata.items():
+        loc_slices = slices[config["sectionDataSetID"][gene]]
+        gene_marker_volumes[gene] = {
             "intensity": gene_data.raw,
-            "slices": slices[config["sectionDataSetID"][gene]],  # list of integer slice indices
+            # list of integer slice indices
+            "slices": (
+                loc_slices - np.asarray(gene_data.offset / gene_data.voxel_dimensions, dtype=int)[0]
+                if loc_slices is not None
+                else None
+            ),
         }
-        for (gene, gene_data) in gene_voxeldata.items()
-    }
 
     group_ids_config = utils.load_json(group_ids_config_path)
 
     L.info("Loading average densities dataframe ...")
     average_densities_df = pd.read_csv(average_densities_path)
     homogenous_regions_df = pd.read_csv(homogenous_regions_path)
 
@@ -928,15 +933,15 @@
         average_densities_df,
         homogenous_regions_df,
         cell_density_stddev,
         region_name=region_name,
         group_ids_config=group_ids_config,
     )
 
-    # Turn index into column so as to ease off the save and load operations on csv files
+    # Turn index into column to ease off the save and load operations on csv files
     fitted_densities_df["brain_region"] = fitted_densities_df.index
 
     L.info("Saving fitted densities to file %s ...", fitted_densities_output_path)
     fitted_densities_df.to_csv(fitted_densities_output_path, index=False)
     if fitting_maps_output_path is not None:
         L.info("Saving fitting maps to file %s ...", fitting_maps_output_path)
         with open(fitting_maps_output_path, mode="w+", encoding="utf-8") as file_:
```

### Comparing `atlas-densities-0.2.3/atlas_densities/app/cli.py` & `atlas-densities-0.2.4/atlas_densities/app/cli.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/combination.py` & `atlas-densities-0.2.4/atlas_densities/app/combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/1.json` & `atlas-densities-0.2.4/atlas_densities/app/data/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/markers/README.rst` & `atlas-densities-0.2.4/atlas_densities/app/data/markers/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml` & `atlas-densities-0.2.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/markers/realigned_slices_bbp.json` & `atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_bbp.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/markers/realigned_slices_ccfv2.json` & `atlas-densities-0.2.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/README.rst` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/gaba_papers.xlsx` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/gaba_papers.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/homogenous_regions.csv` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/homogenous_regions.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/measurements.csv` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/mmc1.xlsx` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc1.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/mmc3.xlsx` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/mmc3.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/non_density_measurements.csv` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/non_density_measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/measurements/std_cells.json` & `atlas-densities-0.2.4/atlas_densities/app/data/measurements/std_cells.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/metadata/README.txt` & `atlas-densities-0.2.4/atlas_densities/app/data/metadata/README.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/metadata/group_ids.json` & `atlas-densities-0.2.4/atlas_densities/app/data/metadata/group_ids.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/metadata/thalamus_metadata.json` & `atlas-densities-0.2.4/atlas_densities/app/data/metadata/thalamus_metadata.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/README.rst` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/composition.yaml` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/composition.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/README.rst` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/probability_map/README.rst` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/data/mtypes/probability_map/probability_map.csv` & `atlas-densities-0.2.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/app/mtype_densities.py` & `atlas-densities-0.2.4/atlas_densities/app/mtype_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/combination/annotations_combinator.py` & `atlas-densities-0.2.4/atlas_densities/combination/annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/combination/markers_combinator.py` & `atlas-densities-0.2.4/atlas_densities/combination/markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/cell_counts.py` & `atlas-densities-0.2.4/atlas_densities/densities/cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/cell_density.py` & `atlas-densities-0.2.4/atlas_densities/densities/cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/excel_reader.py` & `atlas-densities-0.2.4/atlas_densities/densities/excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/excitatory_inhibitory_splitting.py` & `atlas-densities-0.2.4/atlas_densities/densities/excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/fitting.py` & `atlas-densities-0.2.4/atlas_densities/densities/fitting.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,31 +14,30 @@
 
 For each cell type, there are hence three linear fittings.
 To estimate the average density of a cell type T of a brain region R, we select the linear mapping
 obtained for T and the group R it belongs to.
 """
 from __future__ import annotations
 
+import itertools as it
 import logging
 import warnings
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from atlas_commons.typing import AnnotationT, BoolArray, FloatArray
 from scipy.optimize import curve_fit
 from tqdm import tqdm
+from voxcell import RegionMap, voxel_data
 
 from atlas_densities.densities import utils
 from atlas_densities.densities.measurement_to_density import remove_unknown_regions
 from atlas_densities.exceptions import AtlasDensitiesError, AtlasDensitiesWarning
 
-if TYPE_CHECKING:  # pragma: no cover
-    from voxcell import RegionMap
-
 L = logging.getLogger(__name__)
 
 MarkerVolumes = Dict[str, Dict[str, Union[FloatArray, List[int]]]]
 
 
 def create_dataframe_from_known_densities(
     region_names: list[str],
@@ -131,45 +130,48 @@
         annotation: int array of shape (W, H, D) holding the annotation of the whole
             brain model. (The integers W, H and D are the dimensions of the array).
         neuron_density: non-negative float array of shape (W, H, D) where W, H and D are integer
             dimensions. This array holds the volumetric neuron density of the brain model expressed
             in number of neurons per mm^3.
         densities: the data frame returned by
             :fun:`atlas_densities.densities.fitting.create_dataframe_from_known_densities`.
+        hierarchy_info: data frame with columns "descendant_id_set" (set[int]) and "brain_region"
+            (str) and whose index is a list of region ids.
+            See :fun:`atlas_densities.densities.utils.get_hierarchy_info`.
         cell_density_stddevs: (Optional) dict whose keys are brain regions names and whose values
             are standard deviations of average cell densities of the corresponding regions.
             Defaults to None, in which case the output standard deviation is set with the density
             value.
     """
 
     hierarchy_info = hierarchy_info.copy()
     hierarchy_info["id"] = hierarchy_info.index
     hierarchy_info.set_index("brain_region", inplace=True)
     inhibitory_mask = homogenous_regions["cell_type"] == "inhibitory"
 
     for region_name in homogenous_regions[inhibitory_mask]["brain_region"]:
-        desc_id_set = hierarchy_info.at[region_name, "descendant_id_set"]
+        desc_id_set = hierarchy_info.at[region_name, "descendant_ids"]
         id_mask = [id_ in desc_id_set for id_ in hierarchy_info["id"]]
         for child_region_name in hierarchy_info[id_mask].index:
             region_mask = np.isin(
-                annotation, list(hierarchy_info.at[child_region_name, "descendant_id_set"])
+                annotation, list(hierarchy_info.at[child_region_name, "descendant_ids"])
             )
             density = np.mean(neuron_density[region_mask])
             densities.at[child_region_name, "inhibitory_neuron"] = density
             if cell_density_stddevs is None:
                 densities.at[child_region_name, "inhibitory_neuron_standard_deviation"] = density
             else:
                 densities.at[
                     child_region_name, "inhibitory_neuron_standard_deviation"
                 ] = cell_density_stddevs[child_region_name]
 
     excitatory_mask = homogenous_regions["cell_type"] == "excitatory"
 
     for region_name in homogenous_regions[excitatory_mask]["brain_region"]:
-        desc_id_set = hierarchy_info.at[region_name, "descendant_id_set"]
+        desc_id_set = hierarchy_info.at[region_name, "descendant_ids"]
         id_mask = [id_ in desc_id_set for id_ in hierarchy_info["id"]]
         for child_region_name in hierarchy_info[id_mask].index:
             densities.at[child_region_name, "inhibitory_neuron"] = 0.0
             densities.at[child_region_name, "inhibitory_neuron_standard_deviation"] = 0.0
 
 
 def compute_average_intensity(
@@ -206,18 +208,113 @@
 
     if np.any(restricted_mask):
         return np.mean(intensity[restricted_mask])
 
     return 0.0
 
 
+def _add_depths(region_map_df):
+    """Rdd a `depth` column to the `region_map_df` with how deep it is within the hierarchy."""
+    region_map_df["depth"] = 0
+    parent_ids = [
+        -1,
+    ]
+    depth = 1
+    while parent_ids:
+        children_ids = region_map_df[np.isin(region_map_df["parent_id"], list(parent_ids))].index
+        region_map_df.loc[children_ids, "depth"] = depth
+        parent_ids = set(children_ids)
+        depth += 1
+
+
+def _fill_densities(region_map, region_map_df, df):
+    """Fill all `voxel_count` and `density` for each region within `def`.
+
+    This assumes the leaf nodes (ie: the deapest nodes in region_map) have had
+    their values filled in, and thus each of their parents can recursively be
+    filled in.
+    """
+    order_idx = np.argsort(region_map_df.depth.to_numpy())
+
+    ids = region_map_df.index[order_idx[::-1]]
+    for id_ in ids:
+        if id_ not in region_map._children:  # pylint: disable=protected-access
+            continue
+
+        children = region_map._children[id_]  # pylint: disable=protected-access
+
+        if not children:
+            continue
+
+        voxel_count = df.loc[children, "voxel_count"]
+        count = voxel_count.sum()
+        if count:
+            df.loc[id_, "voxel_count"] = count
+            df.loc[id_, "density"] = np.average(df.loc[children, "density"], weights=voxel_count)
+
+
+def _apply_density_slices(gene_marker_volumes):
+    """For each marker in `gene_marker_volumes`, apply the slice mask to the indensities volume."""
+    ret = {}
+    for marker, intensity in gene_marker_volumes.items():
+        intensity, slices = intensity["intensity"], intensity["slices"]
+
+        if slices is None:
+            mask = np.ones_like(intensity, dtype=bool)
+        else:
+            mask = np.zeros_like(intensity, dtype=bool)
+            slices_ = [slice_ for slice_ in slices if 0 <= slice_ < mask.shape[0]]
+            mask[slices_] = True
+
+        ret[marker] = {"intensity": intensity, "slices": slices, "mask": mask}
+
+    return ret
+
+
+def _compute_per_marker_intensity(annotation, gene_marker_volumes):
+    """Compute the average intensity for `id_`, for all makers in `gene_marker_volumes`"""
+    vtiv = voxel_data.ValueToIndexVoxels(annotation)
+
+    count_and_density = []
+    for id_ in vtiv.values:
+        if id_ == 0:
+            continue
+
+        voxel_ids = vtiv.value_to_1d_indices(id_)
+
+        res = []
+        for marker, intensity in gene_marker_volumes.items():
+            mask_voxels = vtiv.ravel(intensity["mask"])[voxel_ids]
+
+            count = mask_voxels.sum()
+
+            if count <= 0:
+                continue
+
+            mean_density = vtiv.ravel(intensity["intensity"])[voxel_ids][mask_voxels].sum() / count
+
+            if mean_density == 0.0:
+                L.warning("Mean density for id=%s and marker=%s", id_, marker)
+
+            count_and_density.append((marker.lower(), id_, count, mean_density))
+
+    res = (
+        pd.DataFrame(count_and_density, columns=["marker", "id", "voxel_count", "density"])
+        .set_index("id")
+        .pivot(columns="marker")
+        .swaplevel(axis=1)
+    )
+    return res
+
+
 def compute_average_intensities(
     annotation: AnnotationT,
     gene_marker_volumes: MarkerVolumes,
     hierarchy_info: pd.DataFrame,
+    region_map,
 ) -> pd.DataFrame:
     """
     Compute the average marker intensity of every region in `hierarchy_info` for every marker
     of `gene_marker_volumes`.
 
     If a region does not intersect any of the slices of a gene marker volume, the average density
     of the marked cell type of this region is set with np.nan.
@@ -228,48 +325,48 @@
         gene_marker_volumes: dict of the form {
                 "gad67": {"intensity": <array>, "slices": <list>},
                 "pv": {"intensity": <array>, "slices": <list>},
                 ...
                 }
             where each intensity array is of shape (W, H, D) and where the items of each slice
             list range in [0, W - 1].
-        hierarchy_info: data frame with colums "descendant_id_set" (set[int]) and "brain_region"
+        hierarchy_info: data frame with colums "descendant_ids" (set[int]) and "brain_region"
             (str) and whose index is a list of region ids.
             See :fun:`atlas_densities.densities.utils.get_hierarchy_info`.
 
     Returns:
         A data frame of the following form (values are fake):
                     gad67  pv   sst    vip
         Isocortex   1.5    1.1  0.2    12.0
         Cerebellum  2.5    0.9  0.1    11.0
         ...         ...   ...    ...    ...
         The index of the data frame is the list of regions `hierarchy_info["brain_region"]`.
         The column labels are the keys of `gene_marker_volumes` in lower case.
     """
-    region_count = len(hierarchy_info["brain_region"])
-    data = np.full((region_count, len(gene_marker_volumes)), np.nan)
-    hierarchy_info = hierarchy_info.set_index("brain_region")
+    gene_marker_volumes = _apply_density_slices(gene_marker_volumes)
+
+    intensity = _compute_per_marker_intensity(annotation, gene_marker_volumes)
+
+    region_map_df = region_map.as_dataframe()
+    _add_depths(region_map_df)
+
     result = pd.DataFrame(
-        data=data,
+        data=np.nan,
         index=hierarchy_info.index,
-        columns=[marker_name.lower() for marker_name in gene_marker_volumes.keys()],
+        columns=[marker_name.lower() for marker_name in gene_marker_volumes],
     )
+    result["brain_region"] = region_map_df.loc[result.index].name
 
-    L.info(
-        "Computing average intensities for %d markers in %d regions ...",
-        len(gene_marker_volumes),
-        region_count,
-    )
-    for region_name in tqdm(result.index):
-        region_mask = np.isin(annotation, list(hierarchy_info.at[region_name, "descendant_id_set"]))
-        for marker, intensity in gene_marker_volumes.items():
-            result.at[region_name, marker.lower()] = compute_average_intensity(
-                intensity["intensity"], region_mask, intensity["slices"]
-            )
+    for marker in gene_marker_volumes:
+        df = pd.DataFrame(data=0.0, index=result.index, columns=["voxel_count", "density"])
+        df.update(intensity[marker.lower()])
+        _fill_densities(region_map, region_map_df, df)
+        result[marker.lower()] = df["density"]
 
+    result = result.set_index("brain_region")
     return result
 
 
 def linear_fitting_xy(
     xdata: list[float], ydata: list[float], sigma: Union[list[float], FloatArray]
 ) -> dict[str, float]:
     """
@@ -281,15 +378,17 @@
         ydata: list of float values with the same length as `xdata`.
         sigma: list of non-negative float values with the same length as `xdata`.
             These are the standard deviations of the values in `ydata`.
             Zero values are replaced by the least positive value if it exists,
             otherwise by 1.0.
 
     Returns:
-        a dict of the form {"coefficient": <float>, "standard_deviation": <float>}.
+        a dict of the form {"coefficient": <float>,
+                            "standard_deviation": <float>,
+                            "r_square": <float>}.
 
     Raises:
        AtlasDensitiesError if some of the `sigma`values are negative.
     """
 
     if len(xdata) == 0:
         return {"coefficient": np.nan, "standard_deviation": np.nan}
@@ -307,23 +406,32 @@
     zero_mask = np.isclose(sigma, 0.0)
     if np.all(zero_mask):
         sigma[zero_mask] = 1.0
     else:
         least_positive = np.min(sigma[~zero_mask])
         sigma[zero_mask] = least_positive / 2.0
 
+    def _optimize_func(x, coefficient):
+        return coefficient * np.array(x)
+
     parameters = curve_fit(
-        lambda x, coefficient: coefficient * x,
+        _optimize_func,
         xdata=xdata,
         ydata=ydata,
         sigma=sigma,
         absolute_sigma=True,
     )
-
-    return {"coefficient": parameters[0][0], "standard_deviation": np.sqrt(parameters[1][0][0])}
+    ss_reg = np.sum((_optimize_func(xdata, parameters[0][0]) - np.mean(ydata)) ** 2)
+    ss_tot = np.sum((np.array(ydata) - _optimize_func(xdata, parameters[0][0])) ** 2) + ss_reg
+    # if total sum of square is null, no variance can be explained by the fitting
+    return {
+        "coefficient": parameters[0][0],
+        "standard_deviation": np.sqrt(parameters[1][0][0]),
+        "r_square": (ss_reg / ss_tot) if ss_tot > 0 else np.nan,
+    }
 
 
 FittingData = Dict[str, Dict[str, Dict[str, float]]]
 
 
 def compute_fitting_coefficients(
     groups: dict[str, set[str]], average_intensities: pd.DataFrame, densities: pd.DataFrame
@@ -346,31 +454,32 @@
         densities: data frame returned by
           :fun:`atlas_densities.densities.fitting.create_dataframe_from_known_densities`.
 
     Returns:
         dict of the form (values are fake):
         {
             "Isocortex" : {
-                "gad67": { "coefficient": 0.85, "standard_deviation": 0.15},
-                "pv": { "coefficient": 1.00, "standard_deviation": 0.5},
-                "sst": { "coefficient": 1.07, "standard_deviation": 0.75},
-                "vip": { "coefficient": 0.95, "standard_deviation": 0.15},
+                "gad67": { "coefficient": 0.85, "standard_deviation": 0.15, "r_square": 0.75},
+                "pv": { "coefficient": 1.00, "standard_deviation": 0.5, "r_square": 0.66},
+                "sst": { "coefficient": 1.07, "standard_deviation": 0.75, "r_square": 0.80},
+                "vip": { "coefficient": 0.95, "standard_deviation": 0.15, "r_square": 0.90},
             },
             "Cerebellum" : {
-                "gad67": { "coefficient": 0.75, "standard_deviation": 0.15},
-                "pv": { "coefficient": 1.10, "standard_deviation": 0.55},
-                "sst": { "coefficient": 1.20, "standard_deviation": 0.45},
-                "vip": { "coefficient": 0.95, "standard_deviation": 0.15},
+                "gad67": { "coefficient": 0.75, "standard_deviation": 0.15, "r_square": 0.55},
+                "pv": { "coefficient": 1.10, "standard_deviation": 0.55, "r_square": 0.40},
+                "sst": { "coefficient": 1.20, "standard_deviation": 0.45, "r_square": 0.58},
+                "vip": { "coefficient": 0.95, "standard_deviation": 0.15, "r_square": 0.77},
             },
            ...
         }
         The keys of the dict are the names of the region groups where separate fittings are
         performed. A "coefficient" value is the value of the linear regression coefficient for a
         given region group and a given cell type.
         The "standard_deviation" value is the standard deviation of the coefficient value.
+        The "r_square" value is the coefficient of determination of the coefficient value.
     """
 
     if len(densities.index) != len(average_intensities.index) or np.any(
         densities.index != average_intensities.index
     ):
         raise AtlasDensitiesError(
             "The data frames `densities` and `average_intensities` have a different index."
@@ -383,15 +492,15 @@
         raise AtlasDensitiesError(
             f"Some marker names are not represented in the densities data"
             f" frame by the corresponding marked cell types: {diff_types}."
         )
 
     result = {
         group_name: {
-            cell_type: {"coefficient": np.nan, "standard_deviation": np.nan}
+            cell_type: {"coefficient": np.nan, "standard_deviation": np.nan, "r_square": np.nan}
             for cell_type in cell_types
         }
         for group_name in groups
     }
 
     clouds: dict[str, dict[str, dict[str, list[float]]]] = {
         group_name: {cell_type: {"xdata": [], "ydata": [], "sigma": []} for cell_type in cell_types}
@@ -402,32 +511,40 @@
         L.info(
             "Building regression data in group %s for %d regions and %d cell types ...",
             group_name,
             len(groups[group_name]),
             len(cell_types),
         )
         for region_name in tqdm(groups[group_name]):
-            for cell_type in cell_types:
-                intensity = average_intensities.at[region_name, cell_type[:-1]]
-                density = densities.at[region_name, cell_type]
-                if not (
-                    np.isnan(density) or np.isnan(intensity) or intensity == 0.0 or density == 0.0
-                ):
-                    assert_msg = f"in region {region_name} for cell type {cell_type}"
-                    assert intensity >= 0.0, "Negative average intensity " + assert_msg
-                    assert density >= 0.0, "Negative density " + assert_msg
-                    standard_deviation = densities.at[
-                        region_name, cell_type + "_standard_deviation"
-                    ]
-                    assert not np.isnan(standard_deviation), "NaN standard deviation " + assert_msg
-                    assert standard_deviation >= 0.0, "Negative standard deviation " + assert_msg
-
-                    clouds[group_name][cell_type]["xdata"].append(intensity)
-                    clouds[group_name][cell_type]["ydata"].append(density)
-                    clouds[group_name][cell_type]["sigma"].append(standard_deviation)
+            if region_name in average_intensities.index:
+                for cell_type in cell_types:
+                    intensity = average_intensities.at[region_name, cell_type[:-1]]
+                    density = densities.at[region_name, cell_type]
+                    if not (
+                        np.isnan(density)
+                        or np.isnan(intensity)
+                        or intensity == 0.0
+                        or density == 0.0
+                    ):
+                        assert_msg = f"in region {region_name} for cell type {cell_type}"
+                        assert intensity >= 0.0, "Negative average intensity " + assert_msg
+                        assert density >= 0.0, "Negative density " + assert_msg
+                        standard_deviation = densities.at[
+                            region_name, cell_type + "_standard_deviation"
+                        ]
+                        assert not np.isnan(standard_deviation), (
+                            "NaN standard deviation " + assert_msg
+                        )
+                        assert standard_deviation >= 0.0, (
+                            "Negative standard deviation " + assert_msg
+                        )
+
+                        clouds[group_name][cell_type]["xdata"].append(intensity)
+                        clouds[group_name][cell_type]["ydata"].append(density)
+                        clouds[group_name][cell_type]["sigma"].append(standard_deviation)
 
         L.info("Computing regression coefficients for %d cell types ...", len(cell_types))
         for cell_type in tqdm(cell_types):
             cloud = clouds[group_name][cell_type]
             result[group_name][cell_type] = linear_fitting_xy(
                 cloud["xdata"], cloud["ydata"], cloud["sigma"]
             )
@@ -463,31 +580,59 @@
         fitting_coefficients: dict returned by
             fun:`atlas_densities.densities.fitting.compute_fitting_coefficients`.
     """
 
     for group_name, region_names in groups.items():
         for region_name in region_names:
             for marker in average_intensities.columns:
-                intensity = average_intensities.at[region_name, marker]
-                cell_type = marker + "+"
-                if np.isnan(densities.at[region_name, cell_type]) and not np.isnan(intensity):
-                    fitting = fitting_coefficients[group_name][cell_type]
-                    if np.isnan(fitting["coefficient"]):
-                        warnings.warn(
-                            f"Interpolating density of region {region_name} for cell type "
-                            f"{cell_type} using NaN fitting coefficient of region group "
-                            f"{group_name}.",
-                            AtlasDensitiesWarning,
-                        )
-                    fitted_value = fitting["coefficient"] * intensity
-                    standard_deviation = fitted_value * fitting["standard_deviation"]
-                    densities.at[region_name, cell_type] = fitted_value
-                    densities.at[
-                        region_name, cell_type + "_standard_deviation"
-                    ] = standard_deviation
+                if region_name in average_intensities.index:
+                    _apply_fitting(
+                        region_name,
+                        marker,
+                        group_name,
+                        average_intensities,
+                        densities,
+                        fitting_coefficients,
+                    )
+
+
+def _apply_fitting(
+    region_name, marker, group_name, average_intensities, densities, fitting_coefficients
+):
+    """
+    Apply the fitting function to a given region and marker based on the corresponding marker
+    intensity.
+
+    Args:
+        region_name: region name
+        marker: ISH marker name
+        group_name: fitting group name
+        average_intensities: pandas data frame returned by
+          :fun:`atlas_densities.densities.fitting.compute_average_intensities`.
+        densities: data frame returned by
+          :fun:`atlas_densities.densities.fitting.create_dataframe_from_known_densities`.
+        fitting_coefficients: dict returned by
+          :fun:`atlas_densities.densities.fitting.compute_fitting_coefficients`.
+    """
+
+    intensity = average_intensities.at[region_name, marker]
+    cell_type = marker + "+"
+    if np.isnan(densities.at[region_name, cell_type]) and not np.isnan(intensity):
+        fitting = fitting_coefficients[group_name][cell_type]
+        if np.isnan(fitting["coefficient"]):
+            warnings.warn(
+                f"Interpolating density of region {region_name} for cell type "
+                f"{cell_type} using NaN fitting coefficient of region group "
+                f"{group_name}.",
+                AtlasDensitiesWarning,
+            )
+        fitted_value = fitting["coefficient"] * intensity
+        standard_deviation = fitted_value * fitting["standard_deviation"]
+        densities.at[region_name, cell_type] = fitted_value
+        densities.at[region_name, cell_type + "_standard_deviation"] = standard_deviation
 
 
 def _check_homogenous_regions_sanity(homogenous_regions: pd.DataFrame) -> None:
     """
     Raise an error if `homogenous_regions` has unexpected entries.
     """
 
@@ -524,15 +669,15 @@
     if np.any(negative_mask):
         raise AtlasDensitiesError(
             f"`average_densities` has a negative measurement or a negative standard deviation "
             f"for the following entries: {average_densities[negative_mask]}"
         )
 
 
-def _get_group_names(region_map: "RegionMap", group_ids_config: dict) -> dict[str, set[str]]:
+def _get_group_names(region_map: RegionMap, group_ids_config: dict) -> dict[str, set[str]]:
     """
     Get AIBS names for regions in several region groups of interest.
 
     Args:
         region_map: object to navigate the mouse brain regions hierarchy
             (instantiated from AIBS 1.json).
         group_ids_config: mapping of regions to their constituent ids
@@ -540,15 +685,15 @@
     Returns:
         A dictionary whose keys are region group names and whose values are
         sets of brain region names.
     """
 
     group_ids = utils.get_group_ids(region_map, group_ids_config)
 
-    # Make the Rest group stable under taking descendants
+    # Make the Rest group stable undertaking descendants
     # The name of any ascendant region of the Cerebellum and
     #    Isocortex groups are removed from the names of the Rest group. This makes sure that
     #    the set of names of the Rest group is closed under taking descendants.
     isocortex_id = region_map.find("Isocortex", attr="name").pop()
     cerebellum_id = region_map.find("Cerebellum", attr="name").pop()
     ascendant_ids = set(region_map.get(isocortex_id, attr="id", with_ascendants=True)) | set(
         region_map.get(cerebellum_id, attr="id", with_ascendants=True)
@@ -557,16 +702,30 @@
 
     return {
         group_name: {region_map.get(id_, attr="name") for id_ in group_ids[group_name]}
         for group_name in ["Cerebellum group", "Isocortex group", "Rest"]
     }
 
 
+def _get_group_region_names(groups):
+    """
+    Create a set of the union of AIBS region names that belong to the given groups.
+
+    Args:
+        groups: dictionary from group name to list of region name.
+
+    Returns:
+        A list of region names.
+    """
+
+    return list(set(it.chain.from_iterable(groups.values())))
+
+
 def linear_fitting(  # pylint: disable=too-many-arguments
-    region_map: "RegionMap",
+    region_map: RegionMap,
     annotation: AnnotationT,
     neuron_density: FloatArray,
     gene_marker_volumes: MarkerVolumes,
     average_densities: pd.DataFrame,
     homogenous_regions: pd.DataFrame,
     cell_density_stddevs: Optional[dict[str, float]] = None,
     region_name: str = "root",
@@ -585,14 +744,17 @@
     set to NaN.
 
     Args:
         region_map: RegionMap object to navigate the brain region hierarchy. Used to
             define the regions whose cell densities will be computed.
         annotation: int array of shape (W, H, D) holding the annotation of the whole
             brain model. (The integers W, H and D are the dimensions of the array).
+        neuron_density: non-negative float array of shape (W, H, D) where W, H and D are integer
+            dimensions. This array holds the volumetric neuron density of the brain model expressed
+            in number of neurons per mm^3.
         gene_marker_volumes: dict of the form {
                   "gad67": {"intensity": <array>, "slices": <list>},
                   "pv": {"intensity": <array>, "slices": <list>},
                   ...
                 }
             where each intensity array is of shape (W, H, D) and where the items of each slice
             list range in [0, W - 1]. The keys "gad67", "pv", ... are gene marker names and the
@@ -600,15 +762,15 @@
             data frame.
         average_densities: a data frame whose columns are described in
             :func:`atlas_densities.app.densities.compile_measurements` and where all
             measurements are of type "cell density" in number of cells per mm^3.
         homogenous_regions: data frame with two columns, brain_region and cell_type.
             The brain_region column holds region names and the values of the cell_type column are
             "inhibitory" or "excitatory" depending on whether every neuron of the region is
-            inhibitory or excitatory. Note that the "inhibitory" cell type will superseded by
+            inhibitory or excitatory. Note that the "inhibitory" cell type will supersede by
             its synonym "gad67+" in the output data frame.
         cell_density_stddevs: dict whose keys are brain regions names and whose values are
             standard deviations of average cell densities of the corresponding regions.
         region_name: (str) name of the root region of interest
         group_ids_config: mapping of regions to their constituent ids
 
     Returns:
@@ -651,21 +813,29 @@
             "inhibitory_neuron": "gad67+",
             "inhibitory_neuron_standard_deviation": "gad67+_standard_deviation",
         },
         inplace=True,
     )
 
     L.info("Computing average intensities ...")
+    groups = _get_group_names(region_map, group_ids_config)
+    # Limit the fitting to the regions groups.
+    indexes = np.isin(
+        hierarchy_info["brain_region"].to_numpy(),
+        _get_group_region_names(groups),
+        invert=True,
+    )
     average_intensities = compute_average_intensities(
-        annotation, gene_marker_volumes, hierarchy_info
+        annotation,
+        gene_marker_volumes,
+        hierarchy_info.drop(hierarchy_info.index[indexes]),
+        region_map,
     )
 
-    L.info("Getting group names ...")
-    # We want group region names to be stable under taking descendants
-    groups = _get_group_names(region_map, group_ids_config)
-
     L.info("Computing fitting coefficients ...")
-    fitting_coefficients = compute_fitting_coefficients(groups, average_intensities, densities)
+    fitting_coefficients = compute_fitting_coefficients(
+        groups, average_intensities, densities.drop(densities.index[indexes])
+    )
     L.info("Fitting unknown average densities ...")
     fit_unknown_densities(groups, average_intensities, densities, fitting_coefficients)
 
     return densities, fitting_coefficients
```

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/glia_densities.py` & `atlas-densities-0.2.4/atlas_densities/densities/glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/inhibitory_neuron_densities_optimization.py` & `atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 allow comparisons with the former approach of the same article.
 
 The main function resolves a linear program which aims at minimizing the absolute differences
 between output cell counts and input estimates while enforcing the consistency of cell count sums
 across the brain region hierarchy.
 
 The file ``doc/source/bbpp82_628_linear_program.pdf`` serves as a documentation of the linear
-program, see Section 2 in particular. The initalization of the linear program relies on average
-density estimates, obtained obtained for instance via the ``fitting`` module. We refer to these
+program, see Section 2 in particular. The initialization of the linear program relies on average
+density estimates, obtained for instance via the ``fitting`` module. We refer to these
 estimates as the initial estimates.
 
 The output are volumetric density nrrd files, one for each of the aforementioned inhibitory
 neuron types. Volumetric densities are derived from the cell counts obtained as the solution of
 the previous linear program.
 
 A note on the linear program:
@@ -32,48 +32,153 @@
 which are taken for certain (when the "confidence" numbers ``sigma_{i, m}`` are close to 0.0)
 and with NaN otherwise. If ``x_result.at[(id_, marker)]`` is set to NaN, then a decision variable
 ``x_{i, m}`` is introduced where i = id_ and m = marker. Once the program is resolved,
 ``x_result.at[(id_, marker)]`` is set with the solution value of ``x_{i, m}``. Similarly, the
 variable deltas used in this module corresponds to the decision variables ``delta_{r, m}`` of
 the pdf file.
 """
+from __future__ import annotations
 
 import logging
 import warnings
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Set, Tuple
 
 import numpy as np
 import pandas as pd
 from atlas_commons.typing import AnnotationT, FloatArray
 from scipy.optimize import linprog
 from tqdm import tqdm
-from voxcell import RegionMap
+from voxcell import RegionMap, voxel_data
 
 from atlas_densities.densities import utils
 from atlas_densities.densities.inhibitory_neuron_densities_helper import (
     average_densities_to_cell_counts,
-    check_region_counts_consistency,
     get_cell_types,
-    replace_inf_with_none,
-    resize_average_densities,
 )
 from atlas_densities.exceptions import AtlasDensitiesError, AtlasDensitiesWarning
 
 L = logging.getLogger(__name__)
 
 SKIP = np.inf  # Used to signify that a delta variable of the linear program should be removed
 KEEP = np.nan  # Used to signify that a delta variable should be added to the linear program
+MinMaxPair = Tuple[float, Optional[float]]
+
+
+def _resize_average_densities(
+    average_densities: pd.DataFrame, hierarchy_info: pd.DataFrame
+) -> pd.DataFrame:
+    """
+    Resize the `average_densities` data frame in such a way that the resized index coincides with
+    `hierarchy_info["brain_region"]`.
+
+    Missing entries are set to ``np.nan``.
+
+    average_densities: a data frame whose columns are described in
+            :func:`atlas_densities.densities.fitting.linear_fitting` containing the average
+            cell densities of brain regions and their associated standard deviations. Columns are
+            labelled by T and T_standard_deviation for various cell types T. The index of
+            `average_densities` is a list of region names.
+    hierarchy_info: data frame returned by
+        :func:`atlas_densities.densities.utils.get_hierarchy_info`.
+
+    Returns: a data frame containing all the entries of `average_densities` and whose index is
+        `hierarchy_info["brain_region"]`. New entries are set to ``np.nan``.
+
+    """
+    resized = pd.DataFrame(
+        np.nan, index=hierarchy_info["brain_region"], columns=average_densities.columns
+    )
+    resized.loc[average_densities.index] = average_densities
+
+    return resized
+
+
+def _check_region_counts_consistency(
+    region_counts: pd.DataFrame, hierarchy_info: pd.DataFrame, tolerance: float = 0.0
+) -> None:
+    """
+    Check that cell counts considered as certain are consistent across the brain regions hierarchy.
+
+    Args:
+        region_counts: data frame returned by
+            :fun:`densities.inhibitory_densities_helper.average_densities_to_cell_counts`.
+            A region is understood as a region of the brain hierarchy and includes all descendant
+            subregions.
+        hierarchy_info: data frame returned by
+            :func:`atlas_densities.densities.utils.get_hierarchy_info`.
+        tolerance: non-negative float number used as tolerance when comparing counts.
+            Defaults to 0.0.
+
+    Raises:
+        AtlasDensitiesError if the sum of the cell counts of some leaf regions, all given with
+        certainty, exceeds the cell count of an ancestor, also given with certainty.
+
+    """
+
+    def _check_descendants_consistency(region_name: str, id_set: Set[int], cell_type: str):
+        standard_deviation = f"{cell_type}_standard_deviation"
+
+        if region_counts.at[region_name, standard_deviation] != 0.0:
+            return
+
+        # count is certain, since standard_deviation is 0
+        count = region_counts.at[region_name, cell_type]
+        descendants_names = hierarchy_info.loc[list(id_set), "brain_region"]
+        zero_std_mask = region_counts.loc[descendants_names, standard_deviation] == 0.0
+        mask = zero_std_mask & (region_counts.loc[descendants_names, cell_type] > count + tolerance)
+        descendants_counts = region_counts.loc[descendants_names, cell_type][mask]
+        if not descendants_counts.empty:
+            raise AtlasDensitiesError(
+                f"Counts of {cell_type} cells in regions {list(descendants_names)} all exceed "
+                f"the count of its ancestor region {region_name} and each count is given "
+                f"for certain. The counts {descendants_counts} are all larger than "
+                f"{count}."
+            )
+
+        names_with_certainty = descendants_names[zero_std_mask.to_list()].to_list()
+        leaf_names = [
+            hierarchy_info.at[id_, "brain_region"]
+            for id_ in id_set
+            if len(hierarchy_info.at[id_, "descendant_ids"]) == 1
+            and hierarchy_info.at[id_, "brain_region"] in names_with_certainty
+        ]
+        leaves_count_sum = np.sum(region_counts.loc[leaf_names, cell_type])
+        if leaves_count_sum > count + tolerance:
+            raise AtlasDensitiesError(
+                f"The sum of the counts of {cell_type} cells in leaf regions",
+                " which are given with certainty, exceeds the count of the ancestor"
+                f" region {region_name}, also given with certainty: "
+                f"{leaves_count_sum} > {count}.",
+            )
+
+    for _, region_name, id_set in hierarchy_info[["brain_region", "descendant_ids"]].itertuples():
+        for cell_type in get_cell_types(region_counts):
+            _check_descendants_consistency(region_name, id_set, cell_type)
+
+
+def _replace_inf_with_none(bounds: FloatArray) -> List[MinMaxPair]:
+    """
+    Replace the upper bounds equal to ``np.inf`` by None so as to comply with
+    the `bounds` interface of scipy.optimize.linprog.
+
+    Args:
+        bounds: float array of shape (N, 2). Values in `bounds[..., 1]` can be
+            ``np.inf`` to indicate the absence of a constraining upper bound.
+
+    Return:
+        list of pairs (min, max) where min is a float and max either a float or None.
+    """
+    return [(float(min_), None if np.isinf(max_) else float(max_)) for min_, max_ in bounds]
 
 
 def _compute_region_cell_counts(
     annotation: AnnotationT,
     density: FloatArray,
     voxel_volume: float,
     hierarchy_info: "pd.DataFrame",
-    with_descendants: bool = True,
 ) -> "pd.DataFrame":
     """
     Compute the cell count of every 3D region in `annotation` labeled by a unique
     id in `ids` wrt cell `density`.
 
     Args:
         annotation: int array of shape (W, H, D) holding the annotation of the whole AIBS
@@ -81,44 +186,35 @@
         density: float array of shape `annotation.shape` holding the volumetric density of a
             given cell type. The value assigned to a voxel represents the cell density in this
             voxel expressed in number of cells per mm^3.
         voxel_volume: volume in mm^3 of a voxel in any of the volumetric input arrays.
             This is (25 * 1e-6) ** 3 for an AIBS atlas nrrd file with 25um resolution.
         hierarchy_info: data frame returned by
             :func:`atlas_densities.densities.utils.get_hierarchy_info`.
-        with_descendants: if True, a computed cell count refers to the entire 3D region
-            designated by a region name, including all descendants subregions. Otherwise, the
-            computed cell count is the cell count of the 3D region labeled by the unique region
-            identifier. Defaults to True.
 
     Returns:
         DataFrame of the following form (values are fake):
              brain_region                    cell_count
         10   Basic cell groups and regions   200.30
         123  Cerebrum                         75.05
              ...                             ...
         The index is the sorted list of all region identifiers.
     """
+    vtiv = voxel_data.ValueToIndexVoxels(annotation)
+    density = vtiv.ravel(density)
+
     id_counts = []
-    for id_ in tqdm(hierarchy_info.index):
-        mask = annotation == id_
-        id_counts.append(np.sum(density[mask]) * voxel_volume)
+    for id_ in hierarchy_info.index:
+        indices = vtiv.value_to_1d_indices(id_)
+        id_counts.append(np.sum(density[indices]) * voxel_volume)
 
     result = pd.DataFrame(
         {"brain_region": hierarchy_info["brain_region"], "cell_count": id_counts},
         index=hierarchy_info.index,
     )
-
-    if with_descendants:
-        counts = []
-        for id_set in tqdm(hierarchy_info["descendant_id_set"]):
-            count = result.loc[list(id_set), "cell_count"].sum()
-            counts.append(count)
-        result["cell_count"] = counts
-
     return result
 
 
 def set_known_values(
     region_counts: pd.DataFrame,
     id_counts: pd.DataFrame,
     hierarchy_info: pd.DataFrame,
@@ -170,15 +266,15 @@
     assert np.all(hierarchy_info.index == id_counts.index)
 
     def _zero_descendants(id_, cell_type, x_result, deltas, hierarchy_info):
         """
         Zeroes the count of `cell_type` cells in every descendant regions of `id_`,
         including `id_`.
         """
-        desc_ids = list(hierarchy_info.at[id_, "descendant_id_set"])
+        desc_ids = list(hierarchy_info.at[id_, "descendant_ids"])
         x_result.loc[desc_ids, cell_type] = 0.0
         desc_names = hierarchy_info.loc[desc_ids, "brain_region"]
         deltas.loc[desc_names, cell_type] = 0.0
 
     L.info("Preparing variables layout ...")
     x_result = pd.DataFrame(
         {cell_type: np.full(len(id_counts), KEEP) for cell_type in cell_types},
@@ -188,15 +284,15 @@
         {cell_type: np.full(len(region_counts), KEEP) for cell_type in cell_types},
         index=region_counts.index,  # indexed by region names (str)
     )
 
     L.info("Setting known values ...")
     # Set delta_{r, m} with `SKIP` if the corresponding cell count estimate is missing.
     # This means that the region r won't impose any constraint wrt to the marker m in the linear
-    # program, i. e., the delta_{r, m} variable is omitted for such r and m.
+    # program, i.e., the delta_{r, m} variable is omitted for such r and m.
     for id_, region_name in zip(hierarchy_info.index, region_counts.index):
         for cell_type in cell_types:
             # A region without cell count estimate for `cell_type` adds no constraint
             # to the linear program.
             if np.isnan(region_counts.at[region_name, cell_type + "_standard_deviation"]):
                 deltas.loc[region_name, cell_type] = SKIP
 
@@ -255,15 +351,15 @@
     Returns:
         a tuple (`bounds`, `x_map`, `deltas_map`) where
         - `bounds` is a float array of shape (N, 2) with N the total number of decision variables.
             ``np.inf`` values in `bounds[..., 1]` indicates that there is no constraining upper
             bound.
         - `x_map` is a dict mapping pairs (id_, cell_type) to indices of `bounds`.
             The keys of this dict corresponds to cell count variables in the linear program.
-        - `deltas_map` is a dict mapping pairs (region_name, cell_type) to to indices of `bounds`.
+        - `deltas_map` is a dict mapping pairs (region_name, cell_type) to indices of `bounds`.
             The keys of this dict corresponds to the slack "delta" variables which represent
             distances of cell count variables to initial estimates.
     """
     x_map = {}
     deltas_map = {}
     bounds = []  # list of pairs (lower_bound, upper_bound)
     cell_types = get_cell_types(x_result)
@@ -336,15 +432,15 @@
                 AtlasDensitiesWarning,
             )
 
     def check_constraint_3e(
         constraint: FloatArray, b_value: float, region_name: str, id_: int
     ) -> bool:
         """
-        Check if `contraint` is a valid inequality constraint of type (3e).
+        Check if `constraint` is a valid inequality constraint of type (3e).
 
         Returns:
             True if the constraint is not void.
 
         Raises:
            AtlasDensitiesWarning if an inconsistency is detected.
         """
@@ -365,17 +461,15 @@
 
         return False
 
     a_ub = []
     b_ub = []
     variable_count = len(x_map) + len(deltas_map)
     cell_types = get_cell_types(region_counts)
-    for id_, region_name, set_ in zip(
-        hierarchy_info.index, hierarchy_info["brain_region"], hierarchy_info["descendant_id_set"]
-    ):
+    for id_, region_name, set_ in hierarchy_info[["brain_region", "descendant_ids"]].itertuples():
         for cell_type in cell_types:
             if (region_name, cell_type) in deltas_map:
                 constraint = np.zeros((variable_count,), dtype=float)
                 b_value = region_counts.at[region_name, cell_type]
                 for desc_id in set_:
                     if (desc_id, cell_type) in x_map:
                         constraint[x_map[(desc_id, cell_type)]] = 1.0
@@ -475,81 +569,61 @@
 
     Returns:
         a pair of data frames (`region_counts`, `id_counts`).
         - `region_counts` has the return value format of
             :fun:`densities.inhibitory_densities_helper.average_densities_to_cell_counts`.
             It holds region cell counts as well as associated standard deviations.
         - `id_counts` has the return value format of
-            :fun:`densities.inhbitory_densities_helper.average_densities_to_cell_counts` except
+            :fun:`densities.inhibitory_densities_helper.average_densities_to_cell_counts` except
             that its index is a list of unique integer region identifiers.
             It holds the cell counts of the 3D regions labeled by a unique identifier, as well as
             associated standard deviations (descendant subregions are excluded).
     """
     L.info("Computing the volume of every 3D region ...")
     volumes = utils.compute_region_volumes(annotation, voxel_volume, hierarchy_info)
 
     L.info("Computing cell count estimates in every 3D region ...")
     region_counts = average_densities_to_cell_counts(average_densities, volumes)
 
-    # Detect cell counts inconsistency between a region and its descendants when
-    # estimates are deemed as certain.
-    check_region_counts_consistency(region_counts, hierarchy_info)
+    _check_region_counts_consistency(region_counts, hierarchy_info)
 
     L.info("Computing cell count estimates in atomic 3D region ...")
     volumes.drop("volume", axis=1, inplace=True)
     volumes.rename(columns={"id_volume": "volume"}, inplace=True)
     id_counts = average_densities_to_cell_counts(average_densities, volumes)
     id_counts.index = volumes.index  # unique integer identifiers
 
     return region_counts, id_counts
 
 
 def _check_variables_consistency(
     x_result: pd.DataFrame,
-    deltas: pd.DataFrame,
     cell_types: List[str],
     neuron_counts: pd.DataFrame,
     hierarchy_info: pd.DataFrame,
 ) -> None:
     """
-    Raises an error if a delta variable indexed by (region_name, cell_type) is set with a non-NaN
-    value whereas an x_result variable indexed by (desc_id, cell_type) is set with a NaN value for
-    some descendant id of region_name.
-
     Raises also an error if a cell count value marked as final in `x_result` exceeds its
     prescribed upper bound from `neuron_counts`.
 
     Args:
         x_result: see return value of :fun:`set_known_values`.
-        deltas: idem
         cell_types: list of cell type names, e.g., ["pv+", "sst+", "vip+", "gad67+"].
         hierarchy_info: data frame returned by
             :func:`atlas_densities.densities.utils.get_hierarchy_info`.
         neuron_counts: data frame with one column "cell_count" holding the neuron count each 3D
             region labeled by an integer identifier in `neuron_count.index`.
 
     Raises:
-        AtlasDensitiesError if on the the following assumptions is violated:
-        - if cell count estimate of a region is known with certainty for a given cell type,
-        then the cell count of every descendant region is also known with certainty.
-        - a cell count estimate which is given for certain does not
+        AtlasDensitiesError if a cell count estimate which is given for certain exceeds the neuron
+        count constraint.
     """
     cell_count_tolerance = 1e-2  # absolute tolerance to rule out round-off errors
-    for region_name, id_, id_set in zip(
-        deltas.index, hierarchy_info.index, hierarchy_info["descendant_id_set"]
-    ):
+    for id_ in hierarchy_info.index:
         for cell_type in cell_types:
-            if np.isfinite(deltas.loc[region_name, cell_type]):
-                for desc_id in id_set:
-                    if np.isnan(x_result.loc[desc_id, cell_type]):
-                        raise AtlasDensitiesError(
-                            f"Cell count estimate of region named '{region_name}' for cell type "
-                            f"{cell_type} was given for certain whereas the cell count of "
-                            f"descendant id {desc_id} is not certain."
-                        )
             neuron_count = neuron_counts.loc[id_, "cell_count"]
             if (
                 not np.isnan(x_result.loc[id_, cell_type])
                 and x_result.loc[id_, cell_type] > neuron_count
             ):
                 if x_result.loc[id_, cell_type] <= neuron_count + cell_count_tolerance:
                     x_result.loc[id_, cell_type] = neuron_count
@@ -658,33 +732,33 @@
 
     Raises:
         AtlasDensitiesError if some inconsistency in the input data has been detected or if the
         linear program cannot be solved.
     """
 
     hierarchy_info = utils.get_hierarchy_info(RegionMap.from_dict(hierarchy), root=region_name)
-    average_densities = resize_average_densities(average_densities, hierarchy_info)
-
-    L.info("Initialization of the linear program: started")
-    region_counts, id_counts = _compute_initial_cell_counts(
-        annotation, voxel_volume, average_densities, hierarchy_info
-    )
+    average_densities = _resize_average_densities(average_densities, hierarchy_info)
 
     L.info("Retrieving overall neuron counts in atomic 3D regions ...")
     neuron_counts = _compute_region_cell_counts(
-        annotation, neuron_density, voxel_volume, hierarchy_info, with_descendants=False
+        annotation, neuron_density, voxel_volume, hierarchy_info
     )
     assert np.all(neuron_counts["cell_count"] >= 0.0)
 
+    L.info("Initialization of the linear program: started")
+    region_counts, id_counts = _compute_initial_cell_counts(
+        annotation, voxel_volume, average_densities, hierarchy_info
+    )
+
     L.info("Setting the known values ...")
     x_result, deltas = set_known_values(region_counts, id_counts, hierarchy_info)
     # We assume that if the cell count of `cell_type` in `region_name` is known with certainty
     # then the same holds in every descendant subregion.
     _check_variables_consistency(
-        x_result, deltas, get_cell_types(region_counts), neuron_counts, hierarchy_info
+        x_result, get_cell_types(region_counts), neuron_counts, hierarchy_info
     )
 
     L.info("Setting variable bounds and further inequality constraints ...")
     bounds, x_map, deltas_map = create_bounds(x_result, deltas, neuron_counts)
     variable_count = len(x_map) + len(deltas_map)
     assert set(x_map.values()) == set(range(len(x_map)))
     assert set(deltas_map.values()) == set(range(len(x_map), variable_count))
@@ -708,15 +782,15 @@
             variable_count,
             len(b_ub),
         )
         result = linprog(
             c=c_row,
             A_ub=a_ub,
             b_ub=b_ub,
-            bounds=replace_inf_with_none(bounds),
+            bounds=_replace_inf_with_none(bounds),
             method="highs",
         )
         if not result.success:
             raise AtlasDensitiesError(
                 "The linear program minimizing the distances to cell count estimates couldn't "
                 "be solved."
             )
```

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/inhibitory_neuron_density.py` & `atlas-densities-0.2.4/atlas_densities/densities/inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/measurement_to_density.py` & `atlas-densities-0.2.4/atlas_densities/densities/measurement_to_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
              brain region                    cell density
         5    Basic cell groups and regions   0.005
         123  Cerebrum                        0.001
         ...  ...                             ...
         The index is the sorted list of all region identifiers.
     """
     densities = []
-    descendants = hierarchy_info["descendant_id_set"]
+    descendants = hierarchy_info["descendant_ids"]
     for iset_ in tqdm(range(len(descendants))):
         mask = np.isin(annotation, list(descendants.iloc[iset_]))
         densities.append(np.sum(cell_density[mask]) / np.count_nonzero(mask))
 
     return pd.DataFrame(
         {"brain_region": hierarchy_info["brain_region"], "cell density": densities},
         index=hierarchy_info.index,
@@ -241,15 +241,15 @@
     )  # Expected: 2 resp. 5 for the usual 25um and 10um AIBS resolutions.
     mask_50um = (measurements["measurement_type"] == "cell count per slice") & (
         measurements["measurement_unit"] == "number of cells per 50-micrometer-thick slice"
     )
     cell_counts_per_slice = measurements[mask_50um]
     hierarchy_info = hierarchy_info.set_index("brain_region")
     for index, row in cell_counts_per_slice.iterrows():
-        id_set = hierarchy_info.loc[row["brain_region"], "descendant_id_set"]
+        id_set = hierarchy_info.loc[row["brain_region"], "descendant_ids"]
         average_slice_volume = voxel_volume * get_average_voxel_count_per_slice(
             id_set, annotation, thickness
         )
         cell_counts_per_slice.at[index, "measurement"] /= average_slice_volume
         cell_counts_per_slice.at[index, "standard_deviation"] /= average_slice_volume
         cell_counts_per_slice.at[index, "measurement_type"] = "cell density"
         cell_counts_per_slice.at[index, "measurement_unit"] = "number of cells per mm^3"
```

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_composition.py` & `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/create.py` & `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import numpy as np
 from atlas_commons.typing import FloatArray
 from joblib import Parallel, delayed
 from tqdm import tqdm
+from voxcell.voxel_data import ValueToIndexVoxels
 
 from atlas_densities.densities.mtype_densities_from_map.utils import (
     _check_probability_map_consistency,
     _merge_probability_maps,
 )
 from atlas_densities.exceptions import AtlasDensitiesError
 
@@ -91,42 +92,45 @@
     # get info on regions
     region_info = (
         region_map.as_dataframe()
         .reset_index()
         .set_index("acronym")
         .loc[probability_map.index.get_level_values("region")]
         .reset_index()[["region", "id"]]
+        .drop_duplicates(subset="region")
+        .reset_index(drop=True)
     )
-    region_acronyms = set(region_info.region)
-
-    region_masks = {
-        region_acronym: annotation.raw == region_id
-        for _, region_acronym, region_id in region_info.itertuples()
-    }
+    annotation_index = ValueToIndexVoxels(annotation.raw)
 
     # ensure output directory exists
     Path(output_dirpath).mkdir(exist_ok=True, parents=True)
 
     def _create_densities_for_metype(metype: str) -> Optional[Tuple[str, str]]:
         coefficients: Dict[str, Dict[str, Any]] = {}
-        for region_acronym in region_acronyms:
+        for region_acronym in region_info.region:
             coefficients[region_acronym] = {
                 molecular_type: probability_map.at[(region_acronym, molecular_type), metype]
                 for molecular_type in list(molecular_type_densities.keys())
                 if (region_acronym, molecular_type) in probability_map.index
             }
 
-        metype_density = np.zeros(annotation.shape, dtype=float)
-        for region_acronym in region_acronyms:
-            region_mask = region_masks[region_acronym]
+        # perform the manipulation in the 1d flat array
+        metype_density = np.zeros(np.prod(annotation.shape), dtype=float)
+
+        for region_acronym, region_id in region_info.itertuples(index=False):
+
+            region_indices = annotation_index.value_to_1d_indices(region_id)
             for molecular_type, coefficient in coefficients[region_acronym].items():
                 if coefficient <= 0.0:
                     continue
-                density = molecular_type_densities[molecular_type]
-                metype_density[region_mask] += density[region_mask] * coefficient
+                density = annotation_index.ravel(molecular_type_densities[molecular_type])
+                metype_density[region_indices] += density[region_indices] * coefficient
+
+        # reshape the 1d metype_density array back to the annotation's shape
+        metype_density = annotation_index.unravel(metype_density)
 
         if np.any(metype_density):
             # save density file
             metype_filename = f"{metype}_{synapse_class}_densities.nrrd"
             filepath = str(Path(output_dirpath) / metype_filename)
             annotation.with_data(metype_density).save_nrrd(filepath)
```

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_map/utils.py` & `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_map/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/mtype_densities_from_profiles.py` & `atlas-densities-0.2.4/atlas_densities/densities/mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/refined_inhibitory_neuron_densities.py` & `atlas-densities-0.2.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 The algorithm is presented in "Atlas of inhibitory neurons in the mouse brain" by D. Dimitri
 Rodarie et al., to appear in <journal>.
 
 This code supersedes the inhibitory_neuron_densities module, which is maintained to allow
 comparisons with the former approach of "A Cell Atlas for the Mouse Brain" by C. Eroe et
 al., 2018.
 """
+from __future__ import annotations
 
 import copy
 import logging
 from typing import TYPE_CHECKING, Dict, List
 
 import numpy as np
 from atlas_commons.typing import AnnotationT, BoolArray, FloatArray
 from tqdm import tqdm
 from voxcell import RegionMap
 
 from atlas_densities.densities.inhibitory_neuron_densities_helper import (
     average_densities_to_cell_counts,
+    get_cell_types,
 )
 from atlas_densities.densities.utils import compute_region_volumes, get_hierarchy_info
 
 if TYPE_CHECKING:  # pragma: no cover
     import pandas as pd
 
 L = logging.getLogger(__name__)
@@ -364,15 +366,15 @@
 
 
 def create_inhibitory_neuron_densities(  # pylint: disable=too-many-locals
     hierarchy: dict,
     annotation: AnnotationT,
     voxel_volume: float,
     neuron_density: FloatArray,
-    average_densities: "pd.DataFrame",
+    average_densities: pd.DataFrame,
     region_name: str = "root",
 ) -> Dict[str, FloatArray]:
     """
     Create a 3D float array for each cell type labelling the columns of `average_densities`.
 
     Voxel values are cell density values expressed in number of cells per mm^3.
     For a given `annotation` array, a non-zero annotated voxel
@@ -424,23 +426,23 @@
     L.info("Computing region volumes ...")
     volumes = compute_region_volumes(annotation, voxel_volume, hierarchy_info)
 
     # We compute cell counts from average densities as we will
     # modify cell densities recursively starting from the leaves
     L.info("Computing region cell counts ...")
     region_counts = average_densities_to_cell_counts(average_densities, volumes)
-    cell_types = {column.replace("_standard_deviation", "") for column in region_counts.columns}
+    cell_types = get_cell_types(region_counts)
 
     density_helper = VolumetricDensityHelper(
         annotation,
         voxel_volume,
         neuron_density,
         region_counts,
         "gad67+",
-        list(cell_types - {"gad67+"}),
+        list(set(cell_types) - {"gad67+"}),
     )
 
     L.info("Making leaf region cell counts consistent ...")
     leaf_ids = [id_ for id_ in hierarchy_info.index if region_map.is_leaf_id(id_)]
     hierarchy_leaf_info = hierarchy_info[hierarchy_info.index.isin(leaf_ids)]
     leaf_region_counts = density_helper.compute_consistent_leaf_counts(hierarchy_leaf_info)
     L.info("Making remaining region cell counts consistent ...")
```

### Comparing `atlas-densities-0.2.3/atlas_densities/densities/utils.py` & `atlas-densities-0.2.4/atlas_densities/densities/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 import scipy.misc
 import scipy.ndimage
 from atlas_commons.typing import AnnotationT, BoolArray, FloatArray
-from tqdm import tqdm
 
 from atlas_densities.exceptions import AtlasDensitiesError, AtlasDensitiesWarning
 from atlas_densities.utils import copy_array
 
 if TYPE_CHECKING:  # pragma: no cover
     from voxcell import RegionMap  # type: ignore
 
@@ -64,19 +63,19 @@
         copy: If True, a deepcopy of the input is normalized and returned. Otherwise, the input is
              normalized in place. Defaults to True.
 
     Returns:
         3D array, the normalized marker intensity array.
     """
 
-    outside_mean = np.mean(
-        marker_intensity[np.logical_and((annotation == region_id), (marker_intensity > 0.0))]
-    )
     output_intensity = copy_array(marker_intensity, copy=copy)
-    output_intensity -= outside_mean * threshold_scale_factor
+    mask_low_filter = np.logical_and((annotation == region_id), (marker_intensity > 0.0))
+    if np.any(mask_low_filter):
+        outside_mean = np.mean(marker_intensity[mask_low_filter])
+        output_intensity -= outside_mean * threshold_scale_factor
     output_intensity[output_intensity < 0.0] = 0.0
     max_intensity = np.max(output_intensity)
     if max_intensity > 0:
         output_intensity /= max_intensity
     else:
         warn(
             f"The thresholding of the dataset according to the intensity in region id={region_id} "
@@ -401,24 +400,23 @@
         assert name not in groups
         groups[name] = materialize(node)
 
     return groups
 
 
 def get_group_ids(region_map: "RegionMap", config: dict, _skip_check=False) -> dict[str, set[int]]:
-
     """
     Get AIBS structure ids for several region groups of interest.
 
     The groups below have been selected because specific count information is available
     in the scientific literature.
 
     Args:
         region_map: object to navigate the mouse brain regions hierarchy
-            (instantied from AIBS 1.json).
+            (instantiated from AIBS 1.json).
         config: mapping of regions to their constituent ids
     Returns:
         A dictionary whose keys are region group names and whose values are
         sets of structure identifiers.
     """
     ret = _interpret_region_groups(region_map, config)
     if not _skip_check:
@@ -455,45 +453,43 @@
 
 
 def get_hierarchy_info(
     region_map: "RegionMap",
     root: str = "Basic cell groups and regions",
 ) -> "pd.DataFrame":
     """
-    Returns the name and the descendant_id_set of each region that can be found by `region_map`.
+    Returns the name and the descendant_ids of each region that can be found by `region_map`.
 
     Note: We assume that the hierarchy file has unique brain region names.
 
     Args:
         region_map: RegionMap object to navigate the brain regions hierarchy.
         root: (Optional) root of the hierarchy tree used by `region_map`. Defaults to
             "Basic cell groups and regions" which corresponds to the AIBS whole mouse
             brain in AIBS 1.json.
 
     Returns:
         returns a dataframe with index a list of unique region ids and two columns
         (values are fake)
-                 descendant_id_set    brain_region
+                 descendant_ids    brain_region
             1    {1, 3}               "Cerebellum"
             2    {2, 4, 10}           "Isocortex"
                  ...             ...
         The index consists in the sorted list of the identifiers of every region recorded in
-        `region_map` under root. The column `descendant_id_set` holds for each region the set of
+        `region_map` under root. The column `descendant_ids` holds for each region the set of
         identifiers of the descendants including the region itself. `brain region` is the list of
         every region name.
 
     """
     region_ids = list(region_map.find(root, attr="name", with_descendants=True))
     region_ids.sort()
-    descendant_id_sets = [
-        region_map.find(id_, attr="id", with_descendants=True) for id_ in region_ids
-    ]
+    descendant_ids = [region_map.find(id_, attr="id", with_descendants=True) for id_ in region_ids]
     region_names = [region_map.get(id_, attr="name") for id_ in region_ids]
     data_frame = pd.DataFrame(
-        {"brain_region": region_names, "descendant_id_set": descendant_id_sets},
+        {"brain_region": region_names, "descendant_ids": descendant_ids},
         index=region_ids,
     )
 
     return data_frame
 
 
 def compute_region_volumes(
@@ -521,27 +517,26 @@
              ...                             ...
         The index is the sorted list of all region identifiers.
         The column `id_volume` holds the volumes of the brain regions of `annotation`
         which are labeled by a single identifier (descendant subregions are excluded).
         The latter column is created only if `hierarchy_info` has no `id_set` column,
         in which case its index is made of unique integer identifiers.
     """
-    id_volumes = []
-    for id_ in tqdm(hierarchy_info.index):
-        id_volumes.append(np.count_nonzero(annotation == id_) * voxel_volume)
-
     result = pd.DataFrame(
         {
             "brain_region": hierarchy_info["brain_region"],
-            "id_volume": id_volumes,
+            "id_volume": 0.0,
         },
         index=hierarchy_info.index,
     )
 
+    ids, counts = np.unique(annotation, return_counts=True)
+    result["id_volume"] = pd.Series(counts * voxel_volume, index=ids)
+
     volumes = []
-    for id_ in tqdm(hierarchy_info.index):
-        id_set = hierarchy_info.loc[id_, "descendant_id_set"]
+    for id_ in hierarchy_info.index:
+        id_set = hierarchy_info.loc[id_, "descendant_ids"]
         volume = result.loc[list(id_set), "id_volume"].sum()
         volumes.append(volume)
     result["volume"] = volumes
 
     return result
```

### Comparing `atlas-densities-0.2.3/atlas_densities/utils.py` & `atlas-densities-0.2.4/atlas_densities/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/atlas_densities.egg-info/PKG-INFO` & `atlas-densities-0.2.4/atlas_densities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.2.3
+Version: 0.2.4
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: |banner|
         
@@ -269,16 +269,19 @@
         We fit here transfer functions that describe the relation between mean ISH expression in regions of
         the mouse brain and literature regional density estimates (see `Rodarie et al. (2022)`_ for more
         details). This step leverages AIBS ISH marker datasets (in their expression form, see also
         `fit_average_densities_ccfv2_config.yaml`_) and the previously computed
         literature density values.
         These transfer functions are used to obtain first estimates of neuron densities in regions not
         covered by literature.
-        The result of the following command is a list of first density estimates for each neuron type and
-        for each region of the annotation volume.
+        
+        The results of the following command includes a csv file (`first_estimates.csv`) storing the list
+        of first density estimates for each neuron type and for each region of the annotation volume.
+        The `fitting.json` output file contains the coefficients fitted by the algorithm together with their
+        respective standard deviation and `coefficient of determination`_ (`r_square`).
         
         .. code-block:: bash
         
             # make output folder
             mkdir -p data/ccfv2/first_estimates
         
             atlas-densities cell-densities fit-average-densities                                            \
@@ -436,15 +439,15 @@
         
         The development of this software was supported by funding to the Blue Brain Project, a research
         center of the École polytechnique fédérale de Lausanne (EPFL), from the Swiss government’s ETH Board
         of the Swiss Federal Institutes of Technology.
         
         For license and authors, see LICENSE.txt and AUTHORS.txt respectively.
         
-        Copyright © 2022 Blue Brain Project/EPFL
+        Copyright (c) 2022-2024 Blue Brain Project/EPFL
         
         .. _`Allen Institute for Brain Science (AIBS)`: https://alleninstitute.org/what-we-do/brain-science/
         .. _`Eroe et al. (2018)`: https://www.frontiersin.org/articles/10.3389/fninf.2018.00084/full
         .. _`Kim et al. (2017)`: https://www.sciencedirect.com/science/article/pii/S0092867417310693
         .. _`Markram et al. (2015)`: https://www.cell.com/cell/fulltext/S0092-8674(15)01191-5
         .. _`Rodarie et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010739
         .. _`Roussel et al. (2022)`: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010058
@@ -453,14 +456,15 @@
         .. _`DeepAtlas`: https://github.com/BlueBrain/Deep-Atlas
         .. _`fit_average_densities_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
         .. _`combine_markers_ccfv2_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
         .. _`mmc1.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc1.xlsx
         .. _`mmc3.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/mmc3.xlsx
         .. _`gaba_papers.xlsx`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/measurements/gaba_papers.xlsx
         .. _`mtypes_probability_map_config.yaml`: https://github.com/BlueBrain/atlas-densities/blob/main/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+        .. _`coefficient of determination`: https://en.wikipedia.org/wiki/Coefficient_of_determination
         
         .. substitutions
         
         .. |banner| image:: doc/source/static/atlas-densities.jpg
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `atlas-densities-0.2.3/atlas_densities.egg-info/SOURCES.txt` & `atlas-densities-0.2.4/atlas_densities.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 doc/source/readme.rst
 doc/source/static/atlas-densities.jpg
 tests/1.json
 tests/__init__.py
 tests/markers_config.yaml
 tests/mocking_tools.py
 tests/test_utils.py
+tests/utils.py
 tests/app/__init__.py
 tests/app/test_cell_densities.py
 tests/app/test_combination.py
 tests/app/test_mtype_densities.py
 tests/app/test_refined_inhibitory_neuron_densities.py
 tests/combination/__init__.py
 tests/combination/test_annotations_combinator.py
```

### Comparing `atlas-densities-0.2.3/doc/Makefile` & `atlas-densities-0.2.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/doc/source/bbpp82_628_linear_program.pdf` & `atlas-densities-0.2.4/doc/source/bbpp82_628_linear_program.pdf`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/doc/source/conf.py` & `atlas-densities-0.2.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/doc/source/index.rst` & `atlas-densities-0.2.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/doc/source/static/atlas-densities.jpg` & `atlas-densities-0.2.4/doc/source/static/atlas-densities.jpg`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/setup.py` & `atlas-densities-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "openpyxl>=3.0.3",
         "pandas>=1.0.3",
         "PyYAML>=5.3.1",
         # Since version 1.6.0, scipy.optimize.linprog has fast, new methods for large, sparse problems
         # from the HiGHS library. We use the "highs" method in the densities module.
         "scipy>=1.6.0",
         "tqdm>=4.44.1",
-        "voxcell>=3.0.0",
+        "voxcell>=3.1.8",  # ValueToIndexVoxels ravel/unravel
     ],
     extras_require={
         "tests": [
             "pytest>=4.4.0",
         ],
     },
     packages=find_packages(),
```

### Comparing `atlas-densities-0.2.3/tests/1.json` & `atlas-densities-0.2.4/tests/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/app/test_cell_densities.py` & `atlas-densities-0.2.4/tests/app/test_cell_densities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """test cell_densities"""
+
 import json
 from pathlib import Path
 
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import pandas.testing as pdt
@@ -29,36 +30,21 @@
 from tests.densities.test_inhibitory_neuron_density import get_inhibitory_neuron_input_data
 from tests.densities.test_measurement_to_density import (
     get_expected_output as get_average_densities_expected_output,
 )
 from tests.densities.test_measurement_to_density import (
     get_input_data as get_measurement_to_density_input_data,
 )
+from tests.utils import write_json
 
 TEST_PATH = Path(__file__).parent.parent
 DATA_PATH = TEST_PATH.parent / "atlas_densities" / "app" / "data"
 MEASUREMENTS_PATH = DATA_PATH / "measurements"
 
 
-def _get_cell_density_result(runner):
-    args = [
-        "cell-density",
-        "--hierarchy-path",
-        str(Path(TEST_PATH, "1.json")),
-        "--annotation-path",
-        "annotation.nrrd",
-        "--nissl-path",
-        "nissl.nrrd",
-        "--output-path",
-        "overall_cell_density.nrrd",
-    ]
-
-    return runner.invoke(tested.app, args)
-
-
 def test_cell_density():
     input_ = {
         "annotation": np.array(
             [
                 [[512, 512, 1143]],
                 [[512, 512, 1143]],
                 [[477, 56, 485]],
@@ -73,53 +59,54 @@
         ),
     }
     voxel_dimensions = [25] * 3
     runner = CliRunner()
     with runner.isolated_filesystem():
         for name, array in input_.items():
             VoxelData(array, voxel_dimensions=voxel_dimensions).save_nrrd(f"{name}.nrrd")
-        result = _get_cell_density_result(runner)
+
+        args = [
+            # fmt: off
+            "cell-density",
+            "--hierarchy-path", TEST_PATH / "1.json",
+            "--annotation-path", "annotation.nrrd",
+            "--nissl-path", "nissl.nrrd",
+            "--output-path", "overall_cell_density.nrrd",
+            # fmt: on
+        ]
+
+        result = runner.invoke(tested.app, args)
 
         assert result.exit_code == 0
+
         voxel_data = VoxelData.load_nrrd("overall_cell_density.nrrd")
         assert voxel_data.raw.dtype == float
 
         # An error should be raised if annotation and nissl don't use the same voxel dimensions
         VoxelData(np.ones((3, 1, 3)), voxel_dimensions=[10] * 3).save_nrrd("nissl.nrrd")
-        result = _get_cell_density_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "voxel_dimensions" in str(result.exception)
 
 
-def _get_glia_cell_densities_result(runner):
+def test_glia_cell_densities():
     args = [
+        # fmt: off
         "glia-cell-densities",
-        "--annotation-path",
-        "annotation.nrrd",
-        "--hierarchy-path",
-        str(Path(TEST_PATH, "1.json")),
-        "--cell-density-path",
-        "cell_density.nrrd",
-        "--glia-density-path",
-        "glia_density.nrrd",
-        "--astrocyte-density-path",
-        "astrocyte_density.nrrd",
-        "--oligodendrocyte-density-path",
-        "oligodendrocyte_density.nrrd",
-        "--microglia-density-path",
-        "microglia_density.nrrd",
-        "--glia-proportions-path",
-        "glia_proportions.json",
-        "--output-dir",
-        "densities",
+        "--annotation-path", "annotation.nrrd",
+        "--hierarchy-path", TEST_PATH / "1.json",
+        "--cell-density-path", "cell_density.nrrd",
+        "--glia-density-path", "glia_density.nrrd",
+        "--astrocyte-density-path", "astrocyte_density.nrrd",
+        "--oligodendrocyte-density-path", "oligodendrocyte_density.nrrd",
+        "--microglia-density-path", "microglia_density.nrrd",
+        "--glia-proportions-path", "glia_proportions.json",
+        "--output-dir", "densities",
+        # fmt: on
     ]
 
-    return runner.invoke(tested.app, args)
-
-
-def test_glia_cell_densities():
     glia_cell_count = sum(glia_cell_counts().values())
     input_ = get_glia_input_data(glia_cell_count)
     runner = CliRunner()
     with runner.isolated_filesystem():
         voxel_dimensions = (25, 25, 25)
         VoxelData(input_["annotation"], voxel_dimensions=voxel_dimensions).save_nrrd(
             "annotation.nrrd"
@@ -127,120 +114,108 @@
         VoxelData(input_["cell_density"], voxel_dimensions=voxel_dimensions).save_nrrd(
             "cell_density.nrrd"
         )
         for glia_type, unconstrained_density in input_["glia_densities"].items():
             VoxelData(unconstrained_density, voxel_dimensions=voxel_dimensions).save_nrrd(
                 glia_type + "_density.nrrd"
             )
-        with open("glia_proportions.json", "w", encoding="utf-8") as out:
-            json.dump(input_["glia_proportions"], out)
-        result = _get_glia_cell_densities_result(runner)
+
+        write_json("glia_proportions.json", input_["glia_proportions"])
+
+        result = runner.invoke(tested.app, args)
         assert result.exit_code == 0
 
         neuron_density = VoxelData.load_nrrd("densities/neuron_density.nrrd")
         assert neuron_density.raw.dtype == np.float64
-        npt.assert_array_equal(neuron_density.shape, input_["annotation"].shape)
+        assert neuron_density.shape == input_["annotation"].shape
         assert np.all(neuron_density.raw >= 0.0)
 
         oligodendrocyte_density = VoxelData.load_nrrd("densities/oligodendrocyte_density.nrrd")
         assert oligodendrocyte_density.raw.dtype == np.float64
-        npt.assert_array_equal(neuron_density.shape, input_["annotation"].shape)
+        assert neuron_density.shape == input_["annotation"].shape
 
         # Check that an exception is thrown if voxel dimensions aren't consistent
         VoxelData(input_["cell_density"], voxel_dimensions=(10, 10, 10)).save_nrrd(
             "cell_density.nrrd"
         )
-        result = _get_glia_cell_densities_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "voxel_dimensions" in str(result.exception)
 
         # Check that an exception is thrown if the input cell density has negative values
         input_["cell_density"][0, 0, 0] = -1.0
         VoxelData(input_["cell_density"], voxel_dimensions=(10, 10, 10)).save_nrrd(
             "cell_density.nrrd"
         )
-        result = _get_glia_cell_densities_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "Negative density value" in str(result.exception)
 
 
-def _get_inh_and_exc_neuron_densities_result(runner):
+def test_inhibitory_and_excitatory_neuron_densities():
     args = [
+        # fmt: off
         "inhibitory-and-excitatory-neuron-densities",
-        "--annotation-path",
-        "annotation.nrrd",
-        "--hierarchy-path",
-        str(Path(TEST_PATH, "1.json")),
-        "--gad1-path",
-        "gad1.nrrd",
-        "--nrn1-path",
-        "nrn1.nrrd",
-        "--neuron-density-path",
-        "neuron_density.nrrd",
-        "--output-dir",
-        "densities",
+        "--annotation-path", "annotation.nrrd",
+        "--hierarchy-path", TEST_PATH / "1.json",
+        "--gad1-path", "gad1.nrrd",
+        "--nrn1-path", "nrn1.nrrd",
+        "--neuron-density-path", "neuron_density.nrrd",
+        "--output-dir", "densities",
+        # fmt: on
     ]
 
-    return runner.invoke(tested.app, args)
-
-
-def test_inhibitory_and_excitatory_neuron_densities():
     inhibitory_df = extract_inhibitory_neurons_dataframe(Path(MEASUREMENTS_PATH, "mmc1.xlsx"))
     neuron_count = inhibitory_data(inhibitory_df)["neuron_count"]
     input_ = get_inhibitory_neuron_input_data(neuron_count)
     runner = CliRunner()
     with runner.isolated_filesystem():
         voxel_dimensions = (25, 25, 25)
         for name in ["annotation", "neuron_density", "gad1", "nrn1"]:
             VoxelData(input_[name], voxel_dimensions=voxel_dimensions).save_nrrd(name + ".nrrd")
 
-        result = _get_inh_and_exc_neuron_densities_result(runner)
+        result = runner.invoke(tested.app, args)
         assert result.exit_code == 0
 
         inh_neuron_density = VoxelData.load_nrrd("densities/inhibitory_neuron_density.nrrd")
         assert inh_neuron_density.raw.dtype == np.float64
-        npt.assert_array_equal(inh_neuron_density.shape, input_["annotation"].shape)
+        assert inh_neuron_density.shape == input_["annotation"].shape
         assert np.all(inh_neuron_density.raw >= 0.0)
 
         exc_neuron_density = VoxelData.load_nrrd("densities/excitatory_neuron_density.nrrd")
         assert exc_neuron_density.raw.dtype == np.float64
-        npt.assert_array_equal(exc_neuron_density.shape, input_["annotation"].shape)
+        assert exc_neuron_density.shape == input_["annotation"].shape
         assert np.all(exc_neuron_density.raw >= 0.0)
 
         # Check that an exception is thrown if voxel dimensions aren't consistent
         VoxelData(input_["neuron_density"], voxel_dimensions=(10, 10, 10)).save_nrrd(
             "neuron_density.nrrd"
         )
-        result = _get_inh_and_exc_neuron_densities_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "voxel_dimensions" in str(result.exception)
 
         # Check that an exception is thrown if the input neuron density has negative values
         input_["neuron_density"][0, 0, 0] = -1.0
         VoxelData(input_["neuron_density"], voxel_dimensions=(25, 25, 25)).save_nrrd(
             "neuron_density.nrrd"
         )
-        result = _get_inh_and_exc_neuron_densities_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "Negative density value" in str(result.exception)
 
 
-def _get_compile_measurements_result(runner):
+@pytest.mark.filterwarnings("ignore::atlas_densities.exceptions.AtlasDensitiesWarning")
+def test_compile_measurements():
     args = [
+        # fmt: off
         "compile-measurements",
-        "--measurements-output-path",
-        "measurements.csv",
-        "--homogenous-regions-output-path",
-        "homogenous_regions.csv",
+        "--measurements-output-path", "measurements.csv",
+        "--homogenous-regions-output-path", "homogenous_regions.csv",
+        # fmt: on
     ]
-
-    return runner.invoke(tested.app, args)
-
-
-@pytest.mark.filterwarnings("ignore::atlas_densities.exceptions.AtlasDensitiesWarning")
-def test_compile_measurements():
     runner = CliRunner()
     with runner.isolated_filesystem():
-        result = _get_compile_measurements_result(runner)
+        result = runner.invoke(tested.app, args)
         assert result.exit_code == 0
 
         dataframe = pd.read_csv("measurements.csv")
 
         assert get_invalid_region_names(dataframe) == {
             "Nucleus of reunions",
             "Nucleus accumbens, core",
@@ -262,44 +237,38 @@
 
         dataframe = pd.read_csv("homogenous_regions.csv")
         assert set(dataframe["cell_type"]) == {"inhibitory", "excitatory"}
 
 
 def _get_measurements_to_average_densities_result(runner, hierarchy_path, measurements_path):
     args = [
+        # fmt: off
         "measurements-to-average-densities",
-        "--hierarchy-path",
-        hierarchy_path,
-        "--annotation-path",
-        "annotation.nrrd",
-        "--region-name",
-        "Basic cell groups and regions",
-        "--cell-density-path",
-        "cell_density.nrrd",
-        "--neuron-density-path",
-        "neuron_density.nrrd",
-        "--measurements-path",
-        measurements_path,
-        "--output-path",
-        "average_densities.csv",
+        "--hierarchy-path", hierarchy_path,
+        "--annotation-path", "annotation.nrrd",
+        "--region-name", "Basic cell groups and regions",
+        "--cell-density-path", "cell_density.nrrd",
+        "--neuron-density-path", "neuron_density.nrrd",
+        "--measurements-path", measurements_path,
+        "--output-path", "average_densities.csv",
+        # fmt: on
     ]
 
     return runner.invoke(tested.app, args)
 
 
 def test_measurements_to_average_densities():
     runner = CliRunner()
     with runner.isolated_filesystem():
         input_ = get_measurement_to_density_input_data()
         voxel_dimensions = input_["voxel_dimensions"]
         for name in ["annotation", "cell_density", "neuron_density"]:
             VoxelData(input_[name], voxel_dimensions=voxel_dimensions).save_nrrd(name + ".nrrd")
         input_["measurements"].to_csv("measurements.csv", index=False)
-        with open("hierarchy.json", "w", encoding="utf-8") as out:
-            json.dump(input_["hierarchy"], out, indent=1, separators=(",", ": "))
+        write_json("hierarchy.json", input_["hierarchy"])
 
         result = _get_measurements_to_average_densities_result(
             runner, hierarchy_path="hierarchy.json", measurements_path="measurements.csv"
         )
 
         assert result.exit_code == 0
 
@@ -315,75 +284,65 @@
         )
         assert result.exit_code == 0
         actual = pd.read_csv("average_densities.csv")
         assert np.all(actual["measurement_type"] == "cell density")
         assert np.all(actual["measurement_unit"] == "number of cells per mm^3")
 
 
-def _get_fitting_result(runner):
+@pytest.mark.filterwarnings("ignore::atlas_densities.exceptions.AtlasDensitiesWarning")
+def test_fit_average_densities():
     args = [
+        # fmt: off
         "fit-average-densities",
-        "--hierarchy-path",
-        "hierarchy.json",
-        "--annotation-path",
-        "annotation.nrrd",
-        "--neuron-density-path",
-        "neuron_density.nrrd",
-        "--gene-config-path",
-        "gene_config.yaml",
-        "--average-densities-path",
-        "average_densities.csv",
-        "--homogenous-regions-path",
-        "homogenous_regions.csv",
-        "--fitted-densities-output-path",
-        "fitted_densities.csv",
-        "--fitting-maps-output-path",
-        "fitting_maps.json",
+        "--hierarchy-path", "hierarchy.json",
+        "--annotation-path", "annotation.nrrd",
+        "--neuron-density-path", "neuron_density.nrrd",
+        "--gene-config-path", "gene_config.yaml",
+        "--average-densities-path", "average_densities.csv",
+        "--homogenous-regions-path", "homogenous_regions.csv",
+        "--fitted-densities-output-path", "fitted_densities.csv",
+        "--fitting-maps-output-path", "fitting_maps.json",
+        # fmt: on
     ]
-
-    return runner.invoke(tested.app, args)
-
-
-@pytest.mark.filterwarnings("ignore::atlas_densities.exceptions.AtlasDensitiesWarning")
-def test_fit_average_densities():
     runner = CliRunner()
     with runner.isolated_filesystem():
         input_ = get_fitting_input_data()
+        input_["gene_marker_volumes"]["gad67"]["slices"] = [-1]  # force offset
+        input_["realigned_slices"][input_["slice_map"]["gad67"]] = [-1]
         for name in ["annotation", "neuron_density"]:
-            VoxelData(input_[name], voxel_dimensions=[25.0] * 3).save_nrrd(name + ".nrrd")
+            VoxelData(
+                input_[name], voxel_dimensions=[25.0] * 3, offset=(-50.0, 100.0, -450.0)
+            ).save_nrrd(name + ".nrrd")
 
         input_["homogenous_regions"].to_csv("homogenous_regions.csv", index=False)
         input_["average_densities"].to_csv("average_densities.csv", index=False)
 
-        with open("hierarchy.json", "w", encoding="utf-8") as out:
-            json.dump(input_["hierarchy"], out, indent=1, separators=(",", ": "))
-
-        with open("realigned_slices.json", "w", encoding="utf-8") as out:
-            json.dump(input_["realigned_slices"], out, indent=1, separators=(",", ": "))
-
-        with open("std_cells.json", "w", encoding="utf-8") as out:
-            json.dump(input_["cell_density_stddevs"], out, indent=1, separators=(",", ": "))
+        write_json("hierarchy.json", input_["hierarchy"])
+        write_json("realigned_slices.json", input_["realigned_slices"])
+        write_json("std_cells.json", input_["cell_density_stddevs"])
 
         with open("gene_config.yaml", "w", encoding="utf-8") as out:
             gene_config = {
                 "inputGeneVolumePath": {},
                 "sectionDataSetID": {},
                 "realignedSlicesPath": "realigned_slices.json",
                 "cellDensityStandardDeviationsPath": "std_cells.json",
             }
             for marker, intensity in input_["gene_marker_volumes"].items():
-                VoxelData(intensity["intensity"], voxel_dimensions=[25.0] * 3).save_nrrd(
-                    marker + ".nrrd"
-                )
+                VoxelData(
+                    intensity["intensity"],
+                    voxel_dimensions=[25.0] * 3,
+                    offset=(-50.0, 100.0, -450.0),
+                ).save_nrrd(marker + ".nrrd")
                 gene_config["inputGeneVolumePath"][marker] = marker + ".nrrd"
                 gene_config["sectionDataSetID"][marker] = input_["slice_map"][marker]
 
             yaml.dump(gene_config, out)
 
-        result = _get_fitting_result(runner)
+        result = runner.invoke(tested.app, args)
         assert result.exit_code == 0
 
         densities = pd.read_csv("fitted_densities.csv")
         assert set(densities.columns) == {
             "brain_region",
             "gad67+",
             "gad67+_standard_deviation",
@@ -400,15 +359,15 @@
             assert np.allclose(fitting_maps["Rest"]["pv+"]["coefficient"], 2.0 / 3.0)
 
         # Check that an exception is thrown if the input neuron density has negative values
         input_["neuron_density"][0, 0, 0] = -1.0
         VoxelData(input_["neuron_density"], voxel_dimensions=(10, 10, 10)).save_nrrd(
             "neuron_density.nrrd"
         )
-        result = _get_fitting_result(runner)
+        result = runner.invoke(tested.app, args)
         assert "Negative density value" in str(result.exception)
 
 
 def test_zero_negative_values():
     array = np.array([0, 1, -0.02], dtype=float)
     with pytest.raises(
         AtlasDensitiesError,
```

### Comparing `atlas-densities-0.2.3/tests/app/test_combination.py` & `atlas-densities-0.2.4/tests/app/test_combination.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,23 +100,21 @@
     runner = CliRunner()
     with runner.isolated_filesystem() as td:
         for name, array in input_.items():
             VoxelData(array, voxel_dimensions=voxel_dimensions).save_nrrd(f"{name}.nrrd")
         result = runner.invoke(
             tested.app,
             [
-                "--log-output-path",
-                str(td),
+                # fmt: off
+                "--log-output-path", td,
                 "combine-markers",
-                "--annotation-path",
-                "annotation.nrrd",
-                "--hierarchy-path",
-                str(TEST_PATH / "1.json"),
-                "--config",
-                str(TEST_PATH / "markers_config.yaml"),
+                "--annotation-path", "annotation.nrrd",
+                "--hierarchy-path", TEST_PATH / "1.json",
+                "--config", TEST_PATH / "markers_config.yaml",
+                # fmt: on
             ],
             catch_exceptions=False,
         )
         assert result.exit_code == 0
         with open("glia_proportions.json", encoding="utf-8") as file_:
             glia_proportions = json.load(file_)
             assert glia_proportions == {
@@ -141,30 +139,25 @@
     )
     VoxelData(array, voxel_dimensions=[25] * 3).save_nrrd(nrrd)
 
     runner = CliRunner()
     result = runner.invoke(
         tested.app,
         [
+            # fmt: off
             "manipulate",
             "--clip",
-            "--base-nrrd",
-            nrrd,
-            "--add",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--add",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--output-path",
-            tmp_path / "manipulate.nrrd",
+            "--base-nrrd", nrrd,
+            "--add", nrrd,
+            "--subtract", nrrd,
+            "--add", nrrd,
+            "--subtract", nrrd,
+            "--subtract", nrrd,
+            "--output-path", tmp_path / "manipulate.nrrd",
+            # fmt: on
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     output = VoxelData.load_nrrd(tmp_path / "manipulate.nrrd")
     assert np.allclose(output.raw, 0.0)
 
@@ -180,43 +173,39 @@
     )
     VoxelData(array, voxel_dimensions=[25] * 3).save_nrrd(nrrd)
 
     runner = CliRunner()
     result = runner.invoke(
         tested.app,
         [
+            # fmt: off
             "manipulate",
             "--clip",
-            "--base-nrrd",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--output-path",
-            tmp_path / "manipulate.nrrd",
+            "--base-nrrd", nrrd,
+            "--subtract", nrrd,
+            "--subtract", nrrd,
+            "--output-path", tmp_path / "manipulate.nrrd",
+            # fmt: on
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     output = VoxelData.load_nrrd(tmp_path / "manipulate.nrrd")
     assert np.allclose(output.raw, 0.0)
 
     runner = CliRunner()
     result = runner.invoke(
         tested.app,
         [
+            # fmt: off
             "manipulate",
-            "--base-nrrd",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--subtract",
-            nrrd,
-            "--output-path",
-            tmp_path / "manipulate.nrrd",
+            "--base-nrrd", nrrd,
+            "--subtract", nrrd,
+            "--subtract", nrrd,
+            "--output-path", tmp_path / "manipulate.nrrd",
+            # fmt: on
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     output = VoxelData.load_nrrd(tmp_path / "manipulate.nrrd")
     assert np.count_nonzero(output.raw < 0) == 2
```

### Comparing `atlas-densities-0.2.3/tests/app/test_mtype_densities.py` & `atlas-densities-0.2.4/tests/app/test_mtype_densities.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,51 +19,45 @@
 from tests.densities.test_mtype_densities_from_profiles import (
     DATA_PATH,
     create_excitatory_neuron_density,
     create_expected_cell_densities,
     create_inhibitory_neuron_density,
     create_slicer_data,
 )
+from tests.utils import write_json
 
 
 def get_result_from_profiles(runner, td):
     return runner.invoke(
         tested.app,
         [
-            "--log-output-path",
-            str(td),
+            # fmt: off
+            "--log-output-path", td,
             "create-from-profile",
-            "--annotation-path",
-            "annotation.nrrd",
-            "--hierarchy-path",
-            "hierarchy.json",
-            "--metadata-path",
-            "metadata.json",
-            "--direction-vectors-path",
-            "direction_vectors.nrrd",
-            "--mtypes-config-path",
-            "config.yaml",
-            "--output-dir",
-            "output_dir",
+            "--annotation-path", "annotation.nrrd",
+            "--hierarchy-path", "hierarchy.json",
+            "--metadata-path", "metadata.json",
+            "--direction-vectors-path", "direction_vectors.nrrd",
+            "--mtypes-config-path", "config.yaml",
+            "--output-dir", "output_dir",
+            # fmt: on
         ],
     )
 
 
 def test_mtype_densities_from_profiles(tmp_path):
     runner = CliRunner()
     with runner.isolated_filesystem(temp_dir=tmp_path) as td:
         create_excitatory_neuron_density().save_nrrd("excitatory_neuron_density.nrrd")
         create_inhibitory_neuron_density().save_nrrd("inhibitory_neuron_density.nrrd")
         data = create_slicer_data()
         data["annotation"].save_nrrd("annotation.nrrd")
         data["annotation"].with_data(data["direction_vectors"]).save_nrrd("direction_vectors.nrrd")
-        with open("metadata.json", "w", encoding="utf-8") as file_:
-            json.dump(data["metadata"], file_)
-        with open("hierarchy.json", "w", encoding="utf-8") as file_:
-            json.dump(data["hierarchy"], file_)
+        write_json("metadata.json", data["metadata"])
+        write_json("hierarchy.json", data["hierarchy"])
         with open("config.yaml", "w", encoding="utf-8") as file_:
             config = {
                 "mtypeToProfileMapPath": str(DATA_PATH / "meta" / "mapping.tsv"),
                 "layerSlicesPath": str(DATA_PATH / "meta" / "layers.tsv"),
                 "densityProfilesDirPath": str(DATA_PATH / "mtypes"),
                 "excitatoryNeuronDensityPath": "excitatory_neuron_density.nrrd",
                 "inhibitoryNeuronDensityPath": "inhibitory_neuron_density.nrrd",
@@ -89,350 +83,320 @@
             yaml.dump(config, file_)
 
         result = get_result_from_profiles(runner, td)
         assert result.exit_code == 1
         assert "neuron density file" in str(result.exception)
 
 
-def get_result_from_probablity_map_(runner, td):
-    return runner.invoke(
-        tested.app,
-        [
-            "--log-output-path",
-            str(td),
-            "create-from-probability-map",
-            "--annotation-path",
-            "annotation.nrrd",
-            "--hierarchy-path",
-            "hierarchy.json",
-            "--probability-map",
-            "probability_map01.csv",
-            "--probability-map",
-            "probability_map02.csv",
-            "--marker",
-            "pv",
-            "pv.nrrd",
-            "--marker",
-            "sst",
-            "sst.nrrd",
-            "--marker",
-            "vip",
-            "vip.nrrd",
-            "--marker",
-            "gad67",
-            "gad67.nrrd",
-            "--marker",
-            "approx_lamp5",
-            "approx_lamp5.nrrd",
-            "--synapse-class",
-            "EXC",
-            "--output-dir",
-            "output_dir",
-        ],
-    )
-
-
-class Test_mtype_densities_from_probability_map:
-    def setup_method(self, method):
-        self.data = create_from_probability_map_data()
-
-    def save_input_data_to_file(self):
-        self.data["annotation"].save_nrrd("annotation.nrrd")
-        with open("hierarchy.json", "w", encoding="utf-8") as file:
-            json.dump(self.data["hierarchy"], file)
+def test_mtype_densities_from_probability_map(tmp_path):
+    data = create_from_probability_map_data()
+    runner = CliRunner()
+    with runner.isolated_filesystem(temp_dir=tmp_path) as td:
+        td = Path(td)
 
-        self.data["probability_map01"].to_csv("probability_map01.csv", index=True)
-        self.data["probability_map02"].to_csv("probability_map02.csv", index=True)
+        data["annotation"].save_nrrd(td / "annotation.nrrd")
+        write_json("hierarchy.json", data["hierarchy"])
+        data["probability_map01"].to_csv(td / "probability_map01.csv", index=True)
+        data["probability_map02"].to_csv(td / "probability_map02.csv", index=True)
 
-        for molecular_type, data in self.data["molecular_type_densities"].items():
+        for molecular_type, raw in data["molecular_type_densities"].items():
             VoxelData(
-                data,
-                voxel_dimensions=self.data["annotation"].voxel_dimensions,
-            ).save_nrrd(f"{molecular_type}.nrrd")
+                raw,
+                voxel_dimensions=data["annotation"].voxel_dimensions,
+            ).save_nrrd(td / f"{molecular_type}.nrrd")
+
+        result = runner.invoke(
+            tested.app,
+            [
+                # fmt: off
+                    "--log-output-path", str(td),
+                    "create-from-probability-map",
+                    "--annotation-path", "annotation.nrrd",
+                    "--hierarchy-path", "hierarchy.json",
+                    "--probability-map", "probability_map01.csv",
+                    "--probability-map", "probability_map02.csv",
+                    "--marker", "pv", "pv.nrrd",
+                    "--marker", "sst", "sst.nrrd",
+                    "--marker", "vip", "vip.nrrd",
+                    "--marker", "gad67", "gad67.nrrd",
+                    "--marker", "approx_lamp5", "approx_lamp5.nrrd",
+                    "--synapse-class", "EXC",
+                    "--output-dir", "output_dir",
+                # fmt: on
+            ],
+        )
+        assert result.exit_code == 0
 
-    def test_output(self, tmp_path):
-        runner = CliRunner()
-        with runner.isolated_filesystem(temp_dir=tmp_path) as td:
-            self.save_input_data_to_file()
-            result = get_result_from_probablity_map_(runner, td)
-            assert result.exit_code == 0
-
-            BPbAC = VoxelData.load_nrrd(str(Path("output_dir") / "BP|bAC_EXC_densities.nrrd"))
-            assert BPbAC.raw.dtype == float
-            npt.assert_array_equal(BPbAC.voxel_dimensions, self.data["annotation"].voxel_dimensions)
-
-            with open(str(Path("output_dir") / "metadata.json"), "r") as file:
-                metadata = json.load(file)
-            assert "BP" in metadata["density_files"]
-            assert "bAC" in metadata["density_files"]["BP"]
-            assert "EXC" == metadata["synapse_class"]
-
-    class Test_mtype_densities_from_composition:
-        @pytest.fixture(scope="session")
-        def class_tmpdir(self, tmpdir_factory):
-            """Create a session scoped temp dir using the class name"""
-            return tmpdir_factory.mktemp(type(self).__name__)
-
-        @pytest.fixture(scope="session")
-        def annotation_path(self, class_tmpdir):
-            path = class_tmpdir.join("annotation.nrrd")
-            VoxelData(
-                np.array([[[101, 102, 103, 104, 105, 106]]], dtype=np.int32),
-                voxel_dimensions=[25] * 3,
-            ).save_nrrd(str(path))
-            return path
-
-        @pytest.fixture(scope="session")
-        def hierarchy_path(self, class_tmpdir):
-            path = class_tmpdir.join("hierarchy.json")
-
-            hierarchy = {
-                "id": 315,
-                "acronym": "Isocortex",
-                "name": "Isocortex",
-                "children": [
-                    {
-                        "id": 500,
-                        "acronym": "MO",
-                        "name": "Somatomotor areas",
-                        "children": [
-                            {
-                                "id": 101,
-                                "acronym": "MO1",
-                                "name": "Somatomotor areas, Layer 1",
-                                "children": [],
-                            },
-                            {
-                                "id": 102,
-                                "acronym": "MO2",
-                                "name": "Somatomotor areas, Layer 2",
-                                "children": [],
-                            },
-                            {
-                                "id": 103,
-                                "acronym": "MO3",
-                                "name": "Somatomotor areas, Layer 3",
-                                "children": [],
-                            },
-                            {
-                                "id": 104,
-                                "acronym": "MO4",
-                                "name": "Somatomotor areas, Layer 4",
-                                "children": [],
-                            },
-                            {
-                                "id": 105,
-                                "acronym": "MO5",
-                                "name": "Somatomotor areas, layer 5",
-                                "children": [],
-                            },
-                            {
-                                "id": 106,
-                                "acronym": "MO6",
-                                "name": "Somatomotor areas, layer 6",
-                                "children": [],
-                            },
-                        ],
-                    },
-                ],
-            }
-            with open(path, "w", encoding="utf-8") as jsonfile:
-                json.dump(hierarchy, jsonfile, indent=1, separators=(",", ": "))
-            return path
-
-        @pytest.fixture(scope="session")
-        def metadata_path(self, class_tmpdir):
-            path = class_tmpdir.join("metadata.json")
-            metadata = {
-                "region": {
-                    "name": "Isocortex",
-                    "query": "Isocortex",
-                    "attribute": "acronym",
-                    "with_descendants": True,
-                },
-                "layers": {
-                    "names": ["layer_1", "layer_2", "layer_3", "layer_4", "layer_5", "layer_6"],
-                    "queries": [
-                        "@.*1[ab]?$",
-                        "@.*2[ab]?$",
-                        "@.*[^/]3[ab]?$",
-                        "@.*4[ab]?$",
-                        "@.*5[ab]?$",
-                        "@.*6[ab]?$",
+        BPbAC = VoxelData.load_nrrd(Path("output_dir") / "BP|bAC_EXC_densities.nrrd")
+        assert BPbAC.raw.dtype == float
+        npt.assert_array_equal(BPbAC.voxel_dimensions, data["annotation"].voxel_dimensions)
+
+        with open(Path("output_dir") / "metadata.json", "r") as file:
+            metadata = json.load(file)
+
+        assert "BP" in metadata["density_files"]
+        assert "bAC" in metadata["density_files"]["BP"]
+        assert "EXC" == metadata["synapse_class"]
+
+
+class Test_mtype_densities_from_composition:
+    @pytest.fixture(scope="session")
+    def class_tmpdir(self, tmpdir_factory):
+        """Create a session scoped temp dir using the class name"""
+        return tmpdir_factory.mktemp(type(self).__name__)
+
+    @pytest.fixture(scope="session")
+    def annotation_path(self, class_tmpdir):
+        path = class_tmpdir.join("annotation.nrrd")
+        VoxelData(
+            np.array([[[101, 102, 103, 104, 105, 106]]], dtype=np.int32),
+            voxel_dimensions=[25] * 3,
+        ).save_nrrd(str(path))
+        return path
+
+    @pytest.fixture(scope="session")
+    def hierarchy_path(self, class_tmpdir):
+        path = class_tmpdir.join("hierarchy.json")
+
+        hierarchy = {
+            "id": 315,
+            "acronym": "Isocortex",
+            "name": "Isocortex",
+            "children": [
+                {
+                    "id": 500,
+                    "acronym": "MO",
+                    "name": "Somatomotor areas",
+                    "children": [
+                        {
+                            "id": 101,
+                            "acronym": "MO1",
+                            "name": "Somatomotor areas, Layer 1",
+                            "children": [],
+                        },
+                        {
+                            "id": 102,
+                            "acronym": "MO2",
+                            "name": "Somatomotor areas, Layer 2",
+                            "children": [],
+                        },
+                        {
+                            "id": 103,
+                            "acronym": "MO3",
+                            "name": "Somatomotor areas, Layer 3",
+                            "children": [],
+                        },
+                        {
+                            "id": 104,
+                            "acronym": "MO4",
+                            "name": "Somatomotor areas, Layer 4",
+                            "children": [],
+                        },
+                        {
+                            "id": 105,
+                            "acronym": "MO5",
+                            "name": "Somatomotor areas, layer 5",
+                            "children": [],
+                        },
+                        {
+                            "id": 106,
+                            "acronym": "MO6",
+                            "name": "Somatomotor areas, layer 6",
+                            "children": [],
+                        },
                     ],
-                    "attribute": "acronym",
-                    "with_descendants": True,
                 },
-            }
-            with open(path, "w", encoding="utf-8") as jsonfile:
-                json.dump(metadata, jsonfile, indent=1)
-
-            return path
-
-        @pytest.fixture(scope="session")
-        def density(self):
-            return VoxelData(
-                np.array([[[0.3, 0.3, 0.3, 0.3, 0.3, 0.3]]], dtype=np.float32),
-                voxel_dimensions=[25] * 3,
-            )
-
-        @pytest.fixture(scope="session")
-        def density_path(self, density, class_tmpdir):
-            path = class_tmpdir.join("density.nrrd")
-            density.save_nrrd(str(path))
-
-            return path
-
-        @pytest.fixture(scope="session")
-        def taxonomy(self):
-            return pd.DataFrame(
+            ],
+        }
+        write_json(path, hierarchy)
+        return path
+
+    @pytest.fixture(scope="session")
+    def metadata_path(self, class_tmpdir):
+        path = class_tmpdir.join("metadata.json")
+        metadata = {
+            "region": {
+                "name": "Isocortex",
+                "query": "Isocortex",
+                "attribute": "acronym",
+                "with_descendants": True,
+            },
+            "layers": {
+                "names": ["layer_1", "layer_2", "layer_3", "layer_4", "layer_5", "layer_6"],
+                "queries": [
+                    "@.*1[ab]?$",
+                    "@.*2[ab]?$",
+                    "@.*[^/]3[ab]?$",
+                    "@.*4[ab]?$",
+                    "@.*5[ab]?$",
+                    "@.*6[ab]?$",
+                ],
+                "attribute": "acronym",
+                "with_descendants": True,
+            },
+        }
+        write_json(path, metadata)
+        return path
+
+    @pytest.fixture(scope="session")
+    def density(self):
+        return VoxelData(
+            np.array([[[0.3, 0.3, 0.3, 0.3, 0.3, 0.3]]], dtype=np.float32),
+            voxel_dimensions=[25] * 3,
+        )
+
+    @pytest.fixture(scope="session")
+    def density_path(self, density, class_tmpdir):
+        path = class_tmpdir.join("density.nrrd")
+        density.save_nrrd(str(path))
+
+        return path
+
+    @pytest.fixture(scope="session")
+    def taxonomy(self):
+        return pd.DataFrame(
+            {
+                "mtype": ["L3_TPC:A", "L3_TPC:B", "L23_MC", "L4_TPC", "L4_LBC", "L4_UPC"],
+                "mClass": ["PYR", "PYR", "INT", "PYR", "INT", "PYR"],
+                "sClass": ["EXC", "EXC", "INH", "EXC", "INH", "EXC"],
+            },
+            columns=["mtype", "mClass", "sClass"],
+        )
+
+    @pytest.fixture(scope="session")
+    def taxonomy_path(self, taxonomy, class_tmpdir):
+        """Creates a taxonomy file and returns its path"""
+        path = class_tmpdir.join("neurons-mtype-taxonomy.tsv")
+        taxonomy.to_csv(path, sep="\t")
+
+        return path
+
+    @pytest.fixture(scope="session")
+    def composition(self):
+        return pd.DataFrame(
+            {
+                "density": [51750.099, 14785.743, 2779.081, 62321.137, 2103.119, 25921.181],
+                "layer": ["layer_3", "layer_3", "layer_3", "layer_4", "layer_4", "layer_4"],
+                "mtype": ["L3_TPC:A", "L3_TPC:B", "L23_MC", "L4_TPC", "L4_LBC", "L4_UPC"],
+            },
+            columns=["density", "layer", "mtype"],
+        )
+
+    @pytest.fixture(scope="session")
+    def composition_path(self, composition, class_tmpdir):
+        path = class_tmpdir.join("composition.yaml")
+        out_dict = {"neurons": []}
+        for row in composition.itertuples():
+            out_dict["neurons"].append(
                 {
-                    "mtype": ["L3_TPC:A", "L3_TPC:B", "L23_MC", "L4_TPC", "L4_LBC", "L4_UPC"],
-                    "mClass": ["PYR", "PYR", "INT", "PYR", "INT", "PYR"],
-                    "sClass": ["EXC", "EXC", "INH", "EXC", "INH", "EXC"],
-                },
-                columns=["mtype", "mClass", "sClass"],
+                    "density": row.density,
+                    "traits": {
+                        "layer": int(row.layer.replace("layer_", "")),
+                        "mtype": row.mtype,
+                    },
+                }
             )
+        with open(path, "w", encoding="utf-8") as yaml_file:
+            yaml.dump(out_dict, yaml_file)
 
-        @pytest.fixture(scope="session")
-        def taxonomy_path(self, taxonomy, class_tmpdir):
-            """Creates a taxonomy file and returns its path"""
-            path = class_tmpdir.join("neurons-mtype-taxonomy.tsv")
-            taxonomy.to_csv(path, sep="\t")
-
-            return path
-
-        @pytest.fixture(scope="session")
-        def composition(self):
-            return pd.DataFrame(
-                {
-                    "density": [51750.099, 14785.743, 2779.081, 62321.137, 2103.119, 25921.181],
-                    "layer": ["layer_3", "layer_3", "layer_3", "layer_4", "layer_4", "layer_4"],
-                    "mtype": ["L3_TPC:A", "L3_TPC:B", "L23_MC", "L4_TPC", "L4_LBC", "L4_UPC"],
-                },
-                columns=["density", "layer", "mtype"],
-            )
+        return path
 
-        @pytest.fixture(scope="session")
-        def composition_path(self, composition, class_tmpdir):
-            path = class_tmpdir.join("composition.yaml")
-            out_dict = {"neurons": []}
-            for row in composition.itertuples():
-                out_dict["neurons"].append(
-                    {
-                        "density": row.density,
-                        "traits": {
-                            "layer": int(row.layer.replace("layer_", "")),
-                            "mtype": row.mtype,
-                        },
-                    }
-                )
-            with open(path, "w", encoding="utf-8") as yaml_file:
-                yaml.dump(out_dict, yaml_file)
-
-            return path
-
-        def test_load_neuronal_mtype_taxonomy(self, taxonomy, taxonomy_path):
-            pdt.assert_frame_equal(tested._load_neuronal_mtype_taxonomy(taxonomy_path), taxonomy)
-
-        def test_validate_mtype_taxonomy(self, taxonomy):
-            tested._validate_mtype_taxonomy(taxonomy)
-
-            wrong_taxonomy = taxonomy.rename(columns={"sClass": "John"})
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_mtype_taxonomy(wrong_taxonomy)
-
-            wrong_taxonomy = taxonomy.drop(columns=["mtype"])
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_mtype_taxonomy(wrong_taxonomy)
-
-            wrong_taxonomy = deepcopy(taxonomy)
-            wrong_taxonomy.loc[1, "sClass"] = "OTHER"
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_mtype_taxonomy(wrong_taxonomy)
-
-        def test_load_neuronal_mtype_composition(self, composition, composition_path):
-            pdt.assert_frame_equal(
-                tested._load_neuronal_mtype_composition(composition_path), composition
-            )
+    def test_load_neuronal_mtype_taxonomy(self, taxonomy, taxonomy_path):
+        pdt.assert_frame_equal(tested._load_neuronal_mtype_taxonomy(taxonomy_path), taxonomy)
 
-        def test_validate_density(self, density):
-            tested._validate_density(density)
+    def test_validate_mtype_taxonomy(self, taxonomy):
+        tested._validate_mtype_taxonomy(taxonomy)
+
+        wrong_taxonomy = taxonomy.rename(columns={"sClass": "John"})
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_mtype_taxonomy(wrong_taxonomy)
+
+        wrong_taxonomy = taxonomy.drop(columns=["mtype"])
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_mtype_taxonomy(wrong_taxonomy)
+
+        wrong_taxonomy = deepcopy(taxonomy)
+        wrong_taxonomy.loc[1, "sClass"] = "OTHER"
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_mtype_taxonomy(wrong_taxonomy)
+
+    def test_load_neuronal_mtype_composition(self, composition, composition_path):
+        pdt.assert_frame_equal(
+            tested._load_neuronal_mtype_composition(composition_path), composition
+        )
+
+    def test_validate_density(self, density):
+        tested._validate_density(density)
+
+        wrong_density = density.with_data(np.zeros_like(density.raw))
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_density(wrong_density)
+
+        wrong_density = deepcopy(density)
+        wrong_density.raw[0, 0, 2] = -10.0
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_density(wrong_density)
+
+    def test_validate_neuronal_mtype_composition(self, composition):
+        tested._validate_neuronal_mtype_composition(composition)
+
+        wrong_composition = composition.copy(deep=True)
+        wrong_composition[["density", 2]] = -1.0
+        with pytest.raises(AtlasDensitiesError):
+            tested._validate_neuronal_mtype_composition(wrong_composition)
+
+    def test_check_taxonomy_composition_congruency(self, taxonomy, composition):
+        tested._check_taxonomy_composition_congruency(taxonomy, composition)
+
+        with pytest.raises(AtlasDensitiesError):
+            tested._check_taxonomy_composition_congruency(taxonomy.drop([1]), composition)
+
+        with pytest.raises(AtlasDensitiesError):
+            tested._check_taxonomy_composition_congruency(taxonomy, composition.drop([2]))
+
+    def test_create_from_composition(
+        self,
+        annotation_path,
+        hierarchy_path,
+        metadata_path,
+        density_path,
+        taxonomy_path,
+        composition_path,
+        class_tmpdir,
+    ):
+        output_dir = class_tmpdir.mkdir("output")
 
-            wrong_density = density.with_data(np.zeros_like(density.raw))
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_density(wrong_density)
-
-            wrong_density = deepcopy(density)
-            wrong_density.raw[0, 0, 2] = -10.0
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_density(wrong_density)
-
-        def test_validate_neuronal_mtype_composition(self, composition):
-            tested._validate_neuronal_mtype_composition(composition)
-
-            wrong_composition = composition.copy(deep=True)
-            wrong_composition[["density", 2]] = -1.0
-            with pytest.raises(AtlasDensitiesError):
-                tested._validate_neuronal_mtype_composition(wrong_composition)
-
-        def test_check_taxonomy_composition_congruency(self, taxonomy, composition):
-            tested._check_taxonomy_composition_congruency(taxonomy, composition)
-
-            with pytest.raises(AtlasDensitiesError):
-                tested._check_taxonomy_composition_congruency(taxonomy.drop([1]), composition)
-
-            with pytest.raises(AtlasDensitiesError):
-                tested._check_taxonomy_composition_congruency(taxonomy, composition.drop([2]))
-
-        def test_create_from_composition(
-            self,
-            annotation_path,
-            hierarchy_path,
-            metadata_path,
-            density_path,
-            taxonomy_path,
-            composition_path,
-            class_tmpdir,
-        ):
-            output_dir = class_tmpdir.mkdir("output")
-
-            runner = CliRunner()
-
-            with runner.isolated_filesystem(temp_dir=class_tmpdir):
-                result = runner.invoke(
-                    tested.create_from_composition,
-                    [
-                        "--annotation-path",
-                        annotation_path,
-                        "--hierarchy-path",
-                        hierarchy_path,
-                        "--metadata-path",
-                        metadata_path,
-                        "--excitatory-neuron-density-path",
-                        density_path,
-                        "--taxonomy-path",
-                        taxonomy_path,
-                        "--composition-path",
-                        composition_path,
-                        "--output-dir",
-                        output_dir,
-                    ],
-                )
+        runner = CliRunner()
 
-                assert result.exit_code == 0, result.output
+        with runner.isolated_filesystem(temp_dir=class_tmpdir):
+            result = runner.invoke(
+                tested.create_from_composition,
+                [
+                    # fmt: off
+                    "--annotation-path", annotation_path,
+                    "--hierarchy-path", hierarchy_path,
+                    "--metadata-path", metadata_path,
+                    "--excitatory-neuron-density-path", density_path,
+                    "--taxonomy-path", taxonomy_path,
+                    "--composition-path", composition_path,
+                    "--output-dir", output_dir,
+                    # fmt: on
+                ],
+            )
 
-                expected_filenames = {
-                    "L3_TPC:A_densities.nrrd",
-                    "L3_TPC:B_densities.nrrd",
-                    "L4_TPC_densities.nrrd",
-                    "L4_UPC_densities.nrrd",
-                }
+            assert result.exit_code == 0, result.output
+
+            expected_filenames = {
+                "L3_TPC:A_densities.nrrd",
+                "L3_TPC:B_densities.nrrd",
+                "L4_TPC_densities.nrrd",
+                "L4_UPC_densities.nrrd",
+            }
 
-                filenames = set(os.listdir(output_dir))
+            filenames = set(os.listdir(output_dir))
 
-                assert filenames == expected_filenames
+            assert filenames == expected_filenames
 
-                for filename in filenames:
-                    data = VoxelData.load_nrrd(str(Path(output_dir, filename)))
-                    assert data.shape == (1, 1, 6)
-                    assert not np.allclose(data.raw, 0.0)
+            for filename in filenames:
+                data = VoxelData.load_nrrd(str(Path(output_dir, filename)))
+                assert data.shape == (1, 1, 6)
+                assert not np.allclose(data.raw, 0.0)
```

### Comparing `atlas-densities-0.2.3/tests/app/test_refined_inhibitory_neuron_densities.py` & `atlas-densities-0.2.4/tests/app/test_refined_inhibitory_neuron_densities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """test cell_densities"""
-import json
 from pathlib import Path
 
 import numpy as np
 import numpy.testing as npt
 from click.testing import CliRunner
 from voxcell import VoxelData  # type: ignore
 
 import atlas_densities.app.cell_densities as tested
 from tests.densities.test_inhibitory_neuron_density_optimization import (
     get_initialization_data as get_optimization_data,
 )
 from tests.densities.test_refined_inhibitory_neuron_density import (
     get_inhibitory_neuron_densities_data,
 )
+from tests.utils import write_json
 
 
 def _get_inhibitory_neuron_densities_result(runner, algorithm=None):
     args = [
+        # fmt: off
         "inhibitory-neuron-densities",
-        "--hierarchy-path",
-        "hierarchy.json",
-        "--annotation-path",
-        "annotation.nrrd",
-        "--neuron-density-path",
-        "neuron_density.nrrd",
-        "--average-densities-path",
-        "average_densities.csv",
-        "--algorithm",
-        "keep-proportions",
-        "--output-dir",
-        "output_dir",
+        "--hierarchy-path", "hierarchy.json",
+        "--annotation-path", "annotation.nrrd",
+        "--neuron-density-path", "neuron_density.nrrd",
+        "--average-densities-path", "average_densities.csv",
+        "--algorithm", "keep-proportions",
+        "--output-dir", "output_dir",
+        # fmt: on
     ]
 
     if algorithm is not None:
         args + ["--algorithm", algorithm]
 
     return runner.invoke(tested.app, args)
 
@@ -45,16 +41,15 @@
         voxel_dimensions = [25] * 3
         VoxelData(input_["annotation"], voxel_dimensions=voxel_dimensions).save_nrrd(
             "annotation.nrrd"
         )
         VoxelData(input_["neuron_density"], voxel_dimensions=voxel_dimensions).save_nrrd(
             "neuron_density.nrrd"
         )
-        with open("hierarchy.json", "w") as file_:
-            json.dump(input_["hierarchy"], file_, indent=1, separators=(",", ": "))
+        write_json("hierarchy.json", input_["hierarchy"])
         input_["average_densities"]["brain_region"] = input_["average_densities"].index
         input_["average_densities"].to_csv("average_densities.csv", index=False)
 
         result = _get_inhibitory_neuron_densities_result(runner, algorithm)
 
         assert result.exit_code == 0
         gad_data = VoxelData.load_nrrd(str(Path("output_dir") / "gad67+_density.nrrd"))
@@ -71,17 +66,16 @@
             npt.assert_array_equal(voxel_data.voxel_dimensions, [25.0] * 3)
             subsum_density = subsum_density + voxel_data.raw
 
         assert np.all(input_["neuron_density"] >= gad_data.raw)
         assert np.all(gad_data.raw >= subsum_density)
 
         # Test assertion in case of invalid hierarchy file
-        with open("hierarchy.json", "w", encoding="utf-8") as file_:
-            hierarchy = {"msg": [input_["hierarchy"], {}]}
-            json.dump(hierarchy, file_, indent=1, separators=(",", ": "))
+        hierarchy = {"msg": [input_["hierarchy"], {}]}
+        write_json("hierarchy.json", hierarchy)
 
         result = _get_inhibitory_neuron_densities_result(runner, algorithm)
         assert "Unexpected JSON layout" in str(result.exception)
 
         # Check that an exception is thrown if the input neuron density has negative values
         input_["neuron_density"][0, 0, 0] = -1.0
         VoxelData(input_["neuron_density"], voxel_dimensions=(10, 10, 10)).save_nrrd(
```

### Comparing `atlas-densities-0.2.3/tests/combination/test_annotations_combinator.py` & `atlas-densities-0.2.4/tests/combination/test_annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/combination/test_markers_combinator.py` & `atlas-densities-0.2.4/tests/combination/test_markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/data/mtypes/mtype-taxonomy.tsv` & `atlas-densities-0.2.4/tests/densities/data/mtypes/mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_cell_counts.py` & `atlas-densities-0.2.4/tests/densities/test_cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_cell_density.py` & `atlas-densities-0.2.4/tests/densities/test_cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_excel_reader.py` & `atlas-densities-0.2.4/tests/densities/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_excitatory_inhibitory_splitting.py` & `atlas-densities-0.2.4/tests/densities/test_excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_fitting.py` & `atlas-densities-0.2.4/tests/densities/test_fitting.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         index=region_names,
     )
     actual = tested.create_dataframe_from_known_densities(region_names, average_densities)
     pdt.assert_frame_equal(actual, expected)
 
 
 @pytest.fixture
-def hierarchy_info():
+def region_map():
     hierarchy = {
         "id": 8,
         "name": "Basic cell groups and regions",
         "acronym": "grey",
         "children": [
             {
                 "id": 920,
@@ -100,15 +100,20 @@
                         "children": [],
                     },
                 ],
             },
         ],
     }
 
-    return utils.get_hierarchy_info(RegionMap.from_dict(hierarchy))
+    return RegionMap.from_dict(hierarchy)
+
+
+@pytest.fixture
+def hierarchy_info(region_map):
+    return utils.get_hierarchy_info(region_map)
 
 
 def test_fill_in_homogenous_regions(hierarchy_info):
     homogenous_regions = pd.DataFrame(
         {
             "brain_region": [
                 "Lobule II",
@@ -222,15 +227,15 @@
     assert np.allclose(actual, 0.1 / 2.0)
     actual = tested.compute_average_intensity(intensity, volume_mask, slices=[-1, 1, 3])
     assert np.allclose(actual, 0.1 / 2.0)
     actual = tested.compute_average_intensity(intensity, volume_mask, slices=[-1, 3])
     assert actual == 0
 
 
-def test_compute_average_intensities(hierarchy_info):
+def test_compute_average_intensities(region_map, hierarchy_info):
     annotation = np.array(
         [[[0, 976], [976, 936]], [[976, 936], [936, 936]]]  # 976 = Lobule II, 936 = "Declive (VI)""
     )
     marker_volumes = {
         "gad67": {
             "intensity": np.array([[[1.0, 1.0], [1.0, 2.0]], [[1.0, 2.0], [2.0, 2.0]]]),
             "slices": [1],
@@ -257,30 +262,35 @@
         {
             "gad67": [7.0 / 4.0, 1.0, 2.0, 1.0, 0.0, 0.0, 0.0, 0.0],
             "pv": [10.0 / 7.0, 2.0, 1.0, 2.0, 0.0, 0.0, 0.0, 0.0],
         },
         index=hierarchy_info["brain_region"],
     )
 
-    actual = tested.compute_average_intensities(annotation, marker_volumes, hierarchy_info)
+    actual = tested.compute_average_intensities(
+        annotation, marker_volumes, hierarchy_info, region_map
+    )
     pdt.assert_frame_equal(actual, expected)
 
 
 def test_linear_fitting_xy():
     actual = tested.linear_fitting_xy([0.0, 1.0, 2.0], [0.0, 2.0, 4.0], [1.0, 1.0, 1.0])
     assert np.allclose(actual["coefficient"], 2.0)
+    assert np.allclose(actual["r_square"], 1.0)
     assert not np.isinf(actual["standard_deviation"])
 
     actual = tested.linear_fitting_xy([0.0, 1.0, 2.0], [0.0, 1.0, 4.0], [1.0, 1.0, 1e-5])
     assert np.allclose(actual["coefficient"], 2.0)
     assert not np.isinf(actual["standard_deviation"])
+    assert np.allclose(actual["r_square"], 0.89286)
 
     actual = tested.linear_fitting_xy([0.0, 1.0, 2.0], [0.0, 2.0, 4.0], [1.0, 0.0, 1.0])
     assert np.allclose(actual["coefficient"], 2.0)
     assert not np.isinf(actual["standard_deviation"])
+    assert np.allclose(actual["r_square"], 1.0)
 
 
 def get_fitting_input_data_(hierarchy_info):
     intensities = pd.DataFrame(
         {
             "gad67": [7.0 / 4.0, 1.0, 2.0, 1.0, np.nan, np.nan, np.nan, np.nan],
             "pv": [10.0 / 7.0, 2.0, 1.0, 2.0, np.nan, np.nan, np.nan, np.nan],
@@ -315,14 +325,18 @@
     for group_name in ["Whole", "Central lobule"]:
         assert actual[group_name]["gad67+"]["coefficient"] == 2.0
         assert actual[group_name]["pv+"]["coefficient"] == 3.0
         assert not np.isinf(actual[group_name]["gad67+"]["standard_deviation"])
         assert not np.isnan(actual[group_name]["gad67+"]["standard_deviation"])
         assert not np.isinf(actual[group_name]["pv+"]["standard_deviation"])
         assert not np.isnan(actual[group_name]["pv+"]["standard_deviation"])
+    assert actual["Whole"]["pv+"]["r_square"] == 1.0
+    assert actual["Whole"]["gad67+"]["r_square"] == 1.0
+    assert np.isnan(actual["Central lobule"]["pv+"]["r_square"])  # only one value so no variation.
+    assert np.isnan(actual["Central lobule"]["gad67+"]["r_square"])
 
 
 def test_compute_fitting_coefficients_exceptions(hierarchy_info):
     data = get_fitting_input_data_(hierarchy_info)
     data["densities"].drop(index=["Central lobule"], inplace=True)
 
     with pytest.raises(AtlasDensitiesError):
```

### Comparing `atlas-densities-0.2.3/tests/densities/test_glia_densities.py` & `atlas-densities-0.2.4/tests/densities/test_glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_inhibitory_neuron_density.py` & `atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_inhibitory_neuron_density_optimization.py` & `atlas-densities-0.2.4/tests/densities/test_inhibitory_neuron_density_optimization.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,98 @@
 import pandas.testing as pdt
 import pytest
 
 import atlas_densities.densities.inhibitory_neuron_densities_optimization as tested
 from atlas_densities.exceptions import AtlasDensitiesError
 
 
+def test_resize_average_densities():
+    average_densities = pd.DataFrame(
+        {
+            "gad67+": [9.0, 12.0],
+            "gad67+_standard_deviation": [0.9, 1.2],
+            "pv+": [1.0, 2.0],
+            "pv+_standard_deviation": [0.1, 0.2],
+            "sst+": [3.0, 4.0],
+            "sst+_standard_deviation": [0.3, 0.4],
+            "vip+": [5.0, 6.0],
+            "vip+_standard_deviation": [0.5, 0.6],
+        },
+        index=["A", "B"],
+    )
+    hierarchy_info = pd.DataFrame(
+        {
+            "brain_region": ["A", "B", "C"],
+        },
+        index=[1, 2, 3],
+    )
+
+    expected = pd.DataFrame(
+        {
+            "gad67+": [9.0, 12.0, np.nan],
+            "gad67+_standard_deviation": [0.9, 1.2, np.nan],
+            "pv+": [1.0, 2.0, np.nan],
+            "pv+_standard_deviation": [0.1, 0.2, np.nan],
+            "sst+": [3.0, 4.0, np.nan],
+            "sst+_standard_deviation": [0.3, 0.4, np.nan],
+            "vip+": [5.0, 6.0, np.nan],
+            "vip+_standard_deviation": [0.5, 0.6, np.nan],
+        },
+        index=hierarchy_info["brain_region"],
+    )
+    actual = tested._resize_average_densities(average_densities, hierarchy_info)
+    pdt.assert_frame_equal(actual, expected)
+
+
+def test_check_region_counts_consistency():
+    region_counts = pd.DataFrame(
+        {
+            "gad67+": [9.0, 12.0, 2.0],
+            "gad67+_standard_deviation": [0.9, 1.2, 1.0],
+            "pv+": [1.0, 1.0, 1.0],
+            "pv+_standard_deviation": [0.1, 0.2, 0.3],
+            "sst+": [3.0, 4.0, 5.0],
+            "sst+_standard_deviation": [0.3, 0.4, 0.5],
+            "vip+": [5.0, 6.0, 7.0],
+            "vip+_standard_deviation": [0.5, 0.6, 0.7],
+        },
+        index=["A", "B", "C"],
+    )
+    hierarchy_info = pd.DataFrame(
+        {"brain_region": ["A", "B", "C"], "descendant_ids": [{1, 2, 3}, {2}, {3}]},
+        index=[1, 2, 3],
+    )
+
+    # Uncertain or consistent
+    tested._check_region_counts_consistency(region_counts, hierarchy_info)
+    region_counts.loc["A", "gad67+_standard_deviation"] = 0.0
+    tested._check_region_counts_consistency(region_counts, hierarchy_info)
+
+    # Inconsistent parent-child count inequality
+    region_counts.loc["B", "gad67+_standard_deviation"] = 0.0
+    with pytest.raises(AtlasDensitiesError, match=r"gad67\+.*exceed"):
+        tested._check_region_counts_consistency(region_counts, hierarchy_info)
+
+    # The sum of the cell counts of the children regions B and C exceeds the count
+    # of the parent region A.
+    region_counts.loc["B", "gad67+_standard_deviation"] = 1.2  # restores valid value
+    region_counts.loc["A", "pv+_standard_deviation"] = 0.0
+    region_counts.loc["B", "pv+_standard_deviation"] = 0.0
+    region_counts.loc["C", "pv+_standard_deviation"] = 0.0
+    with pytest.raises(AtlasDensitiesError, match=r"sum of the counts.*pv\+.*exceeds.*region A"):
+        tested._check_region_counts_consistency(region_counts, hierarchy_info)
+
+
+def test_replace_inf_with_none():
+    bounds = np.array([[0.1, 1.0], [-1.0, np.inf]])
+    result = [(0.1, 1.0), (-1.0, None)]
+
+    assert repr(result) == repr(tested._replace_inf_with_none(bounds))
+
+
 def test_create_volumetric_densities():
     annotation = np.array([[[1, 1, 2]]], dtype=int)
     neuron_density = np.array([[[0.5, 0.5, 1.0]]])
     neuron_counts = pd.DataFrame({"cell_count": [4.0, 4.0]}, index=[1, 2])
     cell_types = ["pv+", "sst+"]
     x_result = pd.DataFrame({"pv+": [3.0, 1.0], "sst+": [1.0, 3.0]}, index=[1, 2])
 
@@ -195,29 +279,14 @@
         "vip+": np.array([[[1.0, 1.0]]]),
     }
 
     for cell_type, density in densities.items():
         npt.assert_array_almost_equal(density, expected[cell_type])
 
 
-def test_error_on_sigmas_inconsistencies():
-    # Test that an error is raised when our simplifying assumption between the x's and the deltas
-    # is violated
-    data = get_initialization_data_3()
-    data["average_densities"].at["root", "pv+_standard_deviation"] = 0.0
-    with pytest.raises(AtlasDensitiesError, match="not certain"):
-        tested.create_inhibitory_neuron_densities(
-            data["hierarchy"],
-            data["annotation"],
-            data["voxel_volume"],
-            data["neuron_density"],
-            data["average_densities"],
-        )
-
-
 def get_initialization_data_4():
     hierarchy = {
         "id": 8,
         "name": "root",
         "children": [
             {
                 "id": 1,
@@ -338,36 +407,29 @@
             "brain_region": [
                 "Central lobule",
                 "Lobule II",
                 "Lobule II, granular layer",
                 "Lobule II, Purkinje layer",
                 "Lobule II, molecular layer",
             ],
-            "descendant_id_set": [
-                {920, 976, 10708, 10709, 10710},
-                {976, 10708, 10709, 10710},
-                {10708},
-                {10709},
-                {10710},
-            ],
         },
         index=[920, 976, 10708, 10709, 10710],
     )
 
 
 def test_compute_region_cell_counts():
     annotation = np.array([[[920, 10710, 10710], [10709, 10708, 976], [10708, 10710, 10709]]])
     cell_density = np.array([[[1.0, 1.0 / 3.0, 1.0 / 3.0], [0.5, 0.5, 1.0], [0.5, 1.0 / 3.0, 0.5]]])
     voxel_volume = 2.0
 
     hierarchy_info = get_hierarchy_info()
     cell_counts = pd.DataFrame(
         {
             "brain_region": hierarchy_info["brain_region"],
-            "cell_count": 2 * np.array([5.0, 4.0, 1.0, 1.0, 1.0]),
+            "cell_count": 2 * np.array([1.0, 1.0, 1.0, 1.0, 1.0]),
         },
         index=hierarchy_info.index,
     )
 
     pdt.assert_frame_equal(
         cell_counts,  # expected
         tested._compute_region_cell_counts(
```

### Comparing `atlas-densities-0.2.3/tests/densities/test_measurement_to_density.py` & `atlas-densities-0.2.4/tests/densities/test_measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_composition.py` & `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_map.py` & `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_map.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_mtype_densities_from_profiles.py` & `atlas-densities-0.2.4/tests/densities/test_mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_optimization_initialization.py` & `atlas-densities-0.2.4/tests/densities/test_optimization_initialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import atlas_densities.densities.inhibitory_neuron_densities_optimization as tested
 from atlas_densities.exceptions import AtlasDensitiesError
 
 
 @pytest.fixture
 def counts_data_1():
     hierarchy_info = pd.DataFrame(
-        {"brain_region": ["A", "B"], "descendant_id_set": [{1}, {2}]}, index=[1, 2]
+        {"brain_region": ["A", "B"], "descendant_ids": [{1}, {2}]}, index=[1, 2]
     )
     region_counts = pd.DataFrame(
         {
             "gad67+": [9.0, 12.0],
             "gad67+_standard_deviation": [0.9, 1.2],
             "pv+": [1.0, 2.0],
             "pv+_standard_deviation": [0.1, 0.2],
@@ -158,15 +158,15 @@
     )
 
 
 @pytest.fixture
 def counts_data_2():
     hierarchy_info = pd.DataFrame(
         # A is now a parent region of B
-        {"brain_region": ["A", "B"], "descendant_id_set": [{1, 2}, {2}]},
+        {"brain_region": ["A", "B"], "descendant_ids": [{1, 2}, {2}]},
         index=[1, 2],
     )
     region_counts = pd.DataFrame(
         {
             "gad67+": [0.0, 1.0],  # zero cell count for A
             "gad67+_standard_deviation": [0.0, 1.2],  # zero standard deviation for A
             "pv+": [2.0, 1.0],
@@ -331,15 +331,15 @@
         {"cell_count": [1.0, 3.0, 3.0], "brain_region": ["A", "B", "C"]},
         index=[1, 2, 3],
     )
 
 
 def counts_data_3():
     hierarchy_info = pd.DataFrame(
-        {"brain_region": ["A", "B", "C"], "descendant_id_set": [{1, 2, 3}, {2}, {3}]},
+        {"brain_region": ["A", "B", "C"], "descendant_ids": [{1, 2, 3}, {2}, {3}]},
         index=[1, 2, 3],
     )
     region_counts = pd.DataFrame(
         {
             "gad67+": [5.5, 3.0, 2.0],
             "gad67+_standard_deviation": [1.0, 0.1, 0.1],
             "pv+": [2.0, 1.0, 1.0],
@@ -567,15 +567,15 @@
 
     npt.assert_array_almost_equal(expected_bounds, bounds)
 
 
 @pytest.fixture
 def aub_and_bub_data():
     hierarchy_info = pd.DataFrame(
-        {"brain_region": ["A", "B", "C"], "descendant_id_set": [{1, 2, 3}, {2}, {3}]},
+        {"brain_region": ["A", "B", "C"], "descendant_ids": [{1, 2, 3}, {2}, {3}]},
         index=[1, 2, 3],
     )
     x_map, deltas_map = expected_maps()
 
     return {
         "x_result": expected_x_result(),
         "region_counts": counts_data_3()["region_counts"],
```

### Comparing `atlas-densities-0.2.3/tests/densities/test_refined_inhibitory_neuron_density.py` & `atlas-densities-0.2.4/tests/densities/test_refined_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/densities/test_utils.py` & `atlas-densities-0.2.4/tests/densities/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,28 @@
     # Return a modified copy of the input
     actual = tested.normalize_intensity(marker, annotation_raw)
     npt.assert_array_almost_equal(actual, expected)
     npt.assert_array_equal(marker, original_marker)
     # In place modification
     actual = tested.normalize_intensity(marker, annotation_raw, copy=False)
     npt.assert_array_almost_equal(marker, expected)
+    # Test outside with no intensity
+    marker = np.array(
+        [
+            [
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 1.0, 0.0],
+                [0.0, 3.0, 5.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+            ]
+        ],
+        dtype=float,
+    )
+    actual = tested.normalize_intensity(marker, annotation_raw, copy=True)
+    npt.assert_array_almost_equal(marker / np.max(marker), actual)
 
 
 def test_compensate_cell_overlap():
     annotation_raw = np.array(
         [
             [
                 [0, 0, 0, 0],
@@ -335,15 +349,15 @@
             "brain_region": [
                 "Central lobule",
                 "Lobule II",
                 "Lobule II, granular layer",
                 "Lobule II, Purkinje layer",
                 "Lobule II, molecular layer",
             ],
-            "descendant_id_set": [
+            "descendant_ids": [
                 {920, 976, 10708, 10709, 10710},
                 {976, 10708, 10709, 10710},
                 {10708},
                 {10709},
                 {10710},
             ],
         },
```

### Comparing `atlas-densities-0.2.3/tests/markers_config.yaml` & `atlas-densities-0.2.4/tests/markers_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/mocking_tools.py` & `atlas-densities-0.2.4/tests/mocking_tools.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tests/test_utils.py` & `atlas-densities-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.2.3/tox.ini` & `atlas-densities-0.2.4/tox.ini`

 * *Files identical despite different names*

