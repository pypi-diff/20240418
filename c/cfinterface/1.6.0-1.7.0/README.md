# Comparing `tmp/cfinterface-1.6.tar.gz` & `tmp/cfinterface-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.6.tar", last modified: Fri Apr 12 20:29:53 2024, max compression
+gzip compressed data, was "cfinterface-1.7.0.tar", last modified: Thu Apr 18 20:06:35 2024, max compression
```

## Comparing `cfinterface-1.6.tar` & `cfinterface-1.7.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 20:28:51.000000 cfinterface-1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-12 20:29:53.058245 cfinterface-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-12 20:28:51.000000 cfinterface-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.042245 cfinterface-1.6/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-12 20:29:53.000000 cfinterface-1.6/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:29:53.058245 cfinterface-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 20:28:51.000000 cfinterface-1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 20:05:24.000000 cfinterface-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-18 20:06:35.782373 cfinterface-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 20:05:24.000000 cfinterface-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.770373 cfinterface-1.7.0/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-18 20:05:24.000000 cfinterface-1.7.0/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-18 20:06:35.000000 cfinterface-1.7.0/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-18 20:06:35.000000 cfinterface-1.7.0/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:06:35.000000 cfinterface-1.7.0/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 20:06:35.000000 cfinterface-1.7.0/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 20:06:35.000000 cfinterface-1.7.0/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.774373 cfinterface-1.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:06:35.782373 cfinterface-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-18 20:05:24.000000 cfinterface-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.778373 cfinterface-1.7.0/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:06:35.782373 cfinterface-1.7.0/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 20:05:24.000000 cfinterface-1.7.0/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.6/LICENSE.md` & `cfinterface-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/PKG-INFO` & `cfinterface-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.6.0
+Version: 1.7.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.6/README.md` & `cfinterface-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.7.0/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/adapters/components/repository.py` & `cfinterface-1.7.0/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/adapters/reading/repository.py` & `cfinterface-1.7.0/cfinterface/adapters/reading/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/adapters/writing/repository.py` & `cfinterface-1.7.0/cfinterface/adapters/writing/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/block.py` & `cfinterface-1.7.0/cfinterface/components/block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/datetimefield.py` & `cfinterface-1.7.0/cfinterface/components/literalfield.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,55 @@
-from datetime import datetime
-import pandas as pd  # type: ignore
 from typing import Optional
-
+import pandas as pd  # type: ignore
 from cfinterface.components.field import Field
 
 
-class DatetimeField(Field):
+class LiteralField(Field):
     """
-    Class for representing an datetime field for being read from and
-    written to a file. The format to read and write the value is given
-    by an optional argument.
+    Class for representing an literal field for being read from and
+    written to a file.
     """
 
-    __slots__ = ["__format"]
+    __slots__ = []
 
     def __init__(
         self,
-        size: int = 16,
+        size: int = 80,
         starting_position: int = 0,
-        format: str = "%Y/%m/%d",
-        value: Optional[datetime] = None,
+        value: Optional[str] = None,
     ) -> None:
         super().__init__(size, starting_position, value)
-        self.__format = format
 
     # Override
