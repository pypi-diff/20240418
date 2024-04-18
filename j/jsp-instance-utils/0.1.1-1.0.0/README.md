# Comparing `tmp/jsp_instance_utils-0.1.1.tar.gz` & `tmp/jsp_instance_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsp_instance_utils-0.1.1.tar", last modified: Thu Apr 18 11:10:10 2024, max compression
+gzip compressed data, was "jsp_instance_utils-1.0.0.tar", last modified: Thu Apr 18 15:04:46 2024, max compression
```

## Comparing `jsp_instance_utils-0.1.1.tar` & `jsp_instance_utils-1.0.0.tar`

### file list

```diff
@@ -1,509 +1,515 @@
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.249930 jsp_instance_utils-0.1.1/
--rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_instance_utils-0.1.1/LICENSE
--rw-r--r--   0 qwerty     (501) staff       (20)       58 2024-04-18 09:33:03.000000 jsp_instance_utils-0.1.1/MANIFEST.in
--rw-r--r--   0 qwerty     (501) staff       (20)     6443 2024-04-18 11:10:10.249828 jsp_instance_utils-0.1.1/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)     4318 2024-04-18 08:50:15.000000 jsp_instance_utils-0.1.1/README.md
--rw-r--r--   0 qwerty     (501) staff       (20)      904 2024-04-18 11:08:08.000000 jsp_instance_utils-0.1.1/pyproject.toml
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.185861 jsp_instance_utils-0.1.1/resources/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.185978 jsp_instance_utils-0.1.1/resources/jsp_instances/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.217850 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/
--rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:28:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz5.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:28:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz6.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz7.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz8.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz9.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1731 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1743 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1748 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1745 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1746 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2409 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2373 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2397 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2390 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2381 2024-04-18 09:29:15.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2623 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2625 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2623 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2597 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2599 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3586 2024-04-18 09:29:16.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3600 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3595 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3582 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3574 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3491 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3498 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3501 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3490 2024-04-18 09:29:17.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3437 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4775 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4803 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4753 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4765 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4785 2024-04-18 09:29:18.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4387 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4319 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4362 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4350 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4375 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5964 2024-04-18 09:29:19.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5973 2024-04-18 09:29:20.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5970 2024-04-18 09:29:20.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5975 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5952 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1732 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu41.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1746 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu42.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1743 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu43.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1750 2024-04-18 09:29:23.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu44.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1747 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu45.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2410 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu46.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2392 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu47.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2389 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu48.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2380 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu49.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2378 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu50.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2615 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu51.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2614 2024-04-18 09:29:24.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu52.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2617 2024-04-18 09:29:25.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu53.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2622 2024-04-18 09:29:25.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu54.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2606 2024-04-18 09:29:25.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu55.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3602 2024-04-18 09:29:25.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu56.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3588 2024-04-18 09:29:25.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu57.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3588 2024-04-18 09:29:26.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu58.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3546 2024-04-18 09:29:26.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu59.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3556 2024-04-18 09:29:26.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu60.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3481 2024-04-18 09:29:26.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu61.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3472 2024-04-18 09:29:26.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu62.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3492 2024-04-18 09:29:27.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu63.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3479 2024-04-18 09:29:27.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu64.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3461 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu65.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4761 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu66.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4788 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu67.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4770 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu68.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4763 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu69.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4800 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu70.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4369 2024-04-18 09:29:28.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu71.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4370 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu72.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4344 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu73.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4348 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu74.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4363 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu75.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5957 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu76.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5960 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu77.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5955 2024-04-18 09:29:29.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu78.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5992 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu79.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5930 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu80.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      153 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ft06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      501 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ft10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      500 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ft20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      256 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      256 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      252 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      249 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      253 2024-04-18 09:28:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      378 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      380 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      372 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      379 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      375 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      497 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:46.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      500 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      753 2024-04-18 09:28:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      744 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1002 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1000 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      992 2024-04-18 09:28:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      993 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1493 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1488 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1485 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1489 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1488 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1202 2024-04-18 09:28:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1197 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1187 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1195 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1195 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      505 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      496 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/orb10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      986 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      992 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      993 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      984 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1581 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1582 2024-04-18 09:28:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1580 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1587 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1590 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2473 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2466 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2460 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2466 2024-04-18 09:28:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2483 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2468 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2462 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2469 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2482 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2463 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1185 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1191 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1185 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1188 2024-04-18 09:28:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1184 2024-04-18 09:28:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1191 2024-04-18 09:28:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1176 2024-04-18 09:28:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1189 2024-04-18 09:28:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1184 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1586 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1584 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1575 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1589 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1577 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1583 2024-04-18 09:28:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1579 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1578 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1585 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1584 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2164 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2171 2024-04-18 09:28:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2173 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2170 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2163 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2179 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2175 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2165 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2175 2024-04-18 09:28:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2167 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2361 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2370 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2375 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2365 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2362 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2369 2024-04-18 09:29:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2372 2024-04-18 09:29:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2364 2024-04-18 09:29:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2367 2024-04-18 09:29:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2364 2024-04-18 09:29:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta41.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3259 2024-04-18 09:29:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta42.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3245 2024-04-18 09:29:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta43.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3259 2024-04-18 09:29:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta44.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3256 2024-04-18 09:29:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta45.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta46.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3265 2024-04-18 09:29:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta47.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3248 2024-04-18 09:29:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta48.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta49.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3263 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta50.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3942 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta51.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3929 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta52.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3932 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta53.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3941 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta54.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3942 2024-04-18 09:29:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta55.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3935 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta56.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3936 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta57.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3954 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta58.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3931 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta59.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3938 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta60.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5417 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta61.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5425 2024-04-18 09:29:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta62.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5403 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta63.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5406 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta64.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta65.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta66.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta67.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5421 2024-04-18 09:29:11.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta68.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5427 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta69.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5415 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta70.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10828 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta71.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10824 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta72.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10819 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta73.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10846 2024-04-18 09:29:12.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta74.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10833 2024-04-18 09:29:13.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta75.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10816 2024-04-18 09:29:13.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta76.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10823 2024-04-18 09:29:13.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta77.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10811 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta78.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10827 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta79.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10816 2024-04-18 09:29:14.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta80.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn04.txt
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.247854 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/
--rw-r--r--   0 qwerty     (501) staff       (20)      516 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz5.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      516 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz6.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz7.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:30.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz8.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz9.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1750 2024-04-18 09:29:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1762 2024-04-18 09:29:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1767 2024-04-18 09:29:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1764 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1765 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2428 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2392 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2416 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2409 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2400 2024-04-18 09:29:59.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2652 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2654 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2652 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2626 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2628 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3615 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3629 2024-04-18 09:30:00.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3624 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3611 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3603 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3530 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3537 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3540 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3529 2024-04-18 09:30:01.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3476 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4814 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4842 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4792 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4804 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4824 2024-04-18 09:30:02.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4436 2024-04-18 09:30:03.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4368 2024-04-18 09:30:03.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4411 2024-04-18 09:30:03.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4399 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4424 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6013 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6022 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6019 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6024 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6001 2024-04-18 09:30:04.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1751 2024-04-18 09:30:05.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu41.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1765 2024-04-18 09:30:05.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu42.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1762 2024-04-18 09:30:05.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu43.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1769 2024-04-18 09:30:05.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu44.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1766 2024-04-18 09:30:05.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu45.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2429 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu46.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2411 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu47.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2408 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu48.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2399 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu49.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2397 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu50.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2644 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu51.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2643 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu52.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2646 2024-04-18 09:30:06.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu53.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2651 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu54.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2635 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu55.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3631 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu56.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3617 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu57.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3617 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu58.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3575 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu59.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3585 2024-04-18 09:30:07.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu60.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3520 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu61.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3511 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu62.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3531 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu63.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3518 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu64.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3500 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu65.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4800 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu66.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4827 2024-04-18 09:30:08.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu67.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4809 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu68.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4802 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu69.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4839 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu70.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4418 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu71.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4419 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu72.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4393 2024-04-18 09:30:09.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu73.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4397 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu74.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4412 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu75.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6006 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu76.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6009 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu77.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6004 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu78.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     6041 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu79.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5979 2024-04-18 09:30:10.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu80.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      152 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ft06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      510 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ft10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ft20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      255 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      255 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      251 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      248 2024-04-18 09:29:31.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      252 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      377 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      379 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      371 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      378 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      374 2024-04-18 09:29:32.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      501 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      496 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      497 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      512 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:29:33.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      509 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      767 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      758 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:34.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1021 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1019 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1011 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1012 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1013 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1522 2024-04-18 09:29:35.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1517 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1514 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1518 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1517 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1216 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1211 2024-04-18 09:29:36.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1201 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1209 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1209 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      514 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      512 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:37.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      505 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1005 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1013 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1011 2024-04-18 09:29:38.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1012 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1003 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1600 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1601 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1599 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1606 2024-04-18 09:29:39.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1609 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2522 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2515 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2509 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2515 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2532 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2517 2024-04-18 09:29:40.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2511 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2518 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2531 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2512 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1199 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1204 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1205 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1199 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1202 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta05.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1198 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta06.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1205 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta07.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta08.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1203 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta09.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1198 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta10.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1605 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta11.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1603 2024-04-18 09:29:43.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta12.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1594 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta13.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1608 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta14.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1596 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta15.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1602 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta16.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1598 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta17.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1597 2024-04-18 09:29:44.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta18.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1604 2024-04-18 09:29:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta19.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     1603 2024-04-18 09:29:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta20.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2183 2024-04-18 09:29:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta21.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2190 2024-04-18 09:29:45.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta22.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2192 2024-04-18 09:29:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta23.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2189 2024-04-18 09:29:47.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta24.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2182 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta25.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2198 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta26.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2194 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta27.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2184 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta28.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2194 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta29.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2186 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta30.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2390 2024-04-18 09:29:48.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta31.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2399 2024-04-18 09:29:49.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta32.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2404 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta33.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2394 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta34.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2391 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta35.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2398 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta36.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2401 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta37.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2393 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta38.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2396 2024-04-18 09:29:50.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta39.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2393 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta40.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta41.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3288 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta42.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3274 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta43.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3288 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta44.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3285 2024-04-18 09:29:51.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta45.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta46.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3294 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta47.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3277 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta48.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta49.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3292 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta50.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3991 2024-04-18 09:29:52.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta51.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3978 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta52.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3981 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta53.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3990 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta54.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3991 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta55.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3984 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta56.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3985 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta57.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     4003 2024-04-18 09:29:53.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta58.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3980 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta59.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     3987 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta60.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5466 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta61.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5474 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta62.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5452 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta63.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5455 2024-04-18 09:29:54.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta64.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta65.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta66.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta67.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5470 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta68.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5476 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta69.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     5464 2024-04-18 09:29:55.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta70.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10927 2024-04-18 09:29:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta71.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10923 2024-04-18 09:29:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta72.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10918 2024-04-18 09:29:56.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta73.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10945 2024-04-18 09:29:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta74.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10932 2024-04-18 09:29:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta75.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10915 2024-04-18 09:29:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta76.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10922 2024-04-18 09:29:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta77.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10910 2024-04-18 09:29:57.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta78.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10926 2024-04-18 09:29:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta79.txt
--rw-r--r--   0 qwerty     (501) staff       (20)    10915 2024-04-18 09:29:58.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta80.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn01.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn02.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn03.txt
--rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:42.000000 jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn04.txt
--rw-r--r--   0 qwerty     (501) staff       (20)      458 2024-04-18 11:10:10.250234 jsp_instance_utils-0.1.1/setup.cfg
--rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_instance_utils-0.1.1/setup.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.186144 jsp_instance_utils-0.1.1/src/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.248287 jsp_instance_utils-0.1.1/src/jsp_instance_utils/
--rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-18 09:10:46.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils/__init__.py
--rw-r--r--   0 qwerty     (501) staff       (20)      474 2024-04-18 11:02:25.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils/benchmark_instances.py
--rw-r--r--   0 qwerty     (501) staff       (20)     6292 2024-04-18 09:35:05.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils/jsp_instance_parser.py
--rw-r--r--   0 qwerty     (501) staff       (20)     4897 2024-04-18 09:46:29.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils/jsp_or_tools_solver.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 11:10:10.249201 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/
--rw-r--r--   0 qwerty     (501) staff       (20)     6443 2024-04-18 11:10:10.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)    21058 2024-04-18 11:10:10.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/SOURCES.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 11:10:10.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/dependency_links.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 09:24:26.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/not-zip-safe
--rw-r--r--   0 qwerty     (501) staff       (20)       91 2024-04-18 11:10:10.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/requires.txt
--rw-r--r--   0 qwerty     (501) staff       (20)       19 2024-04-18 11:10:10.000000 jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.612800 jsp_instance_utils-1.0.0/
+-rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_instance_utils-1.0.0/LICENSE
+-rw-r--r--   0 qwerty     (501) staff       (20)       58 2024-04-18 09:33:03.000000 jsp_instance_utils-1.0.0/MANIFEST.in
+-rw-r--r--   0 qwerty     (501) staff       (20)     5056 2024-04-18 15:04:46.612730 jsp_instance_utils-1.0.0/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)     2834 2024-04-18 15:02:33.000000 jsp_instance_utils-1.0.0/README.md
+-rw-r--r--   0 qwerty     (501) staff       (20)     1001 2024-04-18 15:02:33.000000 jsp_instance_utils-1.0.0/pyproject.toml
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.548727 jsp_instance_utils-1.0.0/resources/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.548839 jsp_instance_utils-1.0.0/resources/jsp_instances/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.580696 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/
+-rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:28:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz5.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:28:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz6.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz7.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz8.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1607 2024-04-18 09:28:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz9.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1731 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1743 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1748 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1745 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1746 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2409 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2373 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2397 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2390 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2381 2024-04-18 09:29:15.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2623 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2625 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2623 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2597 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2599 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3586 2024-04-18 09:29:16.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3600 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3595 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3582 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3574 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3491 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3498 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3501 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3490 2024-04-18 09:29:17.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3437 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4775 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4803 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4753 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4765 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4785 2024-04-18 09:29:18.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4387 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4319 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4362 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4350 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4375 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5964 2024-04-18 09:29:19.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5973 2024-04-18 09:29:20.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5970 2024-04-18 09:29:20.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5975 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5952 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1732 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu41.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1746 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu42.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1743 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu43.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1750 2024-04-18 09:29:23.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu44.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1747 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu45.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2410 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu46.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2392 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu47.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2389 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu48.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2380 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu49.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2378 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu50.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2615 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu51.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2614 2024-04-18 09:29:24.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu52.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2617 2024-04-18 09:29:25.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu53.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2622 2024-04-18 09:29:25.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu54.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2606 2024-04-18 09:29:25.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu55.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3602 2024-04-18 09:29:25.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu56.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3588 2024-04-18 09:29:25.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu57.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3588 2024-04-18 09:29:26.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu58.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3546 2024-04-18 09:29:26.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu59.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3556 2024-04-18 09:29:26.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu60.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3481 2024-04-18 09:29:26.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu61.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3472 2024-04-18 09:29:26.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu62.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3492 2024-04-18 09:29:27.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu63.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3479 2024-04-18 09:29:27.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu64.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3461 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu65.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4761 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu66.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4788 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu67.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4770 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu68.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4763 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu69.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4800 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu70.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4369 2024-04-18 09:29:28.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu71.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4370 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu72.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4344 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu73.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4348 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu74.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4363 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu75.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5957 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu76.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5960 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu77.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5955 2024-04-18 09:29:29.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu78.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5992 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu79.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5930 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu80.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      153 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ft06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      501 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ft10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      500 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ft20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      256 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      256 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      252 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      249 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      253 2024-04-18 09:28:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      378 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      380 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      372 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      379 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      375 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      497 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:46.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      500 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      753 2024-04-18 09:28:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      744 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      746 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1002 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1000 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      992 2024-04-18 09:28:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      993 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1493 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1488 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1485 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1489 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1488 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1202 2024-04-18 09:28:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1197 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1187 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1195 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1195 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      505 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      503 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      504 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      496 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:28:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/orb10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      986 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      992 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      993 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      984 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1581 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1582 2024-04-18 09:28:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1580 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1587 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1590 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2473 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2466 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2460 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2466 2024-04-18 09:28:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2483 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2468 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2462 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2469 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2482 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2463 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1185 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1191 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1185 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1188 2024-04-18 09:28:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1184 2024-04-18 09:28:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1191 2024-04-18 09:28:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1176 2024-04-18 09:28:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1189 2024-04-18 09:28:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1184 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1586 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1584 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1575 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1589 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1577 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1583 2024-04-18 09:28:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1579 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1578 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1585 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1584 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2164 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2171 2024-04-18 09:28:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2173 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2170 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2163 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2179 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2175 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2165 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2175 2024-04-18 09:28:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2167 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2361 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2370 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2375 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2365 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2362 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2369 2024-04-18 09:29:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2372 2024-04-18 09:29:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2364 2024-04-18 09:29:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2367 2024-04-18 09:29:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2364 2024-04-18 09:29:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta41.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3259 2024-04-18 09:29:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta42.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3245 2024-04-18 09:29:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta43.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3259 2024-04-18 09:29:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta44.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3256 2024-04-18 09:29:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta45.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta46.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3265 2024-04-18 09:29:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta47.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3248 2024-04-18 09:29:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta48.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3257 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta49.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3263 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta50.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3942 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta51.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3929 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta52.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3932 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta53.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3941 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta54.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3942 2024-04-18 09:29:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta55.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3935 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta56.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3936 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta57.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3954 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta58.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3931 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta59.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3938 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta60.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5417 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta61.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5425 2024-04-18 09:29:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta62.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5403 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta63.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5406 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta64.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta65.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta66.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5423 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta67.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5421 2024-04-18 09:29:11.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta68.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5427 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta69.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5415 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta70.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10828 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta71.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10824 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta72.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10819 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta73.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10846 2024-04-18 09:29:12.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta74.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10833 2024-04-18 09:29:13.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta75.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10816 2024-04-18 09:29:13.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta76.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10823 2024-04-18 09:29:13.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta77.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10811 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta78.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10827 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta79.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10816 2024-04-18 09:29:14.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta80.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2207 2024-04-18 09:28:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn04.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.609344 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/
+-rw-r--r--   0 qwerty     (501) staff       (20)      516 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz5.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      516 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz6.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz7.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:30.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz8.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1626 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz9.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1750 2024-04-18 09:29:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1762 2024-04-18 09:29:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1767 2024-04-18 09:29:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1764 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1765 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2428 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2392 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2416 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2409 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2400 2024-04-18 09:29:59.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2652 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2654 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2652 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2626 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2628 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3615 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3629 2024-04-18 09:30:00.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3624 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3611 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3603 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3530 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3537 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3540 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3529 2024-04-18 09:30:01.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3476 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4814 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4842 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4792 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4804 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4824 2024-04-18 09:30:02.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4436 2024-04-18 09:30:03.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4368 2024-04-18 09:30:03.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4411 2024-04-18 09:30:03.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4399 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4424 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6013 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6022 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6019 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6024 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6001 2024-04-18 09:30:04.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1751 2024-04-18 09:30:05.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu41.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1765 2024-04-18 09:30:05.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu42.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1762 2024-04-18 09:30:05.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu43.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1769 2024-04-18 09:30:05.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu44.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1766 2024-04-18 09:30:05.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu45.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2429 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu46.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2411 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu47.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2408 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu48.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2399 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu49.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2397 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu50.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2644 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu51.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2643 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu52.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2646 2024-04-18 09:30:06.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu53.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2651 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu54.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2635 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu55.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3631 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu56.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3617 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu57.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3617 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu58.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3575 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu59.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3585 2024-04-18 09:30:07.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu60.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3520 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu61.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3511 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu62.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3531 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu63.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3518 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu64.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3500 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu65.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4800 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu66.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4827 2024-04-18 09:30:08.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu67.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4809 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu68.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4802 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu69.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4839 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu70.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4418 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu71.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4419 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu72.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4393 2024-04-18 09:30:09.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu73.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4397 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu74.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4412 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu75.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6006 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu76.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6009 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu77.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6004 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu78.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     6041 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu79.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5979 2024-04-18 09:30:10.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu80.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      152 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ft06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      510 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ft10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      499 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ft20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      255 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      255 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      251 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      248 2024-04-18 09:29:31.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      252 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      377 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      379 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      371 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      378 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      374 2024-04-18 09:29:32.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      501 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      496 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      502 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      497 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      498 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      512 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      507 2024-04-18 09:29:33.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      509 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      767 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      758 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:34.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      760 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1021 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1019 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1011 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1012 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1013 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1522 2024-04-18 09:29:35.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1517 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1514 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1518 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1517 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1216 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1211 2024-04-18 09:29:36.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1201 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1209 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1209 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      514 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      512 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      513 2024-04-18 09:29:37.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      505 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      508 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      511 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1005 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1013 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1011 2024-04-18 09:29:38.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1012 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1003 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1600 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1601 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1599 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1606 2024-04-18 09:29:39.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1609 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2522 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2515 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2509 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2515 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2532 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2517 2024-04-18 09:29:40.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2511 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2518 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2531 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2512 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1199 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1204 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1205 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1199 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1202 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta05.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1198 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta06.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1205 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta07.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta08.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1203 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta09.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1198 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta10.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1605 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta11.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1603 2024-04-18 09:29:43.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta12.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1594 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta13.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1608 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta14.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1596 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta15.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1602 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta16.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1598 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta17.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1597 2024-04-18 09:29:44.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta18.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1604 2024-04-18 09:29:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta19.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     1603 2024-04-18 09:29:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta20.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2183 2024-04-18 09:29:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta21.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2190 2024-04-18 09:29:45.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta22.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2192 2024-04-18 09:29:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta23.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2189 2024-04-18 09:29:47.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta24.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2182 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta25.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2198 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta26.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2194 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta27.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2184 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta28.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2194 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta29.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2186 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta30.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2390 2024-04-18 09:29:48.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta31.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2399 2024-04-18 09:29:49.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta32.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2404 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta33.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2394 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta34.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2391 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta35.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2398 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta36.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2401 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta37.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2393 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta38.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2396 2024-04-18 09:29:50.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta39.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2393 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta40.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta41.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3288 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta42.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3274 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta43.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3288 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta44.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3285 2024-04-18 09:29:51.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta45.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta46.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3294 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta47.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3277 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta48.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3286 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta49.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3292 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta50.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3991 2024-04-18 09:29:52.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta51.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3978 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta52.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3981 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta53.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3990 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta54.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3991 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta55.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3984 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta56.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3985 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta57.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     4003 2024-04-18 09:29:53.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta58.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3980 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta59.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     3987 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta60.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5466 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta61.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5474 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta62.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5452 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta63.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5455 2024-04-18 09:29:54.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta64.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta65.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta66.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5472 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta67.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5470 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta68.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5476 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta69.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     5464 2024-04-18 09:29:55.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta70.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10927 2024-04-18 09:29:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta71.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10923 2024-04-18 09:29:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta72.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10918 2024-04-18 09:29:56.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta73.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10945 2024-04-18 09:29:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta74.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10932 2024-04-18 09:29:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta75.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10915 2024-04-18 09:29:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta76.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10922 2024-04-18 09:29:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta77.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10910 2024-04-18 09:29:57.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta78.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10926 2024-04-18 09:29:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta79.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)    10915 2024-04-18 09:29:58.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta80.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn01.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn02.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:41.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn03.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)     2226 2024-04-18 09:29:42.000000 jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn04.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)      458 2024-04-18 15:04:46.613054 jsp_instance_utils-1.0.0/setup.cfg
+-rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_instance_utils-1.0.0/setup.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.549002 jsp_instance_utils-1.0.0/src/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.610792 jsp_instance_utils-1.0.0/src/jsp_instance_utils/
+-rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-18 09:10:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils/__init__.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     6292 2024-04-18 09:35:05.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils/instance_parser.py
+-rw-r--r--   0 qwerty     (501) staff       (20)  1452613 2024-04-18 11:44:41.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils/instances.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1593 2024-04-18 11:52:48.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils/jsp_instance_generator.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     4897 2024-04-18 09:46:29.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils/jsp_or_tools_solver.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.612200 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/
+-rw-r--r--   0 qwerty     (501) staff       (20)     5056 2024-04-18 15:04:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)    21210 2024-04-18 15:04:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 15:04:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 09:24:26.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/not-zip-safe
+-rw-r--r--   0 qwerty     (501) staff       (20)       91 2024-04-18 15:04:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/requires.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)       19 2024-04-18 15:04:46.000000 jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:04:46.612014 jsp_instance_utils-1.0.0/tests/
+-rw-r--r--   0 qwerty     (501) staff       (20)      547 2024-04-18 12:45:33.000000 jsp_instance_utils-1.0.0/tests/test_instance_generator.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     3812 2024-04-18 14:26:16.000000 jsp_instance_utils-1.0.0/tests/test_instance_parser.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      675 2024-04-18 12:42:21.000000 jsp_instance_utils-1.0.0/tests/test_instances.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      257 2024-04-18 11:56:15.000000 jsp_instance_utils-1.0.0/tests/test_or_tools_solver.py
```

### Comparing `jsp_instance_utils-0.1.1/LICENSE` & `jsp_instance_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/pyproject.toml` & `jsp_instance_utils-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsp-instance-utils"
-version = "0.1.1"
-description = "todo"
+version = "1.0.0"
+description = "A package containg benchmark instances for the Job Shop Scheduling Problem (JSP) scraped from "
 readme = "README.md"
 authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@ima.rwth-aachen.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,14 +30,14 @@
     "pytest",
     "pytest-cov",
     "tox",
     "twine"
 ]
 
 [project.urls]
