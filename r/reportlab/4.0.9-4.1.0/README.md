# Comparing `tmp/reportlab-4.0.9.tar.gz` & `tmp/reportlab-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-4.0.9.tar", last modified: Wed Jan 10 10:20:31 2024, max compression
+gzip compressed data, was "reportlab-4.1.0.tar", last modified: Thu Feb  8 12:05:48 2024, max compression
```

## Comparing `reportlab-4.0.9.tar` & `reportlab-4.1.0.tar`

### file list

```diff
@@ -1,762 +1,569 @@
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.748739 reportlab-4.0.9/
--rw-r--r--   0 robin     (1000) robin     (1000)    50739 2024-01-07 11:14:24.000000 reportlab-4.0.9/CHANGES.md
--rw-r--r--   0 robin     (1000) robin     (1000)       53 2019-10-12 07:24:05.000000 reportlab-4.0.9/INSTALL.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2023-06-05 10:15:46.000000 reportlab-4.0.9/LICENSE
--rw-r--r--   0 robin     (1000) robin     (1000)      468 2023-06-05 10:15:46.000000 reportlab-4.0.9/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1354 2024-01-10 10:20:31.745406 reportlab-4.0.9/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)     4994 2023-06-05 10:15:46.000000 reportlab-4.0.9/README.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       72 2019-10-12 07:24:05.000000 reportlab-4.0.9/VERSION.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.572069 reportlab-4.0.9/demos/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.578736 reportlab-4.0.9/demos/colors/
--rw-r--r--   0 robin     (1000) robin     (1000)     2728 2023-06-05 09:49:41.000000 reportlab-4.0.9/demos/colors/colortest.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.578736 reportlab-4.0.9/demos/gadflypaper/
--rw-r--r--   0 robin     (1000) robin     (1000)      105 2019-10-12 07:24:05.000000 reportlab-4.0.9/demos/gadflypaper/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    32486 2023-06-05 09:58:47.000000 reportlab-4.0.9/demos/gadflypaper/gfe.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.582069 reportlab-4.0.9/demos/odyssey/
--rw-r--r--   0 robin     (1000) robin     (1000)     2098 2023-06-05 09:58:47.000000 reportlab-4.0.9/demos/odyssey/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     7649 2023-06-05 09:49:41.000000 reportlab-4.0.9/demos/odyssey/dodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4580 2023-06-05 09:49:41.000000 reportlab-4.0.9/demos/odyssey/fodyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4235 2023-06-05 09:58:47.000000 reportlab-4.0.9/demos/odyssey/odyssey.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10950 2020-10-29 09:10:51.000000 reportlab-4.0.9/demos/odyssey/odyssey.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.582069 reportlab-4.0.9/demos/rlzope/
--rw-r--r--   0 robin     (1000) robin     (1000)     2538 2019-10-12 07:24:05.000000 reportlab-4.0.9/demos/rlzope/readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     6791 2023-06-05 09:58:47.000000 reportlab-4.0.9/demos/rlzope/rlzope.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.582069 reportlab-4.0.9/demos/stdfonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      229 2019-10-12 07:24:05.000000 reportlab-4.0.9/demos/stdfonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     2381 2023-06-05 09:49:41.000000 reportlab-4.0.9/demos/stdfonts/stdfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.582069 reportlab-4.0.9/demos/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      525 2023-06-05 09:49:41.000000 reportlab-4.0.9/demos/tests/testdemos.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.582069 reportlab-4.0.9/docs/
--rw-r--r--   0 robin     (1000) robin     (1000)      313 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     3136 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/Makefile
--rwxr-xr-x   0 robin     (1000) robin     (1000)     1497 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/genAll.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)      143 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/gen_epydoc
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.585402 reportlab-4.0.9/docs/images/
--rw-r--r--   0 robin     (1000) robin     (1000)     9685 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/Edit_Prefs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    28106 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/Python_21.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    29117 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/Python_21_HINT.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    37812 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/fileExchange.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10513 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/jpn.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33898 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/jpnchars.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)      393 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/redsquare.png
--rw-r--r--   0 robin     (1000) robin     (1000)    26548 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/replogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)    16583 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/replogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      924 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/images/testimg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3081 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/make.bat
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.588736 reportlab-4.0.9/docs/reference/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      110 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/reference/build.bat
--rw-r--r--   0 robin     (1000) robin     (1000)     1206 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/reference/genreference.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9927 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/reference/reference.yml
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.588736 reportlab-4.0.9/docs/source/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.588736 reportlab-4.0.9/docs/source/_static/
--rw-r--r--   0 robin     (1000) robin     (1000)      252 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/source/_static/basic.css
--rw-r--r--   0 robin     (1000) robin     (1000)    16419 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/_static/default.css
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.592069 reportlab-4.0.9/docs/source/_templates/
--rw-r--r--   0 robin     (1000) robin     (1000)      167 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/_templates/layout.html
--rw-r--r--   0 robin     (1000) robin     (1000)     1431 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/_templates/page.html
--rw-r--r--   0 robin     (1000) robin     (1000)     6427 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/conf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1345 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/graphics.rst
--rw-r--r--   0 robin     (1000) robin     (1000)     1049 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/index.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      885 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/lib.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      238 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/pdfgen.rst
--rw-r--r--   0 robin     (1000) robin     (1000)      984 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/source/platypus.rst
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.595403 reportlab-4.0.9/docs/userguide/
--rw-r--r--   0 robin     (1000) robin     (1000)     4494 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/app_demos.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17692 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch1_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45531 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch2_graphics.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19934 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch2a_fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30547 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch3_pdffeatures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19314 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch4_platypus_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    23044 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch5_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34555 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch6_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2643 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/ch7_custom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3575 2023-06-05 09:58:47.000000 reportlab-4.0.9/docs/userguide/genuserguide.py
--rw-r--r--   0 robin     (1000) robin     (1000)    52769 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/userguide/graph_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11788 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/userguide/graph_concepts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      490 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/userguide/graph_intro.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12403 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/userguide/graph_shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13522 2023-06-05 09:49:41.000000 reportlab-4.0.9/docs/userguide/graph_widgets.py
--rw-r--r--   0 robin     (1000) robin     (1000)      112 2019-10-12 07:24:05.000000 reportlab-4.0.9/docs/userguide/testfile.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       89 2023-06-05 10:15:46.000000 reportlab-4.0.9/pyproject.toml
--rw-r--r--   0 robin     (1000) robin     (1000)       38 2024-01-10 10:20:31.748739 reportlab-4.0.9/setup.cfg
--rw-r--r--   0 robin     (1000) robin     (1000)    12004 2023-11-13 13:13:43.000000 reportlab-4.0.9/setup.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.575402 reportlab-4.0.9/src/
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.595403 reportlab-4.0.9/src/reportlab/
--rw-r--r--   0 robin     (1000) robin     (1000)      185 2019-10-12 07:24:05.000000 reportlab-4.0.9/src/reportlab/MANIFEST.in
--rw-r--r--   0 robin     (1000) robin     (1000)     1481 2024-01-07 11:10:57.000000 reportlab-4.0.9/src/reportlab/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.605403 reportlab-4.0.9/src/reportlab/fonts/
--rw-r--r--   0 robin     (1000) robin     (1000)      318 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      504 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGarden-changelog.txt
--rw-r--r--   0 robin     (1000) robin     (1000)    17976 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     1318 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGarden-copying.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     4122 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGarden-readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)   519634 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGarden.sfd
--rw-r--r--   0 robin     (1000) robin     (1000)    10351 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGardenMK.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    79824 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/DarkGardenMK.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    65932 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/Vera.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63208 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/VeraBI.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    58716 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/VeraBd.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    63684 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/VeraIt.ttf
--rw-r--r--   0 robin     (1000) robin     (1000)    32084 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_a______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    31966 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_ab_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32019 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_abi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    32115 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_ai_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35377 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_eb_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    38543 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_ebi____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    37518 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_ei_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35380 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/_er_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)     5954 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/fonts/bitstream-vera-license.txt
--rw-r--r--   0 robin     (1000) robin     (1000)     8318 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/callig15.afm
--rw-r--r--   0 robin     (1000) robin     (1000)    59663 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/callig15.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    35500 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/cob_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    50532 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/cobo____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34585 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/com_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    48468 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/coo_____.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    34705 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/sy______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    49593 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/zd______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    75573 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/zx______.pfb
--rw-r--r--   0 robin     (1000) robin     (1000)    96418 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab/fonts/zy______.pfb
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.608736 reportlab-4.0.9/src/reportlab/graphics/
--rw-r--r--   0 robin     (1000) robin     (1000)      274 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.612070 reportlab-4.0.9/src/reportlab/graphics/barcode/
--rw-r--r--   0 robin     (1000) robin     (1000)     1741 2019-10-12 07:24:05.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/README
--rw-r--r--   0 robin     (1000) robin     (1000)      915 2019-10-12 07:24:05.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/TODO
--rw-r--r--   0 robin     (1000) robin     (1000)     5886 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18451 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/code128.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9799 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/code39.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9077 2023-06-05 09:49:41.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/code93.py
--rw-r--r--   0 robin     (1000) robin     (1000)    24345 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/common.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7872 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/dmtx.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18922 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/eanbc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17884 2023-06-05 09:49:41.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/ecc200datamatrix.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3746 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/fourstate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7377 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/lto.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6266 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/qr.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34117 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/qrencoder.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11765 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/test.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8076 2023-06-05 09:49:41.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/usps.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15554 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/usps4s.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17499 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/barcode/widgets.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.615403 reportlab-4.0.9/src/reportlab/graphics/charts/
--rw-r--r--   0 robin     (1000) robin     (1000)      234 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4405 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/areas.py
--rw-r--r--   0 robin     (1000) robin     (1000)    92550 2023-09-29 14:48:35.000000 reportlab-4.0.9/src/reportlab/graphics/charts/axes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    72361 2023-11-06 08:27:35.000000 reportlab-4.0.9/src/reportlab/graphics/charts/barcharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6628 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/dotbox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18934 2023-10-10 09:29:53.000000 reportlab-4.0.9/src/reportlab/graphics/charts/doughnut.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25687 2023-07-12 14:56:14.000000 reportlab-4.0.9/src/reportlab/graphics/charts/legends.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27178 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/linecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    49394 2023-07-14 12:41:28.000000 reportlab-4.0.9/src/reportlab/graphics/charts/lineplots.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1739 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    66794 2023-10-10 10:30:37.000000 reportlab-4.0.9/src/reportlab/graphics/charts/piecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8548 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16132 2023-10-17 09:36:40.000000 reportlab-4.0.9/src/reportlab/graphics/charts/spider.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22945 2023-11-30 12:38:05.000000 reportlab-4.0.9/src/reportlab/graphics/charts/textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11556 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7194 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/charts/utils3d.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15156 2023-07-12 14:25:07.000000 reportlab-4.0.9/src/reportlab/graphics/renderPDF.py
--rw-r--r--   0 robin     (1000) robin     (1000)    29894 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/graphics/renderPM.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37937 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)    37686 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12828 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/renderbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.618736 reportlab-4.0.9/src/reportlab/graphics/samples/
--rw-r--r--   0 robin     (1000) robin     (1000)       69 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/graphics/samples/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3584 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/bubble.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4241 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/clustered_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4188 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/clustered_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1947 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/excelcolors.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3126 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/exploded_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2691 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/filled_radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4267 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/line_chart.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5007 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/linechart_with_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3244 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/radar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1957 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/runall.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3566 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/scatter.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4164 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/scatter_lines.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3766 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/scatter_lines_markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2933 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/simple_pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4284 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/stacked_bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4230 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/samples/stacked_column.py
--rw-r--r--   0 robin     (1000) robin     (1000)    59283 2023-12-22 11:03:06.000000 reportlab-4.0.9/src/reportlab/graphics/shapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16116 2023-06-27 09:43:28.000000 reportlab-4.0.9/src/reportlab/graphics/svgpath.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9433 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/testdrawings.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17237 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/testshapes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1956 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/transform.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12748 2023-10-26 10:50:02.000000 reportlab-4.0.9/src/reportlab/graphics/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25552 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgetbase.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.622070 reportlab-4.0.9/src/reportlab/graphics/widgets/
--rw-r--r--   0 robin     (1000) robin     (1000)      242 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3920 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/adjustableArrow.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13073 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/eventcal.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30233 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/flags.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17504 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8424 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/markers.py
--rw-r--r--   0 robin     (1000) robin     (1000)    31655 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/signsandsymbols.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6932 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/graphics/widgets/table.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.628737 reportlab-4.0.9/src/reportlab/lib/
--rw-r--r--   0 robin     (1000) robin     (1000)     4972 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/PyFontify.py
--rw-r--r--   0 robin     (1000) robin     (1000)      256 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1122 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/abag.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7272 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/arciv.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5770 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/attrmap.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2927 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/boxstuff.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13051 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/lib/codecharts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    39074 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/lib/colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27141 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/corp.py
--rw-r--r--   0 robin     (1000) robin     (1000)      296 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/enums.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2226 2023-06-05 09:49:41.000000 reportlab-4.0.9/src/reportlab/lib/extformat.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13369 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/fontfinder.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3503 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/fonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3804 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/formatters.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1163 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1747 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/logger.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22017 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/normalDate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2001 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/pagesizes.py
--rw-r--r--   0 robin     (1000) robin     (1000)    30699 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2509 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/pygments2xpre.py
--rw-r--r--   0 robin     (1000) robin     (1000)    22859 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/randomtext.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13481 2023-11-01 13:06:46.000000 reportlab-4.0.9/src/reportlab/lib/rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)    39558 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/lib/rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1121 2023-06-05 09:49:41.000000 reportlab-4.0.9/src/reportlab/lib/rltempfile.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18407 2023-11-13 13:00:00.000000 reportlab-4.0.9/src/reportlab/lib/rparsexml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9647 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    17231 2023-12-11 12:14:11.000000 reportlab-4.0.9/src/reportlab/lib/styles.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13145 2023-10-16 09:19:35.000000 reportlab-4.0.9/src/reportlab/lib/testutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9723 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/textsplit.py
--rw-r--r--   0 robin     (1000) robin     (1000)      917 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/units.py
--rw-r--r--   0 robin     (1000) robin     (1000)    43246 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11333 2023-10-09 11:42:27.000000 reportlab-4.0.9/src/reportlab/lib/validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5717 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/lib/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1707 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/license.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.635403 reportlab-4.0.9/src/reportlab/pdfbase/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      275 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1794 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/_can_cmap_data.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32044 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/_cidfontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10141 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2934 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2308 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1829 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_standard.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3187 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2222 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courier.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3664 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3671 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3367 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3672 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3668 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3665 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3667 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2732 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
--rw-r--r--   0 robin     (1000) robin     (1000)   108467 2020-07-24 11:13:36.000000 reportlab-4.0.9/src/reportlab/pdfbase/_glyphlist.py
--rw-r--r--   0 robin     (1000) robin     (1000)    45680 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/acroform.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18768 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/cidfonts.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    90182 2024-01-04 09:24:37.000000 reportlab-4.0.9/src/reportlab/pdfbase/pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15704 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/pdfform.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    29935 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3763 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/pdfpattern.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    10135 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    56426 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfbase/rl_codecs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    53626 2024-01-10 10:20:16.000000 reportlab-4.0.9/src/reportlab/pdfbase/ttfonts.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.635403 reportlab-4.0.9/src/reportlab/pdfgen/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      270 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfgen/__init__.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    82031 2023-08-29 12:44:01.000000 reportlab-4.0.9/src/reportlab/pdfgen/canvas.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5737 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfgen/pathobject.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)     2980 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/pdfgen/pdfgeom.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8422 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/pdfgen/pdfimages.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)    19531 2023-07-13 11:02:38.000000 reportlab-4.0.9/src/reportlab/pdfgen/textobject.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.638737 reportlab-4.0.9/src/reportlab/platypus/
--rwxr-xr-x   0 robin     (1000) robin     (1000)      502 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)    54690 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/doctemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18313 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/figures.py
--rw-r--r--   0 robin     (1000) robin     (1000)    96177 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/platypus/flowables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11246 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/frames.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2753 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/multicol.py
--rw-r--r--   0 robin     (1000) robin     (1000)    93001 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/para.py
--rw-r--r--   0 robin     (1000) robin     (1000)   118012 2023-08-29 12:44:01.000000 reportlab-4.0.9/src/reportlab/platypus/paragraph.py
--rw-r--r--   0 robin     (1000) robin     (1000)   213795 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)    21268 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/tableofcontents.py
--rwxr-xr-x   0 robin     (1000) robin     (1000)   116486 2023-12-11 11:45:07.000000 reportlab-4.0.9/src/reportlab/platypus/tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    12947 2023-06-05 09:58:47.000000 reportlab-4.0.9/src/reportlab/platypus/xpreformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4930 2023-06-05 10:15:46.000000 reportlab-4.0.9/src/reportlab/rl_config.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15120 2024-01-07 10:52:18.000000 reportlab-4.0.9/src/reportlab/rl_settings.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.598736 reportlab-4.0.9/src/reportlab.egg-info/
--rw-r--r--   0 robin     (1000) robin     (1000)     1354 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab.egg-info/PKG-INFO
--rw-r--r--   0 robin     (1000) robin     (1000)    29650 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab.egg-info/SOURCES.txt
--rw-r--r--   0 robin     (1000) robin     (1000)        1 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab.egg-info/dependency_links.txt
--rw-r--r--   0 robin     (1000) robin     (1000)      143 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab.egg-info/requires.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       10 2024-01-10 10:20:31.000000 reportlab-4.0.9/src/reportlab.egg-info/top_level.txt
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.658737 reportlab-4.0.9/tests/
--rw-r--r--   0 robin     (1000) robin     (1000)      913 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/00readme.txt
--rw-r--r--   0 robin     (1000) robin     (1000)       80 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2024-01-08 14:22:19.000000 reportlab-4.0.9/tests/_i_am_actually_a_gif.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2024-01-08 14:22:19.000000 reportlab-4.0.9/tests/_i_am_actually_a_jpeg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3813 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/alpha_test.png
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.665404 reportlab-4.0.9/tests/barcode-out/
--rw-r--r--   0 robin     (1000) robin     (1000)      397 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Codabar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      783 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Code11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      700 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Code128.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      819 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Code128Auto.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2821 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/EAN13.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1341 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/EAN5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2230 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/EAN8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2335 2024-01-08 14:22:22.000000 reportlab-4.0.9/tests/barcode-out/ECC200DataMatrix.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      897 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Extended39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1205 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Extended93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      333 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/FIM.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      515 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/I2of5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3497 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/ISBN.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      415 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/MSI.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1512 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/POSTNET.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2703 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/QR.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3116 2024-01-08 14:22:22.000000 reportlab-4.0.9/tests/barcode-out/QR_with_comma.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      897 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Standard39.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      519 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/Standard93.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2799 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/UPCA.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      867 2024-01-08 14:22:21.000000 reportlab-4.0.9/tests/barcode-out/USPS_4State.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2230 2024-01-08 14:22:22.000000 reportlab-4.0.9/tests/barcode-out/test_cbcim.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2082 2024-01-08 14:22:22.000000 reportlab-4.0.9/tests/barcode-out/test_cbcim.png
--rw-r--r--   0 robin     (1000) robin     (1000)    12180 2024-01-08 14:22:22.000000 reportlab-4.0.9/tests/barcode-out/test_cbcim.tiff
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.715405 reportlab-4.0.9/tests/charts-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     1644 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1506 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1094 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1168 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4004 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3240 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2789 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3742 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2261 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2333 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3630 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2272 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1876 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1846 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2269 2024-01-08 14:22:30.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2281 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3552 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2314 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3616 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2294 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3560 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2272 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3546 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample5d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2681 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3743 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2674 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3727 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2681 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3734 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2714 2024-01-08 14:22:31.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3807 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2763 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2758 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3728 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2730 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3776 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2760 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3744 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1336 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample8a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample8a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1473 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample8b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7542 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample8b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3533 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13857 2024-01-08 14:22:32.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6765 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15564 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7070 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    15568 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample9c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7526 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2619 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample_hatching.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3374 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5299 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3053 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4033 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2873 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3120 2024-01-08 14:22:33.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1889 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2868 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5422 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9274 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4179 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7323 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4250 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7447 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4902 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9053 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4754 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6406 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3043 2024-01-08 14:22:34.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3256 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4149 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2884 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3669 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2807 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3020 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3880 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5378 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3929 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5381 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3440 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5290 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3443 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5291 2024-01-08 14:22:35.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3557 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5286 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3374 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5293 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6746 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    48255 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleStacked1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7900 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46272 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleSymbol1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3121 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4036 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3023 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3116 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2278 2024-01-08 14:22:36.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV0c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5870 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9403 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4426 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7338 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4441 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7450 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5323 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9105 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4561 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6379 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3134 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4004 2024-01-08 14:22:37.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3206 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4118 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2884 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3654 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2900 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3003 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV4d.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4468 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5412 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4780 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5422 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4408 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5332 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4426 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4579 2024-01-08 14:22:38.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4444 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5333 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV5c4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2693 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_sampleDoughnutDDFLabels.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4824 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_sampleDoughnutDDFLabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3065 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_samplePieDDFLabels.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6865 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_samplePieDDFLabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5998 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_sampleSpiderDDFLabels.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    20082 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_ddf_sampleSpiderDDFLabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5913 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1492 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6454 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2174 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7275 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7275 2024-01-08 14:22:39.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4062 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_doughnut_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2473 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2843 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2509 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample2c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2847 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample2c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2078 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2483 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2096 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample3a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2508 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample3a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3597 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample4a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3344 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample4a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6096 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    13106 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6805 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    14174 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6839 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    62954 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7830 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41220 2024-01-08 14:22:40.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2026 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8150 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5337 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    33385 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4702 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10135 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4572 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     9133 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1c.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5909 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10000 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3576 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7027 2024-01-08 14:22:41.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sampleFillPairedData.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2509 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2586 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.gif
--rw-r--r--   0 robin     (1000) robin     (1000)      841 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4232 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2775 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5667 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3940 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3443 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1272 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3899 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample4.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2052 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample4.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6789 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample5.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5057 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample5.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5997 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample6.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5182 2024-01-08 14:22:42.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample6.py
--rw-r--r--   0 robin     (1000) robin     (1000)    16703 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample7.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    23092 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample7.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9320 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample8.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12584 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample8.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10678 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample9.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12623 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample9.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4522 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_bcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7899 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_bcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4414 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_hlcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8690 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_hlcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4681 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_lpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10059 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_lpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3956 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_pcleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3805 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_pcleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4985 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_plpleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6410 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_plpleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7147 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8888 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9287 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1barline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8676 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1barline.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4905 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6067 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8790 2024-01-08 14:22:45.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample2bar.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12069 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample2bar.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5364 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample2line.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6357 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample2line.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1766 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample3.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1182 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample3.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4272 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample4pie.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7677 2024-01-08 14:22:46.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample4pie.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6644 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_scleg.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5397 2024-01-08 14:22:47.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_scleg.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8850 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_spider_sample1.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     4414 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_spider_sample1.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11209 2024-01-08 14:22:43.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_spider_sample2.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10045 2024-01-08 14:22:44.000000 reportlab-4.0.9/tests/charts-out/test_graphics_charts_spider_sample2.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2979 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/encryption.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1908 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/gray-alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1894 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/pythonpowered-gs.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     1077 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/pythonpowered.gif
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.732072 reportlab-4.0.9/tests/render-out/
--rw-r--r--   0 robin     (1000) robin     (1000)     2620 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/410.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1362 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/410.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3227 2024-01-08 14:22:23.000000 reportlab-4.0.9/tests/render-out/Drawing01.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5097 2024-01-08 14:22:23.000000 reportlab-4.0.9/tests/render-out/Drawing01.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2840 2024-01-08 14:22:23.000000 reportlab-4.0.9/tests/render-out/Drawing01.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1020 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing01.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2631 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing02.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5738 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing02.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     3007 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing02.png
--rw-r--r--   0 robin     (1000) robin     (1000)      846 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing02.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8875 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing03.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8724 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing03.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    14909 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing03.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1327 2024-01-08 14:22:24.000000 reportlab-4.0.9/tests/render-out/Drawing03.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2381 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing04.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2791 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing04.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2797 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing04.png
--rw-r--r--   0 robin     (1000) robin     (1000)      858 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing04.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3166 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing05.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3723 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing05.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4704 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing05.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1393 2024-01-08 14:22:25.000000 reportlab-4.0.9/tests/render-out/Drawing05.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6934 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing06.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    10681 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing06.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    13274 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing06.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2886 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing06.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3841 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing07.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5432 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing07.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     6945 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing07.png
--rw-r--r--   0 robin     (1000) robin     (1000)     8298 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing07.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3470 2024-01-08 14:22:26.000000 reportlab-4.0.9/tests/render-out/Drawing08.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     6598 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing08.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     4071 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing08.png
--rw-r--r--   0 robin     (1000) robin     (1000)    10846 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing08.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7159 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing09.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8270 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing09.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    14238 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing09.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1339 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing09.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3102 2024-01-08 14:22:27.000000 reportlab-4.0.9/tests/render-out/Drawing10.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     5774 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing10.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     2309 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing10.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2163 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing10.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2362 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing11.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2957 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing11.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     3355 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing11.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7969 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing11.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10532 2024-01-08 14:22:28.000000 reportlab-4.0.9/tests/render-out/Drawing12.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     8516 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing12.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    19324 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing12.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1219 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing12.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1100 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing14.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     2124 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing14.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)     1235 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing14.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1064 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/Drawing14.py
--rw-r--r--   0 robin     (1000) robin     (1000)      342 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-none.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1011 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-none.py
--rw-r--r--   0 robin     (1000) robin     (1000)      336 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-pdf.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)      352 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-svg.png
--rw-r--r--   0 robin     (1000) robin     (1000)     1012 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/autoclose-svg.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11856 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/fillmode-even-odd.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/fillmode-even-odd.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11803 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/fillmode-non-zero.png
--rw-r--r--   0 robin     (1000) robin     (1000)     7997 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/fillmode-non-zero.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13148 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/hatch.png
--rw-r--r--   0 robin     (1000) robin     (1000)     6477 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/hatch.py
--rw-r--r--   0 robin     (1000) robin     (1000)      904 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/svglib-issue104.png
--rw-r--r--   0 robin     (1000) robin     (1000)    24546 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/textmode.png
--rw-r--r--   0 robin     (1000) robin     (1000)     2027 2024-01-08 14:22:29.000000 reportlab-4.0.9/tests/render-out/textmode.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6504 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/rltw-icon-tr.png
--rwxr-xr-x   0 robin     (1000) robin     (1000)     5650 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/runAll.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2402 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/solid_red_alpha.png
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/tall_red.png
--rw-r--r--   0 robin     (1000) robin     (1000)      288 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test-cross.tiff
--rw-r--r--   0 robin     (1000) robin     (1000)      168 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test-indexed.png
--rw-r--r--   0 robin     (1000) robin     (1000)      157 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test-rgba.png
--rw-r--r--   0 robin     (1000) robin     (1000)     9464 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_charts_textlabels.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6204 2023-10-16 09:20:06.000000 reportlab-4.0.9/tests/test_crypto_algorithms.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1462 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_docs_build.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6506 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_docstrings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3058 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_extra.py
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_geomutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)    14802 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_graphics_barcode.py
--rw-r--r--   0 robin     (1000) robin     (1000)    46252 2023-10-30 08:50:59.000000 reportlab-4.0.9/tests/test_graphics_charts.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32774 2023-04-26 08:44:40.000000 reportlab-4.0.9/tests/test_graphics_images-cairo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46849 2023-04-26 08:44:40.000000 reportlab-4.0.9/tests/test_graphics_images-cairo.png
--rw-r--r--   0 robin     (1000) robin     (1000)    16209 2024-01-08 14:23:00.000000 reportlab-4.0.9/tests/test_graphics_images-libart.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    21349 2024-01-08 14:23:00.000000 reportlab-4.0.9/tests/test_graphics_images-libart.png
--rw-r--r--   0 robin     (1000) robin     (1000)    32774 2024-01-08 14:23:00.000000 reportlab-4.0.9/tests/test_graphics_images.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    46849 2024-01-08 14:23:00.000000 reportlab-4.0.9/tests/test_graphics_images.png
--rw-r--r--   0 robin     (1000) robin     (1000)     3832 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_graphics_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2523 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_graphics_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15835 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_graphics_render.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2628 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_graphics_speed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1893 2023-10-16 09:02:32.000000 reportlab-4.0.9/tests/test_hello.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2609 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2530 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_invariant.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4214 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_issues.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8276 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_lib_colors.py
--rw-r--r--   0 robin     (1000) robin     (1000)    11916 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_lib_normaldate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6062 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_lib_pdfencrypt.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9595 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_lib_rl_safe_eval.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3748 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_lib_sequencer.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13279 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_lib_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5592 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_lib_validators.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2448 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_multibyte_chs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4973 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_multibyte_cht.py
--rw-r--r--   0 robin     (1000) robin     (1000)    25468 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_multibyte_jpn.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6658 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/test_multibyte_kor.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34098 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10749 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_pdfbase_encodings.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3875 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pdfbase_fontembed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     2713 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pdfbase_pdfdoc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    18606 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pdfbase_pdfform.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4120 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pdfbase_pdfmetrics.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1609 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pdfbase_pdfutils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_pdfbase_postscript.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19845 2024-01-10 10:20:16.000000 reportlab-4.0.9/tests/test_pdfbase_ttfonts.py
--rw-r--r--   0 robin     (1000) robin     (1000)      989 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_pdfgen_callback.py
--rw-r--r--   0 robin     (1000) robin     (1000)    48003 2023-06-15 10:04:03.000000 reportlab-4.0.9/tests/test_pdfgen_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6925 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_pdfgen_links.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3133 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_pdfgen_overprint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1850 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_pdfgen_pagemodes.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3168 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/test_platypus_accum.py
--rw-r--r--   0 robin     (1000) robin     (1000)    27202 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_breaking.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5973 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_cjk_wrap.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34694 2023-11-13 13:12:58.000000 reportlab-4.0.9/tests/test_platypus_general.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4149 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_images.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8549 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_indents.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5383 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_index.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6293 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_leftright.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10786 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_lists.py
--rw-r--r--   0 robin     (1000) robin     (1000)   113082 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_platypus_paragraphs.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5094 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_paraparser.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9402 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_pleaseturnover.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8635 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_preformatted.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7373 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_programming.py
--rw-r--r--   0 robin     (1000) robin     (1000)    54547 2023-12-11 11:50:51.000000 reportlab-4.0.9/tests/test_platypus_tables.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13445 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_toc.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3773 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_wrapping.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5183 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_platypus_xref.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4762 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_pyfiles.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7690 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_renderPS.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9773 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_renderSVG.py
--rw-r--r--   0 robin     (1000) robin     (1000)    10814 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_rl_accel.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3423 2023-06-05 09:58:47.000000 reportlab-4.0.9/tests/test_source_chars.py
--rw-r--r--   0 robin     (1000) robin     (1000)    19098 2023-06-05 10:15:46.000000 reportlab-4.0.9/tests/test_table_inrowsplit.py
--rw-r--r--   0 robin     (1000) robin     (1000)    34217 2023-12-11 10:40:03.000000 reportlab-4.0.9/tests/test_table_layout.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1244 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/test_tools_pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1353 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4890 2023-06-05 09:49:41.000000 reportlab-4.0.9/tests/test_widgetbase_tpc.py
--rw-r--r--   0 robin     (1000) robin     (1000)    15476 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/test_widgets_grids.py
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2019-10-12 07:24:05.000000 reportlab-4.0.9/tests/unimportable.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.735406 reportlab-4.0.9/tools/
--rw-r--r--   0 robin     (1000) robin     (1000)      193 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/README
--rw-r--r--   0 robin     (1000) robin     (1000)      160 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/__init__.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.735406 reportlab-4.0.9/tools/docco/
--rw-r--r--   0 robin     (1000) robin     (1000)      292 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/docco/README
--rw-r--r--   0 robin     (1000) robin     (1000)      166 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7791 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/codegrab.py
--rw-r--r--   0 robin     (1000) robin     (1000)    41170 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/docpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    29268 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)    32661 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/graphdocpy.py
--rw-r--r--   0 robin     (1000) robin     (1000)    13738 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/rl_doc_utils.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5898 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/rltemplate.py
--rw-r--r--   0 robin     (1000) robin     (1000)     6939 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/stylesheet.py
--rw-r--r--   0 robin     (1000) robin     (1000)     9899 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/t_parse.py
--rw-r--r--   0 robin     (1000) robin     (1000)     7023 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/yaml.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3284 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/docco/yaml2pdf.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1056 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pdfpath.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.738739 reportlab-4.0.9/tools/pythonpoint/
--rw-r--r--   0 robin     (1000) robin     (1000)     1099 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/README
--rw-r--r--   0 robin     (1000) robin     (1000)      172 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     8840 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/customshapes.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.742072 reportlab-4.0.9/tools/pythonpoint/demos/
--rw-r--r--   0 robin     (1000) robin     (1000)    26616 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/demos/examples.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3670 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/figures.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     4859 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/htu.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     3008 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/leftlogo.a85
--rw-r--r--   0 robin     (1000) robin     (1000)     2198 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/leftlogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    12463 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/lj8100.jpg
--rw-r--r--   0 robin     (1000) robin     (1000)    11730 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/monterey.xml
--rw-r--r--   0 robin     (1000) robin     (1000)    12918 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/outline.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     3429 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/pplogo.gif
--rw-r--r--   0 robin     (1000) robin     (1000)   125666 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/python.gif
--rw-r--r--   0 robin     (1000) robin     (1000)    41307 2023-06-05 09:49:41.000000 reportlab-4.0.9/tools/pythonpoint/demos/pythonpoint.xml
--rw-r--r--   0 robin     (1000) robin     (1000)     1704 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/slidebox.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1855 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/spectrum.png
--rw-r--r--   0 robin     (1000) robin     (1000)    20910 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/demos/vertpython.gif
--rw-r--r--   0 robin     (1000) robin     (1000)     7920 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/pythonpoint/pythonpoint.dtd
--rw-r--r--   0 robin     (1000) robin     (1000)    34726 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/pythonpoint.py
--rw-r--r--   0 robin     (1000) robin     (1000)    28916 2023-06-05 10:15:46.000000 reportlab-4.0.9/tools/pythonpoint/stdparser.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.745406 reportlab-4.0.9/tools/pythonpoint/styles/
--rw-r--r--   0 robin     (1000) robin     (1000)      179 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/__init__.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3179 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/horrible.py
--rw-r--r--   0 robin     (1000) robin     (1000)     5079 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/htu.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3692 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/modern.py
--rw-r--r--   0 robin     (1000) robin     (1000)     3215 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/projection.py
--rw-r--r--   0 robin     (1000) robin     (1000)     4003 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/pythonpoint/styles/standard.py
-drwxr-xr-x   0 robin     (1000) robin     (1000)        0 2024-01-10 10:20:31.745406 reportlab-4.0.9/tools/utils/
--rw-r--r--   0 robin     (1000) robin     (1000)      954 2023-06-05 09:58:47.000000 reportlab-4.0.9/tools/utils/add_bleed.py
--rw-r--r--   0 robin     (1000) robin     (1000)     1891 2019-10-12 07:24:05.000000 reportlab-4.0.9/tools/utils/dumpttf.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.658558 reportlab-4.1.0/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    51054 2024-02-08 12:00:17.000000 reportlab-4.1.0/CHANGES.md
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       53 2023-08-03 11:30:42.000000 reportlab-4.1.0/INSTALL.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1707 2023-08-03 11:30:43.000000 reportlab-4.1.0/LICENSE
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      468 2023-08-03 11:30:43.000000 reportlab-4.1.0/MANIFEST.in
+-rw-r--r--   0 rptlab    (1000) rptlab    (1000)     1354 2024-02-08 12:05:48.658558 reportlab-4.1.0/PKG-INFO
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4994 2023-08-03 11:30:43.000000 reportlab-4.1.0/README.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       72 2023-08-03 11:30:43.000000 reportlab-4.1.0/VERSION.txt
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.334558 reportlab-4.1.0/demos/
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.334558 reportlab-4.1.0/demos/colors/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2728 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/colors/colortest.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.334558 reportlab-4.1.0/demos/gadflypaper/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      105 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/gadflypaper/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32486 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/gadflypaper/gfe.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.338558 reportlab-4.1.0/demos/odyssey/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2098 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/odyssey/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7649 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/odyssey/dodyssey.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4580 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/odyssey/fodyssey.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4235 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/odyssey/odyssey.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10950 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/odyssey/odyssey.txt
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.338558 reportlab-4.1.0/demos/rlzope/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2538 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/rlzope/readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6791 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/rlzope/rlzope.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.338558 reportlab-4.1.0/demos/stdfonts/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      229 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/stdfonts/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2381 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/stdfonts/stdfonts.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.338558 reportlab-4.1.0/demos/tests/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      525 2023-08-03 11:30:42.000000 reportlab-4.1.0/demos/tests/testdemos.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.338558 reportlab-4.1.0/docs/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      313 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3136 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/Makefile
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)     1497 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/genAll.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)      143 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/gen_epydoc
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.342558 reportlab-4.1.0/docs/images/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9685 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/Edit_Prefs.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    28106 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/Python_21.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    29117 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/Python_21_HINT.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    37812 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/fileExchange.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10513 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/jpn.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    33898 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/jpnchars.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12463 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/lj8100.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      393 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/redsquare.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    26548 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/replogo.a85
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    16583 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/replogo.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      924 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/images/testimg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3081 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/make.bat
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.342558 reportlab-4.1.0/docs/reference/
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)      110 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/reference/build.bat
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1206 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/reference/genreference.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9927 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/reference/reference.yml
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.342558 reportlab-4.1.0/docs/source/
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.342558 reportlab-4.1.0/docs/source/_static/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      252 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/_static/basic.css
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    16419 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/_static/default.css
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.342558 reportlab-4.1.0/docs/source/_templates/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      167 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/_templates/layout.html
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1431 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/_templates/page.html
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6427 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/conf.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1345 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/graphics.rst
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1049 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/index.rst
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      885 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/lib.rst
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      238 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/pdfgen.rst
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      984 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/source/platypus.rst
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.394558 reportlab-4.1.0/docs/userguide/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4494 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/app_demos.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17692 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch1_intro.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    45531 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch2_graphics.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    19934 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch2a_fonts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    30547 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch3_pdffeatures.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    19314 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch4_platypus_concepts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    23044 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch5_paragraphs.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34555 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch6_tables.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2643 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/ch7_custom.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3575 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/genuserguide.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    52769 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/graph_charts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11788 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/graph_concepts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      490 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/graph_intro.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12403 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/graph_shapes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13522 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/graph_widgets.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      112 2023-08-03 11:30:43.000000 reportlab-4.1.0/docs/userguide/testfile.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       89 2023-08-03 11:30:43.000000 reportlab-4.1.0/pyproject.toml
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       38 2024-02-08 12:05:48.658558 reportlab-4.1.0/setup.cfg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12004 2024-02-08 11:57:58.000000 reportlab-4.1.0/setup.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.334558 reportlab-4.1.0/src/
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.394558 reportlab-4.1.0/src/reportlab/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      185 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/MANIFEST.in
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1481 2024-02-08 11:57:23.000000 reportlab-4.1.0/src/reportlab/__init__.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.398558 reportlab-4.1.0/src/reportlab/fonts/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      318 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      504 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGarden-changelog.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17976 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGarden-copying-gpl.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1318 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGarden-copying.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4122 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGarden-readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   519634 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGarden.sfd
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10351 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGardenMK.afm
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    79824 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/DarkGardenMK.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    65932 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/Vera.ttf
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    63208 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/VeraBI.ttf
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    58716 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/VeraBd.ttf
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    63684 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/VeraIt.ttf
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32084 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_a______.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    31966 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_ab_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32019 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_abi____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32115 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_ai_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    35377 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_eb_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    38543 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_ebi____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    37518 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_ei_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    35380 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/_er_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5954 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/fonts/bitstream-vera-license.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8318 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/callig15.afm
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    59663 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/callig15.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    35500 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/cob_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    50532 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/cobo____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34585 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/com_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    48468 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/coo_____.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34705 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/sy______.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    49593 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/zd______.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    75573 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/zx______.pfb
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    96418 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab/fonts/zy______.pfb
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.402558 reportlab-4.1.0/src/reportlab/graphics/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      274 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/__init__.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.402558 reportlab-4.1.0/src/reportlab/graphics/barcode/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1741 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/README
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      915 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/TODO
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5886 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18451 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/code128.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9799 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/code39.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9077 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/code93.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    24425 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/common.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7872 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/dmtx.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18922 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/eanbc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17884 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/ecc200datamatrix.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3746 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/fourstate.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7377 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/lto.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6266 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/qr.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34117 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/qrencoder.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11765 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/test.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8076 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/usps.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15681 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/usps4s.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17499 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/barcode/widgets.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.406558 reportlab-4.1.0/src/reportlab/graphics/charts/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      234 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4405 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/areas.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    92550 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/axes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    72361 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/barcharts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6628 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/dotbox.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18934 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/doughnut.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    25687 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/legends.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    27408 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/graphics/charts/linecharts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    51175 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/graphics/charts/lineplots.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1739 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/markers.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    66794 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/piecharts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8548 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/slidebox.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    16132 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/spider.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    22945 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/charts/textlabels.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11556 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7194 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/charts/utils3d.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15156 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/renderPDF.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    29894 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/renderPM.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    37937 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/renderPS.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    37686 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/renderSVG.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12828 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/renderbase.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.410558 reportlab-4.1.0/src/reportlab/graphics/samples/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       69 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3584 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/bubble.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4241 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/clustered_bar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4188 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/clustered_column.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1947 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/excelcolors.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3126 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/exploded_pie.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2691 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/filled_radar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4267 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/line_chart.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5007 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/linechart_with_markers.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3244 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/radar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1957 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/runall.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3566 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/scatter.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4164 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/scatter_lines.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3766 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/scatter_lines_markers.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2933 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/simple_pie.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4284 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/stacked_bar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4230 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/samples/stacked_column.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    59283 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/shapes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    16116 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/svgpath.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9433 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/testdrawings.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17237 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/testshapes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1956 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/transform.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12748 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/graphics/utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    25552 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgetbase.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.410558 reportlab-4.1.0/src/reportlab/graphics/widgets/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      242 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3920 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/adjustableArrow.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13073 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/eventcal.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    30233 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/flags.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17504 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/grids.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8424 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/markers.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    31655 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/signsandsymbols.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6932 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/graphics/widgets/table.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.414558 reportlab-4.1.0/src/reportlab/lib/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4972 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/PyFontify.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      256 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1122 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/abag.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7272 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/arciv.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6419 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/lib/attrmap.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2927 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/boxstuff.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13051 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/codecharts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    39074 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/colors.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    27141 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/corp.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      296 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/enums.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2226 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/extformat.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13369 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/fontfinder.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3503 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/fonts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3804 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/formatters.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1163 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/geomutils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1747 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/logger.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    22017 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/normalDate.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2001 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/pagesizes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    30699 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/pdfencrypt.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2509 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/pygments2xpre.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    22859 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/randomtext.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13481 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/lib/rl_accel.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    39558 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/rl_safe_eval.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1121 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/rltempfile.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18407 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/lib/rparsexml.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9647 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/sequencer.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    17231 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/lib/styles.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13145 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/lib/testutils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9723 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/textsplit.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      917 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/units.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    43246 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11333 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/lib/validators.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5717 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/lib/yaml.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.418558 reportlab-4.1.0/src/reportlab/pdfbase/
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)      275 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1794 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_can_cmap_data.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32044 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_cidfontdata.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10141 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3058 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_macexpert.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2934 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_macroman.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2308 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1829 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_standard.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3187 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_symbol.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3003 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_winansi.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2222 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3664 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courier.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3664 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courierbold.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3664 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3664 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3671 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helvetica.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3670 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3670 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3671 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3367 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_symbol.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3672 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesbold.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3668 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3665 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3667 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesroman.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2732 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   108467 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/_glyphlist.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    45680 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/acroform.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18768 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/cidfonts.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)    90182 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/pdfdoc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15704 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/pdfform.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)    29935 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/pdfmetrics.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3763 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/pdfpattern.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)    10135 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/pdfutils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    56426 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfbase/rl_codecs.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    54067 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/pdfbase/ttfonts.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.418558 reportlab-4.1.0/src/reportlab/pdfgen/
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)      270 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfgen/__init__.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)    82797 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/pdfgen/canvas.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)     5737 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfgen/pathobject.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)     2980 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfgen/pdfgeom.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8422 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfgen/pdfimages.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)    19531 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/pdfgen/textobject.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.422558 reportlab-4.1.0/src/reportlab/platypus/
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)      502 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    54690 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/doctemplate.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18313 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/figures.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    96074 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/platypus/flowables.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10144 2024-02-08 11:55:47.000000 reportlab-4.1.0/src/reportlab/platypus/frames.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2753 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/multicol.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    93001 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/para.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   118012 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/platypus/paragraph.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   213795 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/paraparser.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    21268 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/tableofcontents.py
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)   116486 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/platypus/tables.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12947 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/platypus/xpreformatted.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4930 2023-08-03 11:30:43.000000 reportlab-4.1.0/src/reportlab/rl_config.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15120 2024-01-11 09:45:59.000000 reportlab-4.1.0/src/reportlab/rl_settings.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.654559 reportlab-4.1.0/src/reportlab.egg-info/
+-rw-r--r--   0 rptlab    (1000) rptlab    (1000)     1354 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab.egg-info/PKG-INFO
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18196 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)        1 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      143 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab.egg-info/requires.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       10 2024-02-08 12:05:48.000000 reportlab-4.1.0/src/reportlab.egg-info/top_level.txt
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.510558 reportlab-4.1.0/tests/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      913 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/00readme.txt
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)       80 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1077 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/_i_am_actually_a_gif.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12463 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/_i_am_actually_a_jpeg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3813 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/alpha_test.png
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.554558 reportlab-4.1.0/tests/barcode-out/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      397 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Codabar.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      783 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Code11.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      700 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Code128.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      819 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Code128Auto.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2821 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/EAN13.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1341 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/EAN5.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2230 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/EAN8.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2335 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/ECC200DataMatrix.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      897 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Extended39.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1205 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Extended93.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      333 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/FIM.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      515 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/I2of5.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3497 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/ISBN.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      415 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/MSI.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1512 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/POSTNET.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2703 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/QR.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3116 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/QR_with_comma.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      897 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Standard39.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      519 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/Standard93.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2799 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/UPCA.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      867 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/USPS_4State.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2230 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/test_cbcim.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2082 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/test_cbcim.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12180 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/barcode-out/test_cbcim.tiff
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.578559 reportlab-4.1.0/tests/charts-out/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1644 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0a.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1506 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0a.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1094 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0b.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1168 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0b.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2473 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample1c.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2843 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample1c.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2509 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample2c.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2847 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample2c.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2078 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2483 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2096 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3a.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2508 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3a.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3599 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample4a.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3344 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample4a.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4522 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_bcleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7899 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_bcleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4414 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_hlcleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8690 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_hlcleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4681 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_lpleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10059 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_lpleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3956 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_pcleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3805 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_pcleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4985 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_plpleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6410 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_plpleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7147 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1bar.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8888 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1bar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9287 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1barline.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8676 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1barline.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4907 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1line.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6067 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1line.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8790 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2bar.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12069 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2bar.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5362 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2line.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6357 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2line.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1766 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample3.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1182 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample3.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4272 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample4pie.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7677 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample4pie.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6644 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_scleg.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5397 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_scleg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2979 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/encryption.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1908 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/gray-alpha.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1894 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/pythonpowered-gs.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1077 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/pythonpowered.gif
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.598559 reportlab-4.1.0/tests/render-out/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2620 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/410.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1362 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/410.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3227 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing01.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5097 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing01.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2840 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing01.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1020 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing01.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2631 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing02.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5738 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing02.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3007 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing02.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      846 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing02.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8875 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing03.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8724 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing03.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    14909 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing03.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1327 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing03.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2381 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing04.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2791 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing04.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2797 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing04.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      858 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing04.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3166 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing05.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3723 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing05.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4704 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing05.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1393 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing05.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6934 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing06.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10681 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing06.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13274 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing06.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2886 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing06.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3841 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing07.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5432 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing07.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6945 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing07.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8298 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing07.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3470 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing08.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6598 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing08.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4071 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing08.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10846 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing08.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7159 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing09.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8270 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing09.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    14238 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing09.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1339 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing09.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3102 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing10.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5774 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing10.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2309 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing10.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2163 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing10.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2362 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing11.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2957 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing11.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3355 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing11.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7969 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing11.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10532 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing12.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8516 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing12.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    19324 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing12.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1219 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing12.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1100 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing14.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2124 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing14.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1235 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing14.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1064 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/Drawing14.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      342 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-none.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1011 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-none.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      336 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-pdf.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1012 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-pdf.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      352 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-svg.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1012 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/autoclose-svg.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11856 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/fillmode-even-odd.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7997 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/fillmode-even-odd.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11803 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/fillmode-non-zero.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7997 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/fillmode-non-zero.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13148 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/hatch.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6477 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/hatch.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      904 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/svglib-issue104.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    24546 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/textmode.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2027 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/render-out/textmode.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6504 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/rltw-icon-tr.png
+-rwxrwxr-x   0 rptlab    (1000) rptlab    (1000)     5650 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/runAll.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2402 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/solid_red_alpha.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      172 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/tall_red.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      288 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test-cross.tiff
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      168 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test-indexed.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      157 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test-rgba.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9464 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_charts_textlabels.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6204 2024-01-11 09:45:59.000000 reportlab-4.1.0/tests/test_crypto_algorithms.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1462 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_docs_build.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6506 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_docstrings.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3058 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_extra.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      954 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_geomutils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    14802 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_graphics_barcode.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    46252 2024-01-11 09:45:59.000000 reportlab-4.1.0/tests/test_graphics_charts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32774 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_graphics_images.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    46849 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_graphics_images.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3832 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_graphics_images.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2523 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_graphics_layout.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15835 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_graphics_render.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2628 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_graphics_speed.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1893 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_hello.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2609 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_images.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2530 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_invariant.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4214 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_issues.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8276 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_lib_colors.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11916 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_lib_normaldate.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6062 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_lib_pdfencrypt.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9595 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_lib_rl_safe_eval.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3748 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_lib_sequencer.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13279 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_lib_utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5592 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_lib_validators.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2448 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_multibyte_chs.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4973 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_multibyte_cht.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    25468 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_multibyte_jpn.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6658 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_multibyte_kor.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34098 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_paragraphs.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10749 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfbase_encodings.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3875 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfbase_fontembed.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2713 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_pdfbase_pdfdoc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    18606 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfbase_pdfform.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4120 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_pdfbase_pdfmetrics.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1609 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfbase_pdfutils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3179 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfbase_postscript.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    20408 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_pdfbase_ttfonts.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      989 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_pdfgen_callback.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    48003 2024-01-11 09:45:59.000000 reportlab-4.1.0/tests/test_pdfgen_general.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6925 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pdfgen_links.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3133 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_pdfgen_overprint.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1850 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_pdfgen_pagemodes.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3168 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_accum.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    27172 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_breaking.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6008 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_cjk_wrap.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34629 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_general.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4092 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_images.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8584 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_indents.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5383 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_index.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6293 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_leftright.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10786 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_lists.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   113056 2024-02-08 11:55:47.000000 reportlab-4.1.0/tests/test_platypus_paragraphs.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5094 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_platypus_paraparser.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9402 2023-08-03 11:30:44.000000 reportlab-4.1.0/tests/test_platypus_pleaseturnover.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8635 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_preformatted.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7373 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_programming.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    54547 2024-01-11 09:45:59.000000 reportlab-4.1.0/tests/test_platypus_tables.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13445 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_toc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3773 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_wrapping.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5183 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_platypus_xref.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4762 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_pyfiles.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7690 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_renderPS.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9773 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_renderSVG.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    10814 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_rl_accel.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3423 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_source_chars.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    19098 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_table_inrowsplit.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34217 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_table_layout.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1244 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_tools_pythonpoint.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1353 2023-08-03 11:30:43.000000 reportlab-4.1.0/tests/test_utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4890 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_widgetbase_tpc.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    15476 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/test_widgets_grids.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      166 2023-08-03 11:30:45.000000 reportlab-4.1.0/tests/unimportable.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.602558 reportlab-4.1.0/tools/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      193 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/README
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      160 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/__init__.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.602558 reportlab-4.1.0/tools/docco/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      292 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/README
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      166 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7791 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/codegrab.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    41170 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/docpy.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    29268 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/examples.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    32661 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/graphdocpy.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    13738 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/rl_doc_utils.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5898 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/rltemplate.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     6939 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/stylesheet.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     9899 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/t_parse.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7023 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/yaml.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3284 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/docco/yaml2pdf.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1056 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pdfpath.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.606558 reportlab-4.1.0/tools/pythonpoint/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1099 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/README
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      172 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     8840 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/customshapes.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.626558 reportlab-4.1.0/tools/pythonpoint/demos/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    26616 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/examples.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3670 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/figures.xml
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4859 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/htu.xml
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3008 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/leftlogo.a85
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     2198 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/leftlogo.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12463 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/lj8100.jpg
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    11730 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/monterey.xml
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    12918 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/outline.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3429 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/pplogo.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)   125666 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/python.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    41307 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/pythonpoint.xml
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1704 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/slidebox.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1855 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/spectrum.png
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    20910 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/demos/vertpython.gif
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     7920 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/pythonpoint.dtd
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    34726 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/pythonpoint.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)    28916 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/stdparser.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.654559 reportlab-4.1.0/tools/pythonpoint/styles/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      179 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/__init__.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3179 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/horrible.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     5079 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/htu.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3692 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/modern.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     3215 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/projection.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     4003 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/pythonpoint/styles/standard.py
+drwxrwxr-x   0 rptlab    (1000) rptlab    (1000)        0 2024-02-08 12:05:48.654559 reportlab-4.1.0/tools/utils/
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)      954 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/utils/add_bleed.py
+-rw-rw-r--   0 rptlab    (1000) rptlab    (1000)     1891 2023-08-03 11:30:43.000000 reportlab-4.1.0/tools/utils/dumpttf.py
```

### Comparing `reportlab-4.0.9/CHANGES.md` & `reportlab-4.1.0/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 E.g. to retrieve the changes made between release 3.4 and release 3.5, type::
 
   $ hg log -r 54ce2469ba5c
 
 The contributors lists are in no order and apologies to those accidentally not
 mentioned. If we missed you, please let us know!
 
