# Comparing `tmp/aanalyticsact_1-0.0.1.48.tar.gz` & `tmp/aanalyticsact_1-0.0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact_1-0.0.1.48.tar", last modified: Fri Mar 22 08:31:00 2024, max compression
+gzip compressed data, was "aanalyticsact_1-0.0.1.49.tar", last modified: Thu Apr 18 07:19:37 2024, max compression
```

## Comparing `aanalyticsact_1-0.0.1.48.tar` & `aanalyticsact_1-0.0.1.49.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 08:31:00.601695 aanalyticsact_1-0.0.1.48/
--rw-rw-rw-   0        0        0      191 2024-03-22 08:31:00.601695 aanalyticsact_1-0.0.1.48/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-22 08:31:00.601695 aanalyticsact_1-0.0.1.48/aanalyticsact_1/
--rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1/__init__.py
--rw-rw-rw-   0        0        0       24 2024-03-22 05:30:53.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1/__version__.py
--rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1/actExecute.py
--rw-rw-rw-   0        0        0    18010 2024-03-22 05:30:19.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1/actModuler.py
--rw-rw-rw-   0        0        0     8870 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1/actRunner.py
-drwxrwxrwx   0        0        0        0 2024-03-22 08:31:00.601695 aanalyticsact_1-0.0.1.48/aanalyticsact_1.egg-info/
--rw-rw-rw-   0        0        0      191 2024-03-22 08:31:00.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-03-22 08:31:00.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 08:31:00.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-22 08:31:00.000000 aanalyticsact_1-0.0.1.48/aanalyticsact_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 08:31:00.601695 aanalyticsact_1-0.0.1.48/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-03-22 08:29:19.000000 aanalyticsact_1-0.0.1.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/
+-rw-rw-rw-   0        0        0      191 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.567687 aanalyticsact_1-0.0.1.49/aanalyticsact_1/
+-rw-rw-rw-   0        0        0      151 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-18 07:01:48.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/__version__.py
+-rw-rw-rw-   0        0        0     7109 2023-12-20 04:59:52.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actExecute.py
+-rw-rw-rw-   0        0        0    18010 2024-03-22 05:30:19.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actModuler.py
+-rw-rw-rw-   0        0        0     9139 2024-04-18 06:51:22.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1/actRunner.py
+drwxrwxrwx   0        0        0        0 2024-04-18 07:19:37.567687 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 07:19:37.000000 aanalyticsact_1-0.0.1.49/aanalyticsact_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 07:19:37.583301 aanalyticsact_1-0.0.1.49/setup.cfg
+-rw-rw-rw-   0        0        0      732 2024-04-18 07:19:16.000000 aanalyticsact_1-0.0.1.49/setup.py
```

### Comparing `aanalyticsact_1-0.0.1.48/aanalyticsact_1/actExecute.py` & `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actExecute.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.48/aanalyticsact_1/actModuler.py` & `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actModuler.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact_1-0.0.1.48/aanalyticsact_1/actRunner.py` & `aanalyticsact_1-0.0.1.49/aanalyticsact_1/actRunner.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,16 +106,17 @@
     #22.04.01 si, hr epp 추가
     #22.07.26 iq_ar, lb 추가
     #22.09.01 cl epp 추가
     #22.10.24 ph epp 추가
     #23.02.02 iq_ar epp 추가
     #23.03.03 jp epp 추가
     #23.04.24 mn, ge 추가
