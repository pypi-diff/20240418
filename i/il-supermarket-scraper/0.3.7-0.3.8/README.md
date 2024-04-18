# Comparing `tmp/il-supermarket-scraper-0.3.7.tar.gz` & `tmp/il_supermarket_scraper-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il-supermarket-scraper-0.3.7.tar", last modified: Fri Feb  2 18:31:05 2024, max compression
+gzip compressed data, was "il_supermarket_scraper-0.3.8.tar", last modified: Thu Apr 18 10:08:10 2024, max compression
```

## Comparing `il-supermarket-scraper-0.3.7.tar` & `il_supermarket_scraper-0.3.8.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.884985 il-supermarket-scraper-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-02-02 18:31:05.884985 il-supermarket-scraper-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.872985 il-supermarket-scraper-0.3.7/il_supermarket_scarper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.876985 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/apsx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/bina.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/cerberus.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/multipage_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/publishprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrapper_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.880985 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/bareket.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/bitan.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/cofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/doralon.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/good_pharm.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/hazihinam.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/het_cohen.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/keshet.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/king_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/maayan2000.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/machsani_ashuk.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/nativ_hashed.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/osherad.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/polizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/quik.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/ramilevy.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/salachdabach.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/shufersal.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/shuk_ahir.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/stop_market.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/super_pharm.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/super_sapir.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/super_yuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/superdosh.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/tivtaam.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/victory.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/yellow.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/yohananof.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/zolvebegadol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.880985 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/gzip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/marking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/retrey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.884985 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-02-02 18:31:05.000000 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-02 18:31:05.000000 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 18:31:05.000000 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-02 18:31:05.000000 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-02 18:31:05.000000 il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-02 18:31:05.884985 il-supermarket-scraper-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 18:31:05.884985 il-supermarket-scraper-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-02 18:30:57.000000 il-supermarket-scraper-0.3.7/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.064190 il_supermarket_scraper-0.3.8/il_supermarket_scarper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.068189 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/apsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/bina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/cerberus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/multipage_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/publishprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrapper_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.072189 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bareket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bitan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/cofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/doralon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/good_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/hazihinam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/het_cohen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/keshet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/king_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/maayan2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/machsani_ashuk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/nativ_hashed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/osherad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/polizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/quik.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/ramilevy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/salachdabach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shefa_barcart_ashem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shufersal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/shuk_ahir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/stop_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_pharm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_sapir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_yuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/superdosh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/tivtaam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/victory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/yellow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/yohananof.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/zolvebegadol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/gzip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/marking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/retrey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 10:08:10.000000 il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:08:10.076190 il_supermarket_scraper-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-18 10:08:01.000000 il_supermarket_scraper-0.3.8/tests/test_main.py
```

### Comparing `il-supermarket-scraper-0.3.7/LICENSE.txt` & `il_supermarket_scraper-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/PKG-INFO` & `il_supermarket_scraper-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.3.7
+Version: 0.3.8
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
@@ -16,20 +16,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: retry==0.9.2
 Requires-Dist: mock==4.0.3
 Requires-Dist: requests==2.31.0
-Requires-Dist: lxml==4.9.1
+Requires-Dist: lxml==5.2.1
 Requires-Dist: beautifulsoup4==4.10.0
 Requires-Dist: pymongo==4.2.0
 Requires-Dist: pytz==2022.4
 Requires-Dist: holidays==0.16
 Requires-Dist: cachetools==5.2.0
+Requires-Dist: pytest-playwright==0.4.4
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 
 Israel Supermarket Scraper: Clients to download the data published by the supermarkets.
 =======================================
 This is a scraper for ALL the supermarket chains listed in the GOV.IL site.
```

### Comparing `il-supermarket-scraper-0.3.7/README.md` & `il_supermarket_scraper-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/apsx.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/apsx.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/bina.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/bina.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/cerberus.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/cerberus.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/engine.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/engine.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/matrix.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/matrix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/multipage_web.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/multipage_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from urllib.parse import urlsplit
 import re
 import ntpath