+
+CHANGES  4.1.0 08/02/2024
+-------------------------
+    * No change.  Changes to commercial package, re-released with same version number
+
+CHANGES  4.0.9.1 23/01/2024
+---------------------------
+    * use ttf subsets[0][1:32] fillin
+    * implement drawBoundary as a proper canvas method (removing it from Frame)
+
 CHANGES  4.0.9   08/01/2024
 ---------------------------
     * fix TTFont hmtx bug and force index 0(.notdef) in subsets as better for PDFUA 
 
 CHANGES  4.0.8   11/12/2023
 ---------------------------
     * fix rparsexml bug contributed by Matt Folwell  mjf at pearson co uk
```

### Comparing `reportlab-4.0.9/LICENSE` & `reportlab-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/PKG-INFO` & `reportlab-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 4.0.9
+Version: 4.1.0
 Summary: The Reportlab Toolkit
 Home-page: https://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
 License: BSD license (see license.txt for details), Copyright (c) 2000-2022, ReportLab Inc.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `reportlab-4.0.9/README.txt` & `reportlab-4.1.0/README.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/colors/colortest.py` & `reportlab-4.1.0/demos/colors/colortest.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/gadflypaper/gfe.py` & `reportlab-4.1.0/demos/gadflypaper/gfe.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/odyssey/00readme.txt` & `reportlab-4.1.0/demos/odyssey/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/odyssey/dodyssey.py` & `reportlab-4.1.0/demos/odyssey/dodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/odyssey/fodyssey.py` & `reportlab-4.1.0/demos/odyssey/fodyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/odyssey/odyssey.py` & `reportlab-4.1.0/demos/odyssey/odyssey.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/odyssey/odyssey.txt` & `reportlab-4.1.0/demos/odyssey/odyssey.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/rlzope/readme.txt` & `reportlab-4.1.0/demos/rlzope/readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/rlzope/rlzope.py` & `reportlab-4.1.0/demos/rlzope/rlzope.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/stdfonts/stdfonts.py` & `reportlab-4.1.0/demos/stdfonts/stdfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/demos/tests/testdemos.py` & `reportlab-4.1.0/demos/tests/testdemos.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/Makefile` & `reportlab-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/genAll.py` & `reportlab-4.1.0/docs/genAll.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/Edit_Prefs.gif` & `reportlab-4.1.0/docs/images/Edit_Prefs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/Python_21.gif` & `reportlab-4.1.0/docs/images/Python_21.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/Python_21_HINT.gif` & `reportlab-4.1.0/docs/images/Python_21_HINT.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/fileExchange.gif` & `reportlab-4.1.0/docs/images/fileExchange.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/jpn.gif` & `reportlab-4.1.0/docs/images/jpn.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/jpnchars.jpg` & `reportlab-4.1.0/docs/images/jpnchars.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/lj8100.jpg` & `reportlab-4.1.0/docs/images/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/replogo.a85` & `reportlab-4.1.0/docs/images/replogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/replogo.gif` & `reportlab-4.1.0/docs/images/replogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/images/testimg.gif` & `reportlab-4.1.0/docs/images/testimg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/make.bat` & `reportlab-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/reference/genreference.py` & `reportlab-4.1.0/docs/reference/genreference.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/reference/reference.yml` & `reportlab-4.1.0/docs/reference/reference.yml`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/_static/default.css` & `reportlab-4.1.0/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/_templates/page.html` & `reportlab-4.1.0/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/conf.py` & `reportlab-4.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/graphics.rst` & `reportlab-4.1.0/docs/source/graphics.rst`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/index.rst` & `reportlab-4.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/lib.rst` & `reportlab-4.1.0/docs/source/lib.rst`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/source/platypus.rst` & `reportlab-4.1.0/docs/source/platypus.rst`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/app_demos.py` & `reportlab-4.1.0/docs/userguide/app_demos.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch1_intro.py` & `reportlab-4.1.0/docs/userguide/ch1_intro.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch2_graphics.py` & `reportlab-4.1.0/docs/userguide/ch2_graphics.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch2a_fonts.py` & `reportlab-4.1.0/docs/userguide/ch2a_fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch3_pdffeatures.py` & `reportlab-4.1.0/docs/userguide/ch3_pdffeatures.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch4_platypus_concepts.py` & `reportlab-4.1.0/docs/userguide/ch4_platypus_concepts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch5_paragraphs.py` & `reportlab-4.1.0/docs/userguide/ch5_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch6_tables.py` & `reportlab-4.1.0/docs/userguide/ch6_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/ch7_custom.py` & `reportlab-4.1.0/docs/userguide/ch7_custom.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/genuserguide.py` & `reportlab-4.1.0/docs/userguide/genuserguide.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/graph_charts.py` & `reportlab-4.1.0/docs/userguide/graph_charts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/graph_concepts.py` & `reportlab-4.1.0/docs/userguide/graph_concepts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/graph_shapes.py` & `reportlab-4.1.0/docs/userguide/graph_shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/docs/userguide/graph_widgets.py` & `reportlab-4.1.0/docs/userguide/graph_widgets.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/setup.py` & `reportlab-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #Copyright ReportLab Europe Ltd. 2000-2023
 #see LICENSE for license details
-__version__='4.0.4'
+__version__='4.1.0'
 import os, sys, glob, shutil, re, sysconfig, traceback, io, subprocess
 from urllib.parse import quote as urlquote
 platform = sys.platform
 pjoin = os.path.join
 abspath = os.path.abspath
 isfile = os.path.isfile
 isdir = os.path.isdir
```

