# Comparing `tmp/design.plone.contenttypes-6.2.4.tar.gz` & `tmp/design.plone.contenttypes-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.contenttypes-6.2.4.tar", last modified: Tue Apr 16 13:08:35 2024, max compression
+gzip compressed data, was "design.plone.contenttypes-6.2.5.tar", last modified: Wed Apr 17 09:54:28 2024, max compression
```

## Comparing `design.plone.contenttypes-6.2.4.tar` & `design.plone.contenttypes-6.2.5.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.364347 design.plone.contenttypes-6.2.4/
--rw-r--r--   0 lucabel    (501) staff       (20)    23514 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      665 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      174 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    40771 2024-04-16 13:08:35.364491 design.plone.contenttypes-6.2.4/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    15960 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/README.md
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.273068 design.plone.contenttypes-6.2.4/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7993 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       98 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      383 2024-04-16 13:08:35.365116 design.plone.contenttypes-6.2.4/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3005 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.262208 design.plone.contenttypes-6.2.4/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.273356 design.plone.contenttypes-6.2.4/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.276642 design.plone.contenttypes-6.2.4/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.278923 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/
--rw-r--r--   0 lucabel    (501) staff       (20)      668 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.280341 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      892 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      421 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/interfaces.py
--rw-r--r--   0 lucabel    (501) staff       (20)      930 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/query.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
--rw-r--r--   0 lucabel    (501) staff       (20)      231 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/servizi_correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.286329 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1354 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/additional_help_infos.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/address.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8986 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11818 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6469 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/contatti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1589 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/dataset_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2679 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6212 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1060 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/exclude_from_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1657 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/geolocation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2388 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/info_testata.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2739 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6540 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1606 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/multi_file.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4439 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/news_additional_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1787 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/servizi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1357 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1648 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/strutture_correlate.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10452 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1165 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/update_note.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.287082 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1333 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.287323 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/overrides/.gitkeep
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.263181 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/static/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.287513 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/static/js/
--rw-r--r--   0 lucabel    (501) staff       (20)      262 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/static/js/move_content.js
--rw-r--r--   0 lucabel    (501) staff       (20)      469 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/trasparenza.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.290629 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3813 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8270 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_documenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7290 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_eventi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7550 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_luoghi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8729 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_notizie.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8573 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_persone.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14304 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_servizi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7594 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_uo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3467 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1571 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/export_incarichi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2796 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/move_news_items.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.293537 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     3360 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6399 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6372 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6388 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     8600 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6167 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     9903 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6177 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4760 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3797 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/utils.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3122 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.298704 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      315 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)      210 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      215 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      229 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      271 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      272 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/content/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.299823 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      737 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1382 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3865 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/settings.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.301375 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5779 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/document.py
--rw-r--r--   0 lucabel    (501) staff       (20)      536 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      969 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/pagina_argomento.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.304548 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      458 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1119 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1803 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      411 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)      621 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      829 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      741 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      470 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      445 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/uo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.309381 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)      419 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6263 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      699 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      857 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8557 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4724 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5442 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1487 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      205 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2560 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5028 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1781 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2850 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1864 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    18229 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7946 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.311012 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.264930 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/__pycache__/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.311278 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    82355 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)    82310 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.265169 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.311648 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    82335 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.265400 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.312923 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     1243 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
--rw-r--r--   0 lucabel    (501) staff       (20)    83275 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)     7287 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/plone.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1597 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/update.sh
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/overrides.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.314088 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/
--rw-r--r--   0 lucabel    (501) staff       (20)      516 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3700 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/baseserializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)      483 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      343 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/patches.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2751 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.266754 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.265854 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.323260 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3401 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      331 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     4370 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      286 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2870 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      372 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     8078 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      300 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2156 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      313 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    13732 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      398 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     5133 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1042 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      303 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2196 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      265 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    15346 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      322 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1015 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      355 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3138 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      342 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.326210 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      799 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/actions.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2919 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1040 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1219 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      595 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.326854 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)    19836 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1139 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     4491 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.332810 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     1155 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Bando.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3563 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3327 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3747 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3321 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2501 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      345 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3427 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      506 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3199 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2908 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3456 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3430 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Persona.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3178 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3342 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3149 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3829 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2212 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Venue.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.333099 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/fix_syndication/
--rw-r--r--   0 lucabel    (501) staff       (20)      520 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.333557 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/to_3000/
--rw-r--r--   0 lucabel    (501) staff       (20)      377 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/to_3000/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.333911 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      128 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.334939 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      663 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      504 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/converters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      702 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.337611 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      760 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5795 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6060 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5743 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1658 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5844 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5999 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6016 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.341626 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1548 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2086 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2102 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2837 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7597 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1407 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2360 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3726 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1763 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2502 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/relationfield.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1660 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    16924 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/summary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5316 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3769 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.342288 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      601 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.342987 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/content/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)      368 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      653 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/controlpanel.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.343696 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      605 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2915 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.345110 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      558 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1254 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.345959 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1200 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    11504 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.346766 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      884 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3351 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.347556 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    11248 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.348245 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3805 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/types/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      394 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1628 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/schema_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2315 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4083 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.358596 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11218 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/example.pdf
--rw-r--r--   0 lucabel    (501) staff       (20)    10503 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/example.png
--rw-r--r--   0 lucabel    (501) staff       (20)     1997 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2330 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_base_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1564 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4707 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2563 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_update_note.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1893 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7543 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5613 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6203 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_document.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11615 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13149 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_event.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1640 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14823 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)    12271 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5903 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9850 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19255 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    17028 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2926 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2708 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2526 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_move_news_items_view.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6638 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2798 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_service_scadenziario.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1381 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3533 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13785 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_substructure_creation.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11753 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4714 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6351 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.360440 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    25023 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5033 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/draftjs_converter.py
--rw-r--r--   0 lucabel    (501) staff       (20)    12517 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7001.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6007 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7002.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1808 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7300.py
--rw-r--r--   0 lucabel    (501) staff       (20)    57526 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)      862 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/utils.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.364131 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1308 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1573 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1694 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1466 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1895 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1704 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/mockup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2223 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1623 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-16 13:08:35.276322 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    40771 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    19438 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      130 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      451 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-04-16 13:08:35.000000 design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/top_level.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      659 2024-04-16 13:08:34.000000 design.plone.contenttypes-6.2.4/tox.ini
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.087148 design.plone.contenttypes-6.2.5/
+-rw-r--r--   0 daniele    (501) staff       (20)    23616 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/CHANGES.rst
+-rw-r--r--   0 daniele    (501) staff       (20)       67 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/CONTRIBUTORS.rst
+-rw-r--r--   0 daniele    (501) staff       (20)      585 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/DEVELOP.rst
+-rw-r--r--   0 daniele    (501) staff       (20)    18092 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/LICENSE.GPL
+-rw-r--r--   0 daniele    (501) staff       (20)      665 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/LICENSE.rst
+-rw-r--r--   0 daniele    (501) staff       (20)      174 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/MANIFEST.in
+-rw-r--r--   0 daniele    (501) staff       (20)    41718 2024-04-17 09:54:28.086987 design.plone.contenttypes-6.2.5/PKG-INFO
+-rw-r--r--   0 daniele    (501) staff       (20)    15960 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/README.md
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.917372 design.plone.contenttypes-6.2.5/docs/
+-rw-r--r--   0 daniele    (501) staff       (20)     7993 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/docs/conf.py
+-rw-r--r--   0 daniele    (501) staff       (20)       98 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/docs/index.rst
+-rw-r--r--   0 daniele    (501) staff       (20)       62 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/requirements.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      383 2024-04-17 09:54:28.087663 design.plone.contenttypes-6.2.5/setup.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     3005 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/setup.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.899111 design.plone.contenttypes-6.2.5/src/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.918104 design.plone.contenttypes-6.2.5/src/design/
+-rw-r--r--   0 daniele    (501) staff       (20)       80 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.922900 design.plone.contenttypes-6.2.5/src/design/plone/
+-rw-r--r--   0 daniele    (501) staff       (20)       80 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.928015 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/
+-rw-r--r--   0 daniele    (501) staff       (20)      668 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.931169 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      892 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      421 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/interfaces.py
+-rw-r--r--   0 daniele    (501) staff       (20)      930 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/query.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1755 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
+-rw-r--r--   0 daniele    (501) staff       (20)      231 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/servizi_correlati.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.947444 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1354 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/additional_help_infos.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2403 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/address.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8986 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/argomenti.py
+-rw-r--r--   0 daniele    (501) staff       (20)    11818 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     6469 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/contatti.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1589 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/dataset_correlati.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2679 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6212 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/evento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1060 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/exclude_from_search.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1657 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/geolocation.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2388 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/info_testata.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2739 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6540 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/luogo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1606 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/multi_file.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4439 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/news_additional_fields.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1787 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/servizi_correlati.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1357 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/show_modified.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1648 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/strutture_correlate.py
+-rw-r--r--   0 daniele    (501) staff       (20)    10452 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/trasparenza.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1165 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/update_note.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.950798 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1333 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.951596 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/overrides/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/overrides/.gitkeep
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.900556 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/static/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.952246 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/static/js/
+-rw-r--r--   0 daniele    (501) staff       (20)      262 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/static/js/move_content.js
+-rw-r--r--   0 daniele    (501) staff       (20)      469 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/trasparenza.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.960979 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3813 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/change_news_type.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8270 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_documenti.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7290 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_eventi.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7550 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_luoghi.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8729 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_notizie.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8573 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_persone.py
+-rw-r--r--   0 daniele    (501) staff       (20)    14364 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_servizi.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7594 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_uo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3467 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1571 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/export_incarichi.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2796 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/move_news_items.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.967839 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/
+-rw-r--r--   0 daniele    (501) staff       (20)     3360 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     6399 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     6372 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     6388 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     8600 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     6167 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     9903 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     6177 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     4760 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     3797 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/utils.pt
+-rw-r--r--   0 daniele    (501) staff       (20)     3122 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.978706 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      315 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/cartella_modulistica.py
+-rw-r--r--   0 daniele    (501) staff       (20)      238 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/dataset.py
+-rw-r--r--   0 daniele    (501) staff       (20)      246 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/documento.py
+-rw-r--r--   0 daniele    (501) staff       (20)      283 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/documento_personale.py
+-rw-r--r--   0 daniele    (501) staff       (20)      210 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/evento.py
+-rw-r--r--   0 daniele    (501) staff       (20)      242 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/incarico.py
+-rw-r--r--   0 daniele    (501) staff       (20)      215 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/luogo.py
+-rw-r--r--   0 daniele    (501) staff       (20)      275 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/messaggio.py
+-rw-r--r--   0 daniele    (501) staff       (20)      229 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/modulo.py
+-rw-r--r--   0 daniele    (501) staff       (20)      271 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/pagina_argomento.py
+-rw-r--r--   0 daniele    (501) staff       (20)      238 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)      238 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/pratica.py
+-rw-r--r--   0 daniele    (501) staff       (20)      272 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/punto_di_contatto.py
+-rw-r--r--   0 daniele    (501) staff       (20)      279 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/ricevuta_pagamento.py
+-rw-r--r--   0 daniele    (501) staff       (20)      242 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)      283 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/content/unita_organizzativa.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.980947 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      737 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1382 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3865 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/settings.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.984298 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5779 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/common.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1189 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      618 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/document.py
+-rw-r--r--   0 daniele    (501) staff       (20)      536 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/incarico.py
+-rw-r--r--   0 daniele    (501) staff       (20)      969 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/pagina_argomento.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.991811 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      458 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1119 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/common.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1803 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      411 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/events.py
+-rw-r--r--   0 daniele    (501) staff       (20)      921 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/news.py
+-rw-r--r--   0 daniele    (501) staff       (20)      621 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/pagina_argomento.py
+-rw-r--r--   0 daniele    (501) staff       (20)      829 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)      741 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/punto_di_contatto.py
+-rw-r--r--   0 daniele    (501) staff       (20)      470 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)      445 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/uo.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.000827 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/
+-rw-r--r--   0 daniele    (501) staff       (20)      419 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6263 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)      699 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
+-rw-r--r--   0 daniele    (501) staff       (20)      857 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/dataset.py
+-rw-r--r--   0 daniele    (501) staff       (20)     8557 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/documento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4724 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/documento_personale.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5442 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/incarico.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1487 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/messaggio.py
+-rw-r--r--   0 daniele    (501) staff       (20)      205 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/modulo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2560 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/pagina_argomento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5028 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1781 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/pratica.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2850 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1864 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
+-rw-r--r--   0 daniele    (501) staff       (20)    18229 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7946 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.004001 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/
+-rw-r--r--   0 daniele    (501) staff       (20)      611 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/README.rst
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/__init__.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.902480 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/__pycache__/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.004484 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)    82355 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 daniele    (501) staff       (20)    82310 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.902797 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/en/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.005280 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)    82335 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.903110 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.007095 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
+-rw-r--r--   0 daniele    (501) staff       (20)     1243 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
+-rw-r--r--   0 daniele    (501) staff       (20)    83275 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 daniele    (501) staff       (20)     7287 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/plone.pot
+-rw-r--r--   0 daniele    (501) staff       (20)     1597 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/update.py
+-rwxr-xr-x   0 daniele    (501) staff       (20)      512 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/update.sh
+-rw-r--r--   0 daniele    (501) staff       (20)      712 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/overrides.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.009059 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/
+-rw-r--r--   0 daniele    (501) staff       (20)      516 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3700 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/baseserializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)      483 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      343 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/patches.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2751 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/permissions.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.904823 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.903740 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.026510 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
+-rw-r--r--   0 daniele    (501) staff       (20)      314 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     3401 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      331 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     4370 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      286 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2870 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      372 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     8078 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      300 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2156 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      313 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)    13732 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      398 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     5133 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      292 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     1042 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      303 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2196 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      265 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)    15346 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      322 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     1015 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      355 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     3138 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      342 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2275 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      344 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
+-rw-r--r--   0 daniele    (501) staff       (20)     2275 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.032324 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/
+-rw-r--r--   0 daniele    (501) staff       (20)      799 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/actions.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      193 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     2919 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/catalog.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1040 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/controlpanel.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1219 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      595 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/metadata.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.033460 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/registry/
+-rw-r--r--   0 daniele    (501) staff       (20)    19836 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      618 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/registry/settings.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1139 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/repositorytool.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     4491 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.040965 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/
+-rw-r--r--   0 daniele    (501) staff       (20)     1155 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Bando.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      503 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3563 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3327 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1001 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3747 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Documento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3321 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     2501 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      345 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3427 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      506 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3199 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     2908 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1194 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3456 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3430 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Persona.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3178 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3342 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3149 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3829 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     3775 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     2212 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Venue.xml
+-rw-r--r--   0 daniele    (501) staff       (20)     1194 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.041250 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/fix_syndication/
+-rw-r--r--   0 daniele    (501) staff       (20)      520 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.041769 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/to_3000/
+-rw-r--r--   0 daniele    (501) staff       (20)      377 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
+-rw-r--r--   0 daniele    (501) staff       (20)      275 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/to_3000/registry.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.042059 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/uninstall/
+-rw-r--r--   0 daniele    (501) staff       (20)      128 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.044490 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      663 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      504 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/converters.py
+-rw-r--r--   0 daniele    (501) staff       (20)      702 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/correlati.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.052916 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      760 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     5795 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/documento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6060 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5743 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/news.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1658 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5844 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5999 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6016 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/venue.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.060719 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1548 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2086 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1976 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     2102 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/documento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2837 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7597 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/dxfields.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1407 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/modulo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2360 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3726 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1763 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2502 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/relationfield.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1660 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)    16924 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/summary.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5316 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3769 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/venue.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.061618 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      601 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/configure.zcml
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.062910 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/content/
+-rw-r--r--   0 daniele    (501) staff       (20)       24 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/content/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      664 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/content/add.py
+-rw-r--r--   0 daniele    (501) staff       (20)      368 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/content/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)      653 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/controlpanel.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.064102 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/
+-rw-r--r--   0 daniele    (501) staff       (20)       24 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      605 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     2915 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.065291 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      558 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1254 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/get.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.066067 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1200 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)    11504 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.066943 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      884 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     3351 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.067771 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/types/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/types/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)      404 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/types/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)    11248 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/types/get.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.068475 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/types/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/types/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3805 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/types/adapters.py
+-rw-r--r--   0 daniele    (501) staff       (20)      394 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/types/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1628 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/schema_overrides.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2315 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/setuphandlers.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4083 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/testing.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.078950 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)    11218 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/example.pdf
+-rw-r--r--   0 daniele    (501) staff       (20)    10503 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/example.png
+-rw-r--r--   0 daniele    (501) staff       (20)     1997 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_argomenti.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2330 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_base_serializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1564 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4707 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3169 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_luogo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2563 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1755 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_update_note.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1893 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_change_news_type.py
+-rw-r--r--   0 daniele    (501) staff       (20)     7543 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_bando.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5613 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6203 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_document.py
+-rw-r--r--   0 daniele    (501) staff       (20)    11615 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_documento.py
+-rw-r--r--   0 daniele    (501) staff       (20)    13149 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_event.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1640 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_folder.py
+-rw-r--r--   0 daniele    (501) staff       (20)    14823 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_luogo.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4225 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_modulo.py
+-rw-r--r--   0 daniele    (501) staff       (20)    12271 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_news.py
+-rw-r--r--   0 daniele    (501) staff       (20)     5903 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 daniele    (501) staff       (20)     9850 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_persona.py
+-rw-r--r--   0 daniele    (501) staff       (20)    19255 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_servizio.py
+-rw-r--r--   0 daniele    (501) staff       (20)    17028 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2926 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2708 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2526 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_move_news_items_view.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6638 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2798 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_service_scadenziario.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1381 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
+-rw-r--r--   0 daniele    (501) staff       (20)     3533 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_setup.py
+-rw-r--r--   0 daniele    (501) staff       (20)    13785 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_substructure_creation.py
+-rw-r--r--   0 daniele    (501) staff       (20)    11753 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_summary_serializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4714 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6351 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_vocabularies.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.082067 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)    25023 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     5033 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/draftjs_converter.py
+-rw-r--r--   0 daniele    (501) staff       (20)    12517 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7001.py
+-rw-r--r--   0 daniele    (501) staff       (20)     6007 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7002.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1808 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7300.py
+-rw-r--r--   0 daniele    (501) staff       (20)    57526 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/upgrades.py
+-rw-r--r--   0 daniele    (501) staff       (20)      862 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/utils.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:28.084898 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/
+-rw-r--r--   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/__init__.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1308 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1573 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1694 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/configure.zcml
+-rw-r--r--   0 daniele    (501) staff       (20)     1466 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1895 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1704 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/mockup.py
+-rw-r--r--   0 daniele    (501) staff       (20)     2223 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
+-rw-r--r--   0 daniele    (501) staff       (20)     1623 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
+-rw-r--r--   0 daniele    (501) staff       (20)     4225 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
+drwxr-xr-x   0 daniele    (501) staff       (20)        0 2024-04-17 09:54:27.922491 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/
+-rw-r--r--   0 daniele    (501) staff       (20)    41718 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 daniele    (501) staff       (20)    19438 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      130 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/entry_points.txt
+-rw-r--r--   0 daniele    (501) staff       (20)       20 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        1 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 daniele    (501) staff       (20)      451 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 daniele    (501) staff       (20)        7 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/top_level.txt
+-rw-r--r--   0 daniele    (501) staff       (20)      659 2024-04-17 09:54:27.000000 design.plone.contenttypes-6.2.5/tox.ini
```

### Comparing `design.plone.contenttypes-6.2.4/CHANGES.rst` & `design.plone.contenttypes-6.2.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+6.2.5 (2024-04-17)
+------------------
+
+- check-servizi: fixed check on relation title.
+  [daniele] 
+
+
 6.2.4 (2024-04-16)
 ------------------
 
 - converted some file and image fields as blob fields
   [mamico]