-Homepage = "https://github.com/Alexander-Nasuta/pypitemplate"
+Homepage = "https://github.com/Alexander-Nasuta/jsp-instance-utils/"
 
 [tool.pytest.ini_options]
 addopts = "--cov=jsp_instance_utils -p no:warnings"
 testpaths = [
     "tests",
 ]
```

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz7.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz7.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz8.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz8.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/abz9.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/abz9.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu41.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu41.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu42.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu42.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu43.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu43.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu44.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu44.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu45.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu45.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu46.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu46.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu47.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu47.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu48.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu48.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu49.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu49.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu50.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu50.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu51.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu51.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu52.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu52.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu53.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu53.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu54.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu54.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu55.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu55.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu56.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu56.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu57.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu57.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu58.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu58.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu59.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu59.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu60.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu60.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu61.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu61.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu62.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu62.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu63.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu63.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu64.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu64.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu65.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu65.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu66.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu66.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu67.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu67.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu68.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu68.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu69.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu69.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu70.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu70.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu71.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu71.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu72.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu72.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu73.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu73.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu74.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu74.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu75.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu75.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu76.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu76.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu77.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu77.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu78.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu78.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu79.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu79.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/dmu80.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/dmu80.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/la40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/la40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/swv20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/swv20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta41.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta41.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta42.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta42.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta43.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta43.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta44.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta44.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta45.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta45.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta46.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta46.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta47.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta47.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta48.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta48.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta49.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta49.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta50.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta50.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta51.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta51.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta52.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta52.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta53.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta53.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta54.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta54.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta55.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta55.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta56.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta56.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta57.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta57.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta58.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta58.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta59.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta59.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta60.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta60.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta61.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta61.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta62.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta62.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta63.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta63.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta64.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta64.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta65.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta65.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta66.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta66.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta67.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta67.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta68.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta68.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta69.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta69.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta70.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta70.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta71.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta71.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta72.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta72.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta73.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta73.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta74.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta74.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta75.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta75.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta76.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta76.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta77.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta77.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta78.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta78.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta79.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta79.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/ta80.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/ta80.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/standard/yn04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/standard/yn04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz5.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz5.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz6.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz6.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz7.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz7.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz8.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz8.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/abz9.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/abz9.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu41.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu41.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu42.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu42.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu43.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu43.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu44.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu44.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu45.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu45.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu46.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu46.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu47.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu47.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu48.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu48.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu49.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu49.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu50.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu50.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu51.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu51.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu52.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu52.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu53.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu53.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu54.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu54.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu55.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu55.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu56.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu56.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu57.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu57.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu58.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu58.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu59.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu59.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu60.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu60.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu61.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu61.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu62.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu62.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu63.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu63.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu64.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu64.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu65.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu65.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu66.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu66.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu67.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu67.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu68.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu68.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu69.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu69.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu70.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu70.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu71.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu71.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu72.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu72.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu73.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu73.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu74.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu74.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu75.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu75.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu76.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu76.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu77.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu77.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu78.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu78.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu79.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu79.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/dmu80.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/dmu80.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/la40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/la40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/orb05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/orb05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/swv20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/swv20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta05.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta05.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta06.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta06.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta07.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta07.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta08.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta08.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta09.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta09.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta10.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta10.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta11.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta11.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta12.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta12.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta13.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta13.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta14.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta14.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta15.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta15.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta16.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta16.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta17.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta17.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta18.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta18.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta19.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta19.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta20.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta20.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta21.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta21.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta22.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta22.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta23.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta23.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta24.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta24.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta25.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta25.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta26.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta26.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta27.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta27.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta28.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta28.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta29.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta29.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta30.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta30.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta31.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta31.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta32.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta32.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta33.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta33.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta34.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta34.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta35.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta35.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta36.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta36.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta37.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta37.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta38.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta38.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta39.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta39.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta40.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta40.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta41.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta41.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta42.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta42.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta43.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta43.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta44.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta44.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta45.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta45.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta46.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta46.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta47.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta47.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta48.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta48.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta49.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta49.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta50.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta50.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta51.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta51.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta52.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta52.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta53.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta53.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta54.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta54.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta55.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta55.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta56.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta56.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta57.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta57.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta58.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta58.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta59.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta59.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta60.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta60.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta61.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta61.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta62.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta62.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta63.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta63.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta64.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta64.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta65.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta65.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta66.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta66.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta67.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta67.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta68.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta68.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta69.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta69.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta70.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta70.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta71.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta71.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta72.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta72.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta73.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta73.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta74.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta74.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta75.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta75.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta76.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta76.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta77.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta77.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta78.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta78.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta79.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta79.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/ta80.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/ta80.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn01.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn01.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn02.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn02.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn03.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn03.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/resources/jsp_instances/taillard/yn04.txt` & `jsp_instance_utils-1.0.0/resources/jsp_instances/taillard/yn04.txt`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/src/jsp_instance_utils/jsp_instance_parser.py` & `jsp_instance_utils-1.0.0/src/jsp_instance_utils/instance_parser.py`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/src/jsp_instance_utils/jsp_or_tools_solver.py` & `jsp_instance_utils-1.0.0/src/jsp_instance_utils/jsp_or_tools_solver.py`

 * *Files identical despite different names*