-import lxml
+from lxml import html as lxml_html
+
 import requests
 
 from il_supermarket_scarper.utils.connection import url_connection_retry
 
 
 from il_supermarket_scarper.utils import (
     Logger,
@@ -40,16 +41,15 @@
         """get the number of pages to scarpe"""
 
         response = requests.get(url, timeout=timeout)
         if response.status_code != 200:
             raise ValueError(
                 f"Fetching resources failed from {url}, status code: {response.status_code}"
             )
-
-        html_body = lxml.html.fromstring(response.content)
+        html_body = lxml_html.fromstring(response.content)
 
         total_pages = self.get_total_pages(html_body)
         Logger.info(f"Found {total_pages} pages")
 
         return total_pages
 
     def get_total_pages(self, html):
@@ -116,15 +116,15 @@
 
     def process_links_before_download(
         self, page, limit=None, files_types=None, store_id=None, only_latest=None
     ):
         """additional processing to the links before download"""
         response = self.session_with_cookies_by_chain(page)
 
-        html = lxml.html.fromstring(response.text)
+        html = lxml_html.fromstring(response.text)
 
         file_links, filenames = self.collect_files_details_from_page(html)
         Logger.info(f"Page {page}: Found {len(file_links)} files")
 
         filenames, file_links = self.apply_limit_zip(
             filenames,
             file_links,
```

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/publishprice.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/publishprice.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/engines/web.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/engines/web.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/main.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/main.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrapper_runner.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrapper_runner.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/__init__.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/bareket.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/bareket.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/cofix.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/cofix.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/nativ_hashed.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/nativ_hashed.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/polizer.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/polizer.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/super_pharm.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/super_pharm.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers/tivtaam.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers/tivtaam.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/scrappers_factory.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/scrappers_factory.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/__init__.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/connection.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 import socket
 import random
 from ftplib import FTP_TLS, error_perm
 import subprocess
 import requests
 
-
+from playwright.sync_api import sync_playwright
 from urllib3.exceptions import ReadTimeoutError
 from requests.exceptions import (
     ReadTimeout,
     ConnectionError as RequestsConnectionError,
     ChunkedEncodingError,
 )
 from cachetools import cached, TTLCache
@@ -205,14 +205,27 @@
         )
 
     if chain_cookie_name and not os.path.exists(f"{chain_cookie_name}_cookies.txt"):
         session.cookies.save()
     return response_content
 
 
+def render_webpage(url, extraction):
+    """render website with playwrite"""
+
+    with sync_playwright() as p:
+        browser = p.chromium.launch()
+        page = browser.new_page()
+        page.goto(url)
+        page.wait_for_load_state("networkidle")
+        content = extraction(page)
+        browser.close()
+    return content
+
+
 @url_connection_retry()
 def session_and_check_status(url, timeout=15):
     """use a session to load the response and check status"""
     return session_with_cookies(url, timeout=timeout)
 
 
 def url_retrieve(url, filename, timeout=30):
```

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/file_types.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/gzip_utils.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/gzip_utils.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/logger.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/loop.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/loop.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/marking.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/marking.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/mongo.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/mongo.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/retrey.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/retrey.py`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scarper/utils/status.py` & `il_supermarket_scraper-0.3.8/il_supermarket_scarper/utils/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 import datetime
 import re
 import os
 import enum
 import holidays
 import pytz
-import lxml.html as lh
-from bs4 import BeautifulSoup
-
 from .logger import Logger
-from .connection import session_with_cookies
+from .connection import render_webpage
 
 
-def get_statue_page():
+def get_statue_page(extraction_type):
     """fetch the gov.il site"""
     url = "https://www.gov.il/he/departments/legalInfo/cpfta_prices_regulations"
     # Create a handle, page, to handle the contents of the website
-    return session_with_cookies(url, chain_cookie_name="gov_il")
+
+    def get_from_playwrite(page):
+        if extraction_type == "update_date":
+            content = page.locator('//*[@id="metaData_updateDate_0"]').last.inner_text()
+        elif extraction_type == "links_name":
+            content = page.evaluate(
+                """() => {
+            const links = Array.from(document.querySelectorAll('a'));
+            return links.map(link => link.textContent.trim());
+        }"""
+            )
+        else:
+            raise ValueError(f"type '{extraction_type}' is not valid.")
+        return content
+
+    return render_webpage(url, extraction=get_from_playwrite)
+
+
+def get_cached_page():
+    """get the current cached page"""
+    cache = None
+    with open(
+        os.path.join(
+            os.path.dirname(os.path.abspath(__file__)),
+            "tests",
+            "cpfta_prices_regulations",
+        ),
+        encoding="utf-8",
+    ) as page_cache:
+        cache = page_cache.read()
+    return cache
 
 
 def get_status():
     """get the number of scarper listed on the gov.il site"""
-    page = get_statue_page()
+    links_text = get_statue_page(extraction_type="links_name")
     # Store the contents of the website under doc
-    doc = BeautifulSoup(page.content, features="lxml")
-    # Parse data that are stored between <tr>..</tr> of HTML
     count = 0
-    for element in doc.find_all("strong"):
+    for element in links_text:
         if "לצפייה במחירים" in str(element) or "לצפיה במחירים" in str(element):
             count += 1
 
     return count
 
 
 def get_status_date():
     """get the date change listed on the gov.il site"""
-    page = get_statue_page()
-
-    if page.status_code != 200:
-        Logger.error(f"request as failed, page body is {page}.")
-        raise ValueError("Failed reading the gov.il site.")
-    line_with_date = (
-        lh.fromstring(page.content)
-        .xpath(
-            r"""/html/body/section/div/
-                                                        div[3]/div/span"""
-        )[0]
-        .text
-    )
+    line_with_date = get_statue_page(extraction_type="update_date")
+    print(line_with_date)
     Logger.info(f"line_with_date: {line_with_date}")
 
     dates = re.findall(
         r"([1-9]|1[0-9]|2[0-9]|3[0-1]|0[0-9])(.|-|\/)([1-9]|1[0-2]|0[0-9])(.|-|\/)(20[0-9][0-9])",
         line_with_date,
     )
```

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/PKG-INFO` & `il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-supermarket-scraper
-Version: 0.3.7
+Version: 0.3.8
 Summary: python package that implement a scraping for israeli supermarket data
 Home-page: https://github.com/jladan/package_demo
 Author: Sefi Erlich
 Author-email: erlichsefi@gmail.com
 License: MIT
 Keywords: israel,israeli,scraper,supermarket
 Classifier: Development Status :: 3 - Alpha
@@ -16,20 +16,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: retry==0.9.2
 Requires-Dist: mock==4.0.3
 Requires-Dist: requests==2.31.0
-Requires-Dist: lxml==4.9.1
+Requires-Dist: lxml==5.2.1
 Requires-Dist: beautifulsoup4==4.10.0
 Requires-Dist: pymongo==4.2.0
 Requires-Dist: pytz==2022.4
 Requires-Dist: holidays==0.16
 Requires-Dist: cachetools==5.2.0
+Requires-Dist: pytest-playwright==0.4.4
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 
 Israel Supermarket Scraper: Clients to download the data published by the supermarkets.
 =======================================
 This is a scraper for ALL the supermarket chains listed in the GOV.IL site.
```

### Comparing `il-supermarket-scraper-0.3.7/il_supermarket_scraper.egg-info/SOURCES.txt` & `il_supermarket_scraper-0.3.8/il_supermarket_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `il-supermarket-scraper-0.3.7/setup.py` & `il_supermarket_scraper-0.3.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "il_supermarket_scarper.utils",
     ],
     # Needed for dependencies
     install_requires=required,
     tests_require=dev_required,
     extras_require={"test": ["pytest"]},
     # *strongly* suggested for sharing
-    version="0.3.7",
+    version="0.3.8",
     # The license can be anything you like
     license="MIT",
     description="python package that implement a scraping for israeli supermarket data",
     # We will also need a readme eventually (there will be a warning)
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["israel", "israeli", "scraper", "supermarket"],
```

### Comparing `il-supermarket-scraper-0.3.7/tests/test_integration.py` & `il_supermarket_scraper-0.3.8/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import datetime
-from il_supermarket_scarper.utils.status import get_status, get_status_date
+from il_supermarket_scarper.utils.status import (
+    get_status,
+    get_status_date,
+)
 from il_supermarket_scarper.scrappers_factory import ScraperFactory
 from il_supermarket_scarper.utils.connection import disable_when_outside_israel
 
 
 @disable_when_outside_israel
 def test_scrapers_are_updated():
     """test the number of scrapers are the same as listed at the gov.il site"""
@@ -22,10 +25,8 @@
     assert len(list(set(all_chain_ids))) == len(all_chain_ids)
 
 
 @disable_when_outside_israel
 def test_update_date():
     """test date the site update"""
     date = get_status_date()
-    assert date == datetime.datetime(
-        2024, 1, 28
-    ), "gov il site changed, please check it out."
+    assert date.date() == datetime.datetime(2024, 2, 11).date(), "gov il site changed"
```

### Comparing `il-supermarket-scraper-0.3.7/tests/test_main.py` & `il_supermarket_scraper-0.3.8/tests/test_main.py`

 * *Files identical despite different names*

