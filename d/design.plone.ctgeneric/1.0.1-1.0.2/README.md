# Comparing `tmp/design.plone.ctgeneric-1.0.1.tar.gz` & `tmp/design.plone.ctgeneric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ctgeneric-1.0.1.tar", last modified: Thu Apr 18 15:17:43 2024, max compression
+gzip compressed data, was "design.plone.ctgeneric-1.0.2.tar", last modified: Thu Apr 18 19:18:23 2024, max compression
```

## Comparing `design.plone.ctgeneric-1.0.1.tar` & `design.plone.ctgeneric-1.0.2.tar`

### file list

```diff
@@ -1,99 +1,145 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.460585 design.plone.ctgeneric-1.0.1/
--rw-r--r--   0 cekk       (501) staff       (20)      193 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      673 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      122 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4014 2024-04-18 15:17:43.460634 design.plone.ctgeneric-1.0.1/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2555 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.453475 design.plone.ctgeneric-1.0.1/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7935 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       89 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)      278 2024-04-18 15:17:43.460828 design.plone.ctgeneric-1.0.1/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2602 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.451349 design.plone.ctgeneric-1.0.1/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.453600 design.plone.ctgeneric-1.0.1/src/design/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.454594 design.plone.ctgeneric-1.0.1/src/design/plone/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.455213 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/
--rw-r--r--   0 cekk       (501) staff       (20)     2405 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.455408 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     7290 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/adapters/schema_tweaks.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.456444 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1156 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/address.py
--rw-r--r--   0 cekk       (501) staff       (20)     3157 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/contatti.py
--rw-r--r--   0 cekk       (501) staff       (20)     2313 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/documento.py
--rw-r--r--   0 cekk       (501) staff       (20)     2484 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/evento.py
--rw-r--r--   0 cekk       (501) staff       (20)     2494 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/luogo.py
--rw-r--r--   0 cekk       (501) staff       (20)     1028 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/news.py
--rw-r--r--   0 cekk       (501) staff       (20)     4482 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/persona.py
--rw-r--r--   0 cekk       (501) staff       (20)     1105 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/servizio.py
--rw-r--r--   0 cekk       (501) staff       (20)     1979 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/uo.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.456640 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      573 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)      228 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/indexers.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.456946 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/interfaces/
--rw-r--r--   0 cekk       (501) staff       (20)      259 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/interfaces/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      290 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/interfaces/layer.py
--rw-r--r--   0 cekk       (501) staff       (20)     3550 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/interfaces/settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.457136 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/locales/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1760 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/locales/update.py
--rw-r--r--   0 cekk       (501) staff       (20)      529 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/monkey.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.457236 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.457831 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      745 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/documento.py
--rw-r--r--   0 cekk       (501) staff       (20)      725 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/news.py
--rw-r--r--   0 cekk       (501) staff       (20)      741 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/servizio.py
--rw-r--r--   0 cekk       (501) staff       (20)      782 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/unitaorganizzativa.py
--rw-r--r--   0 cekk       (501) staff       (20)      714 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/venue.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.458236 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2149 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/persona.py
--rw-r--r--   0 cekk       (501) staff       (20)     1372 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/summary.py
--rw-r--r--   0 cekk       (501) staff       (20)      892 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/unita_organizzativa.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.458429 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      626 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/controlpanel.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.458625 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/types/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/types/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2265 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/types/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     1445 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2241 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.460182 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2771 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_base_serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)      313 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_bando.py
--rw-r--r--   0 cekk       (501) staff       (20)      356 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 cekk       (501) staff       (20)      322 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_document.py
--rw-r--r--   0 cekk       (501) staff       (20)     2722 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_documento.py
--rw-r--r--   0 cekk       (501) staff       (20)     6892 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_event.py
--rw-r--r--   0 cekk       (501) staff       (20)     4713 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_luogo.py
--rw-r--r--   0 cekk       (501) staff       (20)     4307 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_modulo.py
--rw-r--r--   0 cekk       (501) staff       (20)     5376 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_news.py
--rw-r--r--   0 cekk       (501) staff       (20)      344 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 cekk       (501) staff       (20)     6137 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_persona.py
--rw-r--r--   0 cekk       (501) staff       (20)     5040 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_servizio.py
--rw-r--r--   0 cekk       (501) staff       (20)     4219 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 cekk       (501) staff       (20)     2880 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_summary_serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)      630 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/utils.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.460480 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1734 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 cekk       (501) staff       (20)     2280 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/document_types_vocabulary.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 15:17:43.454492 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4014 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3633 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      127 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       20 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      188 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        7 2024-04-18 15:17:43.000000 design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.543132 design.plone.ctgeneric-1.0.2/
+-rw-r--r--   0 cekk       (501) staff       (20)      263 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      673 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      110 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4084 2024-04-18 19:18:23.543187 design.plone.ctgeneric-1.0.2/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2555 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.532121 design.plone.ctgeneric-1.0.2/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7935 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       89 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2024-04-18 19:18:23.543407 design.plone.ctgeneric-1.0.2/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2602 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.529536 design.plone.ctgeneric-1.0.2/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.532226 design.plone.ctgeneric-1.0.2/src/design/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.533184 design.plone.ctgeneric-1.0.2/src/design/plone/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.534104 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/
+-rw-r--r--   0 cekk       (501) staff       (20)     2405 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.534403 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      317 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     7290 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/adapters/schema_tweaks.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.535519 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1156 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/address.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3119 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3157 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/contatti.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2313 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/documento.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2484 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/evento.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2494 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/luogo.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1028 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/news.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4482 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/persona.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1105 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/servizio.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1979 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/uo.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.535813 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      916 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      573 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.535917 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.536008 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/static/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     1621 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      228 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/indexers.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.536302 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/interfaces/
+-rw-r--r--   0 cekk       (501) staff       (20)      259 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/interfaces/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      290 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/interfaces/layer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3550 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/interfaces/settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.536786 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/design.plone.ctgeneric.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.530204 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.537000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/en/LC_MESSAGES/design.plone.ctgeneric.mo
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/en/LC_MESSAGES/design.plone.ctgeneric.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1760 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      503 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      529 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/monkey.py
+-rw-r--r--   0 cekk       (501) staff       (20)      401 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/monkey.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.530501 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.537591 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      191 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       89 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      625 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      203 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.537797 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)     3010 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/registry/criteria.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      227 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.538714 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      829 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Documento.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      713 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Event.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      292 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Incarico.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      436 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/News_Item.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      461 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Persona.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      296 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      639 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Servizio.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      624 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      709 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types/Venue.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      779 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/default/types.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.538814 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      132 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.539000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      314 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.539702 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      442 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      745 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/documento.py
+-rw-r--r--   0 cekk       (501) staff       (20)      725 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/news.py
+-rw-r--r--   0 cekk       (501) staff       (20)      741 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/servizio.py
+-rw-r--r--   0 cekk       (501) staff       (20)      782 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/unitaorganizzativa.py
+-rw-r--r--   0 cekk       (501) staff       (20)      714 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/venue.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.540199 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      397 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2149 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/persona.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1372 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/summary.py
+-rw-r--r--   0 cekk       (501) staff       (20)      892 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/unita_organizzativa.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.540490 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      404 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      626 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.540780 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/types/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/types/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      398 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/types/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2265 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/types/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1445 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2241 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.542459 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2771 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_base_serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      313 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_bando.py
+-rw-r--r--   0 cekk       (501) staff       (20)      356 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 cekk       (501) staff       (20)      322 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_document.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2722 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_documento.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6892 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_event.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4713 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_luogo.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4307 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_modulo.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5376 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_news.py
+-rw-r--r--   0 cekk       (501) staff       (20)      344 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6137 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_persona.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5040 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_servizio.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4219 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2880 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_summary_serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      630 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/utils.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.542990 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      996 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1734 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2280 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/document_types_vocabulary.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 19:18:23.533077 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4084 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5789 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      127 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       20 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      188 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        7 2024-04-18 19:18:23.000000 design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/top_level.txt
```

### Comparing `design.plone.ctgeneric-1.0.1/DEVELOP.rst` & `design.plone.ctgeneric-1.0.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/LICENSE.GPL` & `design.plone.ctgeneric-1.0.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/LICENSE.rst` & `design.plone.ctgeneric-1.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/PKG-INFO` & `design.plone.ctgeneric-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ctgeneric
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add-on that implements AGID v2 content types rules
 Home-page: https://github.com/collective/design.plone.ctgeneric
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ctgeneric/
 Project-URL: Source, https://github.com/collective/design.plone.ctgeneric
