# Comparing `tmp/django-gisserver-1.2.7.tar.gz` & `tmp/django-gisserver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gisserver-1.2.7.tar", last modified: Thu Jun  8 09:12:21 2023, max compression
+gzip compressed data, was "django-gisserver-1.3.0.tar", last modified: Thu Apr 18 12:51:52 2024, max compression
```

## Comparing `django-gisserver-1.2.7.tar` & `django-gisserver-1.3.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/
--rw-rw-r--   0 lars      (1000) lars      (1000)    13086 2023-06-08 09:05:07.000000 django-gisserver-1.2.7/CHANGES.md
--rw-rw-r--   0 lars      (1000) lars      (1000)    16725 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)      227 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/MANIFEST.in
--rw-rw-r--   0 lars      (1000) lars      (1000)     5349 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     4027 2023-05-03 13:46:37.000000 django-gisserver-1.2.7/README.md
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/django_gisserver.egg-info/
--rw-rw-r--   0 lars      (1000) lars      (1000)     5349 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     1915 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/SOURCES.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/dependency_links.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-01-11 09:33:57.000000 django-gisserver-1.2.7/django_gisserver.egg-info/not-zip-safe
--rw-rw-r--   0 lars      (1000) lars      (1000)      180 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/requires.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       10 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/top_level.txt
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)       40 2023-06-08 09:05:27.000000 django-gisserver-1.2.7/gisserver/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2108 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/conf.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     5329 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/db.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4596 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/exceptions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    32232 2023-05-03 09:52:03.000000 django-gisserver-1.2.7/gisserver/features.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    12619 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/gisserver/geometries.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/operations/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/operations/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    17012 2023-06-08 09:02:34.000000 django-gisserver-1.2.7/gisserver/operations/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    18635 2023-06-08 09:02:49.000000 django-gisserver-1.2.7/gisserver/operations/wfs20.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/output/
--rw-rw-r--   0 lars      (1000) lars      (1000)     1950 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/gisserver/output/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7954 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1542 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/buffer.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     6198 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/csv.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    11236 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/geojson.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    26913 2023-05-03 13:37:23.000000 django-gisserver-1.2.7/gisserver/output/gml32.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     9189 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/results.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     6113 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/utils.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4603 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/xmlschema.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/
--rw-rw-r--   0 lars      (1000) lars      (1000)      290 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     4864 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/base.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/fes20/
--rw-rw-r--   0 lars      (1000) lars      (1000)      624 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     9747 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/expressions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3507 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/filters.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     8726 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/functions.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2863 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/identifiers.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    23601 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/operators.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    10083 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/query.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     2176 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/sorting.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/gml/
--rw-rw-r--   0 lars      (1000) lars      (1000)     1462 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1065 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3171 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/geometries.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     3553 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/tags.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     1038 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/values.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/queries/
--rw-rw-r--   0 lars      (1000) lars      (1000)      892 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7146 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/adhoc.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     5943 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/base.py
--rw-rw-r--   0 lars      (1000) lars      (1000)     7095 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/stored.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/static/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/static/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)      163 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/static/gisserver/index.css
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/
--rw-rw-r--   0 lars      (1000) lars      (1000)      866 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/index.html
--rw-rw-r--   0 lars      (1000) lars      (1000)      993 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/service_description.html
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/
--rw-rw-r--   0 lars      (1000) lars      (1000)     1041 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)     8675 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)      636 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
--rw-rw-r--   0 lars      (1000) lars      (1000)      538 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_field.html
--rw-rw-r--   0 lars      (1000) lars      (1000)      788 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_type.html
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/gisserver/templatetags/
--rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templatetags/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      204 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templatetags/gisserver_tags.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    34202 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/types.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    13252 2023-06-08 08:38:15.000000 django-gisserver-1.2.7/gisserver/views.py
--rw-rw-r--   0 lars      (1000) lars      (1000)      496 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/setup.cfg
--rwxrwxr-x   0 lars      (1000) lars      (1000)     2471 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13289 2024-04-18 12:51:07.000000 django-gisserver-1.3.0/CHANGES.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)    16725 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/LICENSE
+-rw-rw-r--   0 jan       (1000) jan       (1000)      227 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/MANIFEST.in
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2024-04-18 12:51:52.302746 django-gisserver-1.3.0/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4027 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/README.md
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.290745 django-gisserver-1.3.0/django_gisserver.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2024-04-18 12:51:52.000000 django-gisserver-1.3.0/django_gisserver.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1915 2024-04-18 12:51:52.000000 django-gisserver-1.3.0/django_gisserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-04-18 12:51:52.000000 django-gisserver-1.3.0/django_gisserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2022-09-07 10:15:14.000000 django-gisserver-1.3.0/django_gisserver.egg-info/not-zip-safe
+-rw-rw-r--   0 jan       (1000) jan       (1000)      180 2024-04-18 12:51:52.000000 django-gisserver-1.3.0/django_gisserver.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       10 2024-04-18 12:51:52.000000 django-gisserver-1.3.0/django_gisserver.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.294745 django-gisserver-1.3.0/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       40 2024-04-18 12:51:07.000000 django-gisserver-1.3.0/gisserver/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2108 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/conf.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5329 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/db.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4596 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/exceptions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    32232 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/features.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    12619 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/geometries.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.294745 django-gisserver-1.3.0/gisserver/operations/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/operations/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    17012 2023-06-08 09:30:35.000000 django-gisserver-1.3.0/gisserver/operations/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    18635 2023-06-08 09:31:53.000000 django-gisserver-1.3.0/gisserver/operations/wfs20.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.294745 django-gisserver-1.3.0/gisserver/output/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1950 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/output/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7954 2024-03-04 13:49:55.000000 django-gisserver-1.3.0/gisserver/output/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1542 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/output/buffer.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6179 2024-04-18 12:28:02.000000 django-gisserver-1.3.0/gisserver/output/csv.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    11217 2024-04-18 12:28:02.000000 django-gisserver-1.3.0/gisserver/output/geojson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    26894 2024-04-18 12:28:02.000000 django-gisserver-1.3.0/gisserver/output/gml32.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9224 2024-04-18 12:28:02.000000 django-gisserver-1.3.0/gisserver/output/results.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6113 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/output/utils.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4603 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/output/xmlschema.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.294745 django-gisserver-1.3.0/gisserver/parsers/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      290 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4864 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/base.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/parsers/fes20/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      624 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9747 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/expressions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3507 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/filters.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8726 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/functions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2863 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/identifiers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    23601 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/operators.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    10083 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/query.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2176 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/fes20/sorting.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/parsers/gml/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1462 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/gml/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1065 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/parsers/gml/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3171 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/gml/geometries.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3553 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/parsers/tags.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1038 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/parsers/values.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/queries/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      892 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/queries/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7146 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/queries/adhoc.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5943 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/queries/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7095 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/queries/stored.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.290745 django-gisserver-1.3.0/gisserver/static/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/static/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      163 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/static/gisserver/index.css
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.290745 django-gisserver-1.3.0/gisserver/templates/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/templates/gisserver/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      866 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/index.html
+-rw-rw-r--   0 jan       (1000) jan       (1000)      993 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/service_description.html
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1041 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8675 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      636 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      538 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/feature_field.html
+-rw-rw-r--   0 jan       (1000) jan       (1000)      788 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/feature_type.html
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-04-18 12:51:52.298745 django-gisserver-1.3.0/gisserver/templatetags/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templatetags/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      204 2022-09-07 09:58:17.000000 django-gisserver-1.3.0/gisserver/templatetags/gisserver_tags.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    34202 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/types.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13252 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/gisserver/views.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      496 2024-04-18 12:51:52.302746 django-gisserver-1.3.0/setup.cfg
+-rwxrwxr-x   0 jan       (1000) jan       (1000)     2471 2023-06-07 10:50:30.000000 django-gisserver-1.3.0/setup.py
```

### Comparing `django-gisserver-1.2.7/CHANGES.md` & `django-gisserver-1.3.0/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# 2023-06-08 (1.3.0)
+
+## Updates
+* Django 5 support added.
+
+## Contributors
+We would like to thank the following contributors
+for their work on this release.
+
+   - [tomdtp](https://github.com/tomdtp)
+  
 # 2023-06-08 (1.2.7)
 
 * WFS endpoints now accept a GML version number in their OUTPUTFORMAT.
 
 # 2023-06-07 (1.2.6)
 
 * Workaround for FME doing a DescribeFeatureType with the wrong outputformat.
```

### Comparing `django-gisserver-1.2.7/LICENSE` & `django-gisserver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/PKG-INFO` & `django-gisserver-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.7
+Version: 1.3.0
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -152,7 +153,9 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
+
+
```

### Comparing `django-gisserver-1.2.7/README.md` & `django-gisserver-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/django_gisserver.egg-info/PKG-INFO` & `django-gisserver-1.3.0/django_gisserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.7
+Version: 1.3.0
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -152,7 +153,9 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
+
+
```

### Comparing `django-gisserver-1.2.7/django_gisserver.egg-info/SOURCES.txt` & `django-gisserver-1.3.0/django_gisserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/conf.py` & `django-gisserver-1.3.0/gisserver/conf.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/db.py` & `django-gisserver-1.3.0/gisserver/db.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/exceptions.py` & `django-gisserver-1.3.0/gisserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/features.py` & `django-gisserver-1.3.0/gisserver/features.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/geometries.py` & `django-gisserver-1.3.0/gisserver/geometries.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/operations/base.py` & `django-gisserver-1.3.0/gisserver/operations/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/operations/wfs20.py` & `django-gisserver-1.3.0/gisserver/operations/wfs20.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/output/__init__.py` & `django-gisserver-1.3.0/gisserver/output/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/output/base.py` & `django-gisserver-1.3.0/gisserver/output/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/output/buffer.py` & `django-gisserver-1.3.0/gisserver/output/buffer.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/output/csv.py` & `django-gisserver-1.3.0/gisserver/output/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Output rendering logic for GeoJSON."""
 from __future__ import annotations
 
 import csv
-from datetime import datetime
+from datetime import datetime, timezone
 
 from django.conf import settings
 from django.db import models
-from django.utils.timezone import utc
 
 from gisserver import conf
 from gisserver.db import (
     AsEWKT,
     build_db_annotations,
     get_db_annotation,
     get_db_geometry_selects,
@@ -133,15 +132,15 @@
             if field.type.is_complex_type:
                 for sub_field in field.type.elements:
                     append(sub_field.get_value(value))
             elif isinstance(value, list):
                 # Array field
                 append(",".join(map(str, value)))
             elif isinstance(value, datetime):
-                append(str(value.astimezone(utc)))
+                append(str(value.astimezone(timezone.utc)))
             else:
                 append(value)
         return values
 
     def render_geometry(self, instance: models.Model, field: XsdElement):
         """Render the contents of a geometry value."""
         return field.get_value(instance)
```

### Comparing `django-gisserver-1.2.7/gisserver/output/geojson.py` & `django-gisserver-1.3.0/gisserver/output/geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Output rendering logic for GeoJSON."""
-from datetime import datetime
+from datetime import datetime, timezone
 from decimal import Decimal
 from typing import cast
 
 import orjson
 from django.conf import settings
 from django.contrib.gis.db.models.functions import AsGeoJSON
 from django.db import models
 from django.utils.functional import Promise
-from django.utils.timezone import utc
 
 from gisserver import conf
 from gisserver.db import get_db_geometry_target
 from gisserver.features import FeatureType
 from gisserver.geometries import CRS
 from gisserver.types import XsdComplexType
 
@@ -143,15 +142,15 @@
             geometry_name,
             self.render_geometry(feature_type, instance),
             orjson.dumps(properties, default=_json_default),
         )
 
     def _format_geojson_value(self, value):
         if isinstance(value, datetime):
