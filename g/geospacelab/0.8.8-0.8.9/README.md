# Comparing `tmp/geospacelab-0.8.8.tar.gz` & `tmp/geospacelab-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospacelab-0.8.8.tar", last modified: Fri Mar  1 09:45:48 2024, max compression
+gzip compressed data, was "geospacelab-0.8.9.tar", last modified: Thu Apr 18 07:29:26 2024, max compression
```

## Comparing `geospacelab-0.8.8.tar` & `geospacelab-0.8.9.tar`

### file list

```diff
@@ -1,414 +1,418 @@
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.473462 geospacelab-0.8.8/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.8.8/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)      195 2023-09-29 07:00:51.000000 geospacelab-0.8.8/MANIFEST.in
--rw-r--r--   0 lei       (1000) lei       (1000)    23831 2024-03-01 09:45:48.473462 geospacelab-0.8.8/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    22302 2024-02-26 10:12:04.000000 geospacelab-0.8.8/README.md
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/
--rw-rw-r--   0 lei       (1000) lei       (1000)      800 2024-03-01 09:45:32.000000 geospacelab-0.8.8/geospacelab/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/config/
--rw-rw-r--   0 lei       (1000) lei       (1000)      641 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/config/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/config/_preferences.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/cs/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.8.8/geospacelab/cs/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/cs/_aacgm.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/cs/_apex.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/cs/_cs_base.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.8.8/geospacelab/cs/_geo.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/cs/geo_utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/
--rw-rw-r--   0 lei       (1000) lei       (1000)    20245 2024-03-01 08:49:37.000000 geospacelab-0.8.8/geospacelab/datahub/__dataset_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2023-12-13 08:03:40.000000 geospacelab-0.8.8/geospacelab/datahub/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/__metadata_base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    38910 2023-12-14 06:52:57.000000 geospacelab-0.8.8/geospacelab/datahub/__variable_base__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.8.8/geospacelab/datahub/sources/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/
--rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-04-05 13:39:25.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2473 2023-12-13 08:56:50.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11068 2023-12-13 08:56:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4129 2023-12-13 08:56:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2995 2023-07-14 23:46:55.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7341 2023-07-15 00:06:04.000000 geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      521 2023-12-13 08:56:50.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.449462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      547 2023-12-13 08:56:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12344 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1986 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12460 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1832 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6617 2023-12-13 08:56:50.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12191 2023-12-13 08:56:50.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1956 2023-12-13 08:56:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1881 2023-11-02 11:58:01.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5454 2023-11-01 08:33:57.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l2d/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l2l/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3478 2023-11-01 13:04:17.000000 geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/
--rw-rw-r--   0 lei       (1000) lei       (1000)      701 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5763 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3048 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:07:56.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/abk/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:19:05.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/abk/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/kev/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:50.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/kev/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/muo/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:58.000000 geospacelab-0.8.8/geospacelab/datahub/sources/fmi/miracle/muo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/
--rw-rw-r--   0 lei       (1000) lei       (1000)      496 2023-12-13 08:23:43.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4087 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6378 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3853 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6302 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4622 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5658 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6587 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/loader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5636 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7322 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5699 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/isee/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1258 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6042 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2966 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3175 2023-09-11 08:49:28.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.453462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/
--rw-rw-r--   0 lei       (1000) lei       (1000)      520 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1416 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4991 2023-12-13 09:16:45.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8497 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8346 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      760 2023-11-09 17:53:56.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    11635 2023-11-09 17:40:54.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2023-11-09 17:20:07.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5488 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8275 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12469 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     9531 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1992 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    22500 2024-02-25 11:28:05.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5958 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4297 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/
--rw-rw-r--   0 lei       (1000) lei       (1000)    15784 2024-02-26 08:04:11.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16084 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
--rw-rw-r--   0 lei       (1000) lei       (1000)    14694 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7533 2024-02-25 14:42:28.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8261 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7917 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
--rw-rw-r--   0 lei       (1000) lei       (1000)     7843 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8951 2023-08-30 08:00:15.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6040 2024-02-23 13:59:00.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/
--rw-rw-r--   0 lei       (1000) lei       (1000)    14063 2024-02-28 15:04:57.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2688 2024-02-26 08:32:30.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8495 2024-02-26 09:26:58.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8205 2024-02-26 09:36:42.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.457462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10895 2024-02-28 14:16:34.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2412 2024-02-22 11:01:07.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3495 2024-02-22 07:49:06.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    20049 2024-02-29 11:42:06.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      487 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4809 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10309 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10280 2023-04-20 12:28:27.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
--rw-r--r--   0 lei       (1000) lei       (1000)    11534 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6745 2023-04-19 11:05:17.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10196 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4747 2024-02-15 21:41:42.000000 geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/ncei/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/ncei/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/ncei/dmsp/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/ncei/dmsp/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/
--rw-rw-r--   0 lei       (1000) lei       (1000)      728 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:59:47.000000 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11056 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1850 2023-06-01 13:04:28.000000 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/goesxray/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/solarwind/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/
--rw-rw-r--   0 lei       (1000) lei       (1000)      555 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     8790 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5748 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1986 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/
--rw-rw-r--   0 lei       (1000) lei       (1000)     6719 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7770 2023-12-13 08:23:43.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/magnetometer/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.8.8/geospacelab/datahub/sources/supermag/supermag_api.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2706 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/
--rw-rw-r--   0 lei       (1000) lei       (1000)      559 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9328 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1583 2023-12-13 08:15:20.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9381 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1583 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5426 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/downloader.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/
--rw-rw-r--   0 lei       (1000) lei       (1000)      532 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9498 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/
--rw-rw-r--   0 lei       (1000) lei       (1000)      542 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.461462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    12298 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1613 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)    10428 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1640 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/
--rw-rw-r--   0 lei       (1000) lei       (1000)      542 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9607 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1731 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2731 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/
--rw-rw-r--   0 lei       (1000) lei       (1000)      547 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     9232 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1614 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/
--rw-rw-r--   0 lei       (1000) lei       (1000)    11746 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1614 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1620 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5343 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5375 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6627 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/
--rw-rw-r--   0 lei       (1000) lei       (1000)     5329 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     6227 2023-12-13 08:49:12.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/downloader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/loader.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/variable_config.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/express/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/express/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.8.8/geospacelab/express/dmsp_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8873 2023-12-19 09:00:22.000000 geospacelab-0.8.8/geospacelab/express/eiscat_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     8482 2023-09-20 12:33:19.000000 geospacelab-0.8.8/geospacelab/express/millstonehill_dashboard.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.8.8/geospacelab/express/omni_dashboard.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/future/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/future/empiricalmodels/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/empiricalmodels/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/future/empiricalmodels/ovationprime2010/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.8.8/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/future/satllites/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/satllites/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/satllites/orbit_analyzer.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/future/test_sscws.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/observatory/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/observatory/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.8.8/geospacelab/observatory/constants.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/observatory/earth/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/observatory/earth/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3919 2023-12-13 09:12:51.000000 geospacelab-0.8.8/geospacelab/observatory/earth/_func.py
--rw-rw-r--   0 lei       (1000) lei       (1000)       14 2023-09-05 09:00:48.000000 geospacelab-0.8.8/geospacelab/observatory/earth/constants.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.8.8/geospacelab/observatory/earth/geodesy.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      749 2023-09-05 12:56:38.000000 geospacelab-0.8.8/geospacelab/observatory/earth/sun_position.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.465462 geospacelab-0.8.8/geospacelab/observatory/orbit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.8.8/geospacelab/observatory/orbit/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    15709 2023-12-13 09:16:45.000000 geospacelab-0.8.8/geospacelab/observatory/orbit/sc_orbit.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    25869 2023-11-15 13:43:23.000000 geospacelab-0.8.8/geospacelab/observatory/orbit/utilities.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/observatory/site/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-12-04 10:25:35.000000 geospacelab-0.8.8/geospacelab/observatory/site/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      457 2023-12-05 13:35:36.000000 geospacelab-0.8.8/geospacelab/observatory/site/mixins.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/quantity/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.8.8/geospacelab/quantity/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/toolbox/
--rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.8.8/geospacelab/toolbox/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/toolbox/io/
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/toolbox/io/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/toolbox/io/dialog.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/toolbox/unit/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.8.8/geospacelab/toolbox/unit/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/toolbox/utilities/
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     7063 2023-09-18 18:55:46.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/numpyarray.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3810 2023-08-24 10:51:09.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/numpymath.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/pybasic.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/pyclass.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/pydatetime.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/pylogging.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.8.8/geospacelab/toolbox/utilities/pyos.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/visualization/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.8.8/geospacelab/visualization/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/visualization/mpl/
--rw-rw-r--   0 lei       (1000) lei       (1000)    31607 2023-12-15 13:01:10.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/_helpers.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/axes.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    15132 2023-12-01 14:57:11.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/axis_ticks.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     7091 2023-11-09 08:32:05.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/colormaps.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    17218 2023-12-01 14:59:39.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/dashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/figure.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/
--rw-rw-r--   0 lei       (1000) lei       (1000)     2940 2023-08-22 10:11:11.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/__base__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/geodashboards.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    42782 2024-02-22 11:56:25.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/geopanels.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    33983 2024-02-22 15:14:57.000000 geospacelab-0.8.8/geospacelab/visualization/mpl/panels.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/visualization/plotly/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.8.8/geospacelab/visualization/plotly/__init__.py
--rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.8.8/geospacelab/visualization/plotly/ipanel.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/wrapper/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.8.8/geospacelab/wrapper/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/wrapper/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/LICENSE
--rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/README.md
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/__init__.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/
--rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/__init__.py
--rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/geopack.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t01.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t04.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t89.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t96.py
--rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/test_geopack1.md
--rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/test_geopack1.py
-drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-03-01 09:45:48.469462 geospacelab-0.8.8/geospacelab.egg-info/
--rw-r--r--   0 lei       (1000) lei       (1000)    23831 2024-03-01 09:45:48.000000 geospacelab-0.8.8/geospacelab.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1000) lei       (1000)    15699 2024-03-01 09:45:48.000000 geospacelab-0.8.8/geospacelab.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)        1 2024-03-01 09:45:48.000000 geospacelab-0.8.8/geospacelab.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      234 2024-03-01 09:45:48.000000 geospacelab-0.8.8/geospacelab.egg-info/requires.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)       12 2024-03-01 09:45:48.000000 geospacelab-0.8.8/geospacelab.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1000) lei       (1000)      204 2024-03-01 09:45:48.473462 geospacelab-0.8.8/setup.cfg
--rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2023-11-10 11:11:22.000000 geospacelab-0.8.8/setup.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1515 2021-08-21 16:59:48.000000 geospacelab-0.8.9/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)      195 2023-09-29 07:00:51.000000 geospacelab-0.8.9/MANIFEST.in
+-rw-r--r--   0 lei       (1000) lei       (1000)    23831 2024-04-18 07:29:26.490771 geospacelab-0.8.9/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22302 2024-02-26 10:12:04.000000 geospacelab-0.8.9/README.md
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      800 2024-04-18 07:28:24.000000 geospacelab-0.8.9/geospacelab/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/config/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      641 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/config/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4726 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/config/_preferences.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/cs/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1282 2023-03-01 11:02:12.000000 geospacelab-0.8.9/geospacelab/cs/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      723 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/cs/_aacgm.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      756 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/cs/_apex.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    17124 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/cs/_cs_base.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18253 2022-11-07 08:45:01.000000 geospacelab-0.8.9/geospacelab/cs/_geo.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      604 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/cs/geo_utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/datahub/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    20491 2024-03-27 07:16:13.000000 geospacelab-0.8.9/geospacelab/datahub/__dataset_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    18655 2023-12-13 08:03:40.000000 geospacelab-0.8.9/geospacelab/datahub/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2825 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/__metadata_base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    38936 2024-03-28 09:40:43.000000 geospacelab-0.8.9/geospacelab/datahub/__variable_base__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/datahub/sources/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-12-07 06:22:00.000000 geospacelab-0.8.9/geospacelab/datahub/sources/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      680 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.466771 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-04-05 13:39:25.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2473 2023-12-13 08:56:50.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11449 2024-03-27 07:13:45.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4129 2023-12-13 08:56:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2995 2023-07-14 23:46:55.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8106 2024-03-27 07:23:03.000000 geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      521 2023-12-13 08:56:50.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      547 2023-12-13 08:56:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_fp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12344 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1986 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1499 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4888 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12460 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1832 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1856 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5445 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct16/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6617 2023-12-13 08:56:50.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12185 2024-04-18 06:52:04.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1914 2024-04-18 06:45:26.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1881 2023-11-02 11:58:01.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5454 2023-11-01 08:33:57.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l2d/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l2d/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l2l/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l2l/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3478 2023-11-01 13:04:17.000000 geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      701 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-11-24 08:47:10.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5763 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3048 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2582 2022-11-24 12:20:08.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2023-02-03 18:57:40.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:07:56.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/abk/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:19:05.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/abk/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/kev/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:50.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/kev/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/muo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:18:58.000000 geospacelab-0.8.9/geospacelab/datahub/sources/fmi/miracle/muo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      496 2023-12-13 08:23:43.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4087 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6378 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3853 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1590 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6302 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4622 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2687 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5658 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6587 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/loader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5636 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7322 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1563 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.470771 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5699 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1663 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/isee/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1258 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6042 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2966 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3175 2023-09-11 08:49:28.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      520 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1416 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4991 2023-12-13 09:16:45.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8497 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2709 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8346 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      760 2023-11-09 17:53:56.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11635 2023-11-09 17:40:54.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1546 2023-11-09 17:20:07.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      155 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5488 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8275 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5322 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4347 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12469 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9519 2024-04-10 10:17:26.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4686 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1992 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    22575 2024-03-26 09:05:49.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5958 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4297 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2895 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1517 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15784 2024-02-26 08:04:11.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16088 2024-04-16 15:23:59.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      652 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16337 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2514 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2024-03-11 09:27:09.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14694 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7533 2024-02-25 14:42:28.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8274 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8261 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.474771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7917 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3753 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6371 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7843 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3397 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8951 2023-08-30 08:00:15.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6040 2024-02-23 13:59:00.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14063 2024-02-28 15:04:57.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2688 2024-02-26 08:32:30.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8495 2024-02-26 09:26:58.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8205 2024-02-26 09:36:42.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10895 2024-02-28 14:16:34.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2412 2024-02-22 11:01:07.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3495 2024-02-22 07:49:06.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    20049 2024-02-29 11:42:06.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      487 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4809 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10309 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4902 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10280 2023-04-20 12:28:27.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/
+-rw-r--r--   0 lei       (1000) lei       (1000)    11534 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3360 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6745 2023-04-19 11:05:17.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10196 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3229 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4054 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4747 2024-02-15 21:41:42.000000 geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/ncei/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/ncei/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/ncei/dmsp/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/ncei/dmsp/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      728 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-06-01 06:59:47.000000 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11056 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1850 2023-06-01 13:04:28.000000 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8330 2023-04-19 11:06:29.000000 geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/goesxray/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/goesxray/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/solarwind/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/noaa/swpc/solarwind/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      555 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8790 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5748 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10900 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1551 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1986 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6719 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7767 2024-03-25 14:57:54.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1531 2023-02-06 08:02:57.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3006 2023-02-03 18:57:39.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.478771 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/magnetometer/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5644 2024-03-25 14:32:29.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/magnetometer/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6408 2024-03-25 14:57:54.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/magnetometer/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2002 2024-03-25 15:03:38.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/magnetometer/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5106 2024-03-27 07:54:54.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/magnetometer/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    27422 2023-02-03 11:24:53.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/supermag_api.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2024-03-25 09:28:03.000000 geospacelab-0.8.9/geospacelab/datahub/sources/supermag/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2706 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      559 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9328 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1583 2023-12-13 08:15:20.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2436 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3337 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9381 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1583 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2890 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5546 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5426 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/downloader.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      532 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9498 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3715 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6288 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      542 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12298 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1613 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4335 2022-10-10 08:45:16.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    10428 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1640 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2867 2023-01-15 11:57:47.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3346 2023-01-27 09:35:38.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      542 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    12296 2024-04-05 11:02:58.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1731 2024-04-05 09:04:53.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2720 2024-04-05 09:02:19.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4116 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      547 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     9232 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1614 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    11746 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1614 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2039 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3336 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1620 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5343 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6544 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1585 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3704 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5375 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6627 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1610 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3728 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.482771 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5329 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6227 2023-12-13 08:49:12.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/downloader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1521 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/loader.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1516 2022-02-23 05:03:33.000000 geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/variable_config.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/express/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/express/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     4152 2022-10-18 12:32:59.000000 geospacelab-0.8.9/geospacelab/express/dmsp_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8873 2023-12-19 09:00:22.000000 geospacelab-0.8.9/geospacelab/express/eiscat_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     8482 2023-09-20 12:33:19.000000 geospacelab-0.8.9/geospacelab/express/millstonehill_dashboard.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3937 2022-11-21 13:16:14.000000 geospacelab-0.8.9/geospacelab/express/omni_dashboard.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/future/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/future/empiricalmodels/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/empiricalmodels/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/future/empiricalmodels/ovationprime2010/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/empiricalmodels/ovationprime2010/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    39045 2023-03-01 11:22:40.000000 geospacelab-0.8.9/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/future/satllites/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/satllites/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     5213 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/satllites/orbit_analyzer.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1151 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/future/test_sscws.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/observatory/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/observatory/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       11 2022-09-08 09:38:55.000000 geospacelab-0.8.9/geospacelab/observatory/constants.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/observatory/earth/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/observatory/earth/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3919 2023-12-13 09:12:51.000000 geospacelab-0.8.9/geospacelab/observatory/earth/_func.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)       14 2023-09-05 09:00:48.000000 geospacelab-0.8.9/geospacelab/observatory/earth/constants.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1082 2022-09-08 09:57:47.000000 geospacelab-0.8.9/geospacelab/observatory/earth/geodesy.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      749 2023-09-05 12:56:38.000000 geospacelab-0.8.9/geospacelab/observatory/earth/sun_position.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/observatory/orbit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2022-09-08 10:08:40.000000 geospacelab-0.8.9/geospacelab/observatory/orbit/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15709 2023-12-13 09:16:45.000000 geospacelab-0.8.9/geospacelab/observatory/orbit/sc_orbit.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    25869 2023-11-15 13:43:23.000000 geospacelab-0.8.9/geospacelab/observatory/orbit/utilities.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/observatory/site/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-12-04 10:25:35.000000 geospacelab-0.8.9/geospacelab/observatory/site/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      457 2023-12-05 13:35:36.000000 geospacelab-0.8.9/geospacelab/observatory/site/mixins.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/quantity/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-09-03 10:12:23.000000 geospacelab-0.8.9/geospacelab/quantity/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/toolbox/
+-rw-rw-r--   0 lei       (1000) lei       (1000)       56 2021-07-13 05:22:19.000000 geospacelab-0.8.9/geospacelab/toolbox/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/toolbox/io/
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/toolbox/io/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/toolbox/io/dialog.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/toolbox/unit/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.8.9/geospacelab/toolbox/unit/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/toolbox/utilities/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2021-07-13 05:22:19.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     7063 2023-09-18 18:55:46.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/numpyarray.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3810 2023-08-24 10:51:09.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/numpymath.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     3310 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/pybasic.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     2813 2021-11-29 20:45:17.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/pyclass.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    10865 2023-02-06 11:56:22.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/pydatetime.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)     1816 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/pylogging.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      754 2021-08-21 16:59:48.000000 geospacelab-0.8.9/geospacelab/toolbox/utilities/pyos.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/visualization/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1025 2023-02-06 14:01:52.000000 geospacelab-0.8.9/geospacelab/visualization/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.486771 geospacelab-0.8.9/geospacelab/visualization/mpl/
+-rw-rw-r--   0 lei       (1000) lei       (1000)    31607 2023-12-15 13:01:10.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      825 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      747 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/_helpers.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      328 2021-08-30 07:16:41.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/axes.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    15132 2023-12-01 14:57:11.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/axis_ticks.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     7091 2023-11-09 08:32:05.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/colormaps.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    17218 2024-03-06 12:05:30.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/dashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3335 2021-11-29 20:45:17.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/figure.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2940 2023-08-22 10:11:11.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/__base__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      327 2022-08-30 10:45:18.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)     2847 2022-12-14 09:15:38.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/geodashboards.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    42815 2024-03-02 18:35:30.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/geopanels.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    34644 2024-04-18 07:24:21.000000 geospacelab-0.8.9/geospacelab/visualization/mpl/panels.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab/visualization/plotly/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-10-20 11:58:01.000000 geospacelab-0.8.9/geospacelab/visualization/plotly/__init__.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)      224 2021-10-20 11:58:01.000000 geospacelab-0.8.9/geospacelab/visualization/plotly/ipanel.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab/wrapper/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2021-07-13 05:22:19.000000 geospacelab-0.8.9/geospacelab/wrapper/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab/wrapper/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)     1067 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/LICENSE
+-rw-rw-r--   0 lei       (1000) lei       (1000)    16623 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/README.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:52:29.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/__init__.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/
+-rw-rw-r--   0 lei       (1000) lei       (1000)        0 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/__init__.py
+-rwxrwxr-x   0 lei       (1000) lei       (1000)    48858 2023-03-01 11:38:52.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/geopack.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    40639 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)    76431 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t01.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    75795 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t04.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    14024 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t89.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    65292 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t96.py
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15324 2023-03-01 10:54:57.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/test_geopack1.md
+-rw-rw-r--   0 lei       (1000) lei       (1000)     6669 2023-03-01 11:22:40.000000 geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/test_geopack1.py
+drwxrwxr-x   0 lei       (1000) lei       (1000)        0 2024-04-18 07:29:26.490771 geospacelab-0.8.9/geospacelab.egg-info/
+-rw-r--r--   0 lei       (1000) lei       (1000)    23831 2024-04-18 07:29:26.000000 geospacelab-0.8.9/geospacelab.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1000) lei       (1000)    15942 2024-04-18 07:29:26.000000 geospacelab-0.8.9/geospacelab.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)        1 2024-04-18 07:29:26.000000 geospacelab-0.8.9/geospacelab.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      234 2024-04-18 07:29:26.000000 geospacelab-0.8.9/geospacelab.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)       12 2024-04-18 07:29:26.000000 geospacelab-0.8.9/geospacelab.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1000) lei       (1000)      204 2024-04-18 07:29:26.490771 geospacelab-0.8.9/setup.cfg
+-rw-rw-r--   0 lei       (1000) lei       (1000)     3403 2023-11-10 11:11:22.000000 geospacelab-0.8.9/setup.py
```

### Comparing `geospacelab-0.8.8/LICENSE` & `geospacelab-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/PKG-INFO` & `geospacelab-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.8.8
+Version: 0.8.9
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.8.8/README.md` & `geospacelab-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/__init__.py` & `geospacelab-0.8.9/geospacelab/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2021 GeospaceLab (geospacelab)
 # Author: Lei Cai, Space Physics and Astronomy, University of Oulu
 
 __author__ = "Lei Cai"
 __copyright__ = "Copyright 2021, GeospaceLAB"
 __credits__ = ["Lei Cai"]
 __license__ = "BSD-3-Clause License"
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 __maintainer__ = "Lei Cai"
 __email__ = "lei.cai@oulu.fi"
 __status__ = "Developing"
 __docformat__ = "reStructureText"
 
 
 import geospacelab.config as config