@@ -128,14 +128,20 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.2 (2024-04-18)
+------------------
+
+- Fix wrong release.
+  [cekk]
+
 1.0.1 (2024-04-18)
 ------------------
 
 - Avoid attributerror when getting tipologia_notizia.
   [cekk]
```

### Comparing `design.plone.ctgeneric-1.0.1/README.rst` & `design.plone.ctgeneric-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/docs/conf.py` & `design.plone.ctgeneric-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/setup.py` & `design.plone.ctgeneric-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ctgeneric",
-    version="1.0.1",
+    version="1.0.2",
     description="Add-on that implements AGID v2 content types rules",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
```

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/__init__.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/adapters/schema_tweaks.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/adapters/schema_tweaks.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/address.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/contatti.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/documento.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/evento.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/luogo.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/news.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/persona.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/servizio.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/behaviors/uo.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/behaviors/uo.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/browser/controlpanel.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/interfaces/settings.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/locales/update.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/monkey.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/monkey.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/documento.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/news.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/servizio.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/unitaorganizzativa.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/unitaorganizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/deserializer/venue.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/deserializer/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/persona.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/summary.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/serializer/unita_organizzativa.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/serializer/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/controlpanel.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/restapi/services/types/get.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/setuphandlers.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/testing.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_base_serializer.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_documento.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_event.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_luogo.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_modulo.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_news.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_persona.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_servizio.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_ct_unita_organizzativa.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/tests/test_summary_serializer.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/utils.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/controlapanel_vocabularies.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design/plone/ctgeneric/vocabularies/document_types_vocabulary.py` & `design.plone.ctgeneric-1.0.2/src/design/plone/ctgeneric/vocabularies/document_types_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.ctgeneric-1.0.1/src/design.plone.ctgeneric.egg-info/PKG-INFO` & `design.plone.ctgeneric-1.0.2/src/design.plone.ctgeneric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ctgeneric
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add-on that implements AGID v2 content types rules
 Home-page: https://github.com/collective/design.plone.ctgeneric
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ctgeneric/
 Project-URL: Source, https://github.com/collective/design.plone.ctgeneric
@@ -128,14 +128,20 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.2 (2024-04-18)
+------------------
+
+- Fix wrong release.
+  [cekk]
+
 1.0.1 (2024-04-18)
 ------------------
 
 - Avoid attributerror when getting tipologia_notizia.
   [cekk]
```