-            return value.astimezone(utc)
+            return value.astimezone(timezone.utc)
         elif isinstance(value, models.Model):
             # ForeignKey, not defined as complex type.
             return str(value)
         else:
             return value
 
     def render_geometry(self, feature_type, instance: models.Model) -> bytes:
```

### Comparing `django-gisserver-1.2.7/gisserver/output/gml32.py` & `django-gisserver-1.3.0/gisserver/output/gml32.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 Note that the Django format_html() / mark_safe() logic is not used here,
 as it's quite a performance improvement to just use html.escape().
 """
 from __future__ import annotations
 
 import itertools
 import re
-from datetime import date, datetime, time
+from datetime import date, datetime, time, timezone
 from html import escape
 from typing import cast
 
 from django.contrib.gis import geos
 from django.db import models
 from django.http import HttpResponse
-from django.utils.timezone import utc
 
 from gisserver.db import (
     AsGML,
     build_db_annotations,
     conditional_transform,
     get_db_annotation,
     get_db_geometry_selects,
@@ -302,15 +301,15 @@
         xml_name = xsd_element.xml_name
         if value is None:
             return f'<{xml_name} xsi:nil="true"{extra_xmlns}/>\n'
         elif xsd_element.type.is_complex_type:
             # Expanded foreign relation / dictionary
             return self.render_xml_complex_type(feature_type, xsd_element, value)
         elif isinstance(value, datetime):
-            value = value.astimezone(utc).isoformat()
+            value = value.astimezone(timezone.utc).isoformat()
         elif isinstance(value, (date, time)):
             value = value.isoformat()
         elif isinstance(value, bool):
             value = "true" if value else "false"
         else:
             value = escape(str(value))
```

### Comparing `django-gisserver-1.2.7/gisserver/output/results.py` & `django-gisserver-1.3.0/gisserver/output/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import operator
 from functools import reduce
 from typing import Iterable
 
 import django
 from django.db import models
 from django.utils.functional import cached_property
-from django.utils.timezone import now, utc
+from django.utils.timezone import now
+
+from datetime import timezone
 
 from gisserver.features import FeatureType
 from gisserver.geometries import BoundingBox
 
 from .utils import ChunkedQuerySetIterator, CountingIterator
 
 
@@ -214,15 +216,15 @@
         :param previous: URL of the previous page
         """
         self.results = results
         self._number_matched = number_matched
         self.next = next
         self.previous = previous
         self.date = now()