### Comparing `reportlab-4.0.9/src/reportlab/__init__.py` & `reportlab-4.1.0/src/reportlab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #Copyright ReportLab Europe Ltd. 2000-2023
 #see license.txt for license details
 __doc__="""The Reportlab PDF generation library."""
-Version = "4.0.9"
+Version = "4.1.0"
 __version__=Version
-__date__='20240108'
+__date__='20240208'
 
 import sys, os
 
 __min_python_version__ = (3,7)
 if sys.version_info< __min_python_version__:
     raise ImportError("""reportlab requires %s.%s+; other versions are unsupported.
 If you want to try with other python versions edit line 10 of reportlab/__init__
```

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGarden-copying-gpl.txt` & `reportlab-4.1.0/src/reportlab/fonts/DarkGarden-copying-gpl.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGarden-copying.txt` & `reportlab-4.1.0/src/reportlab/fonts/DarkGarden-copying.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGarden-readme.txt` & `reportlab-4.1.0/src/reportlab/fonts/DarkGarden-readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGarden.sfd` & `reportlab-4.1.0/src/reportlab/fonts/DarkGarden.sfd`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGardenMK.afm` & `reportlab-4.1.0/src/reportlab/fonts/DarkGardenMK.afm`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/DarkGardenMK.pfb` & `reportlab-4.1.0/src/reportlab/fonts/DarkGardenMK.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/Vera.ttf` & `reportlab-4.1.0/src/reportlab/fonts/Vera.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/VeraBI.ttf` & `reportlab-4.1.0/src/reportlab/fonts/VeraBI.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/VeraBd.ttf` & `reportlab-4.1.0/src/reportlab/fonts/VeraBd.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/VeraIt.ttf` & `reportlab-4.1.0/src/reportlab/fonts/VeraIt.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_a______.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_a______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_ab_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_ab_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_abi____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_abi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_ai_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_ai_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_eb_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_eb_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_ebi____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_ebi____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_ei_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_ei_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/_er_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/_er_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/bitstream-vera-license.txt` & `reportlab-4.1.0/src/reportlab/fonts/bitstream-vera-license.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/callig15.afm` & `reportlab-4.1.0/src/reportlab/fonts/callig15.afm`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/callig15.pfb` & `reportlab-4.1.0/src/reportlab/fonts/callig15.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/cob_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/cob_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/cobo____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/cobo____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/com_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/com_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/coo_____.pfb` & `reportlab-4.1.0/src/reportlab/fonts/coo_____.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/sy______.pfb` & `reportlab-4.1.0/src/reportlab/fonts/sy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/zd______.pfb` & `reportlab-4.1.0/src/reportlab/fonts/zd______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/zx______.pfb` & `reportlab-4.1.0/src/reportlab/fonts/zx______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/fonts/zy______.pfb` & `reportlab-4.1.0/src/reportlab/fonts/zy______.pfb`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/README` & `reportlab-4.1.0/src/reportlab/graphics/barcode/README`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/TODO` & `reportlab-4.1.0/src/reportlab/graphics/barcode/TODO`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/__init__.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/__init__.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/code128.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/code128.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/code39.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/code39.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/code93.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/code93.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/common.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,23 +99,29 @@
         if self.quiet:
             w += self.lquiet + self.rquiet
 
 
         self._height = self.barHeight
         self._width = w
 
+    @property
     def width(self):
         self._calculate()
         return self._width
-    width = property(width)
+    @width.setter
+    def width(self,v):
+        pass
 
+    @property
     def height(self):
         self._calculate()
         return self._height
-    height = property(height)
+    @height.setter
+    def height(self,v):
+        pass
 
     def draw(self):
         self._calculate()
         barWidth = self.barWidth
         wx = barWidth * self.ratio
 
         left = self.quiet and self.lquiet or 0
```

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/dmtx.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/dmtx.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/eanbc.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/eanbc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/ecc200datamatrix.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/ecc200datamatrix.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/fourstate.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/fourstate.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/lto.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/lto.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/qr.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/qr.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/qrencoder.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/qrencoder.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/test.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/test.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/usps.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/usps.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/usps4s.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/usps4s.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,23 +303,31 @@
         x = self.tops['F'][1] - self.bottoms['F'][1]
         value = self.__dict__['_barHeight'] = 72*min(max(value/72.0,n),x)
         self.heightSize = (value - n)/(x-n)
 
     widthScale = property(lambda self: min(1,max(0,self.widthSize)))
     heightScale = property(lambda self: min(1,max(0,self.heightSize)))
 
+    @property
     def width(self):
         self.computeSize()
         return self._width
-    width = property(width)
 
+    @property
     def height(self):
         self.computeSize()
         return self._height
-    height = property(height)
+
+    #we ignore attempts to set the dimensions
+    @width.setter
+    def width(self,v):
+        pass
+    @height.setter
+    def height(self,v):
+        pass
 
     def computeSize(self):
         if not getattr(self,'_sized',None):
             ws = self.widthScale
             hs = self.heightScale
             barHeight = self.barHeight
             barWidth = self.barWidth
```

### Comparing `reportlab-4.0.9/src/reportlab/graphics/barcode/widgets.py` & `reportlab-4.1.0/src/reportlab/graphics/barcode/widgets.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/areas.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/areas.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/axes.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/axes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/barcharts.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/barcharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/dotbox.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/dotbox.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/doughnut.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/doughnut.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/legends.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/legends.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/linecharts.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/linecharts.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,15 @@
                         if getattr(lines[rowNo%styleCount],'inFill',False)]
                 ):
             inFillY = self.categoryAxis._y
             inFillX0 = self.valueAxis._x
             inFillX1 = inFillX0 + self.categoryAxis._length
             inFillG = getattr(self,'_inFillG',g)
         yzero = self._yzero
+        bypos = None
 
         # Iterate over data rows.
         for rowNo, row in enumerate(reversed(P) if self.reversePlotOrder else P):
             styleIdx = rowNo % styleCount
             rowStyle = lines[styleIdx]
             strokeColor = rowStyle.strokeColor
             fillColor = getattr(rowStyle,'fillColor',strokeColor)
@@ -335,21 +336,26 @@
             elif hasattr(lines, 'strokeWidth'):
                 strokeWidth = lines.strokeWidth
             else:
                 strokeWidth = None
 
             # Iterate over data columns.
             if lineStyle=='bar':
+                if bypos is None:
+                    x = self.valueAxis
+                    bypos = max(x._y,yzero)
+                    byneg = min(x._y+x._length,yzero)
                 barWidth = getattr(rowStyle,'barWidth',Percentage(50))
                 if isinstance(barWidth,Percentage):
                     hbw = self._hngs*barWidth*0.01
                 else:
                     hbw = barWidth*0.5
                 for x, y in row:
-                    g.add(Rect(x-hbw,min(y,yzero),2*hbw,abs(y-yzero),strokeWidth=strokeWidth,strokeColor=strokeColor,fillColor=fillColor))
+                    _y0 = byneg if y<yzero else bypos
+                    g.add(Rect(x-hbw,_y0,2*hbw,y-_y0,strokeWidth=strokeWidth,strokeColor=strokeColor,fillColor=fillColor))
             elif self.joinedLines or lineStyle=='joinedLine':
                 points = flatten(row)
                 if inFill or isinstance(row,FillPairedData):
                     filler = getattr(rowStyle, 'filler', None)
                     if isinstance(row,FillPairedData):
                         fpoints = points + flatten(reversed(P[row.other]))
                     else:
```

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/lineplots.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/lineplots.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         strokeColor = AttrMapValue(isColorOrNone, desc='Color of a line.'),
         strokeDashArray = AttrMapValue(isListOfNumbersOrNone, desc='Dash array of a line.'),
         fillColor = AttrMapValue(isColorOrNone, desc='Color of infill defaults to the strokeColor.'),
         symbol = AttrMapValue(None, desc='Widget placed at data points.',advancedUsage=1),
         shader = AttrMapValue(None, desc='Shader Class.',advancedUsage=1),
         filler = AttrMapValue(None, desc='Filler Class.',advancedUsage=1),
         name = AttrMapValue(isStringOrNone, desc='Name of the line.'),
+        lineStyle = AttrMapValue(NoneOr(OneOf('line','joinedLine','bar')), desc="What kind of plot this line is",advancedUsage=1),
+        barWidth = AttrMapValue(isNumberOrNone,desc="Percentage of available width to be used for a bar",advancedUsage=1),
         inFill = AttrMapValue(isBoolean, desc='If true flood fill to x axis',advancedUsage=1),
         )
 
 class InFillValue(int):
     def __new__(cls,v,yValue=None):
         self = int.__new__(cls,v)
         self.yValue = yValue
@@ -87,15 +89,15 @@
     """
     _attrMap = AttrMap(BASE=PlotArea,
         reversePlotOrder = AttrMapValue(isBoolean, desc='If true reverse plot order.',advancedUsage=1),
         lineLabelNudge = AttrMapValue(isNumber, desc='Distance between a data point and its label.',advancedUsage=1),
         lineLabels = AttrMapValue(None, desc='Handle to the list of data point labels.'),
         lineLabelFormat = AttrMapValue(None, desc='Formatting string or function used for data point labels.'),
         lineLabelArray = AttrMapValue(None, desc='explicit array of line label values, must match size of data if present.'),
-        joinedLines = AttrMapValue(isNumber, desc='Display data points joined with lines if true.'),
+        #joinedLines = AttrMapValue(isNumber, desc='Display data points joined with lines if true.'),
         strokeColor = AttrMapValue(isColorOrNone, desc='Color used for background border of plot area.'),
         fillColor = AttrMapValue(isColorOrNone, desc='Color used for background interior of plot area.'),
         lines = AttrMapValue(None, desc='Handle of the lines.'),
         xValueAxis = AttrMapValue(None, desc='Handle of the x axis.'),
         yValueAxis = AttrMapValue(None, desc='Handle of the y axis.'),
         data = AttrMapValue(None, desc='Data to be plotted, list of (lists of) x/y tuples.'),
         annotations = AttrMapValue(None, desc='list of callables, will be called with self, xscale, yscale.',advancedUsage=1),
@@ -114,14 +116,15 @@
         self.data = [
             ((1,1), (2,2), (2.5,1), (3,3), (4,5)),
             ((1,2), (2,3), (2.5,2), (3,4), (4,6))
             ]
 
         self.lines = TypedPropertyCollection(LinePlotProperties)
         self.lines.strokeWidth = 1
+        self.joinedLines = 1 # Connect items with straight lines.
         self.lines[0].strokeColor = colors.red
         self.lines[1].strokeColor = colors.blue
 
         self.lineLabels = TypedPropertyCollection(Label)
         self.lineLabelFormat = None
         self.lineLabelArray = None
 
@@ -131,23 +134,28 @@
         # points inside if bar value < 0.  This is different
         # to label dx/dy which are not dependent on the
         # sign of the data.
         self.lineLabelNudge = 10
         # if you have multiple series, by default they butt
         # together.
 
-        # New line chart attributes.
-        self.joinedLines = 1 # Connect items with straight lines.
-
         #private attributes
         self._inFill = None
         self.annotations = []
         self.behindAxes = 0
         self.gridFirst = 0
 
+    @property
+    def joinedLines(self):
+        return self.lines.lineStyle=='joinedLine'
+
+    @joinedLines.setter
+    def joinedLines(self,v):
+        self.lines.lineStyle = 'joinedLine' if v else 'line'
+
     def demo(self):
         """Shows basic use of a line chart."""
 
         drawing = Drawing(400, 200)
 
         data = [
             ((1,1), (2,2), (2.5,1), (3,3), (4,5)),
@@ -288,36 +296,65 @@
             if inFillY is None:
                 inFillY = xA._y
             else:
                 inFillY = yA.scale(inFillY)
             inFillX0 = yA._x
             inFillX1 = inFillX0 + xA._length
             inFillG = getattr(self,'_inFillG',g)
+        bw = None
         lG = getattr(self,'_lineG',g)
         # Iterate over data rows.
         R = range(len(P))
         if self.reversePlotOrder: R = reversed(R)
         for rowNo in R:
             row = P[rowNo]
             styleRowNo = rowNo % styleCount
             rowStyle = lines[styleRowNo]
             strokeColor = getattr(rowStyle,'strokeColor',None)
+            strokeWidth = getattr(rowStyle,'strokeWidth',None)
             fillColor = getattr(rowStyle, 'fillColor', strokeColor)
             inFill = getattr(rowStyle,'inFill',_inFill)
             dash = getattr(rowStyle, 'strokeDashArray', None)
+            lineStyle = getattr(rowStyle,'lineStyle',None)
 
             if hasattr(rowStyle, 'strokeWidth'):
                 width = rowStyle.strokeWidth
             elif hasattr(lines, 'strokeWidth'):
                 width = lines.strokeWidth
             else:
                 width = None
 
             # Iterate over data columns.
-            if self.joinedLines:
+            if lineStyle=='bar':
+                if bw is None:
+                    x = max(map(len,P)) - 1 #the number of gaps
+                    bw = (self.width/x - 1) if x>0 else self.width
+                    barWidth = getattr(rowStyle,'barWidth',Percentage(50))
+                    x = self.yValueAxis
+                    y0 = x.scale(0)
+                    bypos = max(x._y,y0)
+                    byneg = min(x._y+x._length,y0)
+                    xmin = self.xValueAxis._x
+                    xmax = xmin + self.xValueAxis._length
+                    if isinstance(barWidth,Percentage):
+                        bw *= barWidth*0.005
+                    else:
+                        bw = barWidth*0.5
+                for x, y in row:
+                    w = bw
+                    #print(f'{x=} {y=} {y0=} {byneg=} {bypos=}')
+                    _y0 = byneg if y<y0 else bypos
+                    x -= w/2
+                    if x<xmin:
+                        w -= xmin - x
+                        x = xmin
+                    elif x+w > xmax:
+                        w -= xmax - x
+                    g.add(Rect(x,_y0,w,y-_y0,strokeWidth=strokeWidth,strokeColor=strokeColor,fillColor=fillColor))
+            elif lineStyle=='joinedLine':
                 points = flatten(row)
                 if inFill or isinstance(row,FillPairedData):
                     filler = getattr(rowStyle, 'filler', None)
                     if isinstance(row,FillPairedData):
                         fpoints = points + flatten(reversed(P[row.other]))
                     else:
                         fpoints = [inFillX0,inFillY] + points + [inFillX1,inFillY]
```

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/markers.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/piecharts.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/piecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/slidebox.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/spider.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/spider.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/textlabels.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/utils.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/charts/utils3d.py` & `reportlab-4.1.0/src/reportlab/graphics/charts/utils3d.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/renderPDF.py` & `reportlab-4.1.0/src/reportlab/graphics/renderPDF.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/renderPM.py` & `reportlab-4.1.0/src/reportlab/graphics/renderPM.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/renderPS.py` & `reportlab-4.1.0/src/reportlab/graphics/renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/renderSVG.py` & `reportlab-4.1.0/src/reportlab/graphics/renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/renderbase.py` & `reportlab-4.1.0/src/reportlab/graphics/renderbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/bubble.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/bubble.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/clustered_bar.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/clustered_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/clustered_column.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/clustered_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/excelcolors.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/excelcolors.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/exploded_pie.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/exploded_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/filled_radar.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/filled_radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/line_chart.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/line_chart.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/linechart_with_markers.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/linechart_with_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/radar.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/radar.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/runall.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/runall.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/scatter.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/scatter.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/scatter_lines.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/scatter_lines.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/scatter_lines_markers.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/scatter_lines_markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/simple_pie.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/simple_pie.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/stacked_bar.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/samples/stacked_column.py` & `reportlab-4.1.0/src/reportlab/graphics/samples/stacked_column.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/shapes.py` & `reportlab-4.1.0/src/reportlab/graphics/shapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/svgpath.py` & `reportlab-4.1.0/src/reportlab/graphics/svgpath.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/testdrawings.py` & `reportlab-4.1.0/src/reportlab/graphics/testdrawings.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/testshapes.py` & `reportlab-4.1.0/src/reportlab/graphics/testshapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/transform.py` & `reportlab-4.1.0/src/reportlab/graphics/transform.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/utils.py` & `reportlab-4.1.0/src/reportlab/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgetbase.py` & `reportlab-4.1.0/src/reportlab/graphics/widgetbase.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/adjustableArrow.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/adjustableArrow.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/eventcal.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/eventcal.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/flags.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/flags.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/grids.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/markers.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/markers.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/signsandsymbols.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/signsandsymbols.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/graphics/widgets/table.py` & `reportlab-4.1.0/src/reportlab/graphics/widgets/table.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/PyFontify.py` & `reportlab-4.1.0/src/reportlab/lib/PyFontify.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/abag.py` & `reportlab-4.1.0/src/reportlab/lib/abag.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/arciv.py` & `reportlab-4.1.0/src/reportlab/lib/arciv.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/attrmap.py` & `reportlab-4.1.0/src/reportlab/lib/attrmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,34 +95,48 @@
         c = AttrMap(BASE=self,UNWANTED=UNWANTED)
         c.update(kw)
         return c
 
 def validateSetattr(obj,name,value):
     '''validate setattr(obj,name,value)'''
     if rl_config.shapeChecking:
-        map = obj._attrMap
-        if map and name[0]!= '_':
+        aMap = obj._attrMap
+        if aMap and name[0]!= '_':
             #we always allow the inherited values; they cannot
             #be checked until draw time.
             if isinstance(value, DerivedValue):
                 #let it through
                 pass
-            else:            
+            elif name in aMap:
+                validate = aMap[name].validate
                 try:
-                    validate = map[name].validate
-                    if not validate(value):
-                        raise AttributeError("Illegal assignment of '%s' to '%s' in class %s" % (value, name, obj.__class__.__name__))
-                except KeyError:
+                    r = validate(value)
+                except Exception as e:
+                    raise e.__class__(f"{obj.__class__.__name__}.{name} {validate}({value!r})") from e
+                else:
+                    if not r:
+                        raise AttributeError(f"Illegal assignment of {value!r} to {name} in class {obj.__class__.__name__}")
+            else:
+                prop = getattr(obj.__class__,name,None)
+                if isinstance(prop,property):
+                    fset = getattr(prop,'fset',None)
+                    if fset:
+                        fset(obj,value)
+                        return
+                    else:
+                        raise AttributeError(f"{obj.__class__.__name__}.{name} has no setter")
+                else:
                     raise AttributeError("Illegal attribute '%s' in class %s" % (name, obj.__class__.__name__))
     prop = getattr(obj.__class__,name,None)
     if isinstance(prop,property):
-        try:
-            prop.__set__(obj,value)
-        except AttributeError:
-            pass
+        fset = getattr(prop,'fset',None)
+        if fset:
+            fset(obj,value)
+        else:
+            raise AttributeError(f"{obj.__class__.__name__}.{name} has no setter")
     elif name=='__dict__':
         obj.__dict__.clear()
         obj.__dict__.update(value)
     else:
         obj.__dict__[name] = value
 
 def _privateAttrMap(obj,ret=0):
```

### Comparing `reportlab-4.0.9/src/reportlab/lib/boxstuff.py` & `reportlab-4.1.0/src/reportlab/lib/boxstuff.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/codecharts.py` & `reportlab-4.1.0/src/reportlab/lib/codecharts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/colors.py` & `reportlab-4.1.0/src/reportlab/lib/colors.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/corp.py` & `reportlab-4.1.0/src/reportlab/lib/corp.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/extformat.py` & `reportlab-4.1.0/src/reportlab/lib/extformat.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/fontfinder.py` & `reportlab-4.1.0/src/reportlab/lib/fontfinder.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/fonts.py` & `reportlab-4.1.0/src/reportlab/lib/fonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/formatters.py` & `reportlab-4.1.0/src/reportlab/lib/formatters.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/geomutils.py` & `reportlab-4.1.0/src/reportlab/lib/geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/logger.py` & `reportlab-4.1.0/src/reportlab/lib/logger.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/normalDate.py` & `reportlab-4.1.0/src/reportlab/lib/normalDate.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/pagesizes.py` & `reportlab-4.1.0/src/reportlab/lib/pagesizes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/pdfencrypt.py` & `reportlab-4.1.0/src/reportlab/lib/pdfencrypt.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/pygments2xpre.py` & `reportlab-4.1.0/src/reportlab/lib/pygments2xpre.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/randomtext.py` & `reportlab-4.1.0/src/reportlab/lib/randomtext.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/rl_accel.py` & `reportlab-4.1.0/src/reportlab/lib/rl_accel.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/rl_safe_eval.py` & `reportlab-4.1.0/src/reportlab/lib/rl_safe_eval.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/rltempfile.py` & `reportlab-4.1.0/src/reportlab/lib/rltempfile.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/rparsexml.py` & `reportlab-4.1.0/src/reportlab/lib/rparsexml.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/sequencer.py` & `reportlab-4.1.0/src/reportlab/lib/sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/styles.py` & `reportlab-4.1.0/src/reportlab/lib/styles.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/testutils.py` & `reportlab-4.1.0/src/reportlab/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/textsplit.py` & `reportlab-4.1.0/src/reportlab/lib/textsplit.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/units.py` & `reportlab-4.1.0/src/reportlab/lib/units.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/utils.py` & `reportlab-4.1.0/src/reportlab/lib/utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/validators.py` & `reportlab-4.1.0/src/reportlab/lib/validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/lib/yaml.py` & `reportlab-4.1.0/src/reportlab/lib/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_can_cmap_data.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_can_cmap_data.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_cidfontdata.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_cidfontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_macexpert.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_macexpert.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_macroman.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_macroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_standard.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_symbol.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_winansi.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_winansi.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_enc_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courier.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courier.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courierbold.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courierbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courierboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_courieroblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helvetica.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helvetica.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticabold.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticaboldoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_helveticaoblique.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_symbol.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_symbol.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesbold.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesbold.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesbolditalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesitalic.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_timesroman.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_timesroman.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_fontdata_widths_zapfdingbats.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/_glyphlist.py` & `reportlab-4.1.0/src/reportlab/pdfbase/_glyphlist.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/acroform.py` & `reportlab-4.1.0/src/reportlab/pdfbase/acroform.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/cidfonts.py` & `reportlab-4.1.0/src/reportlab/pdfbase/cidfonts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/pdfdoc.py` & `reportlab-4.1.0/src/reportlab/pdfbase/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/pdfform.py` & `reportlab-4.1.0/src/reportlab/pdfbase/pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/pdfmetrics.py` & `reportlab-4.1.0/src/reportlab/pdfbase/pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/pdfpattern.py` & `reportlab-4.1.0/src/reportlab/pdfbase/pdfpattern.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/pdfutils.py` & `reportlab-4.1.0/src/reportlab/pdfbase/pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/rl_codecs.py` & `reportlab-4.1.0/src/reportlab/pdfbase/rl_codecs.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfbase/ttfonts.py` & `reportlab-4.1.0/src/reportlab/pdfbase/ttfonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1156,20 +1156,27 @@
                 asciiReadable = rl_config.ttfAsciiReadable
 
             if asciiReadable:
                 # Let's add the first 128 unicodes to the 0th subset, so ' '
                 # always has code 32 (for word spacing to work) and the ASCII
                 # output is readable
                 #simple asciiReadable setup
-                subset0 = list(range(128))
-                for n in subset0:
-                    A[n] = n
-                self.subsets = [subset0]
-                #self.nextCode = 1  #if doing fillin of [1-31]
-                self.nextCode = 128
+                subset0 = list(range(32,128))   #assume we have all of ASCII
+                charToGlyph = getattr(face,'charToGlyph',None)
+                if charToGlyph:
+                    for n in subset0:
+                        if n in charToGlyph:
+                            A[n] = n
+                else:
+                    for n in subset0:
+                        A[n] = n
+                A[0] = 0
+                self.subsets = [32*[0] + subset0]
+                self.nextCode = 1   #if doing fillin of [1-31]
+                #self.nextCode = 128 #if not doing fillin
             else:
                 self.subsets = [[0]+[32]*32]
                 A[0] = 0
                 self.nextCode = 1
                 A[32] = 32
 
     _multiByte = 1      # We want our own stringwidth
@@ -1209,27 +1216,30 @@
         """Splits text into a number of chunks, each of which belongs to a
         single subset.  Returns a list of tuples (subset, string).  Use subset
         numbers with getSubsetInternalName.  Doc is needed for distinguishing
         subsets when building different documents at the same time."""
         asciiReadable = self._asciiReadable
         try: state = self.state[doc]
         except KeyError: state = self.state[doc] = TTFont.State(asciiReadable,self)
-        #_31skip = 31 if asciiReadable and state.nextCode<32 else -256
+        _31skip = 31 if asciiReadable and state.nextCode<32 else -256
         curSet = -1
         cur = []
         results = []
         if not isUnicode(text):
             text = text.decode('utf-8')     # encoding defaults to utf-8
+        charToGlyph = self.face.charToGlyph
         assignments = state.assignments
         subsets = state.subsets
         #reserveTTFNotdef = rl_config.reserveTTFNotdef we ignore this now
         for code in map(ord,text):
             if code==0xa0: code = 32    #map nbsp into space
             if code in assignments:
                 n = assignments[code]
+            elif code not in charToGlyph:
+                n = 0
             else:
                 if state.frozen:
                     raise pdfdoc.PDFError("Font %s is already frozen, cannot add new character U+%04X" % (self.fontName, code))
                 n = state.nextCode
                 if n&0xFF==32:
                     # make code 32 always be a space character
                     if n!=32: subsets[n >> 8].append(32)
@@ -1238,18 +1248,18 @@
                 if n>32:
                     if not(n&0xFF):
                         subsets.append([0]) #force code 0 in as notdef
                         state.nextCode += 1
                         n = state.nextCode
                     subsets[n >> 8].append(code)
                 else:
-                    #if n==_31skip:
-                    #   #we heve filled in first part of subsets[0] skip past subset[32:127]
-                    #   #this code will be executed once if asciiReadable
-                    #   state.nextCode = 127
+                    if n==_31skip:
+                        #we heve filled in first part of subsets[0] skip past subset[32:127]
+                        #this code will be executed once if asciiReadable
+                        state.nextCode = 127
                     subsets[0][n] = code
                 state.nextCode += 1
                 assignments[code] = n
                 #subsets[n>>8].append(code)
             if (n >> 8) != curSet:
                 if cur:
                     results.append((curSet,bytes(cur)))
```

### Comparing `reportlab-4.0.9/src/reportlab/pdfgen/canvas.py` & `reportlab-4.1.0/src/reportlab/pdfgen/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 #see license.txt for license details
 __version__='3.3.0'
 __doc__="""
 The Canvas object is the primary interface for creating PDF files. See
 doc/reportlab-userguide.pdf for copious examples.
 """
 
-__all__ = ['Canvas']
+__all__ = [
+        'Canvas',
+        'ShowBoundaryValue',
+        ]
 ENABLE_TRACKING = 1 # turn this off to do profile testing w/o tracking
 
 import re
 import hashlib
 from string import digits
 from math import sin, cos, tan, pi
 from reportlab import rl_config
@@ -205,14 +208,23 @@
 def _gradientExtendStr(extend):
     if isinstance(extend,(list,tuple)):
         if len(extend)!=2:
             raise ValueError('wrong length for extend argument' % extend)
         return "[%s %s]" % ['true' if _ else 'false' for _ in extend]
     return "[true true]" if extend else "[false false]"
 
+class ShowBoundaryValue:
+    def __init__(self,color=(0,0,0),width=0.1,dashArray=None):
+        self.color = color
+        self.width = width
+        self.dashArray = dashArray
+
+    def __bool__(self):
+        return self.color is not None and self.width>=0
+
 class Canvas(_PDFColorSetter):
     """This class is the programmer's interface to the PDF file format.  Methods
     are (or will be) provided here to do just about everything PDF can do.
 
     The underlying model to the canvas concept is that of a graphics state machine
     that at any given point in time has a current font, fill color (for figure
     interiors), stroke color (for figure borders), line width and geometric transform, among
@@ -1973,16 +1985,31 @@
         try:
             return self.AcroForm
         except AttributeError:
             from reportlab.pdfbase.acroform import AcroForm
             self._doc._catalog.AcroForm = self.AcroForm = AcroForm(self)
             return self.AcroForm
 
-    @property
-    def drawBoundary(self):
-        if not hasattr(self,'_drawBoundary'):
-            from reportlab.platypus import Frame
-            self._drawBoundary = lambda sb,x,y,w,h: Frame._drawBoundary(self,sb,x,y,w,h)
-        return self._drawBoundary
+    def drawBoundary(self,sb,x1,y1,width,height):
+        "draw a boundary as a rectangle (primarily for debugging)."
+        ss = isinstance(sb,(str,tuple,list)) or isinstance(sb,Color)
+        w = -1
+        da = None
+        if ss:
+            c = toColor(sb,-1)
+            ss = c != -1
+        elif isinstance(sb,ShowBoundaryValue) and sb:
+            c = toColor(sb.color,-1)
+            ss = c != -1
+            if ss:
+                w = sb.width
+                da = sb.dashArray
+        if ss:
+            self.saveState()
+            self.setStrokeColor(c)
+            if w>=0: self.setLineWidth(w)
+            if da: self.setDash(da)
+        self.rect(x1,y1,width,height)
+        if ss: self.restoreState()
 
 if __name__ == '__main__':
     print('For test scripts, look in tests')
```

### Comparing `reportlab-4.0.9/src/reportlab/pdfgen/pathobject.py` & `reportlab-4.1.0/src/reportlab/pdfgen/pathobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfgen/pdfgeom.py` & `reportlab-4.1.0/src/reportlab/pdfgen/pdfgeom.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfgen/pdfimages.py` & `reportlab-4.1.0/src/reportlab/pdfgen/pdfimages.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/pdfgen/textobject.py` & `reportlab-4.1.0/src/reportlab/pdfgen/textobject.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/doctemplate.py` & `reportlab-4.1.0/src/reportlab/platypus/doctemplate.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/figures.py` & `reportlab-4.1.0/src/reportlab/platypus/figures.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/flowables.py` & `reportlab-4.1.0/src/reportlab/platypus/flowables.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 import os
 from copy import deepcopy, copy
 from reportlab.lib.colors import gray, lightgrey
 from reportlab.lib.rl_accel import fp_str
 from reportlab.lib.enums import TA_LEFT, TA_CENTER, TA_RIGHT
 from reportlab.lib.styles import _baseFontName
-from reportlab.lib.utils import strTypes, rl_safe_exec
+from reportlab.lib.utils import strTypes, rl_safe_exec, annotateException
 from reportlab.lib.abag import ABag
 from reportlab.pdfbase import pdfutils
 from reportlab.pdfbase.pdfmetrics import stringWidth
 from reportlab.rl_config import _FUZZ, overlapAttachedSpace, ignoreContainerActions, listWrapOnFakeWidth
 
 __all__ = '''AnchorFlowable BalancedColumns BulletDrawer CallerMacro CondPageBreak DDIndenter DocAssert
         DocAssign DocExec DocIf DocPara DocWhile FailOnDraw FailOnWrap Flowable FrameBG FrameSplitter
@@ -687,18 +687,16 @@
     splitAtTop = False
 
     def __init__(self,flowables,maxHeight=None):
         if not hasattr(KeepTogether,'NullActionFlowable'):
             #cache these on the class
             from reportlab.platypus.doctemplate import NullActionFlowable
             from reportlab.platypus.doctemplate import FrameBreak
-            from reportlab.lib.utils import annotateException
             KeepTogether.NullActionFlowable = NullActionFlowable
             KeepTogether.FrameBreak = FrameBreak
-            self.annotateException = annotateException
 
         if not flowables:
             flowables = [self.NullActionFlowable()]
         self._content = _flowableSublist(flowables)
         self._maxHeight = maxHeight
 
     def __repr__(self):
@@ -709,15 +707,15 @@
         return "%s(%s,maxHeight=%s)" % (self.__class__.__name__,L,self._maxHeight)
 
     def wrap(self, aW, aH):
         dims = []
         try:
             W,H = _listWrapOn(self._content,aW,self.canv,dims=dims)
         except:
-            self.annotateException('\nraised by class %s(%s)@0x%8.8x wrap\n' % (self.__class__.__name__,self.__class__.__module__,id(self)))
+            annotateException('\nraised by class %s(%s)@0x%8.8x wrap\n' % (self.__class__.__name__,self.__class__.__module__,id(self)))
         self._H = H
         self._H0 = dims and dims[0][1] or 0
         self._wrapInfo = aW,aH
         return W, 0xffffff  # force a split
 
     def split(self, aW, aH):
         if getattr(self,'_wrapInfo',None)!=(aW,aH): self.wrap(aW,aH)
```

### Comparing `reportlab-4.0.9/src/reportlab/platypus/frames.py` & `reportlab-4.1.0/src/reportlab/platypus/frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,35 +4,24 @@
 
 __version__='3.5.14'
 
 __doc__="""A frame is a container for content on a page.
 """
 
 __all__ = (
-            'ShowBoundaryValue',
             'Frame',
             )
 
 import logging
 logger = logging.getLogger('reportlab.platypus')
 
 _geomAttr=('x1', 'y1', 'width', 'height', 'leftPadding', 'bottomPadding', 'rightPadding', 'topPadding')
 from reportlab import rl_config
 _FUZZ=rl_config._FUZZ
 
-class ShowBoundaryValue:
-    def __init__(self,color=(0,0,0),width=0.1,dashArray=None):
-        self.color = color
-        self.width = width
-        self.dashArray = dashArray
-
-    def __bool__(self):
-        return self.color is not None and self.width>=0
-
-
 class Frame:
     '''
     A Frame is a piece of space in a document that is filled by the
     "flowables" in the story.  For example in a book like document most
     pages have the text paragraphs in one or two frames.  For generality
     a page might have several frames (for example for 3 column text or
     for text that wraps around a graphic).
@@ -247,41 +236,16 @@
         finally:
             #sometimes canv/_frame aren't still on the flowable
             for a in ('canv', '_frame'):
                 if hasattr(flowable,a):
                     delattr(flowable,a)
         return r
 
-
-    @staticmethod
-    def _drawBoundary(canv,sb,x1,y1,width,height):
-        "draw the frame boundary as a rectangle (primarily for debugging)."
-        from reportlab.lib.colors import Color, toColor
-        ss = isinstance(sb,(str,tuple,list)) or isinstance(sb,Color)
-        w = -1
-        da = None
-        if ss:
-            c = toColor(sb,-1)
-            ss = c != -1
-        elif isinstance(sb,ShowBoundaryValue) and sb:
-            c = toColor(sb.color,-1)
-            ss = c != -1
-            if ss:
-                w = sb.width
-                da = sb.dashArray
-        if ss:
-            canv.saveState()
-            canv.setStrokeColor(c)
-            if w>=0: canv.setLineWidth(w)
-            if da: canv.setDash(da)
-        canv.rect(x1,y1,width,height)
-        if ss: canv.restoreState()
-
-    def drawBoundary(self,canv, __boundary__=None):
-        self._drawBoundary(canv,__boundary__ or self.showBoundary, self._x1, self._y1,
+    def drawBoundary(self, canv, __boundary__=None):
+        canv.drawBoundary(__boundary__ or self.showBoundary, self._x1, self._y1,
                                 self._x2 - self._x1, self._y2 - self._y1)
 
     def addFromList(self, drawlist, canv):
         """Consumes objects from the front of the list until the
         frame is full.  If it cannot fit one object, raises
         an exception."""
```

### Comparing `reportlab-4.0.9/src/reportlab/platypus/multicol.py` & `reportlab-4.1.0/src/reportlab/platypus/multicol.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/para.py` & `reportlab-4.1.0/src/reportlab/platypus/para.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/paragraph.py` & `reportlab-4.1.0/src/reportlab/platypus/paragraph.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/paraparser.py` & `reportlab-4.1.0/src/reportlab/platypus/paraparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/tableofcontents.py` & `reportlab-4.1.0/src/reportlab/platypus/tableofcontents.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/tables.py` & `reportlab-4.1.0/src/reportlab/platypus/tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/platypus/xpreformatted.py` & `reportlab-4.1.0/src/reportlab/platypus/xpreformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/rl_config.py` & `reportlab-4.1.0/src/reportlab/rl_config.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab/rl_settings.py` & `reportlab-4.1.0/src/reportlab/rl_settings.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/src/reportlab.egg-info/PKG-INFO` & `reportlab-4.1.0/src/reportlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportlab
-Version: 4.0.9
+Version: 4.1.0
 Summary: The Reportlab Toolkit
 Home-page: https://www.reportlab.com/
 Author: Andy Robinson, Robin Becker, the ReportLab team and the community
 Author-email: reportlab-users@lists2.reportlab.com
 License: BSD license (see license.txt for details), Copyright (c) 2000-2022, ReportLab Inc.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `reportlab-4.0.9/tests/00readme.txt` & `reportlab-4.1.0/tests/00readme.txt`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/_i_am_actually_a_gif.jpg` & `reportlab-4.1.0/tests/_i_am_actually_a_gif.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/_i_am_actually_a_jpeg.gif` & `reportlab-4.1.0/tests/_i_am_actually_a_jpeg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/alpha_test.png` & `reportlab-4.1.0/tests/alpha_test.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Code11.gif` & `reportlab-4.1.0/tests/barcode-out/Code11.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Code128.gif` & `reportlab-4.1.0/tests/barcode-out/Code128.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Code128Auto.gif` & `reportlab-4.1.0/tests/barcode-out/Code128Auto.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/EAN13.gif` & `reportlab-4.1.0/tests/barcode-out/EAN13.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/EAN5.gif` & `reportlab-4.1.0/tests/barcode-out/EAN5.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/EAN8.gif` & `reportlab-4.1.0/tests/barcode-out/EAN8.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/ECC200DataMatrix.gif` & `reportlab-4.1.0/tests/barcode-out/ECC200DataMatrix.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Extended39.gif` & `reportlab-4.1.0/tests/barcode-out/Extended39.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Extended93.gif` & `reportlab-4.1.0/tests/barcode-out/Extended93.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/I2of5.gif` & `reportlab-4.1.0/tests/barcode-out/I2of5.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/ISBN.gif` & `reportlab-4.1.0/tests/barcode-out/ISBN.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/POSTNET.gif` & `reportlab-4.1.0/tests/barcode-out/POSTNET.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/QR.gif` & `reportlab-4.1.0/tests/barcode-out/QR.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/QR_with_comma.gif` & `reportlab-4.1.0/tests/barcode-out/QR_with_comma.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Standard39.gif` & `reportlab-4.1.0/tests/barcode-out/Standard39.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/Standard93.gif` & `reportlab-4.1.0/tests/barcode-out/Standard93.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/UPCA.gif` & `reportlab-4.1.0/tests/barcode-out/UPCA.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/USPS_4State.gif` & `reportlab-4.1.0/tests/barcode-out/USPS_4State.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/test_cbcim.gif` & `reportlab-4.1.0/tests/barcode-out/test_cbcim.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/test_cbcim.png` & `reportlab-4.1.0/tests/barcode-out/test_cbcim.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/barcode-out/test_cbcim.tiff` & `reportlab-4.1.0/tests/barcode-out/test_cbcim.tiff`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0a.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0a.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0a.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0a.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0b.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0b.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample0b.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_axes_sample0b.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample1.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample1c.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,26 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=200,height=100,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(75,75,375,75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(75,75,75,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(150,75,150,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(225,75,225,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(300,75,300,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(375,75,375,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,112.5,70)
-		v0.add(String(-9.44,-10,'Beer',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,187.5,70)
-		v0.add(String(-10.83,-10,'Wine',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,262.5,70)
-		v0.add(String(-10.275,-10,'Meat',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (.866025,.5,-0.5,.866025,337.5,60)
-		v0.add(String(-23.34,-10,'Cannelloni',textAnchor='start',fontName='Times-Bold',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
-		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,90,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(15,91.585,'red',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,70,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(15,71.585,'green',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,50,10,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(15,51.585,'blue',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(75,90,10,10,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(90,91.585,'yellow',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(75,70,10,10,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(90,71.585,'pink',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(75,50,10,10,rx=0,ry=0,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(90,51.585,'black',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(150,90,10,10,rx=0,ry=0,fillColor=Color(1,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(165,91.585,'white',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4a.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,26 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Line
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=200,height=100,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(50,100,350,100,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,100,50,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(143.75,100,143.75,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,100,237.5,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(331.25,100,331.25,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,95)
-		v0.add(String(-5,-10,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,143.75,95)
-		v0.add(String(-5,-10,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,95)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,331.25,95)
-		v0.add(String(-5,-10,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
-		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,85.585,'red',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,65.585,'green',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,45.585,'blue',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,25.585,'yellow',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,85.585,'pink',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,65.585,'black',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,45.585,'white',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(20,88,30,88,strokeColor=Color(1,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,68,30,68,strokeColor=Color(0,.501961,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,48,30,48,strokeColor=Color(0,0,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,28,30,28,strokeColor=Color(1,1,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(80,88,90,88,strokeColor=Color(1,.752941,.796078,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(80,68,90,68,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(80,48,90,48,strokeColor=Color(1,1,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample4b.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1line.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(50,147.6562,350,147.6562,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,147.6562,50,142.6562,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(143.75,147.6562,143.75,142.6562,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,147.6562,237.5,142.6562,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(331.25,147.6562,331.25,142.6562,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,142.6562)
-		v0.add(String(-5,-10,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[68.75,77.08333,106.25,60.41667,143.75,91.66667,181.25,95.83333,218.75,127.0833,256.25,143.75,293.75,89.58333,331.25,58.33333],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
+		v0.add(String(-26.66,-10,'Jan-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
+		v0.add(String(-28.33,-10,'Feb-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
+		v0.add(String(-29.99,-10,'Mar-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
+		v0.add(String(-28.88,-10,'Apr-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
+		v0.add(String(-31.66,-10,'May-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,143.75,142.6562)
-		v0.add(String(-5,-10,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
+		v0.add(String(-27.22,-10,'Jun-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,142.6562)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
+		v0.add(String(-25,-10,'Jul-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,331.25,142.6562)
-		v0.add(String(-5,-10,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
+		v0.add(String(-30.55,-10,'Aug-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,81.25)
+		v0.add(String(-10,-4,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
+		v0.transform = (1,0,0,1,45,112.5)
 		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,143.75)
+		v0.add(String(-10,-4,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,175)
+		v0.add(String(-10,-4,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6a.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample2c.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,26 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=200,height=100,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(50,175,350,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,50,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,175,125,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,175,200,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,175,275,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,175,350,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,87.5,170)
-		v0.add(String(-9.44,-10,'Beer',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,162.5,170)
-		v0.add(String(-10.83,-10,'Wine',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,170)
-		v0.add(String(-10.275,-10,'Meat',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,312.5,170)
-		v0.add(String(-21.945,-10,'Cannelloni',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
-		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(20,80,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(40,81.585,'red',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(20,60,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(40,61.585,'green',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(20,40,10,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(40,41.585,'blue',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(20,20,10,10,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(40,21.585,'yellow',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(80,80,10,10,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(100,81.585,'pink',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(80,60,10,10,rx=0,ry=0,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(100,61.585,'black',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(80,40,10,10,rx=0,ry=0,fillColor=Color(1,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(100,41.585,'white',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6b.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample4a.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Line
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=200,height=100,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,87.5,45)
-		v0.add(String(-9.44,-10,'Beer',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,162.5,45)
-		v0.add(String(-10.83,-10,'Wine',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,45)
-		v0.add(String(-10.275,-10,'Meat',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,312.5,45)
-		v0.add(String(-21.945,-10,'Cannelloni',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
-		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(55.22,85.585,'RED',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(20,85.585,'red',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(55.22,65.585,'GREEN',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(20,65.585,'green',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(55.22,45.585,'BLUE',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(20,45.585,'blue',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(130.22,85.585,'YELLOW',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(95,85.585,'yellow',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(130.22,65.585,'PINK',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(95,65.585,'pink',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(130.22,45.585,'BLACK',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(95,45.585,'black',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(205.22,85.585,'WHITE',textAnchor='end',fontName='Helvetica',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(170,85.585,'white',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(57.22,88,67.22,88,strokeColor=Color(1,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(57.22,68,67.22,68,strokeColor=Color(0,.501961,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(57.22,48,67.22,48,strokeColor=Color(0,0,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(132.22,88,142.22,88,strokeColor=Color(1,1,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(132.22,68,142.22,68,strokeColor=Color(1,.752941,.796078,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(132.22,48,142.22,48,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(207.22,88,217.22,88,strokeColor=Color(1,1,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample6c.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_scleg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Line, String, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Line(50,100,350,100,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,100,50,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,100,125,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,100,200,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,100,275,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,100,350,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,87.5,95)
-		v0.add(String(-9.44,-10,'Beer',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,162.5,95)
-		v0.add(String(-10.83,-10,'Wine',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,95)
-		v0.add(String(-10.275,-10,'Meat',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,312.5,95)
-		v0.add(String(-21.945,-10,'Cannelloni',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,89.0625,45,89.0625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,167.1875,45,167.1875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-10,-4,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-10,-4,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,128.125)
-		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-10,-4,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[41.54329,133.75,100,156.25,158.4567,133.75,168.1995,60.625,100,10,31.8005,60.625,41.54329,133.75],strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[46.41468,130.9375,100,133.75,138.9711,122.5,148.7139,71.875,100,32.5,56.15746,74.6875,46.41468,130.9375],strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,100,190,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,177.9423,145,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,177.9423,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,100,10,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,22.05771,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,100,22.05771,145,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,100,194.5)
+		v0.add(String(-2.22,-4,'a',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,181.8394,147.25)
+		v0.add(String(-2.5,-4,'b',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,181.8394,52.75)
+		v0.add(String(-2.22,-4,'c',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,100,5.5)
+		v0.add(String(-2.5,-4,'d',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,18.1606,52.75)
+		v0.add(String(-2.22,-4,'e',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,18.1606,147.25)
+		v0.add(String(-1.665,-4,'f',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_axes_sample7c.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2line.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,70 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
+		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[68.75,77.08333,106.25,60.41667,143.75,91.66667,181.25,95.83333,218.75,127.0833,256.25,143.75,293.75,89.58333,331.25,58.33333],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[68.75,79.16667,106.25,62.5,143.75,93.75,181.25,97.91667,218.75,129.1667,256.25,145.8333,293.75,91.66667,331.25,60.41667],strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(143.75,50,143.75,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(331.25,50,331.25,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-5,-10,'10',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
+		v0.add(String(-26.66,-10,'Jan-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,143.75,45)
-		v0.add(String(-5,-10,'20',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
+		v0.add(String(-28.33,-10,'Feb-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,237.5,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
+		v0.add(String(-29.99,-10,'Mar-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,331.25,45)
-		v0.add(String(-5,-10,'40',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(237.5,50,237.5,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,50,232.5,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,81.25,232.5,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,112.5,232.5,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,143.75,232.5,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(237.5,175,232.5,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
+		v0.add(String(-28.88,-10,'Apr-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,232.5,65.625)
-		v0.add(String(-18.88,-4,'Beer',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
+		v0.add(String(-31.66,-10,'May-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,232.5,96.875)
-		v0.add(String(-21.66,-4,'Wine',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
+		v0.add(String(-27.22,-10,'Jun-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,232.5,128.125)
-		v0.add(String(-20.55,-4,'Meat',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
+		v0.add(String(-25,-10,'Jul-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,232.5,159.375)
-		v0.add(String(-43.89,-4,'Cannelloni',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
+		v0.add(String(-30.55,-10,'Aug-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,50)
+		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,81.25)
+		v0.add(String(-10,-4,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,112.5)
+		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,143.75)
+		v0.add(String(-10,-4,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,175)
+		v0.add(String(-10,-4,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_SampleH5c4.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_bcleg.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_SampleH5c4(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,60,50,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,150,300,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,80,100,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,170,250,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,100,150,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,190,200,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,120,200,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,210,150,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,81.25)
-		v0.add(String(-20,-4,'Ying',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,143.75)
-		v0.add(String(-21.66,-4,'Yang',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(24.5,10,18,42.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(69.5,10,18,56.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(114.5,10,18,70.83333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(159.5,10,18,85,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(87.5,10,18,14.16667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(132.5,10,18,21.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(177.5,10,18,28.33333,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(65,10,65,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(155,10,155,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,24.16667,15,24.16667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,38.33333,15,38.33333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,52.5,15,52.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,66.66667,15,66.66667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,80.83333,15,80.83333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,10)
+		v0.add(String(-10,-4,'70',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,24.16667)
+		v0.add(String(-10,-4,'80',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,38.33333)
+		v0.add(String(-10,-4,'90',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,52.5)
+		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,66.66667)
+		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,80.83333)
+		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,95)
+		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_SampleH5c4().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0a.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_pcleg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,28 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Wedge, String, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,60.41667,65,41.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,122.9167,100,41.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (.866025,.5,-0.5,.866025,45,81.25)
-		v0.add(String(-20,2,'Ying',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (.866025,.5,-0.5,.866025,45,143.75)
-		v0.add(String(-21.66,2,'Yang',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(50,50,50,50.86957,90,yradius=50,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(50,50,50,-39.13043,50.86957,yradius=50,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(50,50,50,-105.6522,-39.13043,yradius=50,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(50,50,50,-270,-105.6522,yradius=50,annular=False,fillColor=Color(0,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH0c.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3a.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Line
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=200,height=100,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,85.585,'red',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,65.585,'green',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,45.585,'blue',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(40,25.585,'yellow',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,85.585,'pink',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,65.585,'black',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(100,45.585,'white',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(20,88,30,88,strokeColor=Color(1,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[2,1],strokeOpacity=None))
+		self.add(Line(20,68,30,68,strokeColor=Color(0,.501961,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[2,5],strokeOpacity=None))
+		self.add(Line(20,48,30,48,strokeColor=Color(0,0,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[2,2,5,5],strokeOpacity=None))
+		self.add(Line(20,28,30,28,strokeColor=Color(1,1,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[1,2,3,4],strokeOpacity=None))
+		self.add(Line(80,88,90,88,strokeColor=Color(1,.752941,.796078,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[4,2,3,4],strokeOpacity=None))
+		self.add(Line(80,68,90,68,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[1,2,3,4,5,6],strokeOpacity=None))
+		self.add(Line(80,48,90,48,strokeColor=Color(1,1,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[1],strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH1.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_lpleg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, PolyLine, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,51.5625,65,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,67.1875,25,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,82.8125,100,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,98.4375,110,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,114.0625,185,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,129.6875,225,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,145.3125,95,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,160.9375,20,6.25,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,57.8125,70,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,73.4375,30,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,89.0625,105,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,104.6875,115,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,120.3125,190,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,135.9375,230,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,151.5625,100,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,167.1875,25,6.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,65.625,45,65.625,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,96.875,45,96.875,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,128.125,45,128.125,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,159.375,45,159.375,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,57.8125)
-		v0.add(String(-26.66,-4,'Jan-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,73.4375)
-		v0.add(String(-28.33,-4,'Feb-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,89.0625)
-		v0.add(String(-29.99,-4,'Mar-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,104.6875)
-		v0.add(String(-28.88,-4,'Apr-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,120.3125)
-		v0.add(String(-31.66,-4,'May-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,135.9375)
-		v0.add(String(-27.22,-4,'Jun-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,151.5625)
-		v0.add(String(-25,-4,'Jul-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,167.1875)
-		v0.add(String(-30.55,-4,'Aug-99',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,10,50,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(80,10,80,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(140,10,140,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(170,10,170,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,20,5)
+		v0.add(String(-2.5,-10,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,50,5)
+		v0.add(String(-6.25,-10,'1.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,80,5)
+		v0.add(String(-2.5,-10,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,110,5)
+		v0.add(String(-6.25,-10,'2.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,140,5)
+		v0.add(String(-2.5,-10,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,170,5)
+		v0.add(String(-6.25,-10,'3.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,200,5)
+		v0.add(String(-2.5,-10,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,27,15,27,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,44,15,44,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,61,15,61,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,78,15,78,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,10)
+		v0.add(String(-5,-4,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,27)
+		v0.add(String(-5,-4,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,44)
+		v0.add(String(-5,-4,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,61)
+		v0.add(String(-5,-4,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,78)
+		v0.add(String(-5,-4,'5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,95)
+		v0.add(String(-5,-4,'6',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(PolyLine(points=[20,10,80,27,110,10,140,44,200,78],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[20,27,80,44,110,27,140,61,200,95],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[17,10,20,13,23,10,20,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[77,27,80,30,83,27,80,24],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[107,10,110,13,113,10,110,7],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[137,44,140,47,143,44,140,41],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[197,78,200,81,203,78,200,75],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(17.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(77.5,41.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(107.5,24.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(137.5,58.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(197.5,92.5,5,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2a.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_plpleg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,49 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Wedge, PolyLine, String, Polygon
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(230,54,24,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,78,-57,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,102,20,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,126,50,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,150,92,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,62,6,8,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,86,-49,8,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,110,-30,8,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,134,40,8,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,158,68,8,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,225,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,74,225,74,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,98,225,98,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,122,225,122,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,146,225,146,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,170,225,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,62)
-		v0.add(String(-30.688,-3.2,'Q3 2000',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,86)
-		v0.add(String(-44.912,-3.2,'Year to Date',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,110)
-		v0.add(String(-37.352,-3.2,'12 months',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,134)
-		v0.add(String(-39.576,1.6,'Annualised',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0.add(String(-39.576,-8,'3 years',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,158)
-		v0.add(String(-53.368,-3.2,'Since 07.10.99',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		self.add(Line(80,50,380,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(80,50,80,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(130,50,130,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(180,50,180,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(280,50,280,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(330,50,330,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(380,50,380,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,45)
-		v0.add(String(0,-8,'-15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,130,45)
-		v0.add(String(0,-8,'-10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,180,45)
-		v0.add(String(0,-8,'-5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,230,45)
-		v0.add(String(0,-8,'0',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,280,45)
-		v0.add(String(0,-8,'5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,330,45)
-		v0.add(String(0,-8,'10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,380,45)
-		v0.add(String(0,-8,'15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(0,0,160,100,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(62.675,50,49.594,38.57143,90,yradius=49.594,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(62.675,50,49.594,33.42857,38.57143,yradius=49.594,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(62.675,50,49.594,-54,33.42857,yradius=49.594,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(62.675,50,49.594,-270,-54,yradius=49.594,annular=False,fillColor=Color(0,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=0,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=(84.19303,94.68265,85.49468,97.38556,131.35,94),strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=(102.7974,79.15062,105.2244,80.91398,131.35,79.38926),strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=(111.472,41.14465,114.4238,40.60898,131.35,41.07216),strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=(78.00039,2.833299,78.92744,-0.019871,131.35,6),strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,131.35,94)
+		v0.add(Rect(0,-6,26.65,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(0,-4,'abcdef',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,131.35,79.38926)
+		v0.add(Rect(0,-6,5,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(0,-4,'b',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,131.35,41.07216)
+		v0.add(Rect(0,-6,4.44,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(0,-4,'c',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,131.35,6)
+		v0.add(Rect(0,-6,5,12,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(0,-4,'d',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2b.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample4pie.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,52 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Wedge, String, Rect
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(230,53.42857,24,6.857143,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,77.42857,-57,6.857143,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,101.4286,20,6.857143,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,125.4286,50,6.857143,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,149.4286,92,6.857143,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,63.71429,6,6.857143,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,87.71429,-49,6.857143,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,111.7143,-30,6.857143,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,135.7143,40,6.857143,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,159.7143,68,6.857143,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,225,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,74,225,74,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,98,225,98,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,122,225,122,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,146,225,146,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,170,225,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,62)
-		v0.add(String(-30.688,-3.2,'Q3 2000',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,86)
-		v0.add(String(-44.912,-3.2,'Year to Date',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,110)
-		v0.add(String(-37.352,-3.2,'12 months',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,134)
-		v0.add(String(-39.576,1.6,'Annualised',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0.add(String(-39.576,-8,'3 years',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,158)
-		v0.add(String(-53.368,-3.2,'Since 07.10.99',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		self.add(Line(80,50,380,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(80,50,80,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(130,50,130,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(180,50,180,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(280,50,280,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(330,50,330,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(380,50,380,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,45)
-		v0.add(String(0,-8,'-15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,130,45)
-		v0.add(String(0,-8,'-10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,180,45)
-		v0.add(String(0,-8,'-5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,230,45)
-		v0.add(String(0,-8,'0',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,280,45)
-		v0.add(String(0,-8,'5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,330,45)
-		v0.add(String(0,-8,'10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,380,45)
-		v0.add(String(0,-8,'15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		self.add(Wedge(200,100,50,89.55056,90,yradius=50,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,67.07865,89.55056,yradius=50,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,22.13483,67.07865,yradius=50,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(219.9997,99.88234,50,-22.80899,22.13483,yradius=50,annular=False,fillColor=Color(0,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=[2,2],strokeOpacity=None))
+		self.add(Wedge(200,100,50,-67.75281,-22.80899,yradius=50,annular=False,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,-112.6966,-67.75281,yradius=50,annular=False,fillColor=Color(1,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,-157.6404,-112.6966,yradius=50,annular=False,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,-202.5843,-157.6404,yradius=50,annular=False,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,-247.5281,-202.5843,yradius=50,annular=False,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(200,100,50,-270,-247.5281,yradius=50,annular=False,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(200.2353,159.9995,'0',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(212.1523,158.7565,'ä',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(242.7166,142.1342,'b',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(307.4981,99.36757,'c',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
+		self.add(String(242.2179,57.3661,'d',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(199.7647,40.00046,'e',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(157.449,57.69858,'f',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(140.0001,100.1177,'g',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(157.6152,142.468,'h',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(String(188.309,158.85,'i',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(310,140,20,5,rx=0,ry=0,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(295,139.085,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(310,120,20,5,rx=0,ry=0,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(295,119.085,'ä',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(310,100,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(295,99.085,'b',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(350,140,20,5,rx=0,ry=0,fillColor=Color(0,1,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=[2,2],strokeOpacity=None))
+		self.add(String(335,139.085,'c',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(350,120,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(335,119.085,'d',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(350,100,20,5,rx=0,ry=0,fillColor=Color(1,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(335,99.085,'e',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(390,140,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(375,139.085,'f',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(390,120,20,5,rx=0,ry=0,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(375,119.085,'g',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(390,100,20,5,rx=0,ry=0,fillColor=Color(.541176,.168627,.886275,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(375,99.085,'h',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(430,140,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(415,139.085,'i',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH2c.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,103 +2,99 @@
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String, Line
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(230,53.75,24,7.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,77.75,-57,7.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,101.75,20,7.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,125.75,50,7.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,149.75,99.9,7.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,62.75,6,7.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,86.75,-49,7.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,110.75,-30,7.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,134.75,40,7.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(230,158.75,99.9,7.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,264,57.5)
-		v0.add(String(0,-6,'2.40',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,163,81.5)
-		v0.add(String(0,1.2,'-5.70',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,260,105.5)
-		v0.add(String(0,-6,'2.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,290,129.5)
-		v0.add(String(0,-6,'5.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,339.9,153.5)
-		v0.add(String(0,-6,'9.99',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,246,66.5)
-		v0.add(String(0,-6,'0.60',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,171,90.5)
-		v0.add(String(0,1.2,'-4.90',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,190,114.5)
-		v0.add(String(0,1.2,'-3.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,280,138.5)
-		v0.add(String(0,-6,'4.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,339.9,162.5)
-		v0.add(String(0,-6,'9.99',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		self.add(Line(230,50,230,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,225,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,74,225,74,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,98,225,98,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,122,225,122,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,146,225,146,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,170,225,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,62)
-		v0.add(String(-30.688,-3.2,'Q3 2000',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,86)
-		v0.add(String(-44.912,-3.2,'Year to Date',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,110)
-		v0.add(String(-37.352,-3.2,'12 months',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,134)
-		v0.add(String(-39.576,1.6,'Annualised',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0.add(String(-39.576,-8,'3 years',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,158)
-		v0.add(String(-53.368,-3.2,'Since 07.10.99',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		self.add(Line(80,50,380,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(80,50,80,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(130,50,130,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(180,50,180,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(280,50,280,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(330,50,330,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(380,50,380,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,45)
-		v0.add(String(0,-8,'-15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,130,45)
-		v0.add(String(0,-8,'-10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,180,45)
-		v0.add(String(0,-8,'-5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,230,45)
-		v0.add(String(0,-8,'0',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(56.25,50,25,27.08333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(93.75,50,25,10.41667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(131.25,50,25,41.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(168.75,50,25,45.83333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(206.25,50,25,77.08333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(243.75,50,25,93.75,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(281.25,50,25,39.58333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(318.75,50,25,8.333333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,68.75,77.08333)
+		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,106.25,60.41667)
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,143.75,91.66667)
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,181.25,95.83333)
+		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,218.75,127.0833)
+		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,256.25,143.75)
+		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,293.75,89.58333)
+		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,331.25,58.33333)
+		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
+		v0.add(String(-31.74805,-10,'Jän-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
+		v0.add(String(-34.58496,-10,'Feb-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
+		v0.add(String(-35.2002,-10,'Mär-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
+		v0.add(String(-33.63281,-10,'Äpr-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
+		v0.add(String(-37.00684,-10,'Mäy-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
+		v0.add(String(-31.95801,-10,'Jün-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
+		v0.add(String(-28.39844,-10,'Jül-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
+		v0.add(String(-35.85938,-10,'Äüg-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,50)
+		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,45,81.25)
+		v0.add(String(-10,-4,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,280,45)
-		v0.add(String(0,-8,'5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,112.5)
+		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,330,45)
-		v0.add(String(0,-8,'10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,143.75)
+		v0.add(String(-10,-4,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,380,45)
-		v0.add(String(0,-8,'15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,175)
+		v0.add(String(-10,-4,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5b.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_hlcleg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,69 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Polygon, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+	def __init__(self,width=300,height=150,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,52.97619,50,11.90476,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,115.4762,300,11.90476,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,67.85714,100,11.90476,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,130.3571,250,11.90476,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,82.7381,150,11.90476,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,145.2381,200,11.90476,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,97.61905,200,11.90476,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,160.119,150,11.90476,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,81.25)
-		v0.add(String(-20,-4,'Ying',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,143.75)
-		v0.add(String(-21.66,-4,'Yang',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[42.5,52.5,87.5,66.66667,132.5,80.83333,177.5,95],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[42.5,10,87.5,24.16667,132.5,24.16667,177.5,38.33333],strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[39.5,52.5,42.5,55.5,45.5,52.5,42.5,49.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[84.5,66.66667,87.5,69.66667,90.5,66.66667,87.5,63.66667],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[129.5,80.83333,132.5,83.83333,135.5,80.83333,132.5,77.83333],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[174.5,95,177.5,98,180.5,95,177.5,92],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(40,7.5,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(85,21.66667,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(130,21.66667,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(175,35.83333,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(65,10,65,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(155,10,155,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,24.16667,15,24.16667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,38.33333,15,38.33333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,52.5,15,52.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,66.66667,15,66.66667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,80.83333,15,80.83333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,10)
+		v0.add(String(-10,-4,'70',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,24.16667)
+		v0.add(String(-10,-4,'80',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,38.33333)
+		v0.add(String(-10,-4,'90',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,52.5)
+		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,66.66667)
+		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,80.83333)
+		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,15,95)
+		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleH5c1.py` & `reportlab-4.1.0/tests/render-out/Drawing06.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,23 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, Circle, Wedge, PolyLine, Polygon, Ellipse, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,50,50,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,90,300,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,60,100,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,100,250,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,70,150,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,110,200,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,80,200,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(50,120,150,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,81.25)
-		v0.add(String(-20,-4,'Ying',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,143.75)
-		v0.add(String(-21.66,-4,'Yang',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,50,45)
-		v0.add(String(-2.5,-10,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,125,45)
-		v0.add(String(-5,-10,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-5,-10,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,275,45)
-		v0.add(String(-5,-10,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-5,-10,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(10,10,390,190,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(100,100,20,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(200,100,40,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(300,100,30,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Wedge(330,100,40,-10,40,yradius=None,annular=False,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[120,10,130,20,140,10,150,20,160,10,170,20,180,10,190,20,200,10],strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None,fillColor=Color(0,.501961,0,1)))
+		self.add(Polygon(points=[300,20,350,20,390,80,300,75,330,40],fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Ellipse(50,150,40,20,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(120,150,60,30,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=10,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(220,150,60,30,rx=10,ry=10,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(10,50,'Basic Shapes',textAnchor='start',fontName='Helvetica',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_barcharts_sampleV2c.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2bar.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,103 +2,131 @@
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String, Line
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(59.375,110,18.75,9.6,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(119.375,110,18.75,-22.8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(179.375,110,18.75,8,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(239.375,110,18.75,20,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(299.375,110,18.75,39.96,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(81.875,110,18.75,2.4,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(141.875,110,18.75,-19.6,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(201.875,110,18.75,-12,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(261.875,110,18.75,16,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(321.875,110,18.75,39.96,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,68.75,129.6)
-		v0.add(String(0,-6,'2.40',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,128.75,77.2)
-		v0.add(String(0,1.2,'-5.70',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,188.75,128)
-		v0.add(String(0,-6,'2.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,248.75,140)
-		v0.add(String(0,-6,'5.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,308.75,159.96)
-		v0.add(String(0,-6,'9.99',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,91.25,122.4)
-		v0.add(String(0,-6,'0.60',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,151.25,80.4)
-		v0.add(String(0,1.2,'-4.90',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,211.25,88)
-		v0.add(String(0,1.2,'-3.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,271.25,136)
-		v0.add(String(0,-6,'4.00',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,331.25,159.96)
-		v0.add(String(0,-6,'9.99',textAnchor='middle',fontName='Helvetica',fontSize=6,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,110,350,110,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,110,50,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,110,110,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(170,110,170,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,110,230,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(290,110,290,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,110,350,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,80,50)
-		v0.add(String(-15.344,-8,'Q3 2000',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,140,50)
-		v0.add(String(-22.456,-8,'Year to Date',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,50)
-		v0.add(String(-18.676,-8,'12 months',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,260,50)
-		v0.add(String(-19.788,-8,'Annualised',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0.add(String(-19.788,-17.6,'3 years',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,320,50)
-		v0.add(String(-26.684,-8,'Since 07.10.99',textAnchor='start',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(53.75,50,15,27.08333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(91.25,50,15,10.41667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(128.75,50,15,41.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(166.25,50,15,45.83333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(203.75,50,15,77.08333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(241.25,50,15,93.75,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(278.75,50,15,39.58333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(316.25,50,15,8.333333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(68.75,50,15,29.16667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(106.25,50,15,12.5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(143.75,50,15,43.75,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(181.25,50,15,47.91667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(218.75,50,15,79.16667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(256.25,50,15,95.83333,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(293.75,50,15,41.66667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(331.25,50,15,10.41667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,61.25,77.08333)
+		v0.add(String(0,-4,'Å13',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,98.75,60.41667)
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,136.25,91.66667)
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,173.75,95.83333)
+		v0.add(String(0,-4,'Å22',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,211.25,127.0833)
+		v0.add(String(0,-4,'Å37',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,248.75,143.75)
+		v0.add(String(0,-4,'Å45',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,286.25,89.58333)
+		v0.add(String(0,-4,'Å19',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,323.75,58.33333)
+		v0.add(String(0,-4,'Å4',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,76.25,79.16667)
+		v0.add(String(0,-4,'Å14',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,113.75,62.5)
+		v0.add(String(0,-4,'Å6',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,151.25,93.75)
+		v0.add(String(0,-4,'Å21',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,188.75,97.91667)
+		v0.add(String(0,-4,'Å23',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,226.25,129.1667)
+		v0.add(String(0,-4,'Å38',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,263.75,145.8333)
+		v0.add(String(0,-4,'Å46',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,301.25,91.66667)
+		v0.add(String(0,-4,'Å20',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,338.75,60.41667)
+		v0.add(String(0,-4,'Å5',textAnchor='middle',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,50,50,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(87.5,50,87.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(125,50,125,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(162.5,50,162.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(237.5,50,237.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(275,50,275,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(312.5,50,312.5,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,76.75,48)
+		v0.add(String(-31.74805,-10,'Jän-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,114.25,48)
+		v0.add(String(-34.58496,-10,'Feb-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,151.75,48)
+		v0.add(String(-35.2002,-10,'Mär-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,189.25,48)
+		v0.add(String(-33.63281,-10,'Äpr-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,226.75,48)
+		v0.add(String(-37.00684,-10,'Mäy-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,264.25,48)
+		v0.add(String(-31.95801,-10,'Jün-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,301.75,48)
+		v0.add(String(-28.39844,-10,'Jül-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,339.25,48)
+		v0.add(String(-35.85938,-10,'Äüg-99',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,70,45,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,90,45,90,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,110,45,110,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,130,45,130,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,150,45,150,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,170,45,170,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,81.25,45,81.25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,112.5,45,112.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,143.75,45,143.75,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
 		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(0,-8,'-15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,70)
-		v0.add(String(0,-8,'-10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,81.25)
+		v0.add(String(-10,-4,'15',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,90)
-		v0.add(String(0,-8,'-5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,112.5)
+		v0.add(String(-10,-4,'30',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,110)
-		v0.add(String(0,-8,'0',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,143.75)
+		v0.add(String(-10,-4,'45',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,130)
-		v0.add(String(0,-8,'5',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,150)
-		v0.add(String(0,-8,'10',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,170)
-		v0.add(String(0,-8,'15',textAnchor='middle',fontName='Helvetica',fontSize=8,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,45,175)
+		v0.add(String(-10,-4,'60',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample1c.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample1c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample2c.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample2c.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_legends_sample3a.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_legends_sample3a.gif`

 * *Files 27% similar despite different names*

#### gifbuild

```diff
@@ -4,15 +4,15 @@
 screen colors 2
 screen background 0
 pixel aspect byte 0
 
 screen map
 	sort flag off
 	rgb 255 255 255
-	rgb 255 255 127
+	rgb 255 255 000
 	rgb 254 254 254
 	rgb 253 253 253
 	rgb 252 252 252
 	rgb 251 251 251
 	rgb 250 250 250
 	rgb 249 249 249
 	rgb 248 248 248
@@ -25,15 +25,14 @@
 	rgb 241 241 241
 	rgb 240 240 240
 	rgb 239 239 239
 	rgb 238 238 238
 	rgb 237 237 237
 	rgb 236 236 236
 	rgb 235 235 235
-	rgb 255 223 229
 	rgb 234 234 234
 	rgb 233 233 233
 	rgb 232 232 232
 	rgb 231 231 231
 	rgb 230 230 230
 	rgb 229 229 229
 	rgb 228 228 228
@@ -48,14 +47,15 @@
 	rgb 219 219 219
 	rgb 218 218 218
 	rgb 217 217 217
 	rgb 216 216 216
 	rgb 215 215 215
 	rgb 214 214 214
 	rgb 213 213 213
+	rgb 255 192 203
 	rgb 212 212 212
 	rgb 211 211 211
 	rgb 210 210 210
 	rgb 209 209 209
 	rgb 208 208 208
 	rgb 207 207 207
 	rgb 206 206 206
@@ -84,20 +84,18 @@
 	rgb 180 180 180
 	rgb 179 179 179
 	rgb 178 178 178
 	rgb 177 177 177
 	rgb 176 176 176
 	rgb 175 175 175
 	rgb 174 174 174
-	rgb 127 191 127
 	rgb 173 173 173
 	rgb 172 172 172
 	rgb 171 171 171
 	rgb 170 170 170
-	rgb 255 127 127
 	rgb 169 169 169
 	rgb 168 168 168
 	rgb 167 167 167
 	rgb 166 166 166
 	rgb 165 165 165
 	rgb 164 164 164
 	rgb 163 163 163
@@ -123,33 +121,32 @@
 	rgb 141 141 141
 	rgb 140 140 140
 	rgb 139 139 139
 	rgb 138 138 138
 	rgb 137 137 137
 	rgb 135 135 135
 	rgb 134 134 134
-	rgb 127 127 255
 	rgb 133 133 133
 	rgb 132 132 132
 	rgb 131 131 131
 	rgb 130 130 130
 	rgb 129 129 129
 	rgb 128 128 128
-	rgb 127 127 127
 	rgb 126 126 126
 	rgb 125 125 125
 	rgb 124 124 124
 	rgb 123 123 123
 	rgb 122 122 122
 	rgb 121 121 121
 	rgb 120 120 120
 	rgb 119 119 119
 	rgb 118 118 118
 	rgb 117 117 117
 	rgb 116 116 116
+	rgb 000 128 000
 	rgb 114 114 114
 	rgb 113 113 113
 	rgb 112 112 112
 	rgb 111 111 111
 	rgb 110 110 110
 	rgb 109 109 109
 	rgb 108 108 108
@@ -165,14 +162,15 @@
 	rgb 097 097 097
 	rgb 096 096 096
 	rgb 094 094 094
 	rgb 093 093 093
 	rgb 091 091 091
 	rgb 089 089 089
 	rgb 087 087 087
+	rgb 255 000 000
 	rgb 086 086 086
 	rgb 085 085 085
 	rgb 083 083 083
 	rgb 081 081 081
 	rgb 079 079 079
 	rgb 078 078 078
 	rgb 077 077 077
@@ -200,14 +198,15 @@
 	rgb 047 047 047
 	rgb 044 044 044
 	rgb 043 043 043
 	rgb 042 042 042
 	rgb 041 041 041
 	rgb 040 040 040
 	rgb 039 039 039
+	rgb 000 000 255
 	rgb 038 038 038
 	rgb 037 037 037
 	rgb 036 036 036
 	rgb 032 032 032
 	rgb 031 031 031
 	rgb 030 030 030
 	rgb 029 029 029
@@ -259,98 +258,99 @@
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
 	rgb 000 000 000
+	rgb 000 000 000
 end
 
 image # 1
 image left 0
 image top 0
 image interlaced
 image bits 200 by 100 hex
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c630900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000035f0000000000023f3600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000014c11000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000024c000000000008896700000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000191b0500240d00000924af10000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002181811000019000613150f006a6707120b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000070b1983c743bb72233763ccd10000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000084a68cc8313bc1099e9576bb006a673a881d00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000005656005656005656005600000000000000000000339e003897558943a91900b4100000000000000000000000000000000000000000000000000000001616161600001616160000000000000000000000448b00658e00bd006a6700b50c6a966b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000005656005656005656005600000000000000000000339b004684000011c41800af1000000000000000000000000000000000000000000000000000000016161616000016161600000000000000000000004488003d8f00bc006a6700b20e6a91b60c0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000039a30011c965672c928711bf330000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000449d006f3c06c4006f6c00b9156f6c5ea50500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000426119002a7d3f00086e635d26000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044a44e3b002e6726545320643a54531a673d00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000478b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000035c701100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c610900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000035d0000000000023f3600000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000014bf1000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000024c000000000008856500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000181a0500230d00000923ad10000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002171711000018000613150f00686507120b00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000006eaf953c723bb52133743ccc10000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000080a489c7313bbf099b9274b90068653a841c00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000009f9f009f9f009f9f009f00000000000000000000339b003894548543a71800b2100000000000000000000000000000000000000000000000000000002c2c2c2c00002c2c2c0000000000000000000000448800638b00bb00686500b30c689369000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000009f9f009f9f009f9f009f000000000000000000003398004680000011c21700ad100000000000000000000000000000000000000000000000000000002c2c2c2c00002c2c2c00000000000000000000004484003d8c00ba00686500b00e688eb40c0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000039a10011c863652b8f8311bd330000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000449a006d3c06c2006d6a00b7156d6a5ca30500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000425f1800297a3f00086c615b25000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044a24e3b002e652553521f623a535219653d00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000047880000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000035a6e1100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003342000000195e000000000000000000044b28000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006c8800000025c00000000000000000000c9f47000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000092a050000191b0500240d00000f220000190421000000000000000000000000000000000000000000000000000000000000000000000000000000448812140000bc0000211a0000032406008647091209000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000018952bc25270b1983c743bb722484b867b3dc966ae46000000000000000000000000000000000000000000000000000000000000000000000000000044a88ac73500bc007e4e9e42058038ba158647547317000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000051510000000000515100000000000000000000004b8b00ae1c339e003897558943a355658d00bd0059770000000000000000000000000000000000007f00007f7f7f00000000000000000000000000004488005a9200bc003815956a5062002a07868d550000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000051510000000000515100000000000000000000000ea0458200339b004684000011b408001100bc00547a0000000000000000000000000000000000007f00007f7f7f00000000000000000000000000004488003c8b00bc005f54686a6477000013868bab0400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000249543350439a30011c965672c8ba04c6707c3005c8100000000000000000000000000000000000000000000000000000000000000000000000000004497007b3306c400bb278b8730ca4e6d148d4e7b9000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000022867a8b81426119002a7d3f00056a6e092f66214f580a00000000000000000000000000000000000000000000000000000000000000000000000000055a602c002e67214171305e00377e2d0c5b4a226731000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000009649102c4a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000001d6f8345000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003342000000185c000000000000000000044b27000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000006a8400000024be0000000000000000000c9c47000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000929050000181a0500230d00000f210000180420000000000000000000000000000000000000000000000000000000000000000000000000000000448412140000ba000020190000032306008247091209000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000017922ac0516eaf953c723bb521484b82783dc864ac46000000000000000000000000000000000000000000000000000000000000000000000000000044a686c63500ba007b4e9b42057c38b8158247537116000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000087870000000000878700000000000000000000004b8800ac1b339b003894548543a154638a00bb005775000000000000000000000000000000000000cd0000cdcdcd0000000000000000000000000000448400588f00ba00381592685060002907828a540000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000087870000000000878700000000000000000000000e9d457e003398004680000011b208001100ba005377000000000000000000000000000000000000cd0000cdcdcd00000000000000000000000000004484003c8800ba005d53666862750000138288a90400000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000239243350439a10011c863652b889d4c6507c1005a7d0000000000000000000000000000000000000000000000000000000000000000000000000000449400783306c200b926888330c94e6b148a4e788d00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000218277887d425f1800297a3f0005686c092f64204f560a0000000000000000000000000000000000000000000000000000000000000000000000000005585e2b002e6520416f305c00377b2d0c594a216531000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000009349102b4a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000001c6d7f45000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000003342000000195e000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000195e00000000590800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000006c8800000025c000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000025c0000000004806002a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000448812140000bc0412070a1200000f220000000000000000000000000000000000000000000000000000000000000000000000000000000000000000111108120d061203bc0421000015043f970c000f2200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000044a88ac73500bc089c5d1dcb06464b857d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000075a117bc450a9307c666ad481fcc1071ac38464b857d000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000078780000787878787800000000000000000000004488005a9200bc00725d00b806a255658e0000000000000000000000000000000000000000000000000000000000000000000000000000000000000007ba038e752d3500bc00577a00b010399400a255658e000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000078780000787878787800000000000000000000004488003c8b00bc00725d00b806b309001100000000000000000000000000000000000000000000000000000000000000000000000000000000000000008e5457b95f0000bc00527c00af10399400b3090011000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000004497007b3306c400628d33c52989a14c67000000000000000000000000000000000000000000000000000000000000000000000000000000000000000031be0494690006c4005a8300b61832a72689a14c67000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000055a602c002e67210a793e5e2305696f0a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003a002a14002e67224e5924643703621e05696f0a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000003342000000185c000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000185c00000000570800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000006a8400000024be00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000024be00000000480600290000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000448412140000ba0412070a1200000f210000000000000000000000000000000000000000000000000000000000000000000000000000000000000000111108120d061203ba0420000015043f940c000f2100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000044a686c63500ba08995b1cca06464b817a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000739e16ba450a9007c564ab481ecb106faa38464b817a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000c3c30000c3c3c3c3c30000000000000000000000448400588f00ba00705b00b606a054638b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000007b8038b732d3500ba00557700ae10399100a054638b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000c3c30000c3c3c3c3c300000000000000000000004484003c8800ba00705b00b606b109001100000000000000000000000000000000000000000000000000000000000000000000000000000000000000008b5355b75d0000ba00517900ad10399100b1090011000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000449400783306c200608a33c428859e4c65000000000000000000000000000000000000000000000000000000000000000000000000000000000000000031bc0491670006c200587f00b41732a525859e4c65000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000005585e2b002e65200a763e5c2205676d0a0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000003a002914002e65214e5723623703601d05676d0a000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044b280c630900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c9f4714c11000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000001112030a110007270400864700af100004260600111108120d061203000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000076ad06347d246859aa00864700af1019833ca91e75a117bc450a9307000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000010000010101000000000000000000000000000003b711650d8a6255a00d864700af10834900668a07ba038e752d3500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000010000010101000000000000000000000000000000607e6d009a32000c07864700af109954004795008e5457b95f0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000000006c42f0052b94e77028d4e00b61845a400743b0031be0494690000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-0000000000000000000000000000000000000000000000000000000000000000000000000000000000006e0000004d7c1c0c5b4a1b6437004061360000003a002a140000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000003d5c4a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
-000000000000000000000000000000000000000000000000000000000000000000000000000000004c580000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000044b270c610900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c9c4714bf1000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000001112030a110007260400824700ad100004250600111108120d061203000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000074ab06347a236657a800824700ad10187f3ca71d739e16ba450a9007000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000010000010101000000000000000000000000000003b511630d8660549d0d824700ad107f4900648607b8038b732d3500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+00000000000000000000000000000000000000000100000101010000000000000000000000000000005e7b6b009732000c07824700ad109653004792008b5355b75d0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000000006c22f0051b74e75028a4e00b41745a200723b0031bc0491670000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+0000000000000000000000000000000000000000000000000000000000000000000000000000000000006c0000004d791b0c594a1a623700405f360000003a0029140000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000003d5a4a00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
+000000000000000000000000000000000000000000000000000000000000000000000000000000004c560000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
 0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_linecharts_sampleCandleStick.py` & `reportlab-4.1.0/tests/render-out/fillmode-non-zero.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, PolyLine, Line, Rect, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Path
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+class ExplodedDrawing_FillModeDrawing(_DrawingEditorMixin,Drawing):
+	def __init__(self,width=600.0,height=200.0,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(PolyLine(points=[42.5,40,87.5,55,132.5,70,177.5,85],strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(42.5,25,42.5,34,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(37.5,25,47.5,25,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(42.5,49,42.5,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(37.5,55,47.5,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(32.5,34,20,15,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(32.5,40,52.5,40,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(87.5,40,87.5,49,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(82.5,40,92.5,40,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(87.5,64,87.5,70,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(82.5,70,92.5,70,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(77.5,49,20,15,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(77.5,55,97.5,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(132.5,55,132.5,64,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(127.5,55,137.5,55,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(132.5,79,132.5,85,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(127.5,85,137.5,85,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(122.5,64,20,15,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(122.5,70,142.5,70,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(177.5,70,177.5,79,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(172.5,70,182.5,70,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(177.5,94,177.5,100,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(172.5,100,182.5,100,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(167.5,79,20,15,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(167.5,85,187.5,85,strokeColor=Color(0,0,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,20,200,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,20,20,15,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(65,20,65,15,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,20,110,15,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(155,20,155,15,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,20,200,15,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,20,20,105,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,25,15,25,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,40,15,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,55,15,55,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,70,15,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,85,15,85,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,100,15,100,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,25)
-		v0.add(String(-10,-4,'90',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,40)
-		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,55)
-		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,70)
-		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,85)
-		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,100)
-		v0.add(String(-15,-4,'140',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,-1,0,200)
+		v0.add(Rect(1,1,599,199,rx=0,ry=0,fillColor=None,fillOpacity=1,strokeColor=Color(0,0,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1=v0._nn(Group())
+		v1.transform = (.5,0,0,.5,0,0)
+		v1.add(Path(points=[250,75,323,301,131,161,369,161,177,301],operators=[0,1,1,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.309017,.951057,-0.951057,.309017,306.21,249)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.809017,-0.587785,.587785,-0.809017,175.16,193.2)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (1,0,0,1,314.26,161)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.809017,.587785,-0.587785,-0.809017,221.16,268.8)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.309017,-0.951057,.951057,.309017,233.21,126.98)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1.add(Path(points=[600,81,659.0945,81,707,128.9055,707,188,707,247.0945,659.0945,295,600,295,540.9055,295,493,247.0945,493,188,493,128.9055,540.9055,81,600,81,600,139,627.062,139,649,160.938,649,188,649,215.062,627.062,237,600,237,572.938,237,551,215.062,551,188,551,160.938,572.938,139,600,139],operators=[0,2,2,2,2,3,0,2,2,2,2,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,707,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,546.5,280.6647)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,546.5,95.33528)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,.5,-0.5,-0.866025,624.5,230.4352)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,-1,1,0,551,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,.5,-0.5,.866025,624.5,145.5648)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1.add(Path(points=[950,81,1009.094,81,1057,128.9055,1057,188,1057,247.0945,1009.094,295,950,295,890.9055,295,843,247.0945,843,188,843,128.9055,890.9055,81,950,81,950,139,922.938,139,901,160.938,901,188,901,215.062,922.938,237,950,237,977.062,237,999,215.062,999,188,999,160.938,977.062,139,950,139],operators=[0,2,2,2,2,3,0,2,2,2,2,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,1057,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,896.5,280.6647)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,896.5,95.33528)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,974.5,230.4352)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,901,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,974.5,145.5648)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_FillModeDrawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_lineplots_sample1b.py` & `reportlab-4.1.0/tests/render-out/Drawing08.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,84 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, PolyLine, Circle
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,125,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,350,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,50,110,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(170,50,170,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,50,200,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(230,50,230,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(290,50,290,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(350,50,350,45,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,110,45)
-		v0.add(String(-6.25,-10,'1.0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,170,45)
-		v0.add(String(-6.25,-10,'2.0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,45)
-		v0.add(String(-6.25,-10,'2.5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,230,45)
-		v0.add(String(-6.25,-10,'3.0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,290,45)
-		v0.add(String(-6.25,-10,'4.0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,350,45)
-		v0.add(String(-6.25,-10,'5.0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(50,50,50,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,50,45,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,67.85714,45,67.85714,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,85.71429,45,85.71429,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,103.5714,45,103.5714,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,121.4286,45,121.4286,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,139.2857,45,139.2857,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,157.1429,45,157.1429,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(50,175,45,175,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,50)
-		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,67.85714)
-		v0.add(String(-5,-4,'1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,85.71429)
-		v0.add(String(-5,-4,'2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,103.5714)
-		v0.add(String(-5,-4,'3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,121.4286)
-		v0.add(String(-5,-4,'4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,139.2857)
-		v0.add(String(-5,-4,'5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,157.1429)
-		v0.add(String(-5,-4,'6',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,45,175)
-		v0.add(String(-5,-4,'7',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(PolyLine(points=[110,67.85714,170,85.71429,200,67.85714,230,103.5714,290,139.2857],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[110,85.71429,170,103.5714,200,85.71429,260,139.2857,290,157.1429],strokeColor=Color(0,0,1,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(110,67.85714,2.5,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(170,85.71429,2.5,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(200,67.85714,2.5,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(230,103.5714,2.5,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(290,139.2857,2.5,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,110,77.85714)
-		v0.add(String(-3.75,-4,' 1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,170,95.71429)
-		v0.add(String(-3.75,-4,' 2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,77.85714)
-		v0.add(String(-3.75,-4,' 1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,230,113.5714)
-		v0.add(String(-3.75,-4,' 3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,290,149.2857)
-		v0.add(String(-3.75,-4,' 5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Circle(110,85.71429,2.5,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(170,103.5714,2.5,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(200,85.71429,2.5,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(260,139.2857,2.5,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Circle(290,157.1429,2.5,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,110,95.71429)
-		v0.add(String(-3.75,-4,' 2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,170,113.5714)
-		v0.add(String(-3.75,-4,' 3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,200,95.71429)
-		v0.add(String(-3.75,-4,' 2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,260,149.2857)
-		v0.add(String(-3.75,-4,' 5',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,290,167.1429)
-		v0.add(String(-3.75,-4,' 6',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,10,10)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,2,150,10)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (2,0,0,1,10,125)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,.57735,1,250,125)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0a.py` & `reportlab-4.1.0/tests/render-out/Drawing01.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Ellipse, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Ellipse(200,100,50,50,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(200,40,'a',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(50,50,300,100,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(180,100,'Hello World',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
+		self.add(String(180,86,b'Special characters \xc2\xa2\xc2\xa9\xc2\xae\xc2\xa3\xce\xb1\xce\xb2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample0b.py` & `reportlab-4.1.0/tests/render-out/autoclose-svg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Ellipse, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Path
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+class ExplodedDrawing_AutoCloseDrawing(_DrawingEditorMixin,Drawing):
+	def __init__(self,width=100.0,height=100.0,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Ellipse(210,100,60,50,fillColor=Color(0,.545098,.545098,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(210,40,'a',textAnchor='middle',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,-1,0,100)
+		v1=v0._nn(Group())
+		v1.transform = (1,0,0,-1,0,100)
+		v1.add(Path(points=[10,10,10,90,20,90,20,10,30,10,30,90,40,90,40,10,50,10,50,90,60,90,60,10,70,10,70,90,80,90,80,10],operators=[0,1,1,1,3,0,1,1,1,0,1,1,1,3,0,1,1,1],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,1,1),fillOpacity=1,strokeColor=Color(1,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_AutoCloseDrawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_piecharts_sample3.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Wedge
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Wedge(200,100,75,-176.4,90,yradius=75,annular=False,fillColor=Color(.27451,.509804,.705882,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Wedge(200,100,75,-180,-176.4,yradius=75,annular=False,fillColor=Color(.847059,.74902,.847059,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Wedge(200,100,75,-270,-180,yradius=75,annular=False,fillColor=Color(.392157,.584314,.929412,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(80,150,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(100,151.585,'before',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(80,130,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(100,131.585,'after',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_bcleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_bcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_bcleg.py` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1barline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,60 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Line, String, Polygon
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Polygon, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=300,height=150,*args,**kw):
+	def __init__(self,width=400,height=250,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(24.5,10,18,42.5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(69.5,10,18,56.66667,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(114.5,10,18,70.83333,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(159.5,10,18,85,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(87.5,10,18,14.16667,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(132.5,10,18,21.25,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(177.5,10,18,28.33333,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(65,10,65,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(155,10,155,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,24.16667,15,24.16667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,38.33333,15,38.33333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,52.5,15,52.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,66.66667,15,66.66667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,80.83333,15,80.83333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(26.25,70,25,130.7692,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(118.75,70,25,143.8462,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(211.25,70,25,156.9231,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(303.75,70,25,170,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(53.75,70,25,91.53846,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(146.25,70,25,32.69231,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(238.75,70,25,111.1538,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(331.25,70,25,39.23077,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(81.25,70,25,82.38462,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(173.75,70,25,98.07692,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(266.25,70,25,66.69231,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(358.75,70,25,120.3077,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[66.25,136.6923,158.75,97.46154,251.25,156.3077,343.75,162.8462],strokeColor=Color(1,.647059,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[66.25,83.07692,158.75,84.38462,251.25,187.6923,343.75,109.2308],strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[61.25,83.07692,66.25,88.07692,71.25,83.07692,66.25,78.07692],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[153.75,84.38462,158.75,89.38462,163.75,84.38462,158.75,79.38462],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[246.25,187.6923,251.25,192.6923,256.25,187.6923,251.25,182.6923],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[338.75,109.2308,343.75,114.2308,348.75,109.2308,343.75,104.2308],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,70,390,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,70,20,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(112.5,70,112.5,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(205,70,205,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(297.5,70,297.5,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(390,70,390,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,70,20,240,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,70,15,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,135.3846,15,135.3846,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(20,200.7692,15,200.7692,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,10)
-		v0.add(String(-10,-4,'70',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,15,70)
+		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,24.16667)
-		v0.add(String(-10,-4,'80',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,1,15,135.3846)
+		v0.add(String(-10,-4,'50',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,38.33333)
-		v0.add(String(-10,-4,'90',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,52.5)
+		v0.transform = (1,0,0,1,15,200.7692)
 		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,66.66667)
-		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,80.83333)
-		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,95)
-		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Rect(12.5,15,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(32.5,16.585,'series 0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(87.5,15,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(107.5,16.585,'series 1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(162.5,15,10,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(182.5,16.585,'series 2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(237.5,20,247.5,20,strokeColor=Color(1,.647059,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(257.5,16.585,'series 3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Line(312.5,20,322.5,20,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Polygon(points=[312.5,20,317.5,25,322.5,20,317.5,15],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(332.5,16.585,'series 4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_hlcleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_hlcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_hlcleg.py` & `reportlab-4.1.0/tests/render-out/Drawing07.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Polygon, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=300,height=150,*args,**kw):
+	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(0,0,300,150,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[42.5,52.5,87.5,66.66667,132.5,80.83333,177.5,95],strokeColor=Color(1,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[42.5,10,87.5,24.16667,132.5,24.16667,177.5,38.33333],strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=1,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[39.5,52.5,42.5,55.5,45.5,52.5,42.5,49.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[84.5,66.66667,87.5,69.66667,90.5,66.66667,87.5,63.66667],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[129.5,80.83333,132.5,83.83333,135.5,80.83333,132.5,77.83333],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[174.5,95,177.5,98,180.5,95,177.5,92],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(40,7.5,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(85,21.66667,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(130,21.66667,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(175,35.83333,5,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,200,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,20,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(65,10,65,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(110,10,110,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(155,10,155,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(200,10,200,5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,20,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,10,15,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,24.16667,15,24.16667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,38.33333,15,38.33333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,52.5,15,52.5,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,66.66667,15,66.66667,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,80.83333,15,80.83333,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,95,15,95,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,10)
-		v0.add(String(-10,-4,'70',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,24.16667)
-		v0.add(String(-10,-4,'80',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,38.33333)
-		v0.add(String(-10,-4,'90',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,52.5)
-		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,66.66667)
-		v0.add(String(-15,-4,'110',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,80.83333)
-		v0.add(String(-15,-4,'120',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,95)
-		v0.add(String(-15,-4,'130',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,40.70117,'röt',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,28,20,5,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,26.70117,'blue',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(186.9238,14,20,5,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(145,12.70117,'green',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(261.9238,42,20,5,rx=0,ry=0,fillColor=Color(1,.752941,.796078,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,40.70117,'pink',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(261.9238,28,20,5,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(220,26.70117,'yellow',textAnchor='start',fontName='Vera',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Polygon(points=[294.1667,2.5,294.1667,4.166667,292.5,4.166667,292.5,5.833333,294.1667,5.833333,294.1667,7.5,295.8333,7.5,295.8333,5.833333,297.5,5.833333,297.5,4.166667,295.8333,4.166667,295.8333,2.5],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.transform = (1,0,0,1,10,10)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.965926,.258819,-0.258819,.965926,150,10)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (.866025,.5,-0.5,.866025,300,10)
+		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_lpleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_lpleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_pcleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_pcleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_plpleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_plpleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1bar.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1bar.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1barline.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample1barline.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample1barline.py` & `reportlab-4.1.0/tests/render-out/fillmode-even-odd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, PolyLine, Polygon, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, Path
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=250,*args,**kw):
+class ExplodedDrawing_FillModeDrawing(_DrawingEditorMixin,Drawing):
+	def __init__(self,width=600.0,height=200.0,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(26.25,70,25,130.7692,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(118.75,70,25,143.8462,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(211.25,70,25,156.9231,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(303.75,70,25,170,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(53.75,70,25,91.53846,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(146.25,70,25,32.69231,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(238.75,70,25,111.1538,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(331.25,70,25,39.23077,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(81.25,70,25,82.38462,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(173.75,70,25,98.07692,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(266.25,70,25,66.69231,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Rect(358.75,70,25,120.3077,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[66.25,136.6923,158.75,97.46154,251.25,156.3077,343.75,162.8462],strokeColor=Color(1,.647059,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(PolyLine(points=[66.25,83.07692,158.75,84.38462,251.25,187.6923,343.75,109.2308],strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[61.25,83.07692,66.25,88.07692,71.25,83.07692,66.25,78.07692],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[153.75,84.38462,158.75,89.38462,163.75,84.38462,158.75,79.38462],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[246.25,187.6923,251.25,192.6923,256.25,187.6923,251.25,182.6923],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[338.75,109.2308,343.75,114.2308,348.75,109.2308,343.75,104.2308],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,70,390,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,70,20,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(112.5,70,112.5,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(205,70,205,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(297.5,70,297.5,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(390,70,390,65,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,70,20,240,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,70,15,70,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,135.3846,15,135.3846,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
-		self.add(Line(20,200.7692,15,200.7692,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=10,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,70)
-		v0.add(String(-5,-4,'0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,135.3846)
-		v0.add(String(-10,-4,'50',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,15,200.7692)
-		v0.add(String(-15,-4,'100',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(12.5,15,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(32.5,16.585,'series 0',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(87.5,15,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(107.5,16.585,'series 1',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(162.5,15,10,10,rx=0,ry=0,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(182.5,16.585,'series 2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(237.5,20,247.5,20,strokeColor=Color(1,.647059,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(257.5,16.585,'series 3',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Line(312.5,20,322.5,20,strokeColor=Color(0,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Polygon(points=[312.5,20,317.5,25,322.5,20,317.5,15],fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(332.5,16.585,'series 4',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		v0.transform = (1,0,0,-1,0,200)
+		v0.add(Rect(1,1,599,199,rx=0,ry=0,fillColor=None,fillOpacity=1,strokeColor=Color(0,0,1,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1=v0._nn(Group())
+		v1.transform = (.5,0,0,.5,0,0)
+		v1.add(Path(points=[250,75,323,301,131,161,369,161,177,301],operators=[0,1,1,1,1,3],isClipPath=0,autoclose='svg',fillMode=0,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.309017,.951057,-0.951057,.309017,306.21,249)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.809017,-0.587785,.587785,-0.809017,175.16,193.2)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (1,0,0,1,314.26,161)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.809017,.587785,-0.587785,-0.809017,221.16,268.8)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.309017,-0.951057,.951057,.309017,233.21,126.98)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1.add(Path(points=[600,81,659.0945,81,707,128.9055,707,188,707,247.0945,659.0945,295,600,295,540.9055,295,493,247.0945,493,188,493,128.9055,540.9055,81,600,81,600,139,627.062,139,649,160.938,649,188,649,215.062,627.062,237,600,237,572.938,237,551,215.062,551,188,551,160.938,572.938,139,600,139],operators=[0,2,2,2,2,3,0,2,2,2,2,3],isClipPath=0,autoclose='svg',fillMode=0,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,707,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,546.5,280.6647)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,546.5,95.33528)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,.5,-0.5,-0.866025,624.5,230.4352)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,-1,1,0,551,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,.5,-0.5,.866025,624.5,145.5648)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1.add(Path(points=[950,81,1009.094,81,1057,128.9055,1057,188,1057,247.0945,1009.094,295,950,295,890.9055,295,843,247.0945,843,188,843,128.9055,890.9055,81,950,81,950,139,922.938,139,901,160.938,901,188,901,215.062,922.938,237,950,237,977.062,237,999,215.062,999,188,999,160.938,977.062,139,950,139],operators=[0,2,2,2,2,3,0,2,2,2,2,3],isClipPath=0,autoclose='svg',fillMode=0,fillColor=Color(1,0,0,1),fillOpacity=1,strokeColor=Color(0,0,0,1),strokeWidth=3,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,1057,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,896.5,280.6647)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,896.5,95.33528)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (.866025,-0.5,.5,.866025,974.5,230.4352)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (0,1,-1,0,901,188)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2=v1._nn(Group())
+		v2.transform = (-0.866025,-0.5,.5,-0.866025,974.5,145.5648)
+		v2.add(Path(points=[16,0,-8,9,-8,-9],operators=[0,1,1,3],isClipPath=0,autoclose='svg',fillMode=1,fillColor=Color(0,0,0,1),fillOpacity=1,strokeColor=None,strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_FillModeDrawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample2bar.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample2bar.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample3.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_sample3.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_sample3.py` & `reportlab-4.1.0/tests/render-out/Drawing10.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,31 @@
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(80,150,10,10,rx=0,ry=0,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(100,151.585,'before',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
-		self.add(Rect(80,130,10,10,rx=0,ry=0,fillColor=Color(0,.501961,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(100,131.585,'after',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1)))
+		self.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,25,25)
+		v0.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,25,25)
+		v1=v0._nn(Group())
+		v1.transform = (1,0,0,1,25,25)
+		v1.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v1.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		v0=self._nn(Group())
+		v0.transform = (1,0,0,1,25,25)
+		v1=v0._nn(Group())
+		v1.transform = (1,0,0,1,25,25)
+		v2=v1._nn(Group())
+		v2.transform = (1,0,0,1,25,25)
+		v2.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v2.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/charts-out/test_graphics_charts_special_scleg.gif` & `reportlab-4.1.0/tests/charts-out/test_graphics_charts_special_scleg.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/encryption.gif` & `reportlab-4.1.0/tests/encryption.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/gray-alpha.png` & `reportlab-4.1.0/tests/gray-alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/pythonpowered-gs.gif` & `reportlab-4.1.0/tests/pythonpowered-gs.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/pythonpowered.gif` & `reportlab-4.1.0/tests/pythonpowered.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/410.png` & `reportlab-4.1.0/tests/render-out/410.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/410.py` & `reportlab-4.1.0/tests/render-out/410.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing01.gif` & `reportlab-4.1.0/tests/render-out/Drawing01.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing01.jpg` & `reportlab-4.1.0/tests/render-out/Drawing01.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing01.png` & `reportlab-4.1.0/tests/render-out/Drawing01.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing01.py` & `reportlab-4.1.0/tests/render-out/Drawing09.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Rect
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(50,50,300,100,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(180,100,'Hello World',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
-		self.add(String(180,86,b'Special characters \xc2\xa2\xc2\xa9\xc2\xae\xc2\xa3\xce\xb1\xce\xb2',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(1,0,0,1)))
+		self.add(String(20,20,'I should be totally horizontal and enclosed in a box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(Rect(18,18,249.64,16,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0=self._nn(Group())
+		v0.transform = (.965926,.258819,-0.258819,.965926,0,50)
+		v0.add(String(20,20,'I should slope up by 15 degrees, so my right end is higher than my left',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		v0.add(Rect(18,18,342.64,16,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/render-out/Drawing02.gif` & `reportlab-4.1.0/tests/render-out/Drawing02.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing02.jpg` & `reportlab-4.1.0/tests/render-out/Drawing02.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing02.png` & `reportlab-4.1.0/tests/render-out/Drawing02.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing02.py` & `reportlab-4.1.0/tests/render-out/Drawing02.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing03.gif` & `reportlab-4.1.0/tests/render-out/Drawing03.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing03.jpg` & `reportlab-4.1.0/tests/render-out/Drawing03.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing03.png` & `reportlab-4.1.0/tests/render-out/Drawing03.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing03.py` & `reportlab-4.1.0/tests/render-out/Drawing03.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing04.gif` & `reportlab-4.1.0/tests/render-out/Drawing04.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing04.jpg` & `reportlab-4.1.0/tests/render-out/Drawing04.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing04.png` & `reportlab-4.1.0/tests/render-out/Drawing04.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing04.py` & `reportlab-4.1.0/tests/render-out/Drawing04.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing05.gif` & `reportlab-4.1.0/tests/render-out/Drawing05.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing05.jpg` & `reportlab-4.1.0/tests/render-out/Drawing05.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing05.png` & `reportlab-4.1.0/tests/render-out/Drawing05.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing05.py` & `reportlab-4.1.0/tests/render-out/Drawing05.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing06.gif` & `reportlab-4.1.0/tests/render-out/Drawing06.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing06.jpg` & `reportlab-4.1.0/tests/render-out/Drawing06.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing06.png` & `reportlab-4.1.0/tests/render-out/Drawing06.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing07.gif` & `reportlab-4.1.0/tests/render-out/Drawing07.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing07.jpg` & `reportlab-4.1.0/tests/render-out/Drawing07.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing07.png` & `reportlab-4.1.0/tests/render-out/Drawing07.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing07.py` & `reportlab-4.1.0/tests/render-out/Drawing11.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,26 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Line, Circle, Ellipse, PolyLine
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
+		self.add(Line(90,100,110,100,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Line(100,90,100,110,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Circle(100,100,10,fillColor=Color(1,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Ellipse(96.66667,103.3333,.666667,2,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Ellipse(103.3333,103.3333,.666667,2,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(PolyLine(points=[93.73538,97.71987,93.77613,97.61088,93.81877,97.50262,93.8633,97.39513,93.9097,97.28842,93.95795,97.18254,94.00804,97.07753,94.05996,96.9734,94.11368,96.87019,94.1692,96.76794,94.2265,96.66667,94.28555,96.56641,94.34635,96.4672,94.40886,96.36907,94.47308,96.27205,94.53899,96.17616,94.60655,96.08143,94.67576,95.9879,94.74659,95.89559,94.81903,95.80453,94.89304,95.71475,94.9686,95.62627,95.0457,95.53913,95.12431,95.45334,95.2044,95.36894,95.28595,95.28595,95.36894,95.2044,95.45334,95.12431,95.53913,95.0457,95.62627,94.9686,95.71475,94.89304,95.80453,94.81903,95.89559,94.74659,95.9879,94.67576,96.08143,94.60655,96.17616,94.53899,96.27205,94.47308,96.36907,94.40886,96.4672,94.34635,96.56641,94.28555,96.66667,94.2265,96.76794,94.1692,96.87019,94.11368,96.9734,94.05996,97.07753,94.00804,97.18254,93.95795,97.28842,93.9097,97.39513,93.8633,97.50262,93.81877,97.61088,93.77613,97.71987,93.73538,97.82955,93.69654,97.93989,93.65962,98.05086,93.62463,98.16242,93.59159,98.27454,93.56049,98.38719,93.53136,98.50033,93.5042,98.61392,93.47902,98.72794,93.45582,98.84235,93.43461,98.9571,93.41541,99.07218,93.39821,99.18754,93.38303,99.30314,93.36985,99.41896,93.3587,99.53496,93.34957,99.65109,93.34247,99.76734,93.33739,99.88365,93.33435,100,93.33333,100.1163,93.33435,100.2327,93.33739,100.3489,93.34247,100.465,93.34957,100.581,93.3587,100.6969,93.36985,100.8125,93.38303,100.9278,93.39821,101.0429,93.41541,101.1577,93.43461,101.2721,93.45582,101.3861,93.47902,101.4997,93.5042,101.6128,93.53136,101.7255,93.56049,101.8376,93.59159,101.9491,93.62463,102.0601,93.65962,102.1705,93.69654,102.2801,93.73538,102.3891,93.77613,102.4974,93.81877,102.6049,93.8633,102.7116,93.9097,102.8175,93.95795,102.9225,94.00804,103.0266,94.05996,103.1298,94.11368,103.2321,94.1692,103.3333,94.2265,103.4336,94.28555,103.5328,94.34635,103.6309,94.40886,103.728,94.47308,103.8238,94.53899,103.9186,94.60655,104.0121,94.67576,104.1044,94.74659,104.1955,94.81903,104.2853,94.89304,104.3737,94.9686,104.4609,95.0457,104.5467,95.12431,104.6311,95.2044,104.714,95.28595,104.7956,95.36894,104.8757,95.45334,104.9543,95.53913,105.0314,95.62627,105.107,95.71475,105.181,95.80453,105.2534,95.89559,105.3242,95.9879,105.3934,96.08143,105.461,96.17616,105.5269,96.27205,105.5911,96.36907,105.6537,96.4672,105.7144,96.56641,105.7735,96.66667,105.8308,96.76794,105.8863,96.87019,105.94,96.9734,105.992,97.07753,106.0421,97.18254,106.0903,97.28842,106.1367,97.39513,106.1812,97.50262,106.2239,97.61088,106.2646,97.71987],strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None,fillColor=Color(0,0,0,1)))
 		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,10,10)
-		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (.965926,.258819,-0.258819,.965926,150,10)
-		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (.866025,.5,-0.5,.866025,300,10)
-		v0.add(Line(0,0,100,0,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,0,0,50,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,10,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,20,10,20,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,30,10,30,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(0,40,10,40,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(10,0,10,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(20,0,20,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(30,0,30,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(40,0,40,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(50,0,50,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(60,0,60,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(70,0,70,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(80,0,80,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(Line(90,0,90,10,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(String(20,35,'Axes',textAnchor='start',fontName='Times-Roman',fontSize=10,fillColor=Color(0,0,0,1),fill=Color(0,0,0,1)))
+		v0.transform = (2,0,0,2,100,-100)
+		v0.add(Line(90,100,110,100,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Line(100,90,100,110,strokeColor=Color(0,.501961,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Circle(100,100,10,fillColor=Color(0,0,1,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Ellipse(96.66667,103.3333,.666667,2,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(Ellipse(103.3333,103.3333,.666667,2,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.add(PolyLine(points=[93.73538,97.71987,93.77613,97.61088,93.81877,97.50262,93.8633,97.39513,93.9097,97.28842,93.95795,97.18254,94.00804,97.07753,94.05996,96.9734,94.11368,96.87019,94.1692,96.76794,94.2265,96.66667,94.28555,96.56641,94.34635,96.4672,94.40886,96.36907,94.47308,96.27205,94.53899,96.17616,94.60655,96.08143,94.67576,95.9879,94.74659,95.89559,94.81903,95.80453,94.89304,95.71475,94.9686,95.62627,95.0457,95.53913,95.12431,95.45334,95.2044,95.36894,95.28595,95.28595,95.36894,95.2044,95.45334,95.12431,95.53913,95.0457,95.62627,94.9686,95.71475,94.89304,95.80453,94.81903,95.89559,94.74659,95.9879,94.67576,96.08143,94.60655,96.17616,94.53899,96.27205,94.47308,96.36907,94.40886,96.4672,94.34635,96.56641,94.28555,96.66667,94.2265,96.76794,94.1692,96.87019,94.11368,96.9734,94.05996,97.07753,94.00804,97.18254,93.95795,97.28842,93.9097,97.39513,93.8633,97.50262,93.81877,97.61088,93.77613,97.71987,93.73538,97.82955,93.69654,97.93989,93.65962,98.05086,93.62463,98.16242,93.59159,98.27454,93.56049,98.38719,93.53136,98.50033,93.5042,98.61392,93.47902,98.72794,93.45582,98.84235,93.43461,98.9571,93.41541,99.07218,93.39821,99.18754,93.38303,99.30314,93.36985,99.41896,93.3587,99.53496,93.34957,99.65109,93.34247,99.76734,93.33739,99.88365,93.33435,100,93.33333,100.1163,93.33435,100.2327,93.33739,100.3489,93.34247,100.465,93.34957,100.581,93.3587,100.6969,93.36985,100.8125,93.38303,100.9278,93.39821,101.0429,93.41541,101.1577,93.43461,101.2721,93.45582,101.3861,93.47902,101.4997,93.5042,101.6128,93.53136,101.7255,93.56049,101.8376,93.59159,101.9491,93.62463,102.0601,93.65962,102.1705,93.69654,102.2801,93.73538,102.3891,93.77613,102.4974,93.81877,102.6049,93.8633,102.7116,93.9097,102.8175,93.95795,102.9225,94.00804,103.0266,94.05996,103.1298,94.11368,103.2321,94.1692,103.3333,94.2265,103.4336,94.28555,103.5328,94.34635,103.6309,94.40886,103.728,94.47308,103.8238,94.53899,103.9186,94.60655,104.0121,94.67576,104.1044,94.74659,104.1955,94.81903,104.2853,94.89304,104.3737,94.9686,104.4609,95.0457,104.5467,95.12431,104.6311,95.2044,104.714,95.28595,104.7956,95.36894,104.8757,95.45334,104.9543,95.53913,105.0314,95.62627,105.107,95.71475,105.181,95.80453,105.2534,95.89559,105.3242,95.9879,105.3934,96.08143,105.461,96.17616,105.5269,96.27205,105.5911,96.36907,105.6537,96.4672,105.7144,96.56641,105.7735,96.66667,105.8308,96.76794,105.8863,96.87019,105.94,96.9734,105.992,97.07753,106.0421,97.18254,106.0903,97.28842,106.1367,97.39513,106.1812,97.50262,106.2239,97.61088,106.2646,97.71987],strokeColor=Color(0,0,0,1),strokeWidth=.526316,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None,fillColor=Color(0,0,0,1)))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/render-out/Drawing08.gif` & `reportlab-4.1.0/tests/render-out/Drawing08.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing08.jpg` & `reportlab-4.1.0/tests/render-out/Drawing08.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing08.png` & `reportlab-4.1.0/tests/render-out/Drawing08.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing09.gif` & `reportlab-4.1.0/tests/render-out/Drawing09.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing09.jpg` & `reportlab-4.1.0/tests/render-out/Drawing09.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing09.png` & `reportlab-4.1.0/tests/render-out/Drawing09.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing09.py` & `reportlab-4.1.0/tests/render-out/autoclose-pdf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Rect
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Path
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
-	def __init__(self,width=400,height=200,*args,**kw):
+class ExplodedDrawing_AutoCloseDrawing(_DrawingEditorMixin,Drawing):
+	def __init__(self,width=100.0,height=100.0,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(String(20,20,'I should be totally horizontal and enclosed in a box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
-		self.add(Rect(18,18,249.64,16,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 		v0=self._nn(Group())
-		v0.transform = (.965926,.258819,-0.258819,.965926,0,50)
-		v0.add(String(20,20,'I should slope up by 15 degrees, so my right end is higher than my left',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
-		v0.add(Rect(18,18,342.64,16,rx=0,ry=0,fillColor=None,fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		v0.transform = (1,0,0,-1,0,100)
+		v1=v0._nn(Group())
+		v1.transform = (1,0,0,-1,0,100)
+		v1.add(Path(points=[10,10,10,90,20,90,20,10,30,10,30,90,40,90,40,10,50,10,50,90,60,90,60,10,70,10,70,90,80,90,80,10],operators=[0,1,1,1,3,0,1,1,1,0,1,1,1,3,0,1,1,1],isClipPath=0,autoclose='pdf',fillMode=1,fillColor=Color(0,0,1,1),fillOpacity=1,strokeColor=Color(1,0,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_AutoCloseDrawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/render-out/Drawing10.gif` & `reportlab-4.1.0/tests/render-out/Drawing10.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing10.jpg` & `reportlab-4.1.0/tests/render-out/Drawing10.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing10.png` & `reportlab-4.1.0/tests/render-out/Drawing10.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing10.py` & `reportlab-4.1.0/tests/render-out/textmode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 #Autogenerated by ReportLab guiedit do not edit
-from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Rect, String
+from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, String, Line, Path
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
-class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
+class ExplodedDrawing_TextRenderModeDrawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,25,25)
-		v0.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v0.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,25,25)
-		v1=v0._nn(Group())
-		v1.transform = (1,0,0,1,25,25)
-		v1.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v1.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
-		v0=self._nn(Group())
-		v0.transform = (1,0,0,1,25,25)
-		v1=v0._nn(Group())
-		v1.transform = (1,0,0,1,25,25)
-		v2=v1._nn(Group())
-		v2.transform = (1,0,0,1,25,25)
-		v2.add(Rect(0,0,100,20,rx=0,ry=0,fillColor=Color(1,1,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		v2.add(String(5,5,'Text in the box',textAnchor='start',fontName='Times-Roman',fontSize=12,fillColor=Color(0,0,0,1)))
+		self.add(String(65,10,'text0',textAnchor='start',fontName='Helvetica',fontSize=80,fillColor=Color(0,0,1,1),strokeColor=Color(1,0,0,1),strokeWidth=1.5,textRenderMode=0))
+		self.add(String(405,20,'text1',textAnchor='end',fontName='Helvetica',fontSize=80,fillColor=Color(0,0,1,1),strokeColor=Color(1,0,0,1),strokeWidth=1.5,textRenderMode=1))
+		self.add(String(190,90,'text2',textAnchor='start',fontName='Helvetica',fontSize=80,fillColor=Color(0,0,1,1),strokeColor=Color(1,0,0,1),strokeWidth=1.5,textRenderMode=2))
+		self.add(String(240,150,'text3',textAnchor='start',fontName='Helvetica',fontSize=40,fillColor=Color(0,.501961,0,1),strokeColor=Color(1,0,1,1),strokeWidth=.5,textRenderMode=2))
+		self.add(String(140,150,'text4',textAnchor='start',fontName='Helvetica',fontSize=40,fillColor=Color(0,.501961,0,1),strokeColor=Color(1,0,1,1),strokeWidth=.5,textRenderMode=1))
+		self.add(String(70,120,'text5',textAnchor='start',fontName='Helvetica',fontSize=40,fillColor=Color(0,.501961,0,1),strokeColor=Color(1,0,1,1),strokeWidth=.5,textRenderMode=0))
+		self.add(Line(40,40,70,70,strokeColor=Color(0,.501961,0,1),strokeWidth=.5,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Path(points=[80,80,110,110,80,110],operators=[0,1,1,3],isClipPath=0,autoclose=None,fillMode=0,fillColor=None,fillOpacity=None,strokeColor=Color(1,1,0,1),strokeWidth=2,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
-	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
+	ExplodedDrawing_TextRenderModeDrawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/render-out/Drawing11.gif` & `reportlab-4.1.0/tests/render-out/Drawing11.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing11.jpg` & `reportlab-4.1.0/tests/render-out/Drawing11.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing11.png` & `reportlab-4.1.0/tests/render-out/Drawing11.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing12.gif` & `reportlab-4.1.0/tests/render-out/Drawing12.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing12.jpg` & `reportlab-4.1.0/tests/render-out/Drawing12.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing12.png` & `reportlab-4.1.0/tests/render-out/Drawing12.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing12.py` & `reportlab-4.1.0/tests/render-out/Drawing12.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing14.gif` & `reportlab-4.1.0/tests/render-out/Drawing14.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing14.jpg` & `reportlab-4.1.0/tests/render-out/Drawing14.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing14.png` & `reportlab-4.1.0/tests/render-out/Drawing14.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/Drawing14.py` & `reportlab-4.1.0/tests/render-out/Drawing14.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 from reportlab.graphics.shapes import _DrawingEditorMixin, Drawing, Group, Image
 from reportlab.lib.colors import Color, CMYKColor, PCMYKColor
 
 class ExplodedDrawing_Drawing(_DrawingEditorMixin,Drawing):
 	def __init__(self,width=400,height=200,*args,**kw):
 		Drawing.__init__(self,width,height,*args,**kw)
 		self.transform = (1,0,0,1,0,0)
-		self.add(Image(0,0,None,None,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7FAD50305FD0>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
-		self.add(Image(380,186,20,14,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7FAD503062A0>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Image(0,0,None,None,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7EFDB125E350>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
+		self.add(Image(380,186,20,14,<PIL.GifImagePlugin.GifImageFile image mode=P size=10x7 at 0x7EFDB125F450>,fillColor=Color(0,0,0,1),fillOpacity=None,strokeColor=Color(0,0,0,1),strokeWidth=1,strokeLineCap=0,strokeLineJoin=0,strokeMiterLimit=0,strokeDashArray=None,strokeOpacity=None))
 
 
 if __name__=="__main__": #NORUNTESTS
 	ExplodedDrawing_Drawing().save(formats=['pdf'],outDir='.',fnRoot=None)
```

### Comparing `reportlab-4.0.9/tests/render-out/autoclose-none.py` & `reportlab-4.1.0/tests/render-out/autoclose-none.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/fillmode-even-odd.png` & `reportlab-4.1.0/tests/render-out/fillmode-even-odd.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/fillmode-non-zero.png` & `reportlab-4.1.0/tests/render-out/fillmode-non-zero.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/hatch.png` & `reportlab-4.1.0/tests/render-out/hatch.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/hatch.py` & `reportlab-4.1.0/tests/render-out/hatch.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/svglib-issue104.png` & `reportlab-4.1.0/tests/render-out/svglib-issue104.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/render-out/textmode.png` & `reportlab-4.1.0/tests/render-out/textmode.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/rltw-icon-tr.png` & `reportlab-4.1.0/tests/rltw-icon-tr.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/runAll.py` & `reportlab-4.1.0/tests/runAll.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/solid_red_alpha.png` & `reportlab-4.1.0/tests/solid_red_alpha.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_charts_textlabels.py` & `reportlab-4.1.0/tests/test_charts_textlabels.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_crypto_algorithms.py` & `reportlab-4.1.0/tests/test_crypto_algorithms.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_docs_build.py` & `reportlab-4.1.0/tests/test_docs_build.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_docstrings.py` & `reportlab-4.1.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_extra.py` & `reportlab-4.1.0/tests/test_extra.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_geomutils.py` & `reportlab-4.1.0/tests/test_geomutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_barcode.py` & `reportlab-4.1.0/tests/test_graphics_barcode.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_charts.py` & `reportlab-4.1.0/tests/test_graphics_charts.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_images-cairo.gif` & `reportlab-4.1.0/tests/test_graphics_images.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_images-cairo.png` & `reportlab-4.1.0/tests/test_graphics_images.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_images.py` & `reportlab-4.1.0/tests/test_graphics_images.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_layout.py` & `reportlab-4.1.0/tests/test_graphics_layout.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_render.py` & `reportlab-4.1.0/tests/test_graphics_render.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_graphics_speed.py` & `reportlab-4.1.0/tests/test_graphics_speed.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_hello.py` & `reportlab-4.1.0/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_images.py` & `reportlab-4.1.0/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_invariant.py` & `reportlab-4.1.0/tests/test_invariant.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_issues.py` & `reportlab-4.1.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_colors.py` & `reportlab-4.1.0/tests/test_lib_colors.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_normaldate.py` & `reportlab-4.1.0/tests/test_lib_normaldate.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_pdfencrypt.py` & `reportlab-4.1.0/tests/test_lib_pdfencrypt.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_rl_safe_eval.py` & `reportlab-4.1.0/tests/test_lib_rl_safe_eval.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_sequencer.py` & `reportlab-4.1.0/tests/test_lib_sequencer.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_utils.py` & `reportlab-4.1.0/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_lib_validators.py` & `reportlab-4.1.0/tests/test_lib_validators.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_multibyte_chs.py` & `reportlab-4.1.0/tests/test_multibyte_chs.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_multibyte_cht.py` & `reportlab-4.1.0/tests/test_multibyte_cht.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_multibyte_jpn.py` & `reportlab-4.1.0/tests/test_multibyte_jpn.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_multibyte_kor.py` & `reportlab-4.1.0/tests/test_multibyte_kor.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_paragraphs.py` & `reportlab-4.1.0/tests/test_paragraphs.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_encodings.py` & `reportlab-4.1.0/tests/test_pdfbase_encodings.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_fontembed.py` & `reportlab-4.1.0/tests/test_pdfbase_fontembed.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_pdfdoc.py` & `reportlab-4.1.0/tests/test_pdfbase_pdfdoc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_pdfform.py` & `reportlab-4.1.0/tests/test_pdfbase_pdfform.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_pdfmetrics.py` & `reportlab-4.1.0/tests/test_pdfbase_pdfmetrics.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_pdfutils.py` & `reportlab-4.1.0/tests/test_pdfbase_pdfutils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_postscript.py` & `reportlab-4.1.0/tests/test_pdfbase_postscript.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfbase_ttfonts.py` & `reportlab-4.1.0/tests/test_pdfbase_ttfonts.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     c.drawString(100,700, 'Unicode TrueType Font Test %d pages' % npages)
     # Draw a table of Unicode characters
     for p in range(npages):
         for fontName in fonts:
             c.setFont(fontName, 10)
             for i in range(32):
                 for j in range(32):
-                    ch = utf8(i * 32 + j+p*alter)
+                    ch = chr(i * 32 + j+p*alter)
                     c.drawString(80 + j * 13 + int(j / 16.0) * 4, 600 - i * 13 - int(i / 8.0) * 8, ch)
         c.showPage()
     c.save()
 
 def show_all_glyphs(fn,fontName='Vera'):
     c = Canvas(outputfile(fn))
     c.setFont('Helvetica', 20)
@@ -302,57 +302,67 @@
             self.assertEqual(coord, 0)
         pdfmetrics.registerFont(font)
         _simple_subset_generation('test_pdfbase_ttffonts_invisible.pdf',2,fonts=('invisible',))
 
     def testSplitString(self):
         "Tests TTFont.splitString"
         doc = PDFDocument()
-        font = TTFont("Vera", "Vera.ttf")
-        text = b"".join(utf8(i) for i in range(511))
-        allchars = b"".join(int2Byte(i) for i in range(256))
+        font = TTFont("Vera", "Vera.ttf", asciiReadable=True)
+        T = list(range(256))
+        for c in sorted(font.face.charToGlyph):
+            if c not in T: T.append(c)
+        text = "".join(map(chr,T))
         #we ignore rserveTTFNotDef by assuming it's always True
         #PDFUA forbids index 0(.notdef) in strings
-        chunks = [(0, allchars[:0xa0]+b' '+allchars[0xa0:])] + [
-                (1, allchars[1:32] + allchars[33:])]# if rl_config.reserveTTFNotdef else
-                #(1, allchars[:32] + allchars[33:-1])]
+        chunks = [(0,
+            b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+            b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00 !"#$%&\''
+            b'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\\]^_`abcdefghijklmno'
+            b'pqrstuvwxyz{|}~\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+            b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+            b'\x00\x00\x00\x00 \x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f'
+            b'\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f'
+            b'\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f'
+            b'\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f'
+            b'\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf'
+            b'\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf'
+            b'\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf'
+            b'\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf'
+            b'\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef'
+            b'\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'),
+         (1,
+            b'\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14'
+            b'\x15\x16\x17\x18\x19\x1a\x1b\x1c')]
         self.assertEqual(font.splitString(text, doc), chunks)
         # Do it twice
         self.assertEqual(font.splitString(text, doc), chunks)
 
-        text = b"".join(utf8(i) for i in range(510, -1, -1))
-        revver = lambda b: map(int2Byte,reversed(b))
-        chunks = [(i[0],b"".join(revver(i[1]))) for i in reversed(chunks)]
-        self.assertEqual(font.splitString(text, doc), chunks)
-
     def testSplitStringSpaces(self):
         # In order for justification (word spacing) to work, the space
         # glyph must have a code 32, and no other character should have
         # that code in any subset, or word spacing will be applied to it.
 
         doc = PDFDocument()
         font = TTFont("Vera", "Vera.ttf")
         text = b"".join(utf8(i) for i in range(512, -1, -1))
         chunks = font.splitString(text, doc)
         state = font.state[doc]
         self.assertEqual(state.assignments[32], 32)
         self.assertEqual(state.subsets[0][32], 32)
-        self.assertEqual(state.subsets[1][32], 32)
 
     def testSubsetInternalName(self):
         "Tests TTFont.getSubsetInternalName"
         doc = PDFDocument()
         font = TTFont("Vera", "Vera.ttf")
         # Actually generate some subsets
         text = b"".join(utf8(i) for i in range(513))
         font.splitString(text, doc)
         self.assertRaises(IndexError, font.getSubsetInternalName, -1, doc)
         self.assertRaises(IndexError, font.getSubsetInternalName, 3, doc)
         self.assertEqual(font.getSubsetInternalName(0, doc), "/F1+0")
-        self.assertEqual(font.getSubsetInternalName(1, doc), "/F1+1")
-        self.assertEqual(font.getSubsetInternalName(2, doc), "/F1+2")
         self.assertEqual(doc.delayedFonts, [font])
 
     def testAddObjectsEmpty(self):
         "TTFont.addObjects should not fail when no characters were used"
         font = TTFont("Vera", "Vera.ttf")
         doc = PDFDocument()
         font.addObjects(doc)
@@ -369,54 +379,47 @@
         self.assertEqual(font.nextCode, 0)
         self.assertEqual(font.subsets, [])
         self.assertEqual(font.assignments, {})
         font.splitString('ba', doc)           # should work
 
     def testParallelConstruction(self):
         "Test that TTFont can be used for different documents at the same time"
-        ttfAsciiReadable = rl_config.ttfAsciiReadable
-        try:
-            rl_config.ttfAsciiReadable = 1
-            doc1 = PDFDocument()
-            doc2 = PDFDocument()
-            font = TTFont("Vera", "Vera.ttf")
-            self.assertEqual(font.splitString('hello ', doc1), [(0, b'hello ')])
-            self.assertEqual(font.splitString('hello ', doc2), [(0, b'hello ')])
-            self.assertEqual(font.splitString(u'\u0410\u0411'.encode('UTF-8'), doc1), [(0, b'\x80\x81')])
-            self.assertEqual(font.splitString(u'\u0412'.encode('UTF-8'), doc2), [(0, b'\x80')])
-            font.addObjects(doc1)
-            self.assertEqual(font.splitString(u'\u0413'.encode('UTF-8'), doc2), [(0, b'\x81')])
-            font.addObjects(doc2)
-        finally:
-            rl_config.ttfAsciiReadable = ttfAsciiReadable
+        doc1 = PDFDocument()
+        doc2 = PDFDocument()
+        font = TTFont("Vera", "Vera.ttf", asciiReadable=1)
+        self.assertEqual(font.splitString('hello ', doc1), [(0, b'hello ')])
+        self.assertEqual(font.splitString('hello ', doc2), [(0, b'hello ')])
+        self.assertEqual(font.splitString('\xae\xab', doc1), [(0, b'\x01\x02')])
+        self.assertEqual(font.splitString('\xab\xae', doc2), [(0, b'\x01\x02')])
+        self.assertEqual(font.splitString('\xab\xae', doc1), [(0, b'\x02\x01')])
+        self.assertEqual(font.splitString('\xae\xab', doc2), [(0, b'\x02\x01')])
+        font.addObjects(doc1)
+        #after addObjects doc1 state is no longer valid, doc2 should be OK
+        self.assertEqual(font.splitString('\xae\xab', doc2), [(0, b'\x02\x01')])
+        font.addObjects(doc2)
 
     def testAddObjects(self):
         "Test TTFont.addObjects"
         # Actually generate some subsets
-        ttfAsciiReadable = rl_config.ttfAsciiReadable
-        try:
-            rl_config.ttfAsciiReadable = 1
-            doc = PDFDocument()
-            font = TTFont("Vera", "Vera.ttf")
-            font.splitString('a', doc)            # create some subset
-            internalName = font.getSubsetInternalName(0, doc)[1:]
-            font.addObjects(doc)
-            pdfFont = doc.idToObject[internalName]
-            self.assertEqual(doc.idToObject['BasicFonts'].dict[internalName], pdfFont)
-            self.assertEqual(pdfFont.Name, internalName)
-            self.assertEqual(pdfFont.BaseFont, "AAAAAA+BitstreamVeraSans-Roman")
-            self.assertEqual(pdfFont.FirstChar, 0)
-            self.assertEqual(pdfFont.LastChar, 127)
-            self.assertEqual(len(pdfFont.Widths.sequence), 128)
-            toUnicode = doc.idToObject[pdfFont.ToUnicode.name]
-            self.assertTrue(toUnicode.content != "")
-            fontDescriptor = doc.idToObject[pdfFont.FontDescriptor.name]
-            self.assertEqual(fontDescriptor.dict['Type'], '/FontDescriptor')
-        finally:
-            rl_config.ttfAsciiReadable = ttfAsciiReadable
+        doc = PDFDocument()
+        font = TTFont("Vera", "Vera.ttf", asciiReadable=1)
+        font.splitString('a', doc)            # create some subset
+        internalName = font.getSubsetInternalName(0, doc)[1:]
+        font.addObjects(doc)
+        pdfFont = doc.idToObject[internalName]
+        self.assertEqual(doc.idToObject['BasicFonts'].dict[internalName], pdfFont)
+        self.assertEqual(pdfFont.Name, internalName)
+        self.assertEqual(pdfFont.BaseFont, "AAAAAA+BitstreamVeraSans-Roman")
+        self.assertEqual(pdfFont.FirstChar, 0)
+        self.assertEqual(pdfFont.LastChar, 127)
+        self.assertEqual(len(pdfFont.Widths.sequence), 128)
+        toUnicode = doc.idToObject[pdfFont.ToUnicode.name]
+        self.assertTrue(toUnicode.content != "")
+        fontDescriptor = doc.idToObject[pdfFont.FontDescriptor.name]
+        self.assertEqual(fontDescriptor.dict['Type'], '/FontDescriptor')
 
     def testMakeToUnicodeCMap(self):
         "Test makeToUnicodeCMap"
         self.assertEqual(makeToUnicodeCMap("TestFont", [ 0x1234, 0x4321, 0x4242 ]),
 """/CIDInit /ProcSet findresource begin
 12 dict begin
 begincmap
```

### Comparing `reportlab-4.0.9/tests/test_pdfgen_callback.py` & `reportlab-4.1.0/tests/test_pdfgen_callback.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfgen_general.py` & `reportlab-4.1.0/tests/test_pdfgen_general.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfgen_links.py` & `reportlab-4.1.0/tests/test_pdfgen_links.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfgen_overprint.py` & `reportlab-4.1.0/tests/test_pdfgen_overprint.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pdfgen_pagemodes.py` & `reportlab-4.1.0/tests/test_pdfgen_pagemodes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_accum.py` & `reportlab-4.1.0/tests/test_platypus_accum.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_breaking.py` & `reportlab-4.1.0/tests/test_platypus_breaking.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from operator import truth
 import unittest
 from reportlab.platypus.flowables import Flowable, KeepTogether, KeepTogetherSplitAtTop
 from reportlab.lib import colors
 from reportlab.lib.units import cm, mm
 from reportlab.lib.enums import TA_LEFT, TA_RIGHT, TA_CENTER, TA_JUSTIFY
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
-from reportlab.platypus import ShowBoundaryValue
 from reportlab.platypus.frames import Frame
 from reportlab.lib.randomtext import randomText, PYTHON
 from reportlab.platypus.doctemplate import PageTemplate, BaseDocTemplate, Indenter, SimpleDocTemplate, LayoutError
 from reportlab.platypus.paragraph import *
-from reportlab.pdfgen.canvas import Canvas
+from reportlab.pdfgen.canvas import Canvas, ShowBoundaryValue
 from reportlab.rl_config import paraFontSizeHeightOffset
 from reportlab.pdfbase.pdfmetrics import stringWidth
 from reportlab.lib.pagesizes import A4, portrait
 
 def myMainPageFrame(canvas, doc):
     "The page frame used for all PDF documents."
```

### Comparing `reportlab-4.0.9/tests/test_platypus_cjk_wrap.py` & `reportlab-4.1.0/tests/test_platypus_cjk_wrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from reportlab.lib.testutils import setOutDir,makeSuiteForClasses, outputfile, printLocation
 setOutDir(__name__)
 import sys, os, unittest
 
 from reportlab.platypus.paragraph import Paragraph
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.platypus.doctemplate import PageTemplate, BaseDocTemplate, PageBreak, NextPageTemplate
-from reportlab.platypus.frames import Frame, ShowBoundaryValue
+from reportlab.platypus.frames import Frame
+from reportlab.pdfgen.canvas import ShowBoundaryValue
 from reportlab.lib.colors import Color
 from reportlab.lib.units import cm
 from reportlab.lib.enums import TA_LEFT, TA_RIGHT, TA_CENTER, TA_JUSTIFY
 
 from reportlab.pdfbase.cidfonts import CIDFont, findCMapFile, UnicodeCIDFont
 from reportlab.pdfbase import pdfmetrics
```

### Comparing `reportlab-4.0.9/tests/test_platypus_general.py` & `reportlab-4.1.0/tests/test_platypus_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 builds a special "document model" in which the frames are added to each page
 and drawn into.
 """
 from reportlab.lib.testutils import setOutDir,makeSuiteForClasses, outputfile, printLocation, mockUrlRead
 from unittest.mock import patch
 setOutDir(__name__)
 import copy, sys, os
-from reportlab.pdfgen import canvas
+from reportlab.pdfgen.canvas import ShowBoundaryValue
 from reportlab import platypus
 from reportlab.platypus import BaseDocTemplate, PageTemplate, Flowable, FrameBreak, KeepTogether, PageBreak, Spacer
 from reportlab.platypus import Paragraph, Preformatted
 from reportlab.platypus import SimpleDocTemplate
 from reportlab.lib.units import inch, cm
 from reportlab.lib.styles import PropertySet, getSampleStyleSheet, ParagraphStyle
 from reportlab.lib import colors
@@ -601,24 +601,23 @@
         story = [Paragraph("The section header", header), d,
                 ]
         doc = SimpleDocTemplate(outputfile('test_drawing_keepwithnext.pdf'))
         doc.build(story)
 
     def test2(self):
         '''ensure showBoundaryValue works as expected'''
-        from reportlab.platypus.frames import ShowBoundaryValue
         assert (1 if ShowBoundaryValue(width=1) else 0) == 1
         assert (1 if ShowBoundaryValue(color=None,width=1) else 0) == 0
         assert (1 if ShowBoundaryValue(width=-1) else 0) == 0
         assert bool(ShowBoundaryValue(width=1)) == True
         assert bool(ShowBoundaryValue(color=None,width=1)) == False
         assert bool(ShowBoundaryValue(width=-1)) == False
 
     def test3(Self):
-        from reportlab.platypus import BalancedColumns, IndexingFlowable, ShowBoundaryValue, NullDraw
+        from reportlab.platypus import BalancedColumns, IndexingFlowable, NullDraw
         doc = SimpleDocTemplate(outputfile('test_balancedcolumns.pdf'))
         styleSheet = getSampleStyleSheet()
 
         class MyIndexingNull(IndexingFlowable, NullDraw):
             _ZEROSIZE = True
             def __init__(self,*args,**kwds):
                 IndexingFlowable.__init__(self,*args,**kwds)
```

### Comparing `reportlab-4.0.9/tests/test_platypus_images.py` & `reportlab-4.1.0/tests/test_platypus_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     furl = fn.replace(os.sep,'/')
     if sys.platform=='win32' and furl[1]==':': furl = furl[0]+'|'+furl[2:]
     if furl[0]!='/': furl = '/'+furl
     return 'file://'+furl
 
 def run():
     from reportlab.platypus import  BaseDocTemplate, PageTemplate, Image, Frame, PageTemplate, \
-                                    ShowBoundaryValue, SimpleDocTemplate, FrameBG, Paragraph, \
-                                    FrameBreak
+                                    SimpleDocTemplate, FrameBG, Paragraph, FrameBreak
     from reportlab.lib.colors import toColor
     from reportlab.lib.utils import _RL_DIR, rl_isfile, open_for_read, fileName2FSEnc, asNative
     from reportlab.lib.styles import getSampleStyleSheet
     styleSheet = getSampleStyleSheet()
     _GIF = os.path.join(testsFolder,'pythonpowered.gif')
     if not rl_isfile(_GIF): _GIF = None
     _GAPNG = os.path.join(testsFolder,'gray-alpha.png')
```

### Comparing `reportlab-4.0.9/tests/test_platypus_indents.py` & `reportlab-4.1.0/tests/test_platypus_indents.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from reportlab.platypus.paragraph import Paragraph
 from reportlab.platypus.frames import Frame
 from reportlab.platypus.doctemplate \
      import PageTemplate, BaseDocTemplate, Indenter, FrameBreak, NextPageTemplate
 from reportlab.platypus.tables import TableStyle, Table
 from reportlab.platypus.paragraph import *
 from reportlab.platypus.paragraph import _getFragWords
-from reportlab.platypus import FrameBG, FrameSplitter, Frame, Spacer, ShowBoundaryValue
-
+from reportlab.platypus import FrameBG, FrameSplitter, Frame, Spacer
+from reportlab.pdfgen.canvas  import ShowBoundaryValue
 
 def myMainPageFrame(canvas, doc):
     "The page frame used for all PDF documents."
 
     canvas.saveState()
 
     canvas.rect(2.5*cm, 2.5*cm, 15*cm, 25*cm)
```

### Comparing `reportlab-4.0.9/tests/test_platypus_index.py` & `reportlab-4.1.0/tests/test_platypus_index.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_leftright.py` & `reportlab-4.1.0/tests/test_platypus_leftright.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_lists.py` & `reportlab-4.1.0/tests/test_platypus_lists.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_paragraphs.py` & `reportlab-4.1.0/tests/test_platypus_paragraphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 """Tests for the reportlab.platypus.paragraphs module.
 """
 __version__='3.3.0'
 from reportlab.lib.testutils import setOutDir,makeSuiteForClasses, outputfile, printLocation, rlSkipUnless
 setOutDir(__name__)
 import sys, os, unittest
 from operator import truth
-from reportlab.pdfgen.canvas import Canvas
+from reportlab.pdfgen.canvas import Canvas, ShowBoundaryValue
 from reportlab.pdfbase.pdfmetrics import stringWidth, registerFont, registerFontFamily
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.platypus.paraparser import ParaParser
 from reportlab.platypus.flowables import Flowable, DocAssert
 from reportlab.lib.colors import Color
 from reportlab.lib.units import cm
 from reportlab.lib.enums import TA_LEFT, TA_RIGHT, TA_CENTER, TA_JUSTIFY
 from reportlab.lib.utils import _className, asBytes, asUnicode, asNative
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.platypus.xpreformatted import XPreformatted
-from reportlab.platypus.frames import Frame, ShowBoundaryValue
+from reportlab.platypus import Frame
 from reportlab.platypus.doctemplate import PageTemplate, BaseDocTemplate, PageBreak, NextPageTemplate
 from reportlab.platypus import tableofcontents
 from reportlab.platypus.tableofcontents import TableOfContents
 from reportlab.platypus.tables import TableStyle, Table
 from reportlab.platypus.paragraph import Paragraph, _getFragWords, _splitWord, _fragWordSplitRep, ABag, pyphen
 from reportlab.rl_config import rtlSupport, trustedHosts, trustedSchemes
 
@@ -167,15 +167,15 @@
         self.assertTrue(
                 uj == u
                 and uj._shyIndices==u._shyIndices, '_shyUnsplit failed')
 
     def test5(self):
         '''some soft hyphenation'''
         from reportlab.pdfgen import canvas
-        from reportlab.platypus import Frame, ShowBoundaryValue, Paragraph
+        from reportlab.platypus import Frame, Paragraph
         from reportlab.lib.styles import ParagraphStyle
 
         pagesize = (80+20, 400)
         c = canvas.Canvas(  outputfile('test_platypus_soft_hyphenation.pdf'), pagesize=pagesize)
         f = Frame(10, 0, 68, 400,
                 showBoundary=ShowBoundaryValue(dashArray=(1,1)),
                 leftPadding=0,
```

### Comparing `reportlab-4.0.9/tests/test_platypus_paraparser.py` & `reportlab-4.1.0/tests/test_platypus_paraparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_pleaseturnover.py` & `reportlab-4.1.0/tests/test_platypus_pleaseturnover.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_preformatted.py` & `reportlab-4.1.0/tests/test_platypus_preformatted.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_programming.py` & `reportlab-4.1.0/tests/test_platypus_programming.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_tables.py` & `reportlab-4.1.0/tests/test_platypus_tables.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_toc.py` & `reportlab-4.1.0/tests/test_platypus_toc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_wrapping.py` & `reportlab-4.1.0/tests/test_platypus_wrapping.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_platypus_xref.py` & `reportlab-4.1.0/tests/test_platypus_xref.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_pyfiles.py` & `reportlab-4.1.0/tests/test_pyfiles.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_renderPS.py` & `reportlab-4.1.0/tests/test_renderPS.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_renderSVG.py` & `reportlab-4.1.0/tests/test_renderSVG.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_rl_accel.py` & `reportlab-4.1.0/tests/test_rl_accel.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_source_chars.py` & `reportlab-4.1.0/tests/test_source_chars.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_table_inrowsplit.py` & `reportlab-4.1.0/tests/test_table_inrowsplit.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_table_layout.py` & `reportlab-4.1.0/tests/test_table_layout.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_tools_pythonpoint.py` & `reportlab-4.1.0/tests/test_tools_pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_utils.py` & `reportlab-4.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_widgetbase_tpc.py` & `reportlab-4.1.0/tests/test_widgetbase_tpc.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tests/test_widgets_grids.py` & `reportlab-4.1.0/tests/test_widgets_grids.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/codegrab.py` & `reportlab-4.1.0/tools/docco/codegrab.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/docpy.py` & `reportlab-4.1.0/tools/docco/docpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/examples.py` & `reportlab-4.1.0/tools/docco/examples.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/graphdocpy.py` & `reportlab-4.1.0/tools/docco/graphdocpy.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/rl_doc_utils.py` & `reportlab-4.1.0/tools/docco/rl_doc_utils.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/rltemplate.py` & `reportlab-4.1.0/tools/docco/rltemplate.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/stylesheet.py` & `reportlab-4.1.0/tools/docco/stylesheet.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/t_parse.py` & `reportlab-4.1.0/tools/docco/t_parse.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/yaml.py` & `reportlab-4.1.0/tools/docco/yaml.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/docco/yaml2pdf.py` & `reportlab-4.1.0/tools/docco/yaml2pdf.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pdfpath.py` & `reportlab-4.1.0/tools/pdfpath.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/README` & `reportlab-4.1.0/tools/pythonpoint/README`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/customshapes.py` & `reportlab-4.1.0/tools/pythonpoint/customshapes.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/examples.py` & `reportlab-4.1.0/tools/pythonpoint/demos/examples.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/figures.xml` & `reportlab-4.1.0/tools/pythonpoint/demos/figures.xml`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/htu.xml` & `reportlab-4.1.0/tools/pythonpoint/demos/htu.xml`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/leftlogo.a85` & `reportlab-4.1.0/tools/pythonpoint/demos/leftlogo.a85`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/leftlogo.gif` & `reportlab-4.1.0/tools/pythonpoint/demos/leftlogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/lj8100.jpg` & `reportlab-4.1.0/tools/pythonpoint/demos/lj8100.jpg`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/monterey.xml` & `reportlab-4.1.0/tools/pythonpoint/demos/monterey.xml`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/outline.gif` & `reportlab-4.1.0/tools/pythonpoint/demos/outline.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/pplogo.gif` & `reportlab-4.1.0/tools/pythonpoint/demos/pplogo.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/python.gif` & `reportlab-4.1.0/tools/pythonpoint/demos/python.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/pythonpoint.xml` & `reportlab-4.1.0/tools/pythonpoint/demos/pythonpoint.xml`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/slidebox.py` & `reportlab-4.1.0/tools/pythonpoint/demos/slidebox.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/spectrum.png` & `reportlab-4.1.0/tools/pythonpoint/demos/spectrum.png`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/demos/vertpython.gif` & `reportlab-4.1.0/tools/pythonpoint/demos/vertpython.gif`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/pythonpoint.dtd` & `reportlab-4.1.0/tools/pythonpoint/pythonpoint.dtd`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/pythonpoint.py` & `reportlab-4.1.0/tools/pythonpoint/pythonpoint.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/stdparser.py` & `reportlab-4.1.0/tools/pythonpoint/stdparser.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/styles/horrible.py` & `reportlab-4.1.0/tools/pythonpoint/styles/horrible.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/styles/htu.py` & `reportlab-4.1.0/tools/pythonpoint/styles/htu.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/styles/modern.py` & `reportlab-4.1.0/tools/pythonpoint/styles/modern.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/styles/projection.py` & `reportlab-4.1.0/tools/pythonpoint/styles/projection.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/pythonpoint/styles/standard.py` & `reportlab-4.1.0/tools/pythonpoint/styles/standard.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/utils/add_bleed.py` & `reportlab-4.1.0/tools/utils/add_bleed.py`

 * *Files identical despite different names*

### Comparing `reportlab-4.0.9/tools/utils/dumpttf.py` & `reportlab-4.1.0/tools/utils/dumpttf.py`

 * *Files identical despite different names*