```

### Comparing `design.plone.contenttypes-6.2.4/DEVELOP.rst` & `design.plone.contenttypes-6.2.5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/LICENSE.GPL` & `design.plone.contenttypes-6.2.5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/LICENSE.rst` & `design.plone.contenttypes-6.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/PKG-INFO` & `design.plone.contenttypes-6.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.4
+Version: 6.2.5
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,17 +20,37 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity>2.6.9
+Requires-Dist: collective.venue[geolocation]
+Requires-Dist: collective.volto.blocksfield
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: plone.formwidget.geolocation
+Requires-Dist: redturtle.volto>=5.0.0
+Requires-Dist: redturtle.bandi
+Requires-Dist: z3c.unconfigure
+Requires-Dist: eea.api.taxonomy
+Requires-Dist: openpyxl
+Requires-Dist: collective.volto.enhancedlinks
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: collective.volto.blocksfield; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -498,14 +518,21 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.5 (2024-04-17)
+------------------
+
+- check-servizi: fixed check on relation title.
+  [daniele] 
+
+
 6.2.4 (2024-04-16)
 ------------------
 
 - converted some file and image fields as blob fields
   [mamico]
```

### Comparing `design.plone.contenttypes-6.2.4/README.md` & `design.plone.contenttypes-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/docs/conf.py` & `design.plone.contenttypes-6.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/setup.py` & `design.plone.contenttypes-6.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.contenttypes",
-    version="6.2.4",
+    version="6.2.5",
     description="DesignItalia contenty types",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/__init__.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/query.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/query.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/adapters/searchabletext_indexers.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/adapters/searchabletext_indexers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/additional_help_infos.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/additional_help_infos.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/address.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/argomenti.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/contatti.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/dataset_correlati.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/dataset_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/descrizione_estesa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/evento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/exclude_from_search.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/geolocation.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/geolocation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/info_testata.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/info_testata.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/luoghi_correlati.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/luoghi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/luogo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/multi_file.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/multi_file.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/news_additional_fields.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/news_additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/servizi_correlati.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/servizi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/show_modified.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/strutture_correlate.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/strutture_correlate.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/trasparenza.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/behaviors/update_note.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/behaviors/update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/change_news_type.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_documenti.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_documenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_eventi.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_eventi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_luoghi.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_luoghi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_notizie.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_notizie.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_persone.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_persone.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_servizi.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_servizi.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         return url
 
     def get_relation_title(self, information_dict, label):
         result = ""
         for item in information_dict[label]:
             if not item:
                 continue