-        self.timestamp = self.date.astimezone(utc).isoformat()
+        self.timestamp = self.date.astimezone(timezone.utc).isoformat()
 
     def get_bounding_box(self) -> BoundingBox:
         """Determine bounding box of all items."""
         # Combine the bounding box of all collections
         return reduce(operator.add, [c.get_bounding_box() for c in self.results])
 
     @cached_property
```

### Comparing `django-gisserver-1.2.7/gisserver/output/utils.py` & `django-gisserver-1.3.0/gisserver/output/utils.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/output/xmlschema.py` & `django-gisserver-1.3.0/gisserver/output/xmlschema.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/base.py` & `django-gisserver-1.3.0/gisserver/parsers/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/__init__.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/expressions.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/expressions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/filters.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/filters.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/functions.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/functions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/identifiers.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/identifiers.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/operators.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/operators.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/query.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/query.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/fes20/sorting.py` & `django-gisserver-1.3.0/gisserver/parsers/fes20/sorting.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/gml/__init__.py` & `django-gisserver-1.3.0/gisserver/parsers/gml/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/gml/base.py` & `django-gisserver-1.3.0/gisserver/parsers/gml/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/gml/geometries.py` & `django-gisserver-1.3.0/gisserver/parsers/gml/geometries.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/tags.py` & `django-gisserver-1.3.0/gisserver/parsers/tags.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/parsers/values.py` & `django-gisserver-1.3.0/gisserver/parsers/values.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/queries/__init__.py` & `django-gisserver-1.3.0/gisserver/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/queries/adhoc.py` & `django-gisserver-1.3.0/gisserver/queries/adhoc.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/queries/base.py` & `django-gisserver-1.3.0/gisserver/queries/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/queries/stored.py` & `django-gisserver-1.3.0/gisserver/queries/stored.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/index.html` & `django-gisserver-1.3.0/gisserver/templates/gisserver/index.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/service_description.html` & `django-gisserver-1.3.0/gisserver/templates/gisserver/service_description.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml` & `django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml` & `django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml` & `django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_field.html` & `django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/feature_field.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_type.html` & `django-gisserver-1.3.0/gisserver/templates/gisserver/wfs/feature_type.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/types.py` & `django-gisserver-1.3.0/gisserver/types.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/gisserver/views.py` & `django-gisserver-1.3.0/gisserver/views.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.7/setup.py` & `django-gisserver-1.3.0/setup.py`

 * *Files identical despite different names*