### Comparing `jsp_instance_utils-0.1.1/src/jsp_instance_utils.egg-info/SOURCES.txt` & `jsp_instance_utils-1.0.0/src/jsp_instance_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -485,16 +485,21 @@
 resources/jsp_instances/taillard/ta79.txt
 resources/jsp_instances/taillard/ta80.txt
 resources/jsp_instances/taillard/yn01.txt
 resources/jsp_instances/taillard/yn02.txt
 resources/jsp_instances/taillard/yn03.txt
 resources/jsp_instances/taillard/yn04.txt
 src/jsp_instance_utils/__init__.py
-src/jsp_instance_utils/benchmark_instances.py
-src/jsp_instance_utils/jsp_instance_parser.py
+src/jsp_instance_utils/instance_parser.py
+src/jsp_instance_utils/instances.py
+src/jsp_instance_utils/jsp_instance_generator.py
 src/jsp_instance_utils/jsp_or_tools_solver.py
 src/jsp_instance_utils.egg-info/PKG-INFO
 src/jsp_instance_utils.egg-info/SOURCES.txt
 src/jsp_instance_utils.egg-info/dependency_links.txt
 src/jsp_instance_utils.egg-info/not-zip-safe
 src/jsp_instance_utils.egg-info/requires.txt
-src/jsp_instance_utils.egg-info/top_level.txt
+src/jsp_instance_utils.egg-info/top_level.txt
+tests/test_instance_generator.py
+tests/test_instance_parser.py
+tests/test_instances.py
+tests/test_or_tools_solver.py
```