-    def _binary_read(self, line: bytes) -> datetime:
-        return datetime.strptime(
+    def _binary_read(self, line: bytes) -> str:
+        return (
             line[self._starting_position : self._ending_position]
             .decode("utf-8")
-            .strip(),
-            self.__format,
+            .strip()
         )
 
     # Override
-    def _textual_read(self, line: str) -> datetime:
-        return datetime.strptime(
-            line[self._starting_position : self._ending_position].strip(),
-            self.__format,
-        )
+    def _textual_read(self, line: str) -> str:
+        return line[self._starting_position : self._ending_position].strip()
 
     # Override
     def _binary_write(self) -> bytes:
         if self.value is None or pd.isnull(self.value):
             return b"".ljust(self.size)
         else:
-            return (
-                self.value.strftime(self.__format)
-                .ljust(self.size)
-                .encode("utf-8")
-            )
+            return self.value.ljust(self.size).encode("utf-8")
 
     # Override
     def _textual_write(self) -> str:
         if self.value is None or pd.isnull(self.value):
             value = ""
         else:
-            value = self.value.strftime(self.__format)
+            value = str(self.value)
         return value.ljust(self._size)
 
     @property
-    def value(self) -> Optional[datetime]:
+    def value(self) -> Optional[str]:
         return self._value
 
     @value.setter
-    def value(self, val: datetime):
+    def value(self, val: str):
         self._value = val
```

### Comparing `cfinterface-1.6/cfinterface/components/defaultblock.py` & `cfinterface-1.7.0/cfinterface/components/defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/defaultregister.py` & `cfinterface-1.7.0/cfinterface/components/defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/defaultsection.py` & `cfinterface-1.7.0/cfinterface/components/defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/field.py` & `cfinterface-1.7.0/cfinterface/components/field.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/floatfield.py` & `cfinterface-1.7.0/cfinterface/components/floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/integerfield.py` & `cfinterface-1.7.0/cfinterface/components/integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/line.py` & `cfinterface-1.7.0/cfinterface/components/line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/register.py` & `cfinterface-1.7.0/cfinterface/components/register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/components/section.py` & `cfinterface-1.7.0/cfinterface/components/section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/data/blockdata.py` & `cfinterface-1.7.0/cfinterface/data/blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/data/registerdata.py` & `cfinterface-1.7.0/cfinterface/data/registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/data/sectiondata.py` & `cfinterface-1.7.0/cfinterface/data/sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/files/blockfile.py` & `cfinterface-1.7.0/cfinterface/files/blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/files/registerfile.py` & `cfinterface-1.7.0/cfinterface/files/registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/files/sectionfile.py` & `cfinterface-1.7.0/cfinterface/files/sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/reading/blockreading.py` & `cfinterface-1.7.0/cfinterface/reading/blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/reading/registerreading.py` & `cfinterface-1.7.0/cfinterface/reading/registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/reading/sectionreading.py` & `cfinterface-1.7.0/cfinterface/reading/sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/writing/blockwriting.py` & `cfinterface-1.7.0/cfinterface/writing/blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/writing/registerwriting.py` & `cfinterface-1.7.0/cfinterface/writing/registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface/writing/sectionwriting.py` & `cfinterface-1.7.0/cfinterface/writing/sectionwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.7.0/cfinterface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.6.0
+Version: 1.7.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.6/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.7.0/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/setup.py` & `cfinterface-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/adapters/components/test_linerepository.py` & `cfinterface-1.7.0/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_block.py` & `cfinterface-1.7.0/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_datetimefield.py` & `cfinterface-1.7.0/tests/components/test_datetimefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,43 @@
     format = "%Y/%m/%d"
     field = DatetimeField(10, 0, format=format)
     line = f"{data}-something-else"
     field.read(line)
     assert field.value == datetime.strptime(data, format)
 
 
+def test_datetimefield_read_format_list():
+    data = "2020/01/10"
+    formats = ["%Y-%m-%d", "%Y/%m/%d"]
+    field = DatetimeField(10, 0, format=formats)
+    line = f"{data}-something-else"
+    field.read(line)
+    assert field.value == datetime.strptime(data, formats[1])
+
+
 def test_datetimefield_write():
     data = "2020/01/10"
     format = "%Y/%m/%d"
     line_before = f"field-{data}-else"
     date_data = datetime.strptime(data, format)
     field = DatetimeField(10, 6, format=format, value=date_data)
     line_after = field.write(line_before)
     assert line_before == line_after
 
 
+def test_datetimefield_write_format_list():
+    data = "2020/01/10"
+    formats = ["%Y-%m-%d", "%Y/%m/%d"]
+    line_before = f"field-{data}-else"
+    date_data = datetime.strptime(data, formats[1])
+    field = DatetimeField(10, 6, format=formats, value=date_data)
+    line_after = field.write(line_before)
+    assert line_before.replace("/", "-") == line_after
+
+
 def test_datetimefield_write_empty():
     field = DatetimeField(5, 0)
     assert len(field.write("")) == 5
 
 
 def test_datetimefield_write_short_line():
     data = "2020/01/10"
```

### Comparing `cfinterface-1.6/tests/components/test_defaultblock.py` & `cfinterface-1.7.0/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_defaultregister.py` & `cfinterface-1.7.0/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_defaultsection.py` & `cfinterface-1.7.0/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_floatfield.py` & `cfinterface-1.7.0/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_integerfield.py` & `cfinterface-1.7.0/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_line.py` & `cfinterface-1.7.0/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_literalfield.py` & `cfinterface-1.7.0/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_register.py` & `cfinterface-1.7.0/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/components/test_section.py` & `cfinterface-1.7.0/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/data/test_blockdata.py` & `cfinterface-1.7.0/tests/data/test_blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/data/test_registerdata.py` & `cfinterface-1.7.0/tests/data/test_registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/data/test_sectiondata.py` & `cfinterface-1.7.0/tests/data/test_sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/files/test_blockfile.py` & `cfinterface-1.7.0/tests/files/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/files/test_registerfile.py` & `cfinterface-1.7.0/tests/files/test_registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/files/test_sectionfile.py` & `cfinterface-1.7.0/tests/files/test_sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/mocks/mock_open.py` & `cfinterface-1.7.0/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/reading/test_blockreading.py` & `cfinterface-1.7.0/tests/reading/test_blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/reading/test_registerreading.py` & `cfinterface-1.7.0/tests/reading/test_registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/reading/test_sectionreading.py` & `cfinterface-1.7.0/tests/reading/test_sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/writing/test_blockwriting.py` & `cfinterface-1.7.0/tests/writing/test_blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/writing/test_registerwriting.py` & `cfinterface-1.7.0/tests/writing/test_registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.6/tests/writing/test_sectionwriting.py` & `cfinterface-1.7.0/tests/writing/test_sectionwriting.py`

 * *Files identical despite different names*