+            if not item.to_object:
+                continue
             result = result + " " + item.to_object.title
         return result
 
     def get_servizi(self, full_report=False):
         if self.is_anonymous():
             return []
         pc = api.portal.get_tool("portal_catalog")
```

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/check_uo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/check_uo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/export_incarichi.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/export_incarichi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/move_news_items.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/move_news_items.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/browser/utils/templates/utils.pt` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/browser/utils/templates/utils.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/controlpanels/settings.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/controlpanels/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/common.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/document.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/incarico.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/events/pagina_argomento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/events/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/common.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/news.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/pagina_argomento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/persona.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/indexers/punto_di_contatto.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/indexers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/bando.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/cartella_modulistica.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/dataset.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/documento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/documento_personale.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/incarico.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/messaggio.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/messaggio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/pagina_argomento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/persona.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/pratica.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/punto_di_contatto.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/servizio.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/interfaces/unita_organizzativa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/interfaces/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/README.rst` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/update.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/locales/update.sh` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/locales/update.sh`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/overrides.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/__init__.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/patches/baseserializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/patches/baseserializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/permissions.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/actions.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/catalog.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/controlpanel.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/diff_tool.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/registry/criteria.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/registry/settings.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/repositorytool.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/rolemap.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Bando.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Dataset.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Document.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Documento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Event.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Incarico.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Modulo.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Modulo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/News_Item.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Persona.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Persona.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Pratica.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types/Venue.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types/Venue.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/default/types.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/correlati.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/documento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/dxfields.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/news.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/persona.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/servizio.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/deserializers/venue.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/deserializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/bando.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/documento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/dxcontent.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/dxcontent.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/dxfields.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/modulo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/persona.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/relationfield.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/relationfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/servizio.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/summary.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/summary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/serializers/venue.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/serializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/content/add.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/content/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/controlpanel.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/navigation/get.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/navigation/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/scadenziario/post.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/scadenziario/post.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/trasparenza/get.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/trasparenza/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/services/types/get.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/restapi/types/adapters.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/schema_overrides.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/schema_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/setuphandlers.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/testing.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/example.pdf` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/example.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/example.png` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/example.png`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_argomenti.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_base_serializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_luogo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_show_modified.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_behavior_update_note.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_behavior_update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_change_news_type.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_bando.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_document.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_documento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_event.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_folder.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_luogo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_modulo.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_news.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_persona.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_servizio.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_custom_service_navigation.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_custom_service_navigation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_move_news_items_view.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_move_news_items_view.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_service_scadenziario.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_service_scadenziario.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_setup.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_substructure_creation.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_substructure_creation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_summary_serializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/tests/test_vocabularies.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/draftjs_converter.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/draftjs_converter.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7001.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7001.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7002.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7002.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/to_7300.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/to_7300.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/upgrades/upgrades.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/utils.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/configure.zcml` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/mockup.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/mockup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/people_vocabulary.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/people_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py` & `design.plone.contenttypes-6.2.5/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/PKG-INFO` & `design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.4
+Version: 6.2.5
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,17 +20,37 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity>2.6.9
+Requires-Dist: collective.venue[geolocation]
+Requires-Dist: collective.volto.blocksfield
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: plone.formwidget.geolocation
+Requires-Dist: redturtle.volto>=5.0.0
+Requires-Dist: redturtle.bandi
+Requires-Dist: z3c.unconfigure
+Requires-Dist: eea.api.taxonomy
+Requires-Dist: openpyxl
+Requires-Dist: collective.volto.enhancedlinks
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: collective.volto.blocksfield; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -498,14 +518,21 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.5 (2024-04-17)
+------------------
+
+- check-servizi: fixed check on relation title.
+  [daniele] 
+
+
 6.2.4 (2024-04-16)
 ------------------
 
 - converted some file and image fields as blob fields
   [mamico]
```

### Comparing `design.plone.contenttypes-6.2.4/src/design.plone.contenttypes.egg-info/SOURCES.txt` & `design.plone.contenttypes-6.2.5/src/design.plone.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.4/tox.ini` & `design.plone.contenttypes-6.2.5/tox.ini`

 * *Files identical despite different names*