```

### Comparing `geospacelab-0.8.8/geospacelab/config/__init__.py` & `geospacelab-0.8.9/geospacelab/config/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/config/_preferences.py` & `geospacelab-0.8.9/geospacelab/config/_preferences.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/__init__.py` & `geospacelab-0.8.9/geospacelab/cs/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/_aacgm.py` & `geospacelab-0.8.9/geospacelab/cs/_aacgm.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/_apex.py` & `geospacelab-0.8.9/geospacelab/cs/_apex.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/_cs_base.py` & `geospacelab-0.8.9/geospacelab/cs/_cs_base.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/_geo.py` & `geospacelab-0.8.9/geospacelab/cs/_geo.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/cs/geo_utilities.py` & `geospacelab-0.8.9/geospacelab/cs/geo_utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/__dataset_base__.py` & `geospacelab-0.8.9/geospacelab/datahub/__dataset_base__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,30 +79,37 @@
         self.kind = kind
         self.dt_fr = dt_fr
         self.dt_to = dt_to
         self.visual = visual
 
         self.label_fields = label_fields
 
-    def add_variable(self, var_name: str, configured_variables=None, variable_class=None, **kwargs) -> __variable_model__:
+    def add_variable(
+            self, var_name: str,
+            configured_variables=None, configured_variable_name=None,
+            variable_class=None, **kwargs) -> __variable_model__:
         """
         Add a variable to the dataset.
 
         :param var_name:
         :param configured_variables:
         :param variable_class:
         :param kwargs:
         :return:
         """
         if variable_class is None:
             variable_class = self.__variable_model__
         if configured_variables is None:
             configured_variables = {}