+    #24.04.16 semicon 추가
     defaultEpp = [["us", "sssamsungnewus"], ["ae", "sssamsung4aeepp"], ["at", "sssamsung4atepp"], ["au", "sssamsung4auepp"], ["be", "sssamsung4beepp"], ["ca", "sssamsung4caepp"], ["ch", "sssamsung4chepp"], ["cn", "sssamsung4cnepp"], ["cz", "sssamsung4czepp"], ["de", "sssamsung4deepp"], ["dk", "sssamsung4dkepp"], ["ee", "sssamsung4eeepp"], ["eg", "sssamsung4egepp"], ["es", "sssamsung4esepp"], ["fi", "sssamsung4fiepp"], ["fr", "sssamsung4frepp"], ["hk", "sssamsung4hkepp"], ["hu", "sssamsung4huepp"], ["id", "sssamsung4idepp"], ["il", "sssamsung4ilepp"], ["in", "sssamsung4inepp"], ["it", "sssamsung4itepp"], ["levant", "sssamsung4levantepp"], ["lt", "sssamsung4ltepp"], ["lv", "sssamsung4lvepp"], ["my", "sssamsung4myepp"], ["n_africa", "sssamsung4nafricaepp"], ["nl", "sssamsung4nlepp"], ["no", "sssamsung4noepp"], ["nz", "sssamsung4nzepp"], ["pk", "sssamsung4pkepp"], ["pt", "sssamsung4ptepp"], ["ru", "sssamsung4ruepp"], ["sa", "sssamsung4saepp"], ["se", "sssamsung4seepp"], ["sec", "sssamsung4secepp"], ["sg", "sssamsung4sgepp"], ["sk", "sssamsung4skepp"], ["th", "sssamsung4thepp"], ["tw", "sssamsung4twepp"], ["uk", "sssamsung4ukepp"], ["vn", "sssamsung4vnepp"], ["za", "sssamsung4zaepp"], ["kz_kz", "sssamsung4kzkzepp"], ["ua", "sssamsung4uaepp"], ["si", "sssssamsung4siepp"], ["hr", "sssamsung4hrepp"], ["cl", "sssamsung4clepp"], ["ph", "sssamsung4phepp"], ["africa_en", "sssamsung4africaenepp"], ["co", "sssamsung4coepp"], ["gr", "sssamsung4grepp"], ["ie", "sssamsung4ieepp"], ["mx", "sssamsung4mxepp"], ["pe", "sssamsung4peepp"], ["pl", "sssamsung4plepp"], ["ro", "sssamsung4roepp"], ["iq_ar", "sssamsung4iqarepp"], ["jp", "sssamsung4jpepp"]]