-        if var_name in configured_variables.keys():
-            configured_variable = configured_variables[var_name]
+        if var_name in configured_variables.keys() or configured_variable_name is not None:
+            if configured_variable_name is None:
+                vn = var_name
+            else:
+                vn = configured_variable_name
+            configured_variable = configured_variables[vn]
             if type(configured_variable) is dict:
                 self[var_name] = variable_class(**configured_variable)
             elif issubclass(configured_variable.__class__, self.__variable_model__):
                 self[var_name] = configured_variable.clone()
             # self[var_name].dataset = self
             self[var_name].visual = self.visual
         else:
@@ -456,14 +463,15 @@
     def data_root_dir(self):
         return self._data_root_dir
 
     @data_root_dir.setter
     def data_root_dir(self, path):
         self._data_root_dir = pathlib.Path(path)
 
+
 class LoaderBase(object):
     """
     Loader Base for loading data from the assigned files
     """
     def __init__(self):
         self.variables = {}
         self.metadata = {}
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/__metadata_base__.py` & `geospacelab-0.8.9/geospacelab/datahub/__metadata_base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/__variable_base__.py` & `geospacelab-0.8.9/geospacelab/datahub/__variable_base__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.tick_labels = None
         self.minor_ticks = None
         self.major_tick_min = None
         self.major_tick_max = None
         self.minor_tick_max = None
         self.reverse = False
         self.visible = True
+        self.shift = None
 
     def config(self, logging=True, **kwargs):
         pyclass.set_object_attributes(self, append=False, logging=logging, **kwargs)
 
 
 class VisualPlotConfig(object):
     """
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -219,18 +219,19 @@
         ca = sign_By * (np.pi/2 - np.arcsin(Bz / Bt))
         ca = np.mod(ca, 2 * np.pi)
 
         if not to_radian:
             ca = ca / np.pi * 180
 
         var_name = 'CA_' + cs
-        var = self.add_variable(var_name)
+        var = self.add_variable(var_name, configured_variables=var_config.configured_variables, configured_variable_name='CA')
         var.value = ca.reshape(ca.size, 1)
         var.label = r'$\theta$'
-        var.unit = 'rad'
+        var.unit = 'degree'
+        var.unit_label = r'($^\circ$)'
         self[var_name] = var
         return self[var_name]
 
     @_validate_IMF_cs
     def add_IMF_AZ(self, cs='GSM', to_radian=False,  **kwargs):
         """
         IMF azimuthal angle in the IMF Bx-By (x-y) plane in the GSE/GSM coordinate system.
@@ -244,18 +245,19 @@
         az = sign_Bx * (np.pi/2 - np.arcsin(By / Bt))
         az = np.mod(az, 2 * np.pi)
 
         if not to_radian:
             az = az / np.pi * 180
 
         var_name = 'AZ_' + cs
-        var = self.add_variable(var_name)
+        var = self.add_variable(var_name, configured_variables=var_config.configured_variables, configured_variable_name='CA')
         var.value = az.reshape(az.size, 1)
         var.label = r'$\phi$'
-        var.unit = 'rad'
+        var.unit = 'degree'
+        var.unit_label = r'($^\circ$)'
         self[var_name] = var
         return self[var_name]
 
     @_validate_IMF_cs
     def add_IMF_EL(self, cs='GSM', to_radian=False,  **kwargs):
         """
         IMF elevation angle in the IMF Bz-Bx (x-y) plane in the GSE/GSM coordinate system.
@@ -269,18 +271,19 @@
         el = sign_Bz * (np.pi / 2 - np.arcsin(Bx / Bt))
         el = np.mod(el, 2 * np.pi)
 
         if not to_radian:
             el = el / np.pi * 180
 
         var_name = 'EL_' + cs
-        var = self.add_variable(var_name)
+        var = self.add_variable(var_name, configured_variables=var_config.configured_variables, configured_variable_name='CA')
         var.value = el.reshape(el.size, 1)
         var.label = r'$\alpha$'
-        var.unit = 'rad'
+        var.unit = 'degree'
+        var.unit_label = r'($^\circ$)'
         self[var_name] = var
         return self[var_name]
 
     def add_NCF(self):
         """
         Solar wind-magnetosphere coupling function by Newell et al., JGR, 2007.
         :return:
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/cdaweb/omni/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/cdaweb/omni/variable_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,9 +242,36 @@
 # set axis attrs
 axis = var.visual.axis
 axis[1].data = "@v.value"
 axis[1].lim = [None, None]
 axis[1].label = '@v.label'
 axis[1].unit = '@v.unit'
 
+configured_variables[var_name] = var
+
+####################################################################################################################
+var_name = 'CA'
+var = Var(name=var_name, ndim=1, variable_type='scalar', visual=visual)
+# set variable attrs
+var.fullname = ''
+var.label = r''
+var.group = r''
+var.unit = ''
+var.depends = {0: depend_0}
+# set plot attrs
+plot_config = var.visual.plot_config
+plot_config.config(**default_plot_config)
+plot_config.line['linestyle'] = ''
+plot_config.line['marker'] = '.'
+plot_config.line['markersize'] = 3
+plot_config.style = '1noE'
+# set axis attrs
+axis = var.visual.axis
+axis[1].data = "@v.value"
+axis[1].lim = [0, 360]
+axis[1].label = '@v.label'
+axis[1].unit = '@v.unit'
+axis[1].ticks = [0, 90, 180, 270, 360]
+
+
+configured_variables[var_name] = var
 
-configured_variables[var_name] = var
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_lp_hm/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/advanced/efi_tct02/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 default_dataset_attrs = {
     'database': esaeo_database,
     'facility': swarm_facility,
     'instrument': 'MAG',
     'product': 'HR_1B',
     'data_file_ext': 'cdf',
     'product_version': 'latest',
-    'data_root_dir': prf.datahub_data_root_dir / 'ESA' / 'SWARM' / 'Level1b',
+    'data_root_dir': prf.datahub_data_root_dir / 'ESA' / 'SWARM' / 'Level1b' / 'MAG_HR',
     'allow_load': True,
     'allow_download': True,
     'force_download': False,
     'data_search_recursive': False,
     'add_AACGM': False,
     'add_APEX': False,
     'quality_control': False,
@@ -63,16 +63,16 @@
     def __init__(self, **kwargs):
         kwargs = basic.dict_set_default(kwargs, **default_dataset_attrs)
 
         super().__init__(**kwargs)
 
         self.database = kwargs.pop('database', 'ESA/EarthOnline')
         self.facility = kwargs.pop('facility', 'SWARM')
-        self.instrument = kwargs.pop('instrument', 'EFI-LP')
-        self.product = kwargs.pop('product', 'HM02')
+        self.instrument = kwargs.pop('instrument', 'MAG')
+        self.product = kwargs.pop('product', 'MAG_HR')
         self.product_version = kwargs.pop('product_version', '')
         self.local_latest_version = ''
         self.allow_download = kwargs.pop('allow_download', False)
         self.force_download = kwargs.pop('force_download', False)
         self.quality_control = kwargs.pop('quality_control', False)
         self.calib_control = kwargs.pop('calib_control', False)
         self.add_AACGM = kwargs.pop('add_AACGM', False)
@@ -100,15 +100,15 @@
 
     def _validate_attrs(self):
         for attr_name in default_attrs_required:
             attr = getattr(self, attr_name)
             if not list(attr):
                 mylog.StreamLogger.warning("The parameter {} is required before loading data!".format(attr_name))
 
-        self.data_root_dir = self.data_root_dir / self.instrument / self.product
+        # self.data_root_dir = self.data_root_dir / self.product
 
         if str(self.product_version) and self.product_version != 'latest':
             self.data_root_dir = self.data_root_dir / self.product_version
         else:
             self.product_version = 'latest'
             self.force_download = False
             mylog.simpleinfo.info(f'Checking the latest version of the data file ...')
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,37 +16,36 @@
 class Downloader(DownloaderModel):
 
     _default_file_name_patterns = ['SW_OPER']
 
     def __init__(
             self, dt_fr, dt_to,
             sat_id=None,
-            data_type='HR_1B',
             file_version=None,
             file_extension='.cdf',
             data_file_root_dir=None,
             ftp_data_dir=None,
             force=True, direct_download=True, **kwargs
     ):
 
         self.sat_id = sat_id
 
         if ftp_data_dir is None:
             ftp_data_dir = f'Level1b/Latest_baselines/MAGx_HR/Sat_{sat_id.upper()}'
 
         if data_file_root_dir is None:
-            data_file_root_dir = prf.datahub_data_root_dir / "ESA" / "SWARM" / "Level1b" / "MAG" / data_type
+            data_file_root_dir = prf.datahub_data_root_dir / "ESA" / "SWARM" / "Level1b" / "MAG_HR"
         file_name_patterns = list(self._default_file_name_patterns)
         file_name_patterns.extend(['MAG' + sat_id.upper(), dt_fr.strftime("%Y%m")])
         super(Downloader, self).__init__(
             dt_fr, dt_to,
             data_file_root_dir=data_file_root_dir,
             ftp_data_dir=ftp_data_dir,
             file_version=file_version,
-            file_extension = file_extension,
+            file_extension=file_extension,
             force=force, direct_download=direct_download,
             file_name_patterns=file_name_patterns, **kwargs
         )
 
     def download(self, **kwargs):
 
         done = super(Downloader, self).download(**kwargs)
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/l1b/mag_hr/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/esa_eo/swarm/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/esa_eo/swarm/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/fmi/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/fmi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/fmi/image/ie/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/fmi/image/ie/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/hpo/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/hpo/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/nowcast/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/kpap/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/kpap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/gfz/snf107/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/gfz/snf107/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/isee/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/isee/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/isee/gnss/tecmap/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/isee/gnss/tecmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/fitted/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/ampere/grd/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/ampere/grd/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/edraur/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         variables['STOPPING_TIME'] = stopping_time
         dt0 = dttool.get_start_of_the_day(starting_time)
 
         # Time and position
         sectime = pybasic.str_join('TIME', pp_key_1, pp_key_2, separator='_', uppercase=True)
         sectime = np.array(dataset.variables[sectime])
         cdfepoch = pybasic.str_join('TIME', 'EPOCH', pp_key_1, pp_key_2, separator='_', uppercase=True)
-        dts = cdflib.cdfepoch.unixtime(np.array(dataset.variables[cdfepoch]), to_np=True)
+        dts = cdflib.cdfepoch.unixtime(np.array(dataset.variables[cdfepoch]))
         dts = dttool.convert_unix_time_to_datetime_cftime(dts)
 
         var_name_nc = pybasic.str_join('ORBIT', pp_key_1, pp_key_2, separator='_', uppercase=True)
         variables['SC_ORBIT_ID'] = np.array(dataset.variables[var_name_nc])
 
         var_name_nc = pybasic.str_join('LATITUDE', pp_key_1, pp_key_2, separator='_', uppercase=True)
         geo_lat = np.array(dataset.variables[var_name_nc])
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/jhuapl/dmsp/ssusi/sdrdisk/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,33 +114,34 @@
         self.data_file_paths.append(file_path_local)
         
         if file_path_local.is_file():
             mylog.simpleinfo.info("The file {} has been downloaded.".format(file_path_local.name))
             if not self.force_download:
                 return
         files_error = []
+        mylog.simpleinfo.info("Downloading {} ...".format(file_path_remote))
         try:
             database.downloadFile(
                 file_path_remote, file_path_local,
                 self.user_fullname, self.user_email, self.user_affiliation,
                 file_format
             )
 
-            mylog.simpleinfo.info("File saved in {}.".format(file_path_local))
+            mylog.simpleinfo.info("--> Saved as {}.".format(file_path_local))
             self.done = True
         except Exception as e:
             try:
                 time.sleep(3)
                 database.downloadFile(
                     file_path_remote, file_path_local,
                     self.user_fullname, self.user_email, self.user_affiliation,
                     file_format
                 )
 
-                mylog.simpleinfo.info("File saved in {}.".format(file_path_local))
+                mylog.simpleinfo.info("--> Saved as {}.".format(file_path_local))
                 self.done = True 
             except:
                 print(e)
                 mylog.StreamLogger.warning(f"Failed to download the file: {file_path_remote}")
         return
     
     @staticmethod
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/gnss/tecmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,24 @@
             soup = bs4.BeautifulSoup(r.text, 'html.parser')
             links = soup.find_all('a', href=True)
             for link in links:
                 href = link['href']
                 if any(href.endswith(s) for s in ['.png', '.tar.gz', '.hdf5']):
                     filename = href.split('/')[-1]
 
-                    match = re.search('\d{4}-\d{2}-\d{2}', filename)
+                    match = re.search(r'\d{4}-\d{2}-\d{2}', filename)
                     thisday = datetime.datetime.strptime(match.group(), '%Y-%m-%d')
                     if thisday < self.dt_fr or thisday > self.dt_to:
                         continue
                     for key, value in locs.items():
                         if '/' + value + '/' in href:
                             site = key
 
                     #site1 = re.search("[@|_][a-zA-Z0-9]*[.]", filename).group(0)[1:-1]
-                    search_pattern = re.search("\d{4}-\d{2}-\d{2}_[a-zA-Z0-9]*", filename).group(0)
+                    search_pattern = re.search(r"\d{4}-\d{2}-\d{2}_[a-zA-Z0-9]*", filename).group(0)
                     sub_dir = search_pattern + '@' + site
                     data_file_dir = self.data_file_root_dir / site / thisday.strftime('%Y') / sub_dir
                     data_file_dir.mkdir(parents=True, exist_ok=True)
 
                     remote_file = requests.get(href)
                     file_path = data_file_dir / filename
                     if file_path.is_file():
@@ -184,22 +184,22 @@
                     if not download_pp and 'GUISDAP pp' in file.kindatdesc:
                         continue
                     file_path = pathlib.Path(file.name)
                     site = file_path.name.split("@")[1][0:3].upper()
                     if '32' in site or '42' in site:
                         site = 'ESR'
 
-                    match = re.search('\d{4}-\d{2}-\d{2}', file_path.name)
+                    match = re.search(r'\d{4}-\d{2}-\d{2}', file_path.name)
                     dt_str = match.group(0)
                     thisday = datetime.datetime.strptime(dt_str, "%Y-%m-%d")
                     if thisday < self.dt_fr or thisday > self.dt_to:
                         continue
 
                     # sub_dir = file_path.name.split('_', maxsplit=1)[1]
-                    search_pattern = re.search("\d{4}-\d{2}-\d{2}_[a-zA-Z0-9]*", file_path.name).group(0)
+                    search_pattern = re.search(r"\d{4}-\d{2}-\d{2}_[a-zA-Z0-9]*", file_path.name).group(0)
                     sub_dir = search_pattern + '@' + site
                     data_file_dir = self.data_file_root_dir / site / dt_str[0:4] / sub_dir
                     data_file_dir.mkdir(parents=True, exist_ok=True)
                     data_file_path = data_file_dir / file_path.name
                     if data_file_path.is_file():
                         mylog.simpleinfo.info("The file {} has been downloaded.".format(data_file_path.name))
                         continue
@@ -385,15 +385,15 @@
         if file_name is None:
             file_name = "EISCAT_archives.txt"
         if file_path is None:
             file_path = self.root_filepath
 
         with open(os.path.join(file_path, file_name), 'w') as out_file:
             for line in self.experiments:
-                line_str = "{0:<17s}{1:<7s}{2:<5s}{3:<6s}{4:<20s}{5:<25s}{6:<20s}{7:<30s}{8:<65s}".format(
+                line_str = "{0:<17s}{1:<7s}{2:<5s}{3:<8s}{4:<30s}{5:<40s}{6:<40s}{7:<80s}{8:<65s}".format(
                     line[0].strftime('%Y-%m-%d %H:%M'), line[1].strftime('%H:%M'),
                     line[7], line[2], line[3], line[4], line[5], line[6], line[8]) + '\n'
                 out_file.write(line_str)
 
 
 def is_date(string, fuzzy=False):
     """
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/examples/eiscat_hdf5_info.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/basic/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/gridded/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/millstonehill/vi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/fitted/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/pfisr/vi/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/e/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s1/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/satellites/dmsp/s4/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/madrigal/utilities.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/nipr/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/nipr/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/nipr/asc/tro_wmi/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/nipr/asc/tro_wmi/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/madrigal/isr/eiscat/variable_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             'GEO_ALT': 'GEO_ALT', 'AACGM_LAT': 'AACGM_LAT', 'AACGM_LON': 'AACGM_LON'}
 
 default_colormap = cm.cmap_jet_modified()
 
 default_axis_dict_2d = {
     1:     {
         'data':     '@d.HEIGHT.value',
-        'lim':      [90, 350],
+        'lim':      [80, 500],
         'label':    'h',
         'unit':     'km',
     },
     2:  {
         'data':     '@v.value',
         'label':    '@v.label',
         'unit':     '@v.unit_label',
@@ -81,15 +81,15 @@
 var.visual.axis[1].config(**default_axis_dict_2d[1])
 var.visual.axis[2].config(**default_axis_dict_2d[2])
 var.visual.axis[2].scale = 'log'
 var.visual.axis[2].lim = [8e9, 9e11]
 # axis = var.visual.axis
 # axis[1].data = "@d.height.value"
 # axis[2].data = "@v.value"
-# axis[1].lim = [90, 350]
+# axis[1].lim = [80, 500]
 # axis[1].label = 'h'
 # axis[1].unit = 'km'
 # axis[2].lim = [8e9, 9e11]
 # axis[2].scale = 'log'
 # axis[2].label = '@v.label'
 # axis[2].unit = '@v.unit_label'
 
@@ -107,15 +107,15 @@
 # set plot attrs
 var.visual.plot_config.config(**default_plot_config)
 var.visual.plot_config.style = '2P'
 # set axis attrs
 axis = var.visual.axis
 axis[1].data = "@d.HEIGHT.value"
 axis[2].data = "@v.value"
-axis[1].lim = [90, 350]
+axis[1].lim = [80, 500]
 axis[1].label = 'h'
 axis[1].unit = 'km'
 axis[2].lim = [100, 2500]
 axis[2].scale = 'linear'
 axis[2].label = '@v.label'
 axis[2].unit = '@v.unit_label'
 
@@ -133,15 +133,15 @@
 # set plot attrs
 var.visual.plot_config.config(**default_plot_config)
 var.visual.plot_config.style = '2P'
 # set axis attrs
 axis = var.visual.axis
 axis[1].data = "@d.HEIGHT.value"
 axis[2].data = "@v.value"
-axis[1].lim = [90, 350]
+axis[1].lim = [80, 500]
 axis[1].label = 'h'
 axis[1].unit = 'km'
 axis[2].lim = [100, 3500]
 axis[2].scale = 'linear'
 axis[2].label = '@v.label'
 axis[2].unit = '@v.unit_label'
 
@@ -159,15 +159,15 @@
 # set plot attrs
 var.visual.plot_config.config(**default_plot_config)
 var.visual.plot_config.style = '2P'
 # set axis attrs
 axis = var.visual.axis
 axis[1].data = "@d.HEIGHT.value"
 axis[2].data = "@v.value"
-axis[1].lim = [90, 350]
+axis[1].lim = [80, 500]
 axis[1].label = 'h'
 axis[1].unit = 'km'
 axis[2].lim = [-400, 400]
 axis[2].scale = 'linear'
 axis[2].label = '@v.label'
 axis[2].unit = '@v.unit_label'
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/superdarn/potmap/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/superdarn/potmap/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
         self.dt_fr = dt_fr
         self.dt_to = dt_to
         if user_id is None:
             self.user_id = prf.user_config['datahub']['supermag']['username']
         self.products = products
 
         self.force_download = force_download
-        self.download()
         self.done = False
+        self.download()
 
     def download(self):
         num_days = dttool.get_diff_days(self.dt_fr, self.dt_to)
         for nd in range(num_days+1):
             this_day = dttool.get_start_of_the_day(self.dt_fr) + datetime.timedelta(days=nd)
             extent = 86400.
 
@@ -139,15 +139,16 @@
             )
             if status == 1:
                 self.save_to_nc(idxdata, file_path)
             else:
                 self.done = False
                 mylog.StreamLogger.error(f'The requested data cannot be downloaded!')
                 return
-            self.download = True
+            self.done = True
+
     def save_to_nc(self, idxdata, file_path):
         def sm_t_to_datetime(tval):
             jd = (tval / 86400.0) + 2440587.5
             timestamp = pd.to_datetime(jd, unit='D', origin='julian')  # format YYYY-MM-DD HH:MM:SS.ssssss
             return timestamp.to_pydatetime()
         vars = {}
         dts = []
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/indices/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/indices/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/supermag/supermag_api.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/supermag/supermag_api.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/champ/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/goce/dns_wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace/wnd_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,81 +4,78 @@
 
 import numpy as np
 import datetime
 
 import geospacelab.datahub as datahub
 from geospacelab.datahub import DatabaseModel, FacilityModel, InstrumentModel, ProductModel
 from geospacelab.datahub.sources.tud import tud_database
-from geospacelab.datahub.sources.tud.grace_fo import grace_facility
+from geospacelab.datahub.sources.tud.swarm import swarm_facility
 from geospacelab.config import prf
 import geospacelab.toolbox.utilities.pybasic as basic
 import geospacelab.toolbox.utilities.pylogging as mylog
 import geospacelab.toolbox.utilities.pydatetime as dttool
-from geospacelab.datahub.sources.tud.grace_fo.dns_acc.loader import Loader as default_Loader
-from geospacelab.datahub.sources.tud.grace_fo.dns_acc.downloader import Downloader as default_Downloader
-import geospacelab.datahub.sources.tud.grace_fo.dns_acc.variable_config as var_config
+from geospacelab.datahub.sources.tud.swarm.dns_acc.loader import Loader as default_Loader
+from geospacelab.datahub.sources.tud.swarm.dns_acc.downloader import Downloader as default_Downloader
+import geospacelab.datahub.sources.tud.swarm.dns_acc.variable_config as var_config
 
 
 default_dataset_attrs = {
     'database': tud_database,
-    'facility': grace_facility,
+    'facility': swarm_facility,
     'instrument': 'ACC',
+    'sat_id': 'C',
     'product': 'DNS-ACC',
     'data_file_ext': 'txt',
-    'product_version': 'v02',
-    'data_root_dir': prf.datahub_data_root_dir / 'TUD' / 'GRACE-FO',
+    'product_version': 'v01',
+    'data_root_dir': prf.datahub_data_root_dir / 'TUD' / 'SWARM',
     'allow_load': True,
     'allow_download': True,
     'force_download': False,
     'data_search_recursive': False,
     'add_AACGM': False,
     'add_APEX': False,
     'label_fields': ['database', 'facility', 'instrument', 'product', 'product_version'],
     'load_mode': 'AUTO',
     'time_clip': True,
 }
 
-default_variable_names_v01 = []
-default_variable_names_v02 = [
+default_variable_names = [
     'SC_DATETIME',
     'SC_GEO_LAT',
     'SC_GEO_LON',
     'SC_GEO_ALT',
     'SC_ARG_LAT',
     'SC_GEO_LST',
     'rho_n',
-    'rho_n_MEAN',
-    'FLAG',
-    'FLAG_MEAN',
     ]
 
 # default_data_search_recursive = True
 
 default_attrs_required = ['sat_id']
 
 
 class Dataset(datahub.DatasetSourced):
     def __init__(self, **kwargs):
         kwargs = basic.dict_set_default(kwargs, **default_dataset_attrs)
 
         super().__init__(**kwargs)
 
         self.database = kwargs.pop('database', 'TUD')
-        self.facility = kwargs.pop('facility', 'GRACE')
+        self.facility = kwargs.pop('facility', 'SWARM')
         self.instrument = kwargs.pop('instrument', 'ACC')
         self.product = kwargs.pop('product', 'DNS-ACC')
         self.product_version = kwargs.pop('product_version', 'v01')
         self.local_latest_version = ''
         self.allow_download = kwargs.pop('allow_download', False)
         self.force_download = kwargs.pop('force_download', False)
         self.add_AACGM = kwargs.pop('add_AACGM', False) 
         self.add_APEX = kwargs.pop('add_APEX', False)
         self._data_root_dir = self.data_root_dir    # Record the initial root dir
 
-        self.sat_id = kwargs.pop('sat_id', 'FO1')
+        self.sat_id = kwargs.pop('sat_id', 'C')
 
         self.metadata = None
 
         allow_load = kwargs.pop('allow_load', False)
 
         # self.config(**kwargs)
 
@@ -103,18 +100,15 @@
 
     def label(self, **kwargs):
         label = super().label()
         return label
 
     def load_data(self, **kwargs):
         self.check_data_files(**kwargs)
-        if self.product_version == 'v01':
-            default_variable_names = default_variable_names_v01
-        else:
-            default_variable_names = default_variable_names_v02 
+
         self._set_default_variables(
             default_variable_names,
             configured_variables=var_config.configured_variables
         )
         for file_path in self.data_file_paths:
             load_obj = self.loader(file_path, file_type='txt', version=self.product_version)
 
@@ -180,20 +174,17 @@
 
         for i in range(diff_months + 1):
             this_day = dttool.get_next_n_months(dt0, i)
 
             initial_file_dir = kwargs.pop(
                 'initial_file_dir', self.data_root_dir
             )
-            if self.sat_id == 'FO1':
-                sat_id='C'
-            else:
-                raise NotImplementedError
+
             file_patterns = [
-                'G' + sat_id,
+                'S' + self.sat_id.upper(),
                 self.product.upper().replace('-', '_'),
                 this_day.strftime('%Y_%m'),
             ]
             # remove empty str
             file_patterns = [pattern for pattern in file_patterns if str(pattern)]
             search_pattern = '*' + '*'.join(file_patterns) + '*'
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             sat_id=None,
             product='DNS-ACC',
             version='v02',
             force=True, direct_download=True, **kwargs
     ):
         if version == 'v01':
             raise ValueError
-        elif version == 'v02':
+        elif 'v02' in version:
             v_str = "version_02"
         else:
             raise NotImplementedError
         if sat_id == 'FO1':
                 sat_id='C'
         else:
             raise NotImplementedError
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if direct_load:
             self.load()
 
     def load(self):
 
         if self.version == 'v01':
             raise ValueError
-        elif self.version == 'v02':
+        elif self.version in ['v02', 'v02b']:
             self.load_v02()
         else:
             raise NotImplementedError
 
 
     def load_v02(self):
         with open(self.file_path, 'r') as f:
@@ -54,8 +54,8 @@
             self.variables['SC_GEO_LON'] = np.array(results[3]).astype(np.float32).reshape(num_rec, 1)
             self.variables['SC_GEO_LAT'] = np.array(results[4]).astype(np.float32).reshape(num_rec, 1)
             self.variables['SC_GEO_LST'] = np.array(results[5]).astype(np.float32).reshape(num_rec, 1)
             self.variables['SC_ARG_LAT'] = np.array(results[6]).astype(np.float32).reshape(num_rec, 1)
             self.variables['rho_n'] = np.array(results[7]).astype(np.float32).reshape(num_rec, 1)
             self.variables['rho_n_MEAN'] = np.array(results[8]).astype(np.float32).reshape(num_rec, 1) 
             self.variables['FLAG'] = np.array(results[9]).astype(np.float32).reshape(num_rec, 1) 
-            self.variables['FLAG_MEAN'] = np.array(results[10]).astype(np.float32).reshape(num_rec, 1)  
+            self.variables['FLAG_MEAN'] = np.array(results[10]).reshape(num_rec, 1)
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 from geospacelab.datahub import DatabaseModel, FacilityModel, InstrumentModel, ProductModel
 from geospacelab.datahub.sources.tud import tud_database
 from geospacelab.datahub.sources.tud.swarm import swarm_facility
 from geospacelab.config import prf
 import geospacelab.toolbox.utilities.pybasic as basic
 import geospacelab.toolbox.utilities.pylogging as mylog
 import geospacelab.toolbox.utilities.pydatetime as dttool
-from geospacelab.datahub.sources.tud.swarm.dns_acc.loader import Loader as default_Loader
-from geospacelab.datahub.sources.tud.swarm.dns_acc.downloader import Downloader as default_Downloader
-import geospacelab.datahub.sources.tud.swarm.dns_acc.variable_config as var_config
+from geospacelab.datahub.sources.tud.swarm.dns_pod.loader import Loader as default_Loader
+from geospacelab.datahub.sources.tud.swarm.dns_pod.downloader import Downloader as default_Downloader
+import geospacelab.datahub.sources.tud.swarm.dns_pod.variable_config as var_config
 
 
 default_dataset_attrs = {
     'database': tud_database,
     'facility': swarm_facility,
-    'instrument': 'ACC',
-    'sat_id': 'C',
-    'product': 'DNS-ACC',
+    'instrument': 'POD',
+    'product': 'DNS-POD',
     'data_file_ext': 'txt',
     'product_version': 'v01',
     'data_root_dir': prf.datahub_data_root_dir / 'TUD' / 'SWARM',
     'allow_load': True,
     'allow_download': True,
     'force_download': False,
     'data_search_recursive': False,
@@ -57,25 +56,25 @@
     def __init__(self, **kwargs):
         kwargs = basic.dict_set_default(kwargs, **default_dataset_attrs)
 
         super().__init__(**kwargs)
 
         self.database = kwargs.pop('database', 'TUD')
         self.facility = kwargs.pop('facility', 'SWARM')
-        self.instrument = kwargs.pop('instrument', 'ACC')
-        self.product = kwargs.pop('product', 'DNS-ACC')
+        self.instrument = kwargs.pop('instrument', 'POD')
+        self.product = kwargs.pop('product', 'DNS-POD')
         self.product_version = kwargs.pop('product_version', 'v01')
         self.local_latest_version = ''
         self.allow_download = kwargs.pop('allow_download', False)
         self.force_download = kwargs.pop('force_download', False)
         self.add_AACGM = kwargs.pop('add_AACGM', False) 
         self.add_APEX = kwargs.pop('add_APEX', False)
         self._data_root_dir = self.data_root_dir    # Record the initial root dir
 
-        self.sat_id = kwargs.pop('sat_id', 'C')
+        self.sat_id = kwargs.pop('sat_id', 'A')
 
         self.metadata = None
 
         allow_load = kwargs.pop('allow_load', False)
 
         # self.config(**kwargs)
 
@@ -159,14 +158,67 @@
         self.add_variable('SC_AACGM_LAT')
         self.add_variable('SC_AACGM_LON')
         self.add_variable('SC_AACGM_MLT')
         self['SC_AACGM_LAT'].value = cs_aacgm['lat'].reshape(self['SC_DATETIME'].value.shape)
         self['SC_AACGM_LON'].value = cs_aacgm['lon'].reshape(self['SC_DATETIME'].value.shape)
         self['SC_AACGM_MLT'].value = cs_aacgm['mlt'].reshape(self['SC_DATETIME'].value.shape)
 
+    def interp_evenly(self, time_res=30, dt_fr=None, dt_to=None):
+        from scipy.interpolate import interp1d
+        import geospacelab.toolbox.utilities.numpymath as nm
+
+        ds_new = datahub.DatasetUser(dt_fr=self.dt_fr, dt_to=self.dt_to, visual=self.visual)
+        ds_new.clone_variables(self)
+        dts = ds_new['SC_DATETIME'].value.flatten()
+        dt0 = dttool.get_start_of_the_day(dts[0])
+        x_0 = np.array([(dt - dt0).total_seconds() for dt in dts])
+        if dt_fr is None:
+            dt_fr = dts[0] - datetime.timedelta(
+                seconds=np.floor(((dts[0] - ds_new.dt_fr).total_seconds() / time_res)) * time_res
+            )
+        if dt_to is None:
+            dt_to = dts[-1] + datetime.timedelta(
+                seconds=np.floor(((ds_new.dt_to - dts[-1]).total_seconds() / time_res)) * time_res
+            )
+        sec_fr = (dt_fr - dt0).total_seconds()
+        sec_to = (dt_to - dt0).total_seconds()
+        x_1 = np.arange(sec_fr, sec_to + time_res / 2, time_res)
+
+        f = interp1d(x_0, x_0, kind='nearest', bounds_error=False, fill_value=(x_0[0], x_0[-1]))
+        pseudo_x = f(x_1)
+        mask = np.abs(pseudo_x - x_1) > time_res / 1.5
+
+        dts_new = np.array([dt0 + datetime.timedelta(seconds=sec) for sec in x_1])
+        ds_new['SC_DATETIME'].value = dts_new.reshape((dts_new.size, 1))
+
+        period_var_dict = {'SC_GEO_LON': 360.,
+                           'SC_AACGM_LON': 360.,
+                           'SC_APEX_LON': 360.,
+                           'SC_GEO_LST': 24.,
+                           'SC_AACGM_MLT': 24.,
+                           'SC_APEX_MLT': 24}
+
+        for var_name in ds_new.keys():
+            if var_name in ['SC_DATETIME']:
+                continue
+            if var_name in period_var_dict.keys():
+                var = ds_new[var_name].value.flatten()
+                var_new = nm.interp_period_data(x_0, var, x_1, period=period_var_dict[var_name], method='linear',
+                                                bounds_error=False)
+                var_new[mask] = np.nan
+                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
+            else:
+                method = 'linear' if 'FLAG' not in var_name else 'nearest'
+                var = ds_new[var_name].value.flatten()
+                f = interp1d(x_0, var, kind=method, bounds_error=False)
+                var_new = f(x_1)
+                var_new[mask] = np.nan
+                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
+        return ds_new
+
     def search_data_files(self, **kwargs):
 
         dt_fr = self.dt_fr
         dt_to = self.dt_to
 
         diff_months = dttool.get_diff_months(dt_fr, dt_to)
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_acc/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/grace_fo/dns_acc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,77 +4,81 @@
 
 import numpy as np
 import datetime
 
 import geospacelab.datahub as datahub
 from geospacelab.datahub import DatabaseModel, FacilityModel, InstrumentModel, ProductModel
 from geospacelab.datahub.sources.tud import tud_database
-from geospacelab.datahub.sources.tud.swarm import swarm_facility
+from geospacelab.datahub.sources.tud.grace_fo import grace_facility
 from geospacelab.config import prf
 import geospacelab.toolbox.utilities.pybasic as basic
 import geospacelab.toolbox.utilities.pylogging as mylog
 import geospacelab.toolbox.utilities.pydatetime as dttool
-from geospacelab.datahub.sources.tud.swarm.dns_pod.loader import Loader as default_Loader
-from geospacelab.datahub.sources.tud.swarm.dns_pod.downloader import Downloader as default_Downloader
-import geospacelab.datahub.sources.tud.swarm.dns_pod.variable_config as var_config
+from geospacelab.datahub.sources.tud.grace_fo.dns_acc.loader import Loader as default_Loader
+from geospacelab.datahub.sources.tud.grace_fo.dns_acc.downloader import Downloader as default_Downloader
+import geospacelab.datahub.sources.tud.grace_fo.dns_acc.variable_config as var_config
 
 
 default_dataset_attrs = {
     'database': tud_database,
-    'facility': swarm_facility,
-    'instrument': 'POD',
-    'product': 'DNS-POD',
+    'facility': grace_facility,
+    'instrument': 'ACC',
+    'product': 'DNS-ACC',
     'data_file_ext': 'txt',
-    'product_version': 'v01',
-    'data_root_dir': prf.datahub_data_root_dir / 'TUD' / 'SWARM',
+    'product_version': 'v02',
+    'data_root_dir': prf.datahub_data_root_dir / 'TUD' / 'GRACE-FO',
     'allow_load': True,
     'allow_download': True,
     'force_download': False,
     'data_search_recursive': False,
     'add_AACGM': False,
     'add_APEX': False,
     'label_fields': ['database', 'facility', 'instrument', 'product', 'product_version'],
     'load_mode': 'AUTO',
     'time_clip': True,
 }
 
-default_variable_names = [
+default_variable_names_v01 = []
+default_variable_names_v02 = [
     'SC_DATETIME',
     'SC_GEO_LAT',
     'SC_GEO_LON',
     'SC_GEO_ALT',
     'SC_ARG_LAT',
     'SC_GEO_LST',
     'rho_n',
+    'rho_n_MEAN',
+    'FLAG',
+    'FLAG_MEAN',
     ]
 
 # default_data_search_recursive = True
 
 default_attrs_required = ['sat_id']
 
 
 class Dataset(datahub.DatasetSourced):
     def __init__(self, **kwargs):
         kwargs = basic.dict_set_default(kwargs, **default_dataset_attrs)
 
         super().__init__(**kwargs)
 
         self.database = kwargs.pop('database', 'TUD')
-        self.facility = kwargs.pop('facility', 'SWARM')
-        self.instrument = kwargs.pop('instrument', 'POD')
-        self.product = kwargs.pop('product', 'DNS-POD')
+        self.facility = kwargs.pop('facility', 'GRACE')
+        self.instrument = kwargs.pop('instrument', 'ACC')
+        self.product = kwargs.pop('product', 'DNS-ACC')
         self.product_version = kwargs.pop('product_version', 'v01')
         self.local_latest_version = ''
         self.allow_download = kwargs.pop('allow_download', False)
         self.force_download = kwargs.pop('force_download', False)
         self.add_AACGM = kwargs.pop('add_AACGM', False) 
         self.add_APEX = kwargs.pop('add_APEX', False)
         self._data_root_dir = self.data_root_dir    # Record the initial root dir
 
-        self.sat_id = kwargs.pop('sat_id', 'A')
+        self.sat_id = kwargs.pop('sat_id', 'FO1')
 
         self.metadata = None
 
         allow_load = kwargs.pop('allow_load', False)
 
         # self.config(**kwargs)
 
@@ -91,23 +95,29 @@
 
     def _validate_attrs(self):
         for attr_name in default_attrs_required:
             attr = getattr(self, attr_name)
             if not attr:
                 mylog.StreamLogger.warning("The parameter {} is required before loading data!".format(attr_name))
 
-        self.data_root_dir = self.data_root_dir / self.product.upper() / self.product_version
+        if self.product_version == 'v02b':
+            self.data_root_dir = self.data_root_dir / self.product.upper() / self.product_version[:-1]
+        else:
+            self.data_root_dir = self.data_root_dir / self.product.upper() / self.product_version
 
     def label(self, **kwargs):
         label = super().label()
         return label
 
     def load_data(self, **kwargs):
         self.check_data_files(**kwargs)
-
+        if self.product_version == 'v01':
+            default_variable_names = default_variable_names_v01
+        else:
+            default_variable_names = default_variable_names_v02 
         self._set_default_variables(
             default_variable_names,
             configured_variables=var_config.configured_variables
         )
         for file_path in self.data_file_paths:
             load_obj = self.loader(file_path, file_type='txt', version=self.product_version)
 
@@ -158,67 +168,14 @@
         self.add_variable('SC_AACGM_LAT')
         self.add_variable('SC_AACGM_LON')
         self.add_variable('SC_AACGM_MLT')
         self['SC_AACGM_LAT'].value = cs_aacgm['lat'].reshape(self['SC_DATETIME'].value.shape)
         self['SC_AACGM_LON'].value = cs_aacgm['lon'].reshape(self['SC_DATETIME'].value.shape)
         self['SC_AACGM_MLT'].value = cs_aacgm['mlt'].reshape(self['SC_DATETIME'].value.shape)
 
-    def interp_evenly(self, time_res=30, dt_fr=None, dt_to=None):
-        from scipy.interpolate import interp1d
-        import geospacelab.toolbox.utilities.numpymath as nm
-
-        ds_new = datahub.DatasetUser(dt_fr=self.dt_fr, dt_to=self.dt_to, visual=self.visual)
-        ds_new.clone_variables(self)
-        dts = ds_new['SC_DATETIME'].value.flatten()
-        dt0 = dttool.get_start_of_the_day(dts[0])
-        x_0 = np.array([(dt - dt0).total_seconds() for dt in dts])
-        if dt_fr is None:
-            dt_fr = dts[0] - datetime.timedelta(
-                seconds=np.floor(((dts[0] - ds_new.dt_fr).total_seconds() / time_res)) * time_res
-            )
-        if dt_to is None:
-            dt_to = dts[-1] + datetime.timedelta(
-                seconds=np.floor(((ds_new.dt_to - dts[-1]).total_seconds() / time_res)) * time_res
-            )
-        sec_fr = (dt_fr - dt0).total_seconds()
-        sec_to = (dt_to - dt0).total_seconds()
-        x_1 = np.arange(sec_fr, sec_to + time_res / 2, time_res)
-
-        f = interp1d(x_0, x_0, kind='nearest', bounds_error=False, fill_value=(x_0[0], x_0[-1]))
-        pseudo_x = f(x_1)
-        mask = np.abs(pseudo_x - x_1) > time_res / 1.5
-
-        dts_new = np.array([dt0 + datetime.timedelta(seconds=sec) for sec in x_1])
-        ds_new['SC_DATETIME'].value = dts_new.reshape((dts_new.size, 1))
-
-        period_var_dict = {'SC_GEO_LON': 360.,
-                           'SC_AACGM_LON': 360.,
-                           'SC_APEX_LON': 360.,
-                           'SC_GEO_LST': 24.,
-                           'SC_AACGM_MLT': 24.,
-                           'SC_APEX_MLT': 24}
-
-        for var_name in ds_new.keys():
-            if var_name in ['SC_DATETIME']:
-                continue
-            if var_name in period_var_dict.keys():
-                var = ds_new[var_name].value.flatten()
-                var_new = nm.interp_period_data(x_0, var, x_1, period=period_var_dict[var_name], method='linear',
-                                                bounds_error=False)
-                var_new[mask] = np.nan
-                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
-            else:
-                method = 'linear' if 'FLAG' not in var_name else 'nearest'
-                var = ds_new[var_name].value.flatten()
-                f = interp1d(x_0, var, kind=method, bounds_error=False)
-                var_new = f(x_1)
-                var_new[mask] = np.nan
-                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
-        return ds_new
-
     def search_data_files(self, **kwargs):
 
         dt_fr = self.dt_fr
         dt_to = self.dt_to
 
         diff_months = dttool.get_diff_months(dt_fr, dt_to)
 
@@ -226,19 +183,22 @@
 
         for i in range(diff_months + 1):
             this_day = dttool.get_next_n_months(dt0, i)
 
             initial_file_dir = kwargs.pop(
                 'initial_file_dir', self.data_root_dir
             )
-
+            if self.sat_id == 'FO1':
+                sat_id='C'
+            else:
+                raise NotImplementedError
             file_patterns = [
-                'S' + self.sat_id.upper(),
+                'G' + sat_id,
                 self.product.upper().replace('-', '_'),
-                this_day.strftime('%Y_%m'),
+                this_day.strftime('%Y_%m'), self.product_version + '.'
             ]
             # remove empty str
             file_patterns = [pattern for pattern in file_patterns if str(pattern)]
             search_pattern = '*' + '*'.join(file_patterns) + '*'
 
             done = super().search_data_files(
                 initial_file_dir=initial_file_dir,
@@ -270,14 +230,66 @@
             product=self.product,
             version=self.product_version,
             force=self.force_download
         )
 
         return download_obj.done
 
+    def interp_evenly(self, time_res=10, time_res_o=10, dt_fr=None, dt_to=None):
+        from scipy.interpolate import interp1d
+        import geospacelab.toolbox.utilities.numpymath as nm
+
+        ds_new = datahub.DatasetUser(dt_fr=self.dt_fr, dt_to=self.dt_to, visual=self.visual)
+        ds_new.clone_variables(self)
+        dts = ds_new['SC_DATETIME'].value.flatten()
+        dt0 = dttool.get_start_of_the_day(dts[0])
+        x_0 = np.array([(dt - dt0).total_seconds() for dt in dts])
+        if dt_fr is None:
+            dt_fr = dts[0] - datetime.timedelta(
+                seconds=np.floor(((dts[0] - ds_new.dt_fr).total_seconds() / time_res)) * time_res
+            )
+        if dt_to is None:
+            dt_to = dts[-1] + datetime.timedelta(
+                seconds=np.floor(((ds_new.dt_to - dts[-1]).total_seconds() / time_res)) * time_res
+            )
+        sec_fr = (dt_fr - dt0).total_seconds()
+        sec_to = (dt_to - dt0).total_seconds()
+        x_1 = np.arange(sec_fr, sec_to + time_res / 2, time_res)
+
+        f = interp1d(x_0, x_0, kind='nearest', bounds_error=False, fill_value=(x_0[0], x_0[-1]))
+        pseudo_x = f(x_1)
+        mask = np.abs(pseudo_x-x_1) > time_res_o/1.5
+
+        dts_new = np.array([dt0 + datetime.timedelta(seconds=sec) for sec in x_1])
+        ds_new['SC_DATETIME'].value = dts_new.reshape((dts_new.size, 1))
+
+        period_var_dict = {'SC_GEO_LON': 360.,
+                           'SC_AACGM_LON': 360.,
+                           'SC_APEX_LON': 360.,
+                           'SC_GEO_LST': 24.,
+                           'SC_AACGM_MLT': 24.,
+                           'SC_APEX_MLT': 24}
+
+        for var_name in ds_new.keys():
+            if var_name in ['SC_DATETIME']:
+                continue
+            if var_name in period_var_dict.keys():
+                var = ds_new[var_name].value.flatten()
+                var_new = nm.interp_period_data(x_0, var, x_1, period=period_var_dict[var_name], method='linear', bounds_error=False)
+                var_new[mask] = np.nan
+                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
+            else:
+                method = 'linear' if 'FLAG' not in var_name else 'nearest'
+                var = ds_new[var_name].value.flatten()
+                f = interp1d(x_0, var, kind=method, bounds_error=False)
+                var_new = f(x_1)
+                var_new[mask] = np.nan
+                ds_new[var_name].value = var_new.reshape((dts_new.size, 1))
+        return ds_new
+
     @property
     def database(self):
         return self._database
 
     @database.setter
     def database(self, value):
         if isinstance(value, str):
```

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/tud/swarm/dns_pod/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/ae/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/ae/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/asysym/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/asysym/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/__init__.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/downloader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/downloader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/loader.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/loader.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/datahub/sources/wdc/dst/variable_config.py` & `geospacelab-0.8.9/geospacelab/datahub/sources/wdc/dst/variable_config.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/express/dmsp_dashboard.py` & `geospacelab-0.8.9/geospacelab/express/dmsp_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/express/eiscat_dashboard.py` & `geospacelab-0.8.9/geospacelab/express/eiscat_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/express/millstonehill_dashboard.py` & `geospacelab-0.8.9/geospacelab/express/millstonehill_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/express/omni_dashboard.py` & `geospacelab-0.8.9/geospacelab/express/omni_dashboard.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py` & `geospacelab-0.8.9/geospacelab/future/empiricalmodels/ovationprime2010/ovationprime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/future/satllites/orbit_analyzer.py` & `geospacelab-0.8.9/geospacelab/future/satllites/orbit_analyzer.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/future/test_sscws.py` & `geospacelab-0.8.9/geospacelab/future/test_sscws.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/observatory/earth/_func.py` & `geospacelab-0.8.9/geospacelab/observatory/earth/_func.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/observatory/earth/geodesy.py` & `geospacelab-0.8.9/geospacelab/observatory/earth/geodesy.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/observatory/earth/sun_position.py` & `geospacelab-0.8.9/geospacelab/observatory/earth/sun_position.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/observatory/orbit/sc_orbit.py` & `geospacelab-0.8.9/geospacelab/observatory/orbit/sc_orbit.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/observatory/orbit/utilities.py` & `geospacelab-0.8.9/geospacelab/observatory/orbit/utilities.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/io/dialog.py` & `geospacelab-0.8.9/geospacelab/toolbox/io/dialog.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/numpyarray.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/numpyarray.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/numpymath.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/numpymath.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/pybasic.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/pybasic.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/pyclass.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/pyclass.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/pydatetime.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/pydatetime.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/pylogging.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/pylogging.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/toolbox/utilities/pyos.py` & `geospacelab-0.8.9/geospacelab/toolbox/utilities/pyos.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/__init__.py` & `geospacelab-0.8.9/geospacelab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/__base__.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/__base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/__init__.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/__init__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/_helpers.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/_helpers.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/axis_ticks.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/colormaps.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/colormaps.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/dashboards.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/dashboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
             if 'major' not in self.extra_axes.keys():
                 ax = self.add_major_axes()
             else:
                 ax = self.extra_axes['major']
         else:
             ax = self.panels[panel_index].axes['major']
 
-        xlim = self.panels[1].axes['major'].get_xlim()
+        xlim = self.panels[0].axes['major'].get_xlim()
         ylim = ax.get_ylim()
         diff_xlim = xlim[1] - xlim[0]
         diff_ylim = ylim[1] - ylim[0]
         x0 = mdates.date2num(dt_fr)
         x0 = (x0 - xlim[0]) / diff_xlim
         x1 = mdates.date2num(dt_to)
         x1 = (x1 - xlim[0]) / diff_xlim
```

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/figure.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/figure.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/__base__.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/__base__.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/geodashboards.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/geodashboards.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/geomap/geopanels.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/geomap/geopanels.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,29 +537,29 @@
         ipm = self().pcolormesh(lon_in, lat_in, data_in, transform=transform, **kwargs)
 
         return ipm
 
     def overlay_contour(
             self,
             data, coords=None, cs=None,
-            regridding=True, grid_res=0.1, interp_method='linear', sparsely=False,
+            regridding=True, grid_res=0.1, interp_method='linear', sparsely=False, data_res=0.5,
             **kwargs,
     ):
         levels = kwargs.pop('levels', 10)
         if cs is None:
             cs = self.cs
 
         cs_new = self.cs_transform(cs_fr=cs, coords=coords)
         lat_in = cs_new['lat']
         lon_in = cs_new['lon']
         data_in = data
         if regridding:
             lon_in, lat_in, data_in = self.grid_data(
                 lon_in, lat_in, data_in, sparsely=sparsely,
-                grid_res=grid_res, interp_method=interp_method)
+                grid_res=grid_res, data_res=data_res, interp_method=interp_method)
             transform = None
         else:
             transform = ccrs.PlateCarree()
 
         ict = self.major_ax.contour(lon_in, lat_in, data_in, levels, transform=transform, **kwargs)
         return ict
```

### Comparing `geospacelab-0.8.8/geospacelab/visualization/mpl/panels.py` & `geospacelab-0.8.9/geospacelab/visualization/mpl/panels.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,18 @@
         label = var.get_visual_axis_attr(axis=2, attr_name='label')
         plot_config = basic.dict_set_default(plot_config, label=label)
         if errorbar == 'off':
             il = ax.plot(x, y, **plot_config)
         elif errorbar == 'on':
             errorbar_config = dict(plot_config)
             errorbar_config.update(var.visual.plot_config.errorbar)
+            y_err = y_err.flatten()
+            if any(y_err < 0):
+                mylog.StreamLogger.warning("Negative values of error detected in {}".format(var))
+                y_err[y_err < 0] = np.nan
             il = ax.errorbar(x.flatten(), y.flatten(), yerr=y_err.flatten(), **errorbar_config)
         if type(il) is not list:
             il = [il]
         self.axes_overview[ax]['lines'].extend(il)
         if self.axes_overview[ax]['legend'] is None:
             self.axes_overview[ax]['legend'] = 'on'
         # elif self.axes_overview[ax]['legend'] == 'off':
@@ -629,15 +633,18 @@
                     except:
                         mylog.StreamLogger.warning("Cannot find the datetime array!")
                         x_data = None
 
         if x_data is None:
             x_data = np.array([self.dt_fr, self.dt_to])
             var.visual.axis[0].mask_gap = False
-
+        x_shift = var.get_visual_axis_attr(axis=0, attr_name='shift')
+        if x_shift is not None:
+            data = x_data.flatten() - datetime.timedelta(seconds=x_shift)
+            x_data = np.reshape(data, x_data.shape)
         y_data = var.get_visual_axis_attr(axis=1, attr_name='data')
         if y_data is None:
             y_data = var.value
             if y_data is None:
                 y_data = np.empty_like(x_data, dtype=np.float32)
                 y_data[::] = np.nan
 
@@ -682,15 +689,18 @@
             try:
                 x_data = depend_0['UT']  # numpy array, type=datetime
             except:
                 x_data = None
             if x_data is None:
                 x_data = np.array([self._xlim[0], self._xlim[1]]).reshape(2, 1)
                 var.visual.axis[0].mask_gap = False
-
+        x_shift = var.get_visual_axis_attr(axis=0, attr_name='shift')
+        if x_shift is not None:
+            data = x_data.flatten() - datetime.timedelta(seconds=x_shift)
+            x_data = np.reshape(data, x_data.shape)
         y_data = var.get_visual_axis_attr(axis=1, attr_name='data')
         if type(y_data) == list:
             y_data = y_data[0]
         if y_data is None:
             y_data = var.get_depend(axis=1, retrieve_data=True)
             y_data_keys = list(y_data.keys())
             y_data = y_data[y_data_keys[0]]
```

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/LICENSE` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/LICENSE`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/README.md` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/README.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/geopack.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/geopack.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/igrf13coeffs.txt`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t01.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t01.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t04.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t04.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t89.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t89.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/t96.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/t96.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/test_geopack1.md` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/test_geopack1.md`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab/wrapper/geopack/geopack/test_geopack1.py` & `geospacelab-0.8.9/geospacelab/wrapper/geopack/geopack/test_geopack1.py`

 * *Files identical despite different names*

### Comparing `geospacelab-0.8.8/geospacelab.egg-info/PKG-INFO` & `geospacelab-0.8.9/geospacelab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospacelab
-Version: 0.8.8
+Version: 0.8.9
 Summary: Collect, manage, and visualize geospace data.
 Home-page: https://github.com/JouleCai/geospacelab
 Author: Lei Cai
 Author-email: lei.cai@oulu.fi
 License: BSD 3-Clause License
 Keywords: Geospace,EISCAT,DMSP,Space weather,Ionosphere,Space,Magnetosphere
 Classifier: Development Status :: 4 - Beta
```

### Comparing `geospacelab-0.8.8/geospacelab.egg-info/SOURCES.txt` & `geospacelab-0.8.9/geospacelab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -168,19 +168,23 @@
 geospacelab/datahub/sources/superdarn/__init__.py
 geospacelab/datahub/sources/superdarn/potmap/__init__.py
 geospacelab/datahub/sources/superdarn/potmap/downloader.py
 geospacelab/datahub/sources/superdarn/potmap/loader.py
 geospacelab/datahub/sources/superdarn/potmap/variable_config.py
 geospacelab/datahub/sources/supermag/__init__.py
 geospacelab/datahub/sources/supermag/supermag_api.py
+geospacelab/datahub/sources/supermag/utilities.py
 geospacelab/datahub/sources/supermag/indices/__init__.py
 geospacelab/datahub/sources/supermag/indices/downloader.py
 geospacelab/datahub/sources/supermag/indices/loader.py
 geospacelab/datahub/sources/supermag/indices/variable_config.py
 geospacelab/datahub/sources/supermag/magnetometer/__init__.py
+geospacelab/datahub/sources/supermag/magnetometer/downloader.py
+geospacelab/datahub/sources/supermag/magnetometer/loader.py
+geospacelab/datahub/sources/supermag/magnetometer/variable_config.py
 geospacelab/datahub/sources/tud/__init__.py
 geospacelab/datahub/sources/tud/downloader.py
 geospacelab/datahub/sources/tud/champ/__init__.py
 geospacelab/datahub/sources/tud/champ/dns_acc/__init__.py
 geospacelab/datahub/sources/tud/champ/dns_acc/downloader.py
 geospacelab/datahub/sources/tud/champ/dns_acc/loader.py
 geospacelab/datahub/sources/tud/champ/dns_acc/variable_config.py
```

### Comparing `geospacelab-0.8.8/setup.py` & `geospacelab-0.8.9/setup.py`

 * *Files identical despite different names*