-    defaultNone = [["us", "sssamsungnewus"], ["sec", "sssamsung4sec"], ["ae", "sssamsung4ae"], ["ae_ar", "sssamsung4aear"], ["africa_en", "sssamsung4africaen"], ["africa_fr", "sssamsung4africafr"], ["africa_pt", "sssamsung4africapt"], ["al", "sssamsung4al"], ["ar", "sssamsung4ar"], ["at", "sssamsung4at"], ["au", "sssamsung4au"], ["ba", "sssamsung4ba"], ["be", "sssamsung4be"], ["be_fr", "sssamsung4befr"], ["bg", "sssamsung4bg"], ["br", "sssamsung4br"], ["ca", "sssamsung4ca"], ["ca_fr", "sssamsung4cafr"], ["ch", "sssamsung4ch"], ["ch_fr", "sssamsung4chfr"], ["cl", "sssamsung4cl"], ["cn", "sssamsung4cn"], ["co", "sssamsung4co"], ["cz", "sssamsung4cz"], ["de", "sssamsung4de"], ["dk", "sssamsung4dk"], ["ee", "sssamsung4ee"], ["eg", "sssamsung4eg"], ["es", "sssamsung4es"], ["fi", "sssamsung4fi"], ["fr", "sssamsung4fr"], ["gr", "sssamsung4gr"], ["hk", "sssamsung4hk"], ["hk_en", "sssamsung4hken"], ["hr", "sssamsung4hr"], ["hu", "sssamsung4hu"], ["id", "sssamsung4id"], ["ie", "sssamsung4ie"], ["il", "sssamsung4il"], ["in", "sssamsung4in"], ["iran", "sssamsung4iran"], ["it", "sssamsung4it"], ["jp", "sssamsung4jp"], ["kz_kz", "sssamsung4kzkz"], ["kz_ru", "sssamsung4kzru"], ["latin", "sssamsung4latin"], ["latin_en", "sssamsung4latinen"], ["levant", "sssamsung4levant"], ["levant_ar", "sssamsung4levantar"], ["lt", "sssamsung4lt"], ["lv", "sssamsung4lv"], ["mk", "sssamsung4mk"], ["mm", "sssamsung4mm"], ["mx", "sssamsung4mx"], ["my", "sssamsung4my"], ["n_africa", "sssamsung4nafrica"], ["nl", "sssamsung4nl"], ["no", "sssamsung4no"], ["nz", "sssamsung4nz"], ["pe", "sssamsung4pe"], ["ph", "sssamsung4ph"], ["pk", "sssamsung4pk"], ["pl", "sssamsung4pl"], ["ps", "sssamsung4ps"], ["pt", "sssamsung4pt"], ["py", "sssamsung4py"], ["ro", "sssamsung4ro"], ["rs", "sssamsung4rs"], ["ru", "sssamsung4ru"], ["sa", "sssamsung4sa"], ["sa_en", "sssamsung4saen"], ["se", "sssamsung4se"], ["sg", "sssamsung4sg"], ["si", "sssamsung4si"], ["sk", "sssamsung4sk"], ["th", "sssamsung4th"], ["tr", "sssamsung4tr"], ["tw", "sssamsung4tw"], ["ua", "sssamsung4ua"], ["uk", "sssamsung4uk"], ["uy", "sssamsung4uy"], ["uz_ru", "sssamsung4uzru"], ["uz_uz", "sssamsung4uzuz"], ["vn", "sssamsung4vn"], ["za", "sssamsung4za"], ["az", "sssamsung4az"], ["bd", "sssamsung4bd"], ["mst_sena", "vrs_samsun0_p4webmstsena_0"], ["mst_sehk", "vrs_samsun0_p6webmstsehk"], ["mst_sebn", "vrs_samsun0_p4websebn"], ["mst_mena", "vrs_samsun0_p4webmstmena"], ["mst_seca", "vrs_samsun0_p4webmstseca"], ["mst_eu", "vrs_samsun0_p4webmsteu_0"], ["mst_seao", "vrs_samsun0_p4webmstseao"], ["iq_ar", "sssamsung4iqar"], ["lb", "sssamsung4lb"], ["mn", "sssamsung4mn"], ["ge", "sssamsung4ge"]]
+    defaultNone = [["us", "sssamsungnewus"], ["sec", "sssamsung4sec"], ["ae", "sssamsung4ae"], ["ae_ar", "sssamsung4aear"], ["africa_en", "sssamsung4africaen"], ["africa_fr", "sssamsung4africafr"], ["africa_pt", "sssamsung4africapt"], ["al", "sssamsung4al"], ["ar", "sssamsung4ar"], ["at", "sssamsung4at"], ["au", "sssamsung4au"], ["ba", "sssamsung4ba"], ["be", "sssamsung4be"], ["be_fr", "sssamsung4befr"], ["bg", "sssamsung4bg"], ["br", "sssamsung4br"], ["ca", "sssamsung4ca"], ["ca_fr", "sssamsung4cafr"], ["ch", "sssamsung4ch"], ["ch_fr", "sssamsung4chfr"], ["cl", "sssamsung4cl"], ["cn", "sssamsung4cn"], ["co", "sssamsung4co"], ["cz", "sssamsung4cz"], ["de", "sssamsung4de"], ["dk", "sssamsung4dk"], ["ee", "sssamsung4ee"], ["eg", "sssamsung4eg"], ["es", "sssamsung4es"], ["fi", "sssamsung4fi"], ["fr", "sssamsung4fr"], ["gr", "sssamsung4gr"], ["hk", "sssamsung4hk"], ["hk_en", "sssamsung4hken"], ["hr", "sssamsung4hr"], ["hu", "sssamsung4hu"], ["id", "sssamsung4id"], ["ie", "sssamsung4ie"], ["il", "sssamsung4il"], ["in", "sssamsung4in"], ["iran", "sssamsung4iran"], ["it", "sssamsung4it"], ["jp", "sssamsung4jp"], ["kz_kz", "sssamsung4kzkz"], ["kz_ru", "sssamsung4kzru"], ["latin", "sssamsung4latin"], ["latin_en", "sssamsung4latinen"], ["levant", "sssamsung4levant"], ["levant_ar", "sssamsung4levantar"], ["lt", "sssamsung4lt"], ["lv", "sssamsung4lv"], ["mk", "sssamsung4mk"], ["mm", "sssamsung4mm"], ["mx", "sssamsung4mx"], ["my", "sssamsung4my"], ["n_africa", "sssamsung4nafrica"], ["nl", "sssamsung4nl"], ["no", "sssamsung4no"], ["nz", "sssamsung4nz"], ["pe", "sssamsung4pe"], ["ph", "sssamsung4ph"], ["pk", "sssamsung4pk"], ["pl", "sssamsung4pl"], ["ps", "sssamsung4ps"], ["pt", "sssamsung4pt"], ["py", "sssamsung4py"], ["ro", "sssamsung4ro"], ["rs", "sssamsung4rs"], ["ru", "sssamsung4ru"], ["sa", "sssamsung4sa"], ["sa_en", "sssamsung4saen"], ["se", "sssamsung4se"], ["sg", "sssamsung4sg"], ["si", "sssamsung4si"], ["sk", "sssamsung4sk"], ["th", "sssamsung4th"], ["tr", "sssamsung4tr"], ["tw", "sssamsung4tw"], ["ua", "sssamsung4ua"], ["uk", "sssamsung4uk"], ["uy", "sssamsung4uy"], ["uz_ru", "sssamsung4uzru"], ["uz_uz", "sssamsung4uzuz"], ["vn", "sssamsung4vn"], ["za", "sssamsung4za"], ["az", "sssamsung4az"], ["bd", "sssamsung4bd"], ["mst_sena", "vrs_samsun0_p4webmstsena_0"], ["mst_sehk", "vrs_samsun0_p6webmstsehk"], ["mst_sebn", "vrs_samsun0_p4websebn"], ["mst_mena", "vrs_samsun0_p4webmstmena"], ["mst_seca", "vrs_samsun0_p4webmstseca"], ["mst_eu", "vrs_samsun0_p4webmsteu_0"], ["mst_seao", "vrs_samsun0_p4webmstseao"], ["iq_ar", "sssamsung4iqar"], ["lb", "sssamsung4lb"], ["mn", "sssamsung4mn"], ["ge", "sssamsung4ge"],["ds-global","sssamsung4b2bsemi"], ["ds-cn","sssamsung4b2bsemicn"],["ds-us","sssamsung4b2bsemius"],["ds-kr","sssamsung4b2bsemikr"],["ds-emea","sssamsung4b2bsemiemea"],["ds-jp","sssamsung4b2csemi"],["ds-total","sssamsung4b2bsemiconductor"]]
 
     if epp == True:
         return rsListGenerator(inputSiteCode, defaultEpp)
     else:
         return rsListGenerator(inputSiteCode, defaultNone)
```

### Comparing `aanalyticsact_1-0.0.1.48/setup.py` & `aanalyticsact_1-0.0.1.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'aanalyticsact_1'
-Version= '0.0.1.48'
+Version= '0.0.1.49'
 URL = 'https://github.com/Glory-Cho/aanalyticsact)1'
 Summary= 'adobe analytics library for Team ACT'
 EMAIL = 'youngkwang.cho@concentrix.com'
 AUTHOR = 'Youngkwang Cho'
 
 here = os.path.abspath(os.path.dirname(__file__))
```

