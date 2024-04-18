# Comparing `tmp/oc_ds_converter-1.0.0.tar.gz` & `tmp/oc_ds_converter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ds_converter-1.0.0.tar", max compression
+gzip compressed data, was "oc_ds_converter-1.0.1.tar", max compression
```

## Comparing `oc_ds_converter-1.0.0.tar` & `oc_ds_converter-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0    22812 2023-10-12 11:02:44.578072 oc_ds_converter-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.571286 oc_ds_converter-1.0.0/oc_ds_converter/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.571392 oc_ds_converter-1.0.0/oc_ds_converter/crossref/__init__.py
--rw-r--r--   0        0        0    26929 2023-10-27 12:16:40.699448 oc_ds_converter-1.0.0/oc_ds_converter/crossref/crossref_processing.py
--rw-r--r--   0        0        0     4216 2023-06-16 10:03:56.571753 oc_ds_converter-1.0.0/oc_ds_converter/crossref/extract_crossref_publishers.py
--rw-r--r--   0        0        0     8938 2023-06-16 10:03:56.571889 oc_ds_converter-1.0.0/oc_ds_converter/crossref/get_not_crossref_ref.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.571970 oc_ds_converter-1.0.0/oc_ds_converter/datacite/__init__.py
--rw-r--r--   0        0        0    21894 2023-10-27 12:16:40.699919 oc_ds_converter-1.0.0/oc_ds_converter/datacite/datacite_processing.py
--rw-r--r--   0        0        0    34644 2023-10-27 12:16:40.700239 oc_ds_converter-1.0.0/oc_ds_converter/datacite/datacite_processing_new.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.572183 oc_ds_converter-1.0.0/oc_ds_converter/datasource/__init__.py
--rw-r--r--   0        0        0      316 2023-06-16 10:03:56.572293 oc_ds_converter-1.0.0/oc_ds_converter/datasource/config.ini
--rw-r--r--   0        0        0     1290 2023-06-16 10:03:56.572386 oc_ds_converter-1.0.0/oc_ds_converter/datasource/datasource.py
--rw-r--r--   0        0        0     3608 2023-06-19 16:57:56.877236 oc_ds_converter-1.0.0/oc_ds_converter/datasource/redis.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.572583 oc_ds_converter-1.0.0/oc_ds_converter/jalc/__init__.py
--rw-r--r--   0        0        0    16655 2023-10-27 12:16:40.701492 oc_ds_converter-1.0.0/oc_ds_converter/jalc/jalc_processing.py
--rw-r--r--   0        0        0     1008 2023-06-16 10:03:56.572938 oc_ds_converter-1.0.0/oc_ds_converter/lib/__init__.py
--rw-r--r--   0        0        0    16849 2023-06-16 10:03:56.573026 oc_ds_converter-1.0.0/oc_ds_converter/lib/cleaner.py
--rw-r--r--   0        0        0     5944 2023-06-16 10:03:56.573150 oc_ds_converter-1.0.0/oc_ds_converter/lib/csvmanager.py
--rw-r--r--   0        0        0     9348 2023-06-16 10:03:56.573295 oc_ds_converter-1.0.0/oc_ds_converter/lib/file_manager.py
--rw-r--r--   0        0        0     6287 2023-10-27 12:16:40.701785 oc_ds_converter-1.0.0/oc_ds_converter/lib/jsonmanager.py
--rw-r--r--   0        0        0     5145 2023-06-16 10:03:56.573514 oc_ds_converter-1.0.0/oc_ds_converter/lib/master_of_regex.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.573599 oc_ds_converter-1.0.0/oc_ds_converter/medra/__init__.py
--rw-r--r--   0        0        0    12155 2023-06-16 10:03:56.573755 oc_ds_converter-1.0.0/oc_ds_converter/medra/medra_processing.py
--rw-r--r--   0        0        0     3767 2023-06-16 10:03:56.573869 oc_ds_converter-1.0.0/oc_ds_converter/metadata_manager.py
--rw-r--r--   0        0        0     1712 2023-06-16 10:03:56.574123 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/__init__.py
--rw-r--r--   0        0        0     9586 2023-06-16 10:03:56.574269 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/arxiv.py
--rw-r--r--   0        0        0     5493 2023-06-16 10:03:56.574388 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/base.py
--rw-r--r--   0        0        0     6337 2023-06-16 10:03:56.574493 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/doi.py
--rw-r--r--   0        0        0     3509 2023-06-16 10:03:56.574640 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/isbn.py
--rw-r--r--   0        0        0     2996 2023-06-16 10:03:56.574743 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/issn.py
--rw-r--r--   0        0        0     8377 2023-06-16 10:03:56.574859 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/jid.py
--rw-r--r--   0        0        0     3770 2023-06-16 10:03:56.574961 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/metadata_manager.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.575080 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/__init__.py
--rw-r--r--   0        0        0     5306 2023-06-16 10:03:56.575228 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py
--rw-r--r--   0        0        0     4880 2023-06-19 16:57:56.877666 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py
--rw-r--r--   0        0        0     5826 2023-06-16 10:03:56.575437 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py
--rw-r--r--   0        0        0     1985 2023-06-16 10:03:56.575523 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py
--rw-r--r--   0        0        0     8701 2023-10-11 12:56:45.461690 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/orcid.py
--rw-r--r--   0        0        0     7153 2023-06-16 10:03:56.575763 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/pmcid.py
--rw-r--r--   0        0        0    16260 2023-06-16 10:03:56.575850 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/pmid.py
--rw-r--r--   0        0        0     5772 2023-06-16 10:03:56.575953 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/ror.py
--rw-r--r--   0        0        0     2043 2023-06-16 10:03:56.576060 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/support.py
--rw-r--r--   0        0        0     5936 2023-06-16 10:03:56.576174 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/url.py
--rw-r--r--   0        0        0     6486 2023-06-16 10:03:56.576281 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/viaf.py
--rw-r--r--   0        0        0     5984 2023-06-16 10:03:56.576382 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/wikidata.py
--rw-r--r--   0        0        0     6165 2023-06-16 10:03:56.576487 oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/wikipedia.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.576581 oc_ds_converter-1.0.0/oc_ds_converter/openaire/__init__.py
--rw-r--r--   0        0        0    33345 2023-10-27 12:16:40.702707 oc_ds_converter-1.0.0/oc_ds_converter/openaire/openaire_processing.py
--rw-r--r--   0        0        0        2 2023-09-11 16:37:46.342974 oc_ds_converter-1.0.0/oc_ds_converter/openaire/support_files/prefix_publishers.json
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.576954 oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/__init__.py
--rw-r--r--   0        0        0     4212 2023-06-16 10:03:56.577093 oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/base.py
--rw-r--r--   0        0        0     5966 2023-10-27 12:16:40.702965 oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/datacite.py
--rw-r--r--   0        0        0    14435 2023-10-26 00:47:11.758928 oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/jalc.py
--rw-r--r--   0        0        0     4727 2023-06-16 10:03:56.577301 oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/nih.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.577377 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/__init__.py
--rw-r--r--   0        0        0     4604 2023-06-16 10:03:56.577498 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/finder_nih.py
--rw-r--r--   0        0        0     7764 2023-06-16 10:03:56.577607 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/get_publishers.py
--rw-r--r--   0        0        0     2373 2023-06-16 10:03:56.577708 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/pubmed_dump_explorer.py
--rw-r--r--   0        0        0    33023 2023-06-16 10:03:56.577936 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/pubmed_processing.py
--rw-r--r--   0        0        0      483 2023-06-16 10:03:56.578122 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
--rw-r--r--   0        0        0   304902 2023-06-16 10:03:56.579122 oc_ds_converter-1.0.0/oc_ds_converter/pubmed/support_files/prefix_publishers.json
--rw-r--r--   0        0        0    11671 2023-06-16 10:03:56.579286 oc_ds_converter-1.0.0/oc_ds_converter/ra_processor.py
--rw-r--r--   0        0        0        0 2023-06-16 10:03:56.579381 oc_ds_converter-1.0.0/oc_ds_converter/run/__init__.py
--rw-r--r--   0        0        0    25153 2023-10-27 12:16:40.703686 oc_ds_converter-1.0.0/oc_ds_converter/run/crossref_process.py
--rw-r--r--   0        0        0     6544 2023-06-16 10:03:56.579609 oc_ds_converter-1.0.0/oc_ds_converter/run/datacite_process.py
--rw-r--r--   0        0        0    11406 2023-10-27 12:16:40.703902 oc_ds_converter-1.0.0/oc_ds_converter/run/datacite_process_new.py
--rw-r--r--   0        0        0    24449 2023-10-27 12:16:40.704202 oc_ds_converter-1.0.0/oc_ds_converter/run/jalc_process.py
--rw-r--r--   0        0        0    25809 2023-10-09 22:40:22.167709 oc_ds_converter-1.0.0/oc_ds_converter/run/openaire_process.py
--rw-r--r--   0        0        0     9518 2023-06-16 10:03:56.580003 oc_ds_converter-1.0.0/oc_ds_converter/run/pubmed_process.py
--rw-r--r--   0        0        0     1036 2023-10-27 12:22:47.283915 oc_ds_converter-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    24279 1970-01-01 00:00:00.000000 oc_ds_converter-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.455704 oc_ds_converter-1.0.1/oc_ds_converter/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.456704 oc_ds_converter-1.0.1/oc_ds_converter/crossref/__init__.py
+-rw-r--r--   0        0        0    27506 2024-04-18 13:08:16.457703 oc_ds_converter-1.0.1/oc_ds_converter/crossref/crossref_processing.py
+-rw-r--r--   0        0        0     4337 2024-04-18 13:08:16.458701 oc_ds_converter-1.0.1/oc_ds_converter/crossref/extract_crossref_publishers.py
+-rw-r--r--   0        0        0     9101 2024-04-18 13:08:16.459704 oc_ds_converter-1.0.1/oc_ds_converter/crossref/get_not_crossref_ref.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.459704 oc_ds_converter-1.0.1/oc_ds_converter/datacite/__init__.py
+-rw-r--r--   0        0        0    38522 2024-04-18 13:08:16.460703 oc_ds_converter-1.0.1/oc_ds_converter/datacite/datacite_processing.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.461708 oc_ds_converter-1.0.1/oc_ds_converter/datasource/__init__.py
+-rw-r--r--   0        0        0      336 2024-04-18 13:08:16.462704 oc_ds_converter-1.0.1/oc_ds_converter/datasource/config.ini
+-rw-r--r--   0        0        0     1329 2024-04-18 13:08:16.462704 oc_ds_converter-1.0.1/oc_ds_converter/datasource/datasource.py
+-rw-r--r--   0        0        0     3702 2024-04-18 13:08:16.463706 oc_ds_converter-1.0.1/oc_ds_converter/datasource/redis.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.464704 oc_ds_converter-1.0.1/oc_ds_converter/jalc/__init__.py
+-rw-r--r--   0        0        0    17007 2024-04-18 13:08:16.465704 oc_ds_converter-1.0.1/oc_ds_converter/jalc/jalc_processing.py
+-rw-r--r--   0        0        0     1025 2024-04-18 13:08:16.466705 oc_ds_converter-1.0.1/oc_ds_converter/lib/__init__.py
+-rw-r--r--   0        0        0    17248 2024-04-18 13:08:16.467705 oc_ds_converter-1.0.1/oc_ds_converter/lib/cleaner.py
+-rw-r--r--   0        0        0     6083 2024-04-18 13:08:16.468706 oc_ds_converter-1.0.1/oc_ds_converter/lib/csvmanager.py
+-rw-r--r--   0        0        0     9573 2024-04-18 13:08:16.469705 oc_ds_converter-1.0.1/oc_ds_converter/lib/file_manager.py
+-rw-r--r--   0        0        0     6423 2024-04-18 13:08:16.470706 oc_ds_converter-1.0.1/oc_ds_converter/lib/jsonmanager.py
+-rw-r--r--   0        0        0     5260 2024-04-18 13:08:16.471706 oc_ds_converter-1.0.1/oc_ds_converter/lib/master_of_regex.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.471706 oc_ds_converter-1.0.1/oc_ds_converter/medra/__init__.py
+-rw-r--r--   0        0        0    12416 2024-04-18 13:08:16.472705 oc_ds_converter-1.0.1/oc_ds_converter/medra/medra_processing.py
+-rw-r--r--   0        0        0     3843 2024-04-18 13:08:16.473705 oc_ds_converter-1.0.1/oc_ds_converter/metadata_manager.py
+-rw-r--r--   0        0        0     1877 2024-04-18 13:08:16.474704 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/__init__.py
+-rw-r--r--   0        0        0     9816 2024-04-18 13:08:16.475703 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/arxiv.py
+-rw-r--r--   0        0        0     5612 2024-04-18 13:08:16.476706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/base.py
+-rw-r--r--   0        0        0     5247 2024-04-18 13:08:16.477705 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/crossref.py
+-rw-r--r--   0        0        0    11303 2024-04-18 13:08:16.478706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/doi.py
+-rw-r--r--   0        0        0     3602 2024-04-18 13:08:16.479707 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/isbn.py
+-rw-r--r--   0        0        0     3069 2024-04-18 13:08:16.479707 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/issn.py
+-rw-r--r--   0        0        0     8567 2024-04-18 13:08:16.480703 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/jid.py
+-rw-r--r--   0        0        0     3845 2024-04-18 13:08:16.480703 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/metadata_manager.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.481705 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/__init__.py
+-rw-r--r--   0        0        0     5443 2024-04-18 13:08:16.482705 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py
+-rw-r--r--   0        0        0     5011 2024-04-18 13:08:16.483705 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py
+-rw-r--r--   0        0        0     5973 2024-04-18 13:08:16.484706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py
+-rw-r--r--   0        0        0     2042 2024-04-18 13:08:16.485706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py
+-rw-r--r--   0        0        0     7243 2024-04-18 13:08:16.485706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/openalex.py
+-rw-r--r--   0        0        0     8915 2024-04-18 13:08:16.486704 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/orcid.py
+-rw-r--r--   0        0        0     7317 2024-04-18 13:08:16.487704 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/pmcid.py
+-rw-r--r--   0        0        0    16651 2024-04-18 13:08:16.488704 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/pmid.py
+-rw-r--r--   0        0        0     5903 2024-04-18 13:08:16.489706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/ror.py
+-rw-r--r--   0        0        0     2094 2024-04-18 13:08:16.489706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/support.py
+-rw-r--r--   0        0        0     6081 2024-04-18 13:08:16.490705 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/url.py
+-rw-r--r--   0        0        0     6637 2024-04-18 13:08:16.491703 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/viaf.py
+-rw-r--r--   0        0        0     6116 2024-04-18 13:08:16.492708 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/wikidata.py
+-rw-r--r--   0        0        0     6304 2024-04-18 13:08:16.493706 oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/wikipedia.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.493706 oc_ds_converter-1.0.1/oc_ds_converter/openaire/__init__.py
+-rw-r--r--   0        0        0    34044 2024-04-18 13:08:16.495703 oc_ds_converter-1.0.1/oc_ds_converter/openaire/openaire_processing.py
+-rw-r--r--   0        0        0        2 2024-04-18 13:08:16.495703 oc_ds_converter-1.0.1/oc_ds_converter/openaire/support_files/prefix_publishers.json
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.496704 oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4315 2024-04-18 13:08:16.497704 oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/base.py
+-rw-r--r--   0        0        0     6110 2024-04-18 13:08:16.498704 oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/datacite.py
+-rw-r--r--   0        0        0    14692 2024-04-18 13:08:16.499705 oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/jalc.py
+-rw-r--r--   0        0        0     4827 2024-04-18 13:08:16.500706 oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/nih.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.500706 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-18 13:08:16.501703 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/finder_nih.py
+-rw-r--r--   0        0        0     7950 2024-04-18 13:08:16.502704 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/get_publishers.py
+-rw-r--r--   0        0        0     2428 2024-04-18 13:08:16.503704 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/pubmed_dump_explorer.py
+-rw-r--r--   0        0        0    35075 2024-04-18 13:08:16.504704 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/pubmed_processing.py
+-rw-r--r--   0        0        0      503 2024-04-18 13:08:16.505721 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
+-rw-r--r--   0        0        0   315988 2024-04-18 13:08:16.509702 oc_ds_converter-1.0.1/oc_ds_converter/pubmed/support_files/prefix_publishers.json
+-rw-r--r--   0        0        0    11903 2024-04-18 13:08:16.510702 oc_ds_converter-1.0.1/oc_ds_converter/ra_processor.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:08:16.511704 oc_ds_converter-1.0.1/oc_ds_converter/run/__init__.py
+-rw-r--r--   0        0        0    25869 2024-04-18 13:08:16.512704 oc_ds_converter-1.0.1/oc_ds_converter/run/crossref_process.py
+-rw-r--r--   0        0        0    29918 2024-04-18 13:08:16.513702 oc_ds_converter-1.0.1/oc_ds_converter/run/datacite_process.py
+-rw-r--r--   0        0        0    25140 2024-04-18 13:08:16.514703 oc_ds_converter-1.0.1/oc_ds_converter/run/jalc_process.py
+-rw-r--r--   0        0        0    26521 2024-04-18 13:08:16.515704 oc_ds_converter-1.0.1/oc_ds_converter/run/openaire_process.py
+-rw-r--r--   0        0        0     9887 2024-04-18 13:08:16.516704 oc_ds_converter-1.0.1/oc_ds_converter/run/pubmed_process.py
+-rw-r--r--   0        0        0    33527 2024-04-18 13:08:16.517704 oc_ds_converter-1.0.1/oc_ds_converter/run/pubmed_process_new.py
+-rw-r--r--   0        0        0     1078 2024-04-18 13:13:46.390529 oc_ds_converter-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    23044 2024-04-18 13:08:16.450708 oc_ds_converter-1.0.1/README.md
+-rw-r--r--   0        0        0    24330 1970-01-01 00:00:00.000000 oc_ds_converter-1.0.1/PKG-INFO
```

### Comparing `oc_ds_converter-1.0.0/README.md` & `oc_ds_converter-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: oc-ds-converter
+Version: 1.0.1
+Summary: A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta.
+License: ISC
+Author: arcangelo7
+Author-email: arcangelomas@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
+Requires-Dist: fakeredis (>=2.14.0,<3.0.0)
+Requires-Dist: filelock (>=3.12.2,<4.0.0)
+Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: ndjson (>=0.3.1,<0.4.0)
+Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pebble (>=5.0.3,<6.0.0)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: self (>=2020.12.3,<2021.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: update (>=0.0.1,<0.0.2)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Requires-Dist: zstandard (>=0.21.0,<0.22.0)
+Description-Content-Type: text/markdown
+
 [<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
 [![Run tests](https://github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/run_tests.yml)
 ![Coverage](https://raw.githubusercontent.com/opencitations/ra_processor/main/test/coverage/coverage.svg)
 <!-- ![PyPI](https://img.shields.io/pypi/pyversions/oc_meta) -->
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/ra_processor)
 
 # OpenCitations Data Sources Converter
@@ -226,7 +263,8 @@
 - [The OpenCitations Data Model](https://link.springer.com/chapter/10.1007/978-3-030-62466-8_28)
 - [OpenCitations Meta](https://doi.org/10.48550/arXiv.2306.16191)
 - [Metadata crosswalk for citation data production in OpenCitations](https://marketplace.sshopencloud.eu/workflow/MHwO4l)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
+
```

#### html2text {}

```diff
@@ -1,8 +1,28 @@
-[[https://img.shields.io/badge/powered%20by-OpenCitations-
+Metadata-Version: 2.1 Name: oc-ds-converter Version: 1.0.1 Summary: A library
+for converting metadata provided by various data sources, e.g. Crossref,
+DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta. License:
+ISC Author: arcangelo7 Author-email: arcangelomas@gmail.com Requires-Python:
+>=3.8,<4.0 Classifier: License :: OSI Approved Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0) Requires-Dist: fakeredis
+(>=2.14.0,<3.0.0) Requires-Dist: filelock (>=3.12.2,<4.0.0) Requires-Dist: lxml
+(>=5.1.0,<6.0.0) Requires-Dist: ndjson (>=0.3.1,<0.4.0) Requires-Dist:
+packaging (>=23.1,<24.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
+pebble (>=5.0.3,<6.0.0) Requires-Dist: poetry (>=1.5.1,<2.0.0) Requires-Dist:
+python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: self
+(>=2020.12.3,<2021.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-Dist:
+tqdm (>=4.65.0,<5.0.0) Requires-Dist: update (>=0.0.1,<0.0.2) Requires-Dist:
+validators (>=0.20.0,<0.21.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Requires-Dist: zstandard (>=0.21.0,<0.22.0) Description-Content-Type: text/
+markdown [[https://img.shields.io/badge/powered%20by-OpenCitations-
 %239931FC?labelColor=2D22DE]](http://opencitations.net) [![Run tests](https://
 github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/
 badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/
 run_tests.yml) ![Coverage](https://raw.githubusercontent.com/opencitations/
 ra_processor/main/test/coverage/coverage.svg) ![GitHub code size in bytes]
 (https://img.shields.io/github/languages/code-size/opencitations/ra_processor)
 # OpenCitations Data Sources Converter This repository contains scripts for
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/crossref/crossref_processing.py` & `oc_ds_converter-1.0.1/oc_ds_converter/crossref/crossref_processing.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,577 +1,577 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
-# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import html
-import re
-import warnings
-from pathlib import Path
-from typing import Optional
-import os
-import os.path
-import json
-import csv
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager import DOIManager
-from oc_ds_converter.oc_idmanager import ORCIDManager
-from oc_ds_converter.oc_idmanager import ISSNManager
-
-from oc_ds_converter.lib.master_of_regex import *
-import fakeredis
-from oc_ds_converter.datasource.redis import RedisDataSource
-from oc_ds_converter.ra_processor import RaProcessor
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Dict, List, Tuple
-from oc_ds_converter.lib.cleaner import Cleaner
-
-
-
-warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
-
-class CrossrefProcessing(RaProcessor):
-
-    def __init__(self, orcid_index:str=None, doi_csv:str=None, publishers_filepath:str=None, testing: bool = True, storage_manager: Optional[StorageManager] = None, citing=True):
-        super(CrossrefProcessing, self).__init__(orcid_index, doi_csv, publishers_filepath)
-        self.citing = citing
-
-        if storage_manager is None:
-            self.storage_manager = SqliteStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self.temporary_manager = InMemoryStorageManager('../memory.json')
-
-        self.doi_m = DOIManager(storage_manager=self.storage_manager)
-        self.orcid_m = ORCIDManager(storage_manager=self.storage_manager)
-        self.issn_m = ISSNManager()
-
-        self.venue_id_man_dict = {"issn": self.issn_m}
-        # Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
-        # main storage_manager  only once the full file is processed. Checks must be done both on tmp and in
-        # storage_manager, so that in case the process breaks while processing a file which does not complete (so
-        # without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
-        # a storage_manager db would be considered to have been processed and thus would be ignored by the process
-        # and lost.
-
-        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
-        self.tmp_orcid_m = ORCIDManager(storage_manager=self.temporary_manager)
-
-
-        self.venue_tmp_id_man_dict = {"issn": self.issn_m}
-
-        if testing:
-            self.BR_redis = fakeredis.FakeStrictRedis()
-            self.RA_redis= fakeredis.FakeStrictRedis()
-
-
-        else:
-            self.BR_redis = RedisDataSource("DB-META-BR")
-            self.RA_redis = RedisDataSource("DB-META-RA")
-
-
-        self._redis_values_br = []
-        self._redis_values_ra = []
-
-
-    def update_redis_values(self, br, ra):
-        self._redis_values_br = br
-        self._redis_values_ra = ra
-
-    def to_validated_id_list(self, norm_id_dict):
-        """this method takes in input a dictionary representing a normalized id, i.e.: {id:"id:000", "schema":"id"} and returns a list containing the validated id if it is valid, and an empty list otheriwse.
-        A first validation try is made by checking its presence in META db. If the id is not in META db yet,
-        a second attempt is made by using the specific id-schema API"""
-        #if self.BR_redis.get(norm_id):
-        valid_id_list = []
-        norm_id = norm_id_dict.get("id")
-        schema = norm_id_dict.get("schema")
-        if schema == "doi":
-            if norm_id in self._redis_values_br:
-                self.tmp_doi_m.storage_manager.set_value(norm_id, True) #In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-                # preso in considerazione negli step successivi
-                valid_id_list.append(norm_id)
-            # if the id is not in redis db, validate it before appending
-            elif self.tmp_doi_m.is_valid(norm_id):#In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-                # preso in considerazione negli step successivi
-                valid_id_list.append(norm_id)
-        elif schema == "orcid":
-            if norm_id in self._redis_values_ra:
-                self.tmp_orcid_m.storage_manager.set_value(norm_id, True) #In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-                # preso in considerazione negli step successivi
-                valid_id_list.append(norm_id)
-            # if the id is not in redis db, validate it before appending
-            elif self.tmp_orcid_m.is_valid(norm_id):#In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-                # preso in considerazione negli step successivi
-                valid_id_list.append(norm_id)
-
-        else:
-            print("Schema not accepted:", norm_id_dict.get("schema"), "in ", norm_id_dict, ". Use 'orcid' or 'doi'.")
-
-
-        return valid_id_list
-
-    def memory_to_storage(self):
-        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
-        if kv_in_memory:
-            self.storage_manager.set_multi_value(kv_in_memory)
-            self.temporary_manager.delete_storage()
-
-
-    def validated_as(self, id_dict):
-        # Check if the validity was already retrieved and thus
-        # a) if it is now saved either in the in-memory database, which only concerns data validated
-        # during the current file processing;
-        # b) or if it is now saved in the storage_manager database, which only concerns data validated
-        # during the previous files processing.
-        # In memory db is checked first because the dimension is smaller and the check is faster and
-        # Because we assume that it is more likely to find the same ids in close positions, e.g.: same
-        # citing id in several citations with different cited ids.
-
-        schema = id_dict["schema"].strip().lower()
-        id = id_dict["identifier"]
-
-        if schema == "orcid":
-            tmp_id_m = self.tmp_orcid_m
-            validity_value = tmp_id_m.validated_as_id(id)
-
-            if validity_value is None:
-                id_m = self.orcid_m
-                validity_value = id_m.validated_as_id(id)
-            return validity_value
-
-        elif schema == "doi":
-            validity_value = self.tmp_doi_m.validated_as_id(id)
-            if validity_value is None:
-                validity_value = self.doi_m.validated_as_id(id)
-            return validity_value
-        else:
-            print("invalid schema in ", id_dict, ". schema should be either doi or orcid.")
-            return None
-
-
-    def get_id_manager(self, schema_or_id, id_man_dict):
-        """Given as input the string of a schema (e.g.:'pmid') and a dictionary mapping strings of
-        the schemas to their id managers, the method returns the correct id manager. Note that each
-        instance of the Preprocessing class needs its own instances of the id managers, in order to
-        avoid conflicts while validating data"""
-        if ":" in schema_or_id:
-            split_id_prefix = schema_or_id.split(":")
-            schema = split_id_prefix[0]
-        else:
-            schema = schema_or_id
-        id_man = id_man_dict.get(schema)
-        return id_man
-
-
-    def dict_to_cache(self, dict_to_be_saved, path):
-        path = Path(path)
-        parent_dir_path = path.parent.absolute()
-        if not os.path.exists(parent_dir_path):
-            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
-        with open(path, "w", encoding="utf-8") as fd:
-            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
-
-    def csv_creator(self, item:dict) -> dict:
-        row = dict()
-        if not 'DOI' in item:
-            return row
-        doi_manager = DOIManager(use_api_service=False)
-        if isinstance(item['DOI'], list):
-            doi = doi_manager.normalise(str(item['DOI'][0]), include_prefix=False)
-        else:
-            doi = doi_manager.normalise(str(item['DOI']), include_prefix=False)
-        if (doi and self.doi_set and doi in self.doi_set) or (doi and not self.doi_set):
-            # create empty row
-            keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
-                    'publisher', 'editor']
-            for k in keys:
-                row[k] = ''
-
-            if 'type' in item:
-                if item['type']:
-                    row['type'] = item['type'].replace('-', ' ')
-
-            # row['id']
-            ids_list = list()
-            ids_list.append(str('doi:' + doi))
-
-            if 'ISBN' in item:
-                if row['type'] in {'book', 'dissertation', 'edited book', 'monograph', 'reference book', 'report', 'standard'}:
-                    self.id_worker(item['ISBN'], ids_list, self.isbn_worker)
-
-            if 'ISSN' in item:
-                if row['type'] in {'book series', 'book set', 'journal', 'proceedings series', 'series', 'standard series'}:
-                    self.id_worker(item['ISSN'], ids_list, self.issn_worker)
-                elif row['type'] == 'report series':
-                    br_id = True
-                    if 'container-title' in item:
-                        if item['container-title']:
-                            br_id = False
-                    if br_id:
-                        self.id_worker(item['ISSN'], ids_list, self.issn_worker)
-            row['id'] = ' '.join(ids_list)
-
-            # row['title']
-            if 'title' in item:
-                if item['title']:
-                    if isinstance(item['title'], list):
-                        text_title = item['title'][0]
-                    else:
-                        text_title = item['title']
-                    soup = BeautifulSoup(text_title, 'html.parser')
-                    title_soup = soup.get_text().replace('\n', '')
-                    title = html.unescape(title_soup)
-                    row['title'] = title
-
-            agents_list = []
-            if 'author' in item:
-                for author in item['author']:
-                    author['role'] = 'author'
-                agents_list.extend(item['author'])
-            if 'editor' in item:
-                for editor in item['editor']:
-                    editor['role'] = 'editor'
-                agents_list.extend(item['editor'])
-            authors_strings_list, editors_string_list = self.get_agents_strings_list(doi, agents_list)
-
-            # row['author']
-            if 'author' in item:
-                row['author'] = '; '.join(authors_strings_list)
-
-            # row['pub_date']
-            if 'issued' in item:
-                if item['issued']['date-parts'][0][0]:
-                    row['pub_date'] = '-'.join([str(y) for y in item['issued']['date-parts'][0]])
-                else:
-                    row['pub_date'] = ''
-
-            # row['venue']
-            row['venue'] = self.get_venue_name(item, row)
-
-            if 'volume' in item:
-                row['volume'] = item['volume']
-            if 'issue' in item:
-                row['issue'] = item['issue']
-            if 'page' in item:
-                row['page'] = self.get_crossref_pages(item)
-
-            row['publisher'] = self.get_publisher_name(doi, item)                        
-
-            if 'editor' in item:
-                row['editor'] = '; '.join(editors_string_list)
-        return self.normalise_unicode(row)
-        
-    def get_crossref_pages(self, item:dict) -> str:
-        '''
-        This function returns the pages interval. 
-
-        :params item: the item's dictionary
-        :type item: dict
-        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
-        '''
-        pages_list = re.split(pages_separator, item['page'])
-        return self.get_pages(pages_list)
-    
-    def get_publisher_name(self, doi:str, item:dict) -> str:
-        '''
-        This function aims to return a publisher's name and id. If a mapping was provided, 
-        it is used to find the publisher's standardized name from its id or DOI prefix. 
-
-        :params doi: the item's DOI
-        :type doi: str
-        :params item: the item's dictionary
-        :type item: dict
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output is only the name. Finally, if there is no publisher, the output is an empty string.
-        '''
-        data = {
-            'publisher': '',
-            'member': None,
-            'prefix': doi.split('/')[0]
-        }
-        for field in {'publisher', 'member', 'prefix'}:
-            if field in item:
-                if item[field]:
-                    data[field] = item[field]
-        publisher = data['publisher']
-        member = data['member']
-        prefix = data['prefix']
-        relevant_member = False
-
-        if self.publishers_mapping and member:
-            if member in self.publishers_mapping:
-                relevant_member = True
-        if self.publishers_mapping:
-            if relevant_member:
-                name = self.publishers_mapping[member]['name']
-                name_and_id = f'{name} [crossref:{member}]'
-            else:
-                member_dict = next(({member:data} for member, data in self.publishers_mapping.items() if prefix in data['prefixes']), None)
-                if member_dict:
-                    member = list(member_dict.keys())[0]
-                    name_and_id = f"{member_dict[member]['name']} [crossref:{member}]"
-                else:
-                    name_and_id = publisher
-        else:
-            name_and_id = f'{publisher} [crossref:{member}]' if member else publisher
-        return name_and_id
-
-
-    def get_venue_name(self, item:dict, row:dict) -> str:
-        '''
-        This method deals with generating the venue's name, followed by id in square brackets, separated by spaces. 
-        HTML tags are deleted and HTML entities escaped. In addition, any ISBN and ISSN are validated. 
-        Finally, the square brackets in the venue name are replaced by round brackets to avoid conflicts with the ids enclosures.
-
-        :params item: the item's dictionary
-        :type item: dict
-        :params row: a CSV row
-        :type row: dict
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'Nutrition & Food Science [issn:0034-6659]'. If the id does not exist, the output is only the name. Finally, if there is no venue, the output is an empty string.
-        '''
-        name_and_id = ''
-        if 'container-title' in item:
-            if item['container-title']:
-                if isinstance(item['container-title'], list):
-                    ventit = str(item['container-title'][0]).replace('\n', '')
-                else:
-                    ventit = str(item['container-title']).replace('\n', '')
-                ven_soup = BeautifulSoup(ventit, 'html.parser')
-                ventit = html.unescape(ven_soup.get_text())
-                ambiguous_brackets = re.search(ids_inside_square_brackets, ventit)
-                if ambiguous_brackets:
-                    match = ambiguous_brackets.group(1)
-                    open_bracket = ventit.find(match) - 1
-                    close_bracket = ventit.find(match) + len(match)
-                    ventit = ventit[:open_bracket] + '(' + ventit[open_bracket + 1:]
-                    ventit = ventit[:close_bracket] + ')' + ventit[close_bracket + 1:]
-                venids_list = list()
-                if 'ISBN' in item:
-                    if row['type'] in {'book chapter', 'book part', 'book section', 'book track', 'reference entry'}:
-                        self.id_worker(item['ISBN'], venids_list, self.isbn_worker)
-
-                if 'ISSN' in item:
-                    if row['type'] in {'book', 'data file', 'dataset', 'edited book', 'journal article', 'journal volume', 'journal issue', 'monograph', 'proceedings', 'peer review', 'reference book', 'reference entry', 'report'}:
-                        self.id_worker(item['ISSN'], venids_list, self.issn_worker)
-                    elif row['type'] == 'report series':
-                        if 'container-title' in item:
-                            if item['container-title']:
-                                self.id_worker(item['ISSN'], venids_list, self.issn_worker)
-                if venids_list:
-                    name_and_id = ventit + ' [' + ' '.join(venids_list) + ']'
-                else:
-                    name_and_id = ventit
-        return name_and_id
-
-    # UPDATED FOR CROSSREF √
-    def extract_all_ids(self, entity_dict, is_first_iteration: bool):
-        all_br = set()
-        all_ra = set()
-
-        if is_first_iteration:
-            # VALIDATE RESPONSIBLE AGENTS IDS FOR THE CITING ENTITY (THE CITING ENTITY DOI IS VALID BY
-            # DEFAULT SINCE IT WAS ASSIGNED BY CROSSREF, WHICH IS ALSO ITS DOI REGISTRATION AGENCY.
-
-            # EXTRA: THE CITING DOI IS VALID BY DEFAULT
-            # d1_br = entity_dict.get("DOI")
-            # if d1_br:
-            #  norm_id = self.doi_m.normalise(d1_br, include_prefix=True)
-            #  if norm_id:
-            #     all_br.add(norm_id)
-
-            if entity_dict.get("author"):
-                for author in entity_dict["author"]:
-                        if "ORCID" in author:
-                            orcid = self.orcid_m.normalise(
-                                author["ORCID"]
-                            )
-                            if orcid:
-                                all_ra.add(orcid)
-
-            if entity_dict.get("editor"):
-                for author in entity_dict["editor"]:
-                        if "ORCID" in author:
-                            orcid = self.orcid_m.normalise(
-                                author["ORCID"]
-                            )
-                            if orcid:
-                                all_ra.add(orcid)
-
-        # RETRIEVE CITED IDS OF A CITING ENTITY
-        else:
-            citations = [x for x in entity_dict["reference"] if x.get("DOI")]
-            for cit in citations:
-                norm_id = self.doi_m.normalise(cit["DOI"], include_prefix=True)
-                if norm_id:
-                    all_br.add(norm_id)
-
-        all_br = list(all_br)
-        all_ra = list(all_ra)
-        return all_br, all_ra
-
-
-    def get_reids_validity_list(self, id_list, redis_db):
-        if redis_db == "ra":
-            valid_ra_ids = []
-            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
-            validity_list_ra = self.RA_redis.mget(id_list)
-            for i, e in enumerate(id_list):
-                if validity_list_ra[i]:
-                    valid_ra_ids.append(e)
-            return valid_ra_ids
-
-        elif redis_db == "br":
-            valid_br_ids = []
-            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
-            validity_list_br = self.BR_redis.mget(id_list)
-            for i, e in enumerate(id_list):
-                if validity_list_br[i]:
-                    valid_br_ids.append(e)
-            return valid_br_ids
-        else:
-            raise ValueError("redis_db must be either 'ra' for responsible agents ids "
-                             "or 'br' for bibliographic resources ids")
-
-    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
-        authors_strings_list = list()
-        editors_string_list = list()
-        dict_orcid = None
-        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list):
-            dict_orcid = self.orcid_finder(doi)
-        agents_list = [
-            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None
-            else v for k, v in agent_dict.items()} for agent_dict in agents_list]
-
-        for agent in agents_list:
-            cur_role = agent['role']
-            f_name = None
-            g_name = None
-            agent_string = None
-            if agent.get('family') and agent.get('given'):
-                f_name = agent['family']
-                g_name = agent['given']
-                agent_string = f_name + ', ' + g_name
-            elif agent.get('name'):
-                agent_string = agent['name']
-                f_name = agent_string.split(",")[0].strip() if "," in agent_string else None
-                g_name = agent_string.split(",")[-1].strip() if "," in agent_string else None
-
-                if f_name and g_name:
-                    agent_string = f_name + ', ' + g_name
-            if agent_string is None:
-                if agent.get('family') and not agent.get('given'):
-                    if g_name:
-                        agent_string = agent['family'] + ', ' + g_name
-                    else:
-                        agent_string = agent['family'] + ', '
-                elif agent.get('given') and not agent.get('family'):
-                    if f_name:
-                        agent_string = f_name + ', ' + agent['given']
-                    else:
-                        agent_string = ', ' + agent['given']
-            orcid = None
-            if 'orcid' in agent:
-                if isinstance(agent['orcid'], list):
-                    orcid = str(agent['orcid'][0])
-                else:
-                    orcid = str(agent['orcid'])
-            elif 'ORCID' in agent:
-                if isinstance(agent['ORCID'], list):
-                    orcid = str(agent['ORCID'][0])
-                else:
-                    orcid = str(agent['ORCID'])
-            if orcid:
-
-                # VALIDATE ORCID HERE (with same procedure used for br identifiers)
-                orcid = self.find_crossref_orcid(orcid)
-                # END: VALIDATE ORCID HERE
-
-            elif dict_orcid and f_name:
-                for ori in dict_orcid:
-                    orc_n: List[str] = dict_orcid[ori].split(', ')
-                    orc_f = orc_n[0].lower()
-                    orc_g = orc_n[1] if len(orc_n) == 2 else None
-                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
-                        if g_name and orc_g:
-                            # If there are several authors with the same surname
-                            if len([person for person in agents_list if 'family' in person if person['family'] if
-                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
-                                        'family'].lower()]) > 1:
-                                # If there are several authors with the same surname and the same given names' initials
-                                if len([person for person in agents_list if 'given' in person if person['given'] if
-                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
-                                    homonyms_list = [person for person in agents_list if 'given' in person if
-                                                     person['given'] if person['given'].lower() == orc_g.lower()]
-                                    # If there are homonyms
-                                    if len(homonyms_list) > 1:
-                                        # If such homonyms have different roles from the current role
-                                        if [person for person in homonyms_list if person['role'] != cur_role]:
-                                            if orc_g.lower() == g_name.lower():
-                                                orcid = ori
-
-                                    else:
-                                        if orc_g.lower() == g_name.lower():
-                                            orcid = ori
-                                elif orc_g[0].lower() == g_name[0].lower():
-                                    orcid = ori
-
-                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
-                            elif any([person for person in agents_list if 'given' in person if person['given'] if
-                                      person['given'].lower() == f_name.lower()]):
-                                if orc_g.lower() == g_name.lower():
-                                    orcid = ori
-                            else:
-                                orcid = ori
-
-                        else:
-                            orcid = ori
-
-            if agent_string and orcid:
-                if not orcid.startswith("orcid:"):
-                    agent_string += ' [' + 'orcid:' + str(orcid) + ']'
-                else:
-                    agent_string += ' [' + str(orcid) + ']'
-            if agent_string:
-                if agent['role'] == 'author':
-                    authors_strings_list.append(agent_string)
-                elif agent['role'] == 'editor':
-                    editors_string_list.append(agent_string)
-        return authors_strings_list, editors_string_list
-
-
-    def find_crossref_orcid(self, identifier):
-        orcid = ""
-        if isinstance(identifier, str):
-            norm_orcid = self.orcid_m.normalise(identifier, include_prefix =True)
-            ## Check orcid presence in memory and storage before validating the id
-            norm_orcid_dict = {"schema":"orcid"}
-            norm_orcid_dict["identifier"] = norm_orcid
-            validity_value_orcid = self.validated_as(norm_orcid_dict)
-
-            if validity_value_orcid is True:
-                orcid = norm_orcid
-
-            elif validity_value_orcid is None:
-                norm_id_dict = {"id": norm_orcid, "schema": "orcid"}
-                if norm_orcid in self.to_validated_id_list(norm_id_dict):
-                    orcid = norm_orcid
-
-
-        return orcid
-
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
+# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import html
+import re
+import warnings
+from pathlib import Path
+from typing import Optional
+import os
+import os.path
+import json
+import csv
+
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager import DOIManager
+from oc_ds_converter.oc_idmanager import ORCIDManager
+from oc_ds_converter.oc_idmanager import ISSNManager
+
+from oc_ds_converter.lib.master_of_regex import *
+import fakeredis
+from oc_ds_converter.datasource.redis import RedisDataSource
+from oc_ds_converter.ra_processor import RaProcessor
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+from typing import Dict, List, Tuple
+from oc_ds_converter.lib.cleaner import Cleaner
+
+
+
+warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
+
+class CrossrefProcessing(RaProcessor):
+
+    def __init__(self, orcid_index:str=None, doi_csv:str=None, publishers_filepath:str=None, testing: bool = True, storage_manager: Optional[StorageManager] = None, citing=True):
+        super(CrossrefProcessing, self).__init__(orcid_index, doi_csv, publishers_filepath)
+        self.citing = citing
+
+        if storage_manager is None:
+            self.storage_manager = SqliteStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self.temporary_manager = InMemoryStorageManager('../memory.json')
+
+        self.doi_m = DOIManager(storage_manager=self.storage_manager)
+        self.orcid_m = ORCIDManager(storage_manager=self.storage_manager)
+        self.issn_m = ISSNManager()
+
+        self.venue_id_man_dict = {"issn": self.issn_m}
+        # Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
+        # main storage_manager  only once the full file is processed. Checks must be done both on tmp and in
+        # storage_manager, so that in case the process breaks while processing a file which does not complete (so
+        # without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
+        # a storage_manager db would be considered to have been processed and thus would be ignored by the process
+        # and lost.
+
+        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
+        self.tmp_orcid_m = ORCIDManager(storage_manager=self.temporary_manager)
+
+
+        self.venue_tmp_id_man_dict = {"issn": self.issn_m}
+
+        if testing:
+            self.BR_redis = fakeredis.FakeStrictRedis()
+            self.RA_redis= fakeredis.FakeStrictRedis()
+
+
+        else:
+            self.BR_redis = RedisDataSource("DB-META-BR")
+            self.RA_redis = RedisDataSource("DB-META-RA")
+
+
+        self._redis_values_br = []
+        self._redis_values_ra = []
+
+
+    def update_redis_values(self, br, ra):
+        self._redis_values_br = br
+        self._redis_values_ra = ra
+
+    def to_validated_id_list(self, norm_id_dict):
+        """this method takes in input a dictionary representing a normalized id, i.e.: {id:"id:000", "schema":"id"} and returns a list containing the validated id if it is valid, and an empty list otheriwse.
+        A first validation try is made by checking its presence in META db. If the id is not in META db yet,
+        a second attempt is made by using the specific id-schema API"""
+        #if self.BR_redis.get(norm_id):
+        valid_id_list = []
+        norm_id = norm_id_dict.get("id")
+        schema = norm_id_dict.get("schema")
+        if schema == "doi":
+            if norm_id in self._redis_values_br:
+                self.tmp_doi_m.storage_manager.set_value(norm_id, True) #In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                # preso in considerazione negli step successivi
+                valid_id_list.append(norm_id)
+            # if the id is not in redis db, validate it before appending
+            elif self.tmp_doi_m.is_valid(norm_id):#In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                # preso in considerazione negli step successivi
+                valid_id_list.append(norm_id)
+        elif schema == "orcid":
+            if norm_id in self._redis_values_ra:
+                self.tmp_orcid_m.storage_manager.set_value(norm_id, True) #In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                # preso in considerazione negli step successivi
+                valid_id_list.append(norm_id)
+            # if the id is not in redis db, validate it before appending
+            elif self.tmp_orcid_m.is_valid(norm_id):#In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                # preso in considerazione negli step successivi
+                valid_id_list.append(norm_id)
+
+        else:
+            print("Schema not accepted:", norm_id_dict.get("schema"), "in ", norm_id_dict, ". Use 'orcid' or 'doi'.")
+
+
+        return valid_id_list
+
+    def memory_to_storage(self):
+        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
+        if kv_in_memory:
+            self.storage_manager.set_multi_value(kv_in_memory)
+            self.temporary_manager.delete_storage()
+
+
+    def validated_as(self, id_dict):
+        # Check if the validity was already retrieved and thus
+        # a) if it is now saved either in the in-memory database, which only concerns data validated
+        # during the current file processing;
+        # b) or if it is now saved in the storage_manager database, which only concerns data validated
+        # during the previous files processing.
+        # In memory db is checked first because the dimension is smaller and the check is faster and
+        # Because we assume that it is more likely to find the same ids in close positions, e.g.: same
+        # citing id in several citations with different cited ids.
+
+        schema = id_dict["schema"].strip().lower()
+        id = id_dict["identifier"]
+
+        if schema == "orcid":
+            tmp_id_m = self.tmp_orcid_m
+            validity_value = tmp_id_m.validated_as_id(id)
+
+            if validity_value is None:
+                id_m = self.orcid_m
+                validity_value = id_m.validated_as_id(id)
+            return validity_value
+
+        elif schema == "doi":
+            validity_value = self.tmp_doi_m.validated_as_id(id)
+            if validity_value is None:
+                validity_value = self.doi_m.validated_as_id(id)
+            return validity_value
+        else:
+            print("invalid schema in ", id_dict, ". schema should be either doi or orcid.")
+            return None
+
+
+    def get_id_manager(self, schema_or_id, id_man_dict):
+        """Given as input the string of a schema (e.g.:'pmid') and a dictionary mapping strings of
+        the schemas to their id managers, the method returns the correct id manager. Note that each
+        instance of the Preprocessing class needs its own instances of the id managers, in order to
+        avoid conflicts while validating data"""
+        if ":" in schema_or_id:
+            split_id_prefix = schema_or_id.split(":")
+            schema = split_id_prefix[0]
+        else:
+            schema = schema_or_id
+        id_man = id_man_dict.get(schema)
+        return id_man
+
+
+    def dict_to_cache(self, dict_to_be_saved, path):
+        path = Path(path)
+        parent_dir_path = path.parent.absolute()
+        if not os.path.exists(parent_dir_path):
+            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
+        with open(path, "w", encoding="utf-8") as fd:
+            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
+
+    def csv_creator(self, item:dict) -> dict:
+        row = dict()
+        if not 'DOI' in item:
+            return row
+        doi_manager = DOIManager(use_api_service=False)
+        if isinstance(item['DOI'], list):
+            doi = doi_manager.normalise(str(item['DOI'][0]), include_prefix=False)
+        else:
+            doi = doi_manager.normalise(str(item['DOI']), include_prefix=False)
+        if (doi and self.doi_set and doi in self.doi_set) or (doi and not self.doi_set):
+            # create empty row
+            keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
+                    'publisher', 'editor']
+            for k in keys:
+                row[k] = ''
+
+            if 'type' in item:
+                if item['type']:
+                    row['type'] = item['type'].replace('-', ' ')
+
+            # row['id']
+            ids_list = list()
+            ids_list.append(str('doi:' + doi))
+
+            if 'ISBN' in item:
+                if row['type'] in {'book', 'dissertation', 'edited book', 'monograph', 'reference book', 'report', 'standard'}:
+                    self.id_worker(item['ISBN'], ids_list, self.isbn_worker)
+
+            if 'ISSN' in item:
+                if row['type'] in {'book series', 'book set', 'journal', 'proceedings series', 'series', 'standard series'}:
+                    self.id_worker(item['ISSN'], ids_list, self.issn_worker)
+                elif row['type'] == 'report series':
+                    br_id = True
+                    if 'container-title' in item:
+                        if item['container-title']:
+                            br_id = False
+                    if br_id:
+                        self.id_worker(item['ISSN'], ids_list, self.issn_worker)
+            row['id'] = ' '.join(ids_list)
+
+            # row['title']
+            if 'title' in item:
+                if item['title']:
+                    if isinstance(item['title'], list):
+                        text_title = item['title'][0]
+                    else:
+                        text_title = item['title']
+                    soup = BeautifulSoup(text_title, 'html.parser')
+                    title_soup = soup.get_text().replace('\n', '')
+                    title = html.unescape(title_soup)
+                    row['title'] = title
+
+            agents_list = []
+            if 'author' in item:
+                for author in item['author']:
+                    author['role'] = 'author'
+                agents_list.extend(item['author'])
+            if 'editor' in item:
+                for editor in item['editor']:
+                    editor['role'] = 'editor'
+                agents_list.extend(item['editor'])
+            authors_strings_list, editors_string_list = self.get_agents_strings_list(doi, agents_list)
+
+            # row['author']
+            if 'author' in item:
+                row['author'] = '; '.join(authors_strings_list)
+
+            # row['pub_date']
+            if 'issued' in item:
+                if item['issued']['date-parts'][0][0]:
+                    row['pub_date'] = '-'.join([str(y) for y in item['issued']['date-parts'][0]])
+                else:
+                    row['pub_date'] = ''
+
+            # row['venue']
+            row['venue'] = self.get_venue_name(item, row)
+
+            if 'volume' in item:
+                row['volume'] = item['volume']
+            if 'issue' in item:
+                row['issue'] = item['issue']
+            if 'page' in item:
+                row['page'] = self.get_crossref_pages(item)
+
+            row['publisher'] = self.get_publisher_name(doi, item)                        
+
+            if 'editor' in item:
+                row['editor'] = '; '.join(editors_string_list)
+        return self.normalise_unicode(row)
+        
+    def get_crossref_pages(self, item:dict) -> str:
+        '''
+        This function returns the pages interval. 
+
+        :params item: the item's dictionary
+        :type item: dict
+        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
+        '''
+        pages_list = re.split(pages_separator, item['page'])
+        return self.get_pages(pages_list)
+    
+    def get_publisher_name(self, doi:str, item:dict) -> str:
+        '''
+        This function aims to return a publisher's name and id. If a mapping was provided, 
+        it is used to find the publisher's standardized name from its id or DOI prefix. 
+
+        :params doi: the item's DOI
+        :type doi: str
+        :params item: the item's dictionary
+        :type item: dict
+        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output is only the name. Finally, if there is no publisher, the output is an empty string.
+        '''
+        data = {
+            'publisher': '',
+            'member': None,
+            'prefix': doi.split('/')[0]
+        }
+        for field in {'publisher', 'member', 'prefix'}:
+            if field in item:
+                if item[field]:
+                    data[field] = item[field]
+        publisher = data['publisher']
+        member = data['member']
+        prefix = data['prefix']
+        relevant_member = False
+
+        if self.publishers_mapping and member:
+            if member in self.publishers_mapping:
+                relevant_member = True
+        if self.publishers_mapping:
+            if relevant_member:
+                name = self.publishers_mapping[member]['name']
+                name_and_id = f'{name} [crossref:{member}]'
+            else:
+                member_dict = next(({member:data} for member, data in self.publishers_mapping.items() if prefix in data['prefixes']), None)
+                if member_dict:
+                    member = list(member_dict.keys())[0]
+                    name_and_id = f"{member_dict[member]['name']} [crossref:{member}]"
+                else:
+                    name_and_id = publisher
+        else:
+            name_and_id = f'{publisher} [crossref:{member}]' if member else publisher
+        return name_and_id
+
+
+    def get_venue_name(self, item:dict, row:dict) -> str:
+        '''
+        This method deals with generating the venue's name, followed by id in square brackets, separated by spaces. 
+        HTML tags are deleted and HTML entities escaped. In addition, any ISBN and ISSN are validated. 
+        Finally, the square brackets in the venue name are replaced by round brackets to avoid conflicts with the ids enclosures.
+
+        :params item: the item's dictionary
+        :type item: dict
+        :params row: a CSV row
+        :type row: dict
+        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'Nutrition & Food Science [issn:0034-6659]'. If the id does not exist, the output is only the name. Finally, if there is no venue, the output is an empty string.
+        '''
+        name_and_id = ''
+        if 'container-title' in item:
+            if item['container-title']:
+                if isinstance(item['container-title'], list):
+                    ventit = str(item['container-title'][0]).replace('\n', '')
+                else:
+                    ventit = str(item['container-title']).replace('\n', '')
+                ven_soup = BeautifulSoup(ventit, 'html.parser')
+                ventit = html.unescape(ven_soup.get_text())
+                ambiguous_brackets = re.search(ids_inside_square_brackets, ventit)
+                if ambiguous_brackets:
+                    match = ambiguous_brackets.group(1)
+                    open_bracket = ventit.find(match) - 1
+                    close_bracket = ventit.find(match) + len(match)
+                    ventit = ventit[:open_bracket] + '(' + ventit[open_bracket + 1:]
+                    ventit = ventit[:close_bracket] + ')' + ventit[close_bracket + 1:]
+                venids_list = list()
+                if 'ISBN' in item:
+                    if row['type'] in {'book chapter', 'book part', 'book section', 'book track', 'reference entry'}:
+                        self.id_worker(item['ISBN'], venids_list, self.isbn_worker)
+
+                if 'ISSN' in item:
+                    if row['type'] in {'book', 'data file', 'dataset', 'edited book', 'journal article', 'journal volume', 'journal issue', 'monograph', 'proceedings', 'peer review', 'reference book', 'reference entry', 'report'}:
+                        self.id_worker(item['ISSN'], venids_list, self.issn_worker)
+                    elif row['type'] == 'report series':
+                        if 'container-title' in item:
+                            if item['container-title']:
+                                self.id_worker(item['ISSN'], venids_list, self.issn_worker)
+                if venids_list:
+                    name_and_id = ventit + ' [' + ' '.join(venids_list) + ']'
+                else:
+                    name_and_id = ventit
+        return name_and_id
+
+    # UPDATED FOR CROSSREF √
+    def extract_all_ids(self, entity_dict, is_first_iteration: bool):
+        all_br = set()
+        all_ra = set()
+
+        if is_first_iteration:
+            # VALIDATE RESPONSIBLE AGENTS IDS FOR THE CITING ENTITY (THE CITING ENTITY DOI IS VALID BY
+            # DEFAULT SINCE IT WAS ASSIGNED BY CROSSREF, WHICH IS ALSO ITS DOI REGISTRATION AGENCY.
+
+            # EXTRA: THE CITING DOI IS VALID BY DEFAULT
+            # d1_br = entity_dict.get("DOI")
+            # if d1_br:
+            #  norm_id = self.doi_m.normalise(d1_br, include_prefix=True)
+            #  if norm_id:
+            #     all_br.add(norm_id)
+
+            if entity_dict.get("author"):
+                for author in entity_dict["author"]:
+                        if "ORCID" in author:
+                            orcid = self.orcid_m.normalise(
+                                author["ORCID"]
+                            )
+                            if orcid:
+                                all_ra.add(orcid)
+
+            if entity_dict.get("editor"):
+                for author in entity_dict["editor"]:
+                        if "ORCID" in author:
+                            orcid = self.orcid_m.normalise(
+                                author["ORCID"]
+                            )
+                            if orcid:
+                                all_ra.add(orcid)
+
+        # RETRIEVE CITED IDS OF A CITING ENTITY
+        else:
+            citations = [x for x in entity_dict["reference"] if x.get("DOI")]
+            for cit in citations:
+                norm_id = self.doi_m.normalise(cit["DOI"], include_prefix=True)
+                if norm_id:
+                    all_br.add(norm_id)
+
+        all_br = list(all_br)
+        all_ra = list(all_ra)
+        return all_br, all_ra
+
+
+    def get_reids_validity_list(self, id_list, redis_db):
+        if redis_db == "ra":
+            valid_ra_ids = []
+            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
+            validity_list_ra = self.RA_redis.mget(id_list)
+            for i, e in enumerate(id_list):
+                if validity_list_ra[i]:
+                    valid_ra_ids.append(e)
+            return valid_ra_ids
+
+        elif redis_db == "br":
+            valid_br_ids = []
+            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
+            validity_list_br = self.BR_redis.mget(id_list)
+            for i, e in enumerate(id_list):
+                if validity_list_br[i]:
+                    valid_br_ids.append(e)
+            return valid_br_ids
+        else:
+            raise ValueError("redis_db must be either 'ra' for responsible agents ids "
+                             "or 'br' for bibliographic resources ids")
+
+    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
+        authors_strings_list = list()
+        editors_string_list = list()
+        dict_orcid = None
+        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list):
+            dict_orcid = self.orcid_finder(doi)
+        agents_list = [
+            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None
+            else v for k, v in agent_dict.items()} for agent_dict in agents_list]
+
+        for agent in agents_list:
+            cur_role = agent['role']
+            f_name = None
+            g_name = None
+            agent_string = None
+            if agent.get('family') and agent.get('given'):
+                f_name = agent['family']
+                g_name = agent['given']
+                agent_string = f_name + ', ' + g_name
+            elif agent.get('name'):
+                agent_string = agent['name']
+                f_name = agent_string.split(",")[0].strip() if "," in agent_string else None
+                g_name = agent_string.split(",")[-1].strip() if "," in agent_string else None
+
+                if f_name and g_name:
+                    agent_string = f_name + ', ' + g_name
+            if agent_string is None:
+                if agent.get('family') and not agent.get('given'):
+                    if g_name:
+                        agent_string = agent['family'] + ', ' + g_name
+                    else:
+                        agent_string = agent['family'] + ', '
+                elif agent.get('given') and not agent.get('family'):
+                    if f_name:
+                        agent_string = f_name + ', ' + agent['given']
+                    else:
+                        agent_string = ', ' + agent['given']
+            orcid = None
+            if 'orcid' in agent:
+                if isinstance(agent['orcid'], list):
+                    orcid = str(agent['orcid'][0])
+                else:
+                    orcid = str(agent['orcid'])
+            elif 'ORCID' in agent:
+                if isinstance(agent['ORCID'], list):
+                    orcid = str(agent['ORCID'][0])
+                else:
+                    orcid = str(agent['ORCID'])
+            if orcid:
+
+                # VALIDATE ORCID HERE (with same procedure used for br identifiers)
+                orcid = self.find_crossref_orcid(orcid)
+                # END: VALIDATE ORCID HERE
+
+            elif dict_orcid and f_name:
+                for ori in dict_orcid:
+                    orc_n: List[str] = dict_orcid[ori].split(', ')
+                    orc_f = orc_n[0].lower()
+                    orc_g = orc_n[1] if len(orc_n) == 2 else None
+                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
+                        if g_name and orc_g:
+                            # If there are several authors with the same surname
+                            if len([person for person in agents_list if 'family' in person if person['family'] if
+                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
+                                        'family'].lower()]) > 1:
+                                # If there are several authors with the same surname and the same given names' initials
+                                if len([person for person in agents_list if 'given' in person if person['given'] if
+                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
+                                    homonyms_list = [person for person in agents_list if 'given' in person if
+                                                     person['given'] if person['given'].lower() == orc_g.lower()]
+                                    # If there are homonyms
+                                    if len(homonyms_list) > 1:
+                                        # If such homonyms have different roles from the current role
+                                        if [person for person in homonyms_list if person['role'] != cur_role]:
+                                            if orc_g.lower() == g_name.lower():
+                                                orcid = ori
+
+                                    else:
+                                        if orc_g.lower() == g_name.lower():
+                                            orcid = ori
+                                elif orc_g[0].lower() == g_name[0].lower():
+                                    orcid = ori
+
+                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
+                            elif any([person for person in agents_list if 'given' in person if person['given'] if
+                                      person['given'].lower() == f_name.lower()]):
+                                if orc_g.lower() == g_name.lower():
+                                    orcid = ori
+                            else:
+                                orcid = ori
+
+                        else:
+                            orcid = ori
+
+            if agent_string and orcid:
+                if not orcid.startswith("orcid:"):
+                    agent_string += ' [' + 'orcid:' + str(orcid) + ']'
+                else:
+                    agent_string += ' [' + str(orcid) + ']'
+            if agent_string:
+                if agent['role'] == 'author':
+                    authors_strings_list.append(agent_string)
+                elif agent['role'] == 'editor':
+                    editors_string_list.append(agent_string)
+        return authors_strings_list, editors_string_list
+
+
+    def find_crossref_orcid(self, identifier):
+        orcid = ""
+        if isinstance(identifier, str):
+            norm_orcid = self.orcid_m.normalise(identifier, include_prefix =True)
+            ## Check orcid presence in memory and storage before validating the id
+            norm_orcid_dict = {"schema":"orcid"}
+            norm_orcid_dict["identifier"] = norm_orcid
+            validity_value_orcid = self.validated_as(norm_orcid_dict)
+
+            if validity_value_orcid is True:
+                orcid = norm_orcid
+
+            elif validity_value_orcid is None:
+                norm_id_dict = {"id": norm_orcid, "schema": "orcid"}
+                if norm_orcid in self.to_validated_id_list(norm_id_dict):
+                    orcid = norm_orcid
+
+
+        return orcid
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/crossref/extract_crossref_publishers.py` & `oc_ds_converter-1.0.1/oc_ds_converter/crossref/extract_crossref_publishers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# -*- coding: utf-8 -*-
-# Copyright (c) 2021, Silvio Peroni <essepuntato@gmail.com>
-# Copyright (c) 2022, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import html
-from csv import QUOTE_NONNUMERIC, DictReader, DictWriter
-from json import loads
-from os.path import exists
-from time import sleep
-
-from requests import get
-
-MAX_TRY = 5
-SLEEPING_TIME = 5
-csv_headers = (
-    "id", "name", "prefix"
-)
-headers = {
-    "User-Agent": 
-    "OpenCitations "
-    "(http://opencitations.net; mailto:contact@opencitations.net)"
-}
-
-
-def get_via_requests(get_url):
-    tentative = 0
-    print("")
-
-    while tentative < MAX_TRY:
-        tentative += 1
-
-        try:
-            print("Getting data from", get_url, "- tentative:", tentative)
-            r = get(get_url, headers=headers, timeout=10)
-            if r.status_code == 200:
-                print("\tdata downloaded")
-                r.encoding = "utf-8"
-
-                return loads(r.text)
-            elif r.status_code == 404:
-                return None
-            else:
-                print("\tdata not downloaded, trying again in ", SLEEPING_TIME, "seconds - status:", r.status_code)
-                sleep(SLEEPING_TIME)
-        except Exception as e:
-            print("\tdata not downloaded, trying again in ", SLEEPING_TIME, "seconds - exception:", e.message)
-            sleep(SLEEPING_TIME)
-
-
-def get_publishers(offset):
-    get_url = "https://api.crossref.org/members?rows=1000&offset=" + str(offset)
-    req = get_via_requests(get_url)
-    
-    if req is not None:
-        r_json = req.get("message")
-        if r_json is not None:
-            offset += 1000
-            print("\tnext offset is", offset)
-            total_results = int(r_json.get("total-results"))
-            items = r_json.get("items")
-
-            return items, offset, total_results
-                
-
-def process(out_path):
-    pub_ids = set()
-
-    if exists(out_path):
-        with open(out_path, encoding="utf8") as f:
-            csv_reader = DictReader(f, csv_headers)
-            for row in csv_reader:
-                pub_ids.add(row["id"])
-
-    # cursor = "*"
-    offset = 0
-    tot = 10000000000
-    pub_count = 0
-    while offset < tot:
-        result, offset, tot = get_publishers(offset)
-
-        if result is not None:
-            for publisher in result:
-                pub_count += 1
-                cur_id = str(publisher["id"])
-                if cur_id not in pub_ids:
-                    pub_ids.add(cur_id)
-                    cur_name = html.unescape(publisher["primary-name"])
-                    prefixes = set()
-                    for prefix in publisher["prefix"]:
-                        prefix_value = prefix["value"]
-                        if prefix_value not in prefixes:
-                            prefixes.add(prefix_value)
-                            store_csv_on_file(out_path, csv_headers, {
-                                "id": cur_id, "name": cur_name, "prefix": prefix_value})
-    
-    if pub_count == tot:
-        print("\n\nAll publishers correctly downloaded")
-    else:
-        print("\n\nOnly %s of the total %s publishers "
-              "have been downloaded" % (pub_count, tot))
-
-def store_csv_on_file(f_path, header, json_obj):
-    f_exists = exists(f_path)
-    with open(f_path, "a", encoding="utf8", newline='') as f:
-        dw = DictWriter(f=f, fieldnames=header, delimiter=',', quotechar='"', quoting=QUOTE_NONNUMERIC)
-        if not f_exists:
-            dw.writeheader()
-        dw.writerow(json_obj)
+# -*- coding: utf-8 -*-
+# Copyright (c) 2021, Silvio Peroni <essepuntato@gmail.com>
+# Copyright (c) 2022, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import html
+from csv import QUOTE_NONNUMERIC, DictReader, DictWriter
+from json import loads
+from os.path import exists
+from time import sleep
+
+from requests import get
+
+MAX_TRY = 5
+SLEEPING_TIME = 5
+csv_headers = (
+    "id", "name", "prefix"
+)
+headers = {
+    "User-Agent": 
+    "OpenCitations "
+    "(http://opencitations.net; mailto:contact@opencitations.net)"
+}
+
+
+def get_via_requests(get_url):
+    tentative = 0
+    print("")
+
+    while tentative < MAX_TRY:
+        tentative += 1
+
+        try:
+            print("Getting data from", get_url, "- tentative:", tentative)
+            r = get(get_url, headers=headers, timeout=10)
+            if r.status_code == 200:
+                print("\tdata downloaded")
+                r.encoding = "utf-8"
+
+                return loads(r.text)
+            elif r.status_code == 404:
+                return None
+            else:
+                print("\tdata not downloaded, trying again in ", SLEEPING_TIME, "seconds - status:", r.status_code)
+                sleep(SLEEPING_TIME)
+        except Exception as e:
+            print("\tdata not downloaded, trying again in ", SLEEPING_TIME, "seconds - exception:", e.message)
+            sleep(SLEEPING_TIME)
+
+
+def get_publishers(offset):
+    get_url = "https://api.crossref.org/members?rows=1000&offset=" + str(offset)
+    req = get_via_requests(get_url)
+    
+    if req is not None:
+        r_json = req.get("message")
+        if r_json is not None:
+            offset += 1000
+            print("\tnext offset is", offset)
+            total_results = int(r_json.get("total-results"))
+            items = r_json.get("items")
+
+            return items, offset, total_results
+                
+
+def process(out_path):
+    pub_ids = set()
+
+    if exists(out_path):
+        with open(out_path, encoding="utf8") as f:
+            csv_reader = DictReader(f, csv_headers)
+            for row in csv_reader:
+                pub_ids.add(row["id"])
+
+    # cursor = "*"
+    offset = 0
+    tot = 10000000000
+    pub_count = 0
+    while offset < tot:
+        result, offset, tot = get_publishers(offset)
+
+        if result is not None:
+            for publisher in result:
+                pub_count += 1
+                cur_id = str(publisher["id"])
+                if cur_id not in pub_ids:
+                    pub_ids.add(cur_id)
+                    cur_name = html.unescape(publisher["primary-name"])
+                    prefixes = set()
+                    for prefix in publisher["prefix"]:
+                        prefix_value = prefix["value"]
+                        if prefix_value not in prefixes:
+                            prefixes.add(prefix_value)
+                            store_csv_on_file(out_path, csv_headers, {
+                                "id": cur_id, "name": cur_name, "prefix": prefix_value})
+    
+    if pub_count == tot:
+        print("\n\nAll publishers correctly downloaded")
+    else:
+        print("\n\nOnly %s of the total %s publishers "
+              "have been downloaded" % (pub_count, tot))
+
+def store_csv_on_file(f_path, header, json_obj):
+    f_exists = exists(f_path)
+    with open(f_path, "a", encoding="utf8", newline='') as f:
+        dw = DictWriter(f=f, fieldnames=header, delimiter=',', quotechar='"', quoting=QUOTE_NONNUMERIC)
+        if not f_exists:
+            dw.writeheader()
+        dw.writerow(json_obj)
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/crossref/get_not_crossref_ref.py` & `oc_ds_converter-1.0.1/oc_ds_converter/crossref/get_not_crossref_ref.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import os
-from argparse import ArgumentParser
-from functools import partial
-from multiprocessing import cpu_count
-from sys import platform
-from typing import List, Tuple
-
-from pebble import ProcessFuture, ProcessPool
-from tqdm import tqdm
-
-from oc_ds_converter.lib.csvmanager import CSVManager
-from oc_ds_converter.lib.file_manager import (call_api, chunks, get_csv_data,
-                                              pathoo, write_csv)
-from oc_ds_converter.lib.jsonmanager import get_all_files, load_json
-from oc_ds_converter.metadata_manager import MetadataManager
-from oc_ds_converter.oc_idmanager import DOIManager
-
-
-def extract_dois_from_dump(crossref_json_dir:str, output_dir:str, max_workers:int) -> None:
-    all_files, targz_fd = get_all_files(crossref_json_dir, cache_filepath=None)
-    all_files = [file for file in all_files 
-        if not os.path.exists(
-            os.path.join(output_dir, 'crossref',
-                os.path.basename(file).replace('.json', '').replace('.gz', '') + '.csv'))
-        and not os.path.exists(
-            os.path.join(output_dir, 'reference',
-                os.path.basename(file).replace('.json', '').replace('.gz', '') + '.csv'))
-        ]
-    doi_manager = DOIManager(use_api_service=False)
-    print('[INFO] Extracting DOIs from the Crossref dump')
-    pbar = tqdm(total=len(all_files))
-    #if platform.startswith('linux') or platform == 'darwin':
-        #os.sched_setaffinity(0, set(range(0, max_workers)))
-    with ProcessPool(max_workers=max_workers) as executor:
-        for filename in all_files:
-            future:ProcessFuture = executor.schedule(
-                function=get_dois, 
-                args=(filename, targz_fd, doi_manager))
-            future.add_done_callback(partial(task_done, output_dir, filename, pbar))
-    pbar.close()
-
-def get_dois(filepath:str, targz_fd, doi_manager:DOIManager) -> Tuple[List[dict], List[dict]]:
-    source_data = load_json(filepath, targz_fd)
-    file_dois = list()
-    dois_in_references = list()
-    if source_data:
-        for item in source_data['items']:
-            citing = doi_manager.normalise(item.get('DOI'))
-            if citing is not None:
-                file_dois.append({'id': citing})
-                if 'reference' in item:
-                    for reference in item['reference']:
-                        cited = doi_manager.normalise(reference.get('DOI'))
-                        if cited is not None:
-                            dois_in_references.append({'id': cited})
-    return file_dois, dois_in_references
-
-def task_done(output_dir:str, filename:str, pbar:tqdm, task_output:ProcessFuture) -> None:
-    filename = os.path.basename(filename).replace('.json', '').replace('.gz', '') + '.csv'
-    crossref, ref_dois = task_output.result()
-    crossref_dir = os.path.join(output_dir, 'crossref')
-    ref_dir = os.path.join(output_dir, 'reference')
-    write_csv(path=os.path.join(crossref_dir, filename), datalist=crossref)
-    write_csv(path=os.path.join(ref_dir, filename), datalist=ref_dois)
-    pbar.update()
-
-def generate_set_of_crossref_dois(crossref_dois_dir:str) -> set:
-    print('[INFO] Storing Crossref DOIs in memory')
-    files = os.listdir(crossref_dois_dir)
-    pbar = tqdm(total=len(files))
-    crossref_dois = set()
-    for file in files:
-        crossref_dois.update(CSVManager.load_csv_column_as_set(os.path.join(crossref_dois_dir, file), 'id'))
-        pbar.update()
-    pbar.close()
-    return crossref_dois
-
-def get_ref_dois_not_in_crossref(crossref_dois:set, ref_dir:str) -> set:
-    print('[INFO] Getting the set of references DOIs not in Crossref')
-    files = os.listdir(ref_dir)
-    pbar = tqdm(total=len(files))
-    ref_not_in_crossref = set()
-    for i, file in enumerate(files):
-        ref_not_in_crossref.update(CSVManager.load_csv_column_as_set(os.path.join(ref_dir, file), 'id'))
-        if i % 1000 == 0:
-            ref_not_in_crossref = ref_not_in_crossref.difference(crossref_dois)
-        pbar.update()
-    pbar.close()
-    ref_not_in_crossref = ref_not_in_crossref.difference(crossref_dois)
-    return ref_not_in_crossref
-
-def store_dois_not_in_crossref(ref_not_in_crossref:set, output_dir:str) -> None:
-    output_dir = os.path.join(output_dir, 'dois_not_in_crossref')
-    counter = 1
-    threshold = 100000
-    for chunk in chunks(list(ref_not_in_crossref), threshold):
-        path = os.path.join(output_dir, f'{counter}-{counter+len(chunk)-1}.csv')
-        datalist = [{'id': doi} for doi in chunk]
-        write_csv(path, datalist)
-        counter += len(chunk)
-
-def extract_metadata(output_dir:str, orcid_doi_filepath:str):
-    dois_not_in_crossref_dir = os.path.join(output_dir, 'dois_not_in_crossref')
-    base_output_dir = os.path.join(dois_not_in_crossref_dir, 'metadata_extracted')
-    processed_dois = {
-        row['id'] for dirpath, _, filenames in os.walk(base_output_dir) 
-            for filename in filenames 
-                for row in get_csv_data(os.path.join(dirpath, filename))}
-    print(len(processed_dois))
-    for filename in os.listdir(dois_not_in_crossref_dir):
-        dois = CSVManager.load_csv_column_as_set(os.path.join(dois_not_in_crossref_dir, filename), 'id').difference(processed_dois)
-        for doi in dois:
-            doi_manager = DOIManager()
-            api_response = call_api(url=f'{doi_manager._api_unknown}{doi}', headers=doi_manager._headers)
-            metadata_manager = MetadataManager(metadata_provider = "unknown", api_response = api_response, orcid_doi_filepath = orcid_doi_filepath)
-            metadata: dict = metadata_manager.extract_metadata()
-            if not metadata.get('id'):
-                metadata['id'] = doi
-            registration_agency = metadata['ra']
-            metadata.pop('valid', None); metadata.pop('ra', None)
-            locals()[f'{registration_agency}_counter'] = 0
-            ra_output_dir = os.path.join(base_output_dir, registration_agency)
-            pathoo(ra_output_dir)
-            output_path = os.path.join(ra_output_dir, f"{locals()[f'{registration_agency}_counter']}.csv")
-            if os.path.exists(output_path):
-                if len(get_csv_data(output_path)) == 10000:
-                    locals()[f'{registration_agency}_counter'] += 1
-            output_path = os.path.join(ra_output_dir, f"{locals()[f'{registration_agency}_counter']}.csv")
-            write_csv(output_path, [metadata], method='a')
-
-if __name__ == '__main__': # pragma: no cover
-    arg_parser = ArgumentParser('meta_process.py', description='This script runs the OCMeta data processing workflow')
-    arg_parser.add_argument('-c', '--crossref_json_dir', dest='crossref_json_dir', required=True, help='Crossref json files directory')
-    arg_parser.add_argument('-o', '--output', dest='output_dir', required=True, help='Directory of the output CSV files to store Crossref and citations DOIS and lower memory requirements')
-    arg_parser.add_argument('-or', '--orcid', dest='orcid_doi_filepath', required=False, help='DOI-ORCID index filepath, to enrich data')
-    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=cpu_count(), type=int, help='Max workers')
-    arg_parser.add_argument('-w', '--wanted', dest='wanted_dois_filepath', required=False, default=None, help='A CSV filepath containing what DOI to process, not mandatory')
-    args = arg_parser.parse_args()
-    if not os.path.exists(os.path.join(args.output_dir, 'dois_not_in_crossref')):
-        extract_dois_from_dump(args.crossref_json_dir, args.output_dir, args.max_workers)
-        crossref_dois = generate_set_of_crossref_dois(os.path.join(args.output_dir, 'crossref'))
-        ref_not_in_crossref = get_ref_dois_not_in_crossref(crossref_dois, os.path.join(args.output_dir, 'reference'))
-        wanted_dois = CSVManager.load_csv_column_as_set(args.wanted_dois_filepath, 'id') if args.wanted_dois_filepath else None
-        if wanted_dois:
-            ref_not_in_crossref = ref_not_in_crossref.intersection(wanted_dois)
-        store_dois_not_in_crossref(ref_not_in_crossref, args.output_dir)
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import os
+from argparse import ArgumentParser
+from functools import partial
+from multiprocessing import cpu_count
+from sys import platform
+from typing import List, Tuple
+
+from pebble import ProcessFuture, ProcessPool
+from tqdm import tqdm
+
+from oc_ds_converter.lib.csvmanager import CSVManager
+from oc_ds_converter.lib.file_manager import (call_api, chunks, get_csv_data,
+                                              pathoo, write_csv)
+from oc_ds_converter.lib.jsonmanager import get_all_files, load_json
+from oc_ds_converter.metadata_manager import MetadataManager
+from oc_ds_converter.oc_idmanager import DOIManager
+
+
+def extract_dois_from_dump(crossref_json_dir:str, output_dir:str, max_workers:int) -> None:
+    all_files, targz_fd = get_all_files(crossref_json_dir, cache_filepath=None)
+    all_files = [file for file in all_files 
+        if not os.path.exists(
+            os.path.join(output_dir, 'crossref',
+                os.path.basename(file).replace('.json', '').replace('.gz', '') + '.csv'))
+        and not os.path.exists(
+            os.path.join(output_dir, 'reference',
+                os.path.basename(file).replace('.json', '').replace('.gz', '') + '.csv'))
+        ]
+    doi_manager = DOIManager(use_api_service=False)
+    print('[INFO] Extracting DOIs from the Crossref dump')
+    pbar = tqdm(total=len(all_files))
+    #if platform.startswith('linux') or platform == 'darwin':
+        #os.sched_setaffinity(0, set(range(0, max_workers)))
+    with ProcessPool(max_workers=max_workers) as executor:
+        for filename in all_files:
+            future:ProcessFuture = executor.schedule(
+                function=get_dois, 
+                args=(filename, targz_fd, doi_manager))
+            future.add_done_callback(partial(task_done, output_dir, filename, pbar))
+    pbar.close()
+
+def get_dois(filepath:str, targz_fd, doi_manager:DOIManager) -> Tuple[List[dict], List[dict]]:
+    source_data = load_json(filepath, targz_fd)
+    file_dois = list()
+    dois_in_references = list()
+    if source_data:
+        for item in source_data['items']:
+            citing = doi_manager.normalise(item.get('DOI'))
+            if citing is not None:
+                file_dois.append({'id': citing})
+                if 'reference' in item:
+                    for reference in item['reference']:
+                        cited = doi_manager.normalise(reference.get('DOI'))
+                        if cited is not None:
+                            dois_in_references.append({'id': cited})
+    return file_dois, dois_in_references
+
+def task_done(output_dir:str, filename:str, pbar:tqdm, task_output:ProcessFuture) -> None:
+    filename = os.path.basename(filename).replace('.json', '').replace('.gz', '') + '.csv'
+    crossref, ref_dois = task_output.result()
+    crossref_dir = os.path.join(output_dir, 'crossref')
+    ref_dir = os.path.join(output_dir, 'reference')
+    write_csv(path=os.path.join(crossref_dir, filename), datalist=crossref)
+    write_csv(path=os.path.join(ref_dir, filename), datalist=ref_dois)
+    pbar.update()
+
+def generate_set_of_crossref_dois(crossref_dois_dir:str) -> set:
+    print('[INFO] Storing Crossref DOIs in memory')
+    files = os.listdir(crossref_dois_dir)
+    pbar = tqdm(total=len(files))
+    crossref_dois = set()
+    for file in files:
+        crossref_dois.update(CSVManager.load_csv_column_as_set(os.path.join(crossref_dois_dir, file), 'id'))
+        pbar.update()
+    pbar.close()
+    return crossref_dois
+
+def get_ref_dois_not_in_crossref(crossref_dois:set, ref_dir:str) -> set:
+    print('[INFO] Getting the set of references DOIs not in Crossref')
+    files = os.listdir(ref_dir)
+    pbar = tqdm(total=len(files))
+    ref_not_in_crossref = set()
+    for i, file in enumerate(files):
+        ref_not_in_crossref.update(CSVManager.load_csv_column_as_set(os.path.join(ref_dir, file), 'id'))
+        if i % 1000 == 0:
+            ref_not_in_crossref = ref_not_in_crossref.difference(crossref_dois)
+        pbar.update()
+    pbar.close()
+    ref_not_in_crossref = ref_not_in_crossref.difference(crossref_dois)
+    return ref_not_in_crossref
+
+def store_dois_not_in_crossref(ref_not_in_crossref:set, output_dir:str) -> None:
+    output_dir = os.path.join(output_dir, 'dois_not_in_crossref')
+    counter = 1
+    threshold = 100000
+    for chunk in chunks(list(ref_not_in_crossref), threshold):
+        path = os.path.join(output_dir, f'{counter}-{counter+len(chunk)-1}.csv')
+        datalist = [{'id': doi} for doi in chunk]
+        write_csv(path, datalist)
+        counter += len(chunk)
+
+def extract_metadata(output_dir:str, orcid_doi_filepath:str):
+    dois_not_in_crossref_dir = os.path.join(output_dir, 'dois_not_in_crossref')
+    base_output_dir = os.path.join(dois_not_in_crossref_dir, 'metadata_extracted')
+    processed_dois = {
+        row['id'] for dirpath, _, filenames in os.walk(base_output_dir) 
+            for filename in filenames 
+                for row in get_csv_data(os.path.join(dirpath, filename))}
+    print(len(processed_dois))
+    for filename in os.listdir(dois_not_in_crossref_dir):
+        dois = CSVManager.load_csv_column_as_set(os.path.join(dois_not_in_crossref_dir, filename), 'id').difference(processed_dois)
+        for doi in dois:
+            doi_manager = DOIManager()
+            api_response = call_api(url=f'{doi_manager._api_unknown}{doi}', headers=doi_manager._headers)
+            metadata_manager = MetadataManager(metadata_provider = "unknown", api_response = api_response, orcid_doi_filepath = orcid_doi_filepath)
+            metadata: dict = metadata_manager.extract_metadata()
+            if not metadata.get('id'):
+                metadata['id'] = doi
+            registration_agency = metadata['ra']
+            metadata.pop('valid', None); metadata.pop('ra', None)
+            locals()[f'{registration_agency}_counter'] = 0
+            ra_output_dir = os.path.join(base_output_dir, registration_agency)
+            pathoo(ra_output_dir)
+            output_path = os.path.join(ra_output_dir, f"{locals()[f'{registration_agency}_counter']}.csv")
+            if os.path.exists(output_path):
+                if len(get_csv_data(output_path)) == 10000:
+                    locals()[f'{registration_agency}_counter'] += 1
+            output_path = os.path.join(ra_output_dir, f"{locals()[f'{registration_agency}_counter']}.csv")
+            write_csv(output_path, [metadata], method='a')
+
+if __name__ == '__main__': # pragma: no cover
+    arg_parser = ArgumentParser('meta_process.py', description='This script runs the OCMeta data processing workflow')
+    arg_parser.add_argument('-c', '--crossref_json_dir', dest='crossref_json_dir', required=True, help='Crossref json files directory')
+    arg_parser.add_argument('-o', '--output', dest='output_dir', required=True, help='Directory of the output CSV files to store Crossref and citations DOIS and lower memory requirements')
+    arg_parser.add_argument('-or', '--orcid', dest='orcid_doi_filepath', required=False, help='DOI-ORCID index filepath, to enrich data')
+    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=cpu_count(), type=int, help='Max workers')
+    arg_parser.add_argument('-w', '--wanted', dest='wanted_dois_filepath', required=False, default=None, help='A CSV filepath containing what DOI to process, not mandatory')
+    args = arg_parser.parse_args()
+    if not os.path.exists(os.path.join(args.output_dir, 'dois_not_in_crossref')):
+        extract_dois_from_dump(args.crossref_json_dir, args.output_dir, args.max_workers)
+        crossref_dois = generate_set_of_crossref_dois(os.path.join(args.output_dir, 'crossref'))
+        ref_not_in_crossref = get_ref_dois_not_in_crossref(crossref_dois, os.path.join(args.output_dir, 'reference'))
+        wanted_dois = CSVManager.load_csv_column_as_set(args.wanted_dois_filepath, 'id') if args.wanted_dois_filepath else None
+        if wanted_dois:
+            ref_not_in_crossref = ref_not_in_crossref.intersection(wanted_dois)
+        store_dois_not_in_crossref(ref_not_in_crossref, args.output_dir)
     extract_metadata(args.output_dir, args.orcid_doi_filepath)
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/datacite/datacite_processing_new.py` & `oc_ds_converter-1.0.1/oc_ds_converter/openaire/openaire_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,771 +1,699 @@
-import html
-import re
-import warnings
-import os
-import fakeredis
-import csv
-import json
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager.doi import DOIManager
-from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
-from oc_ds_converter.lib.master_of_regex import *
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.isbn import ISBNManager
-from oc_ds_converter.datasource.redis import RedisDataSource
-from oc_ds_converter.preprocessing.datacite import DatacitePreProcessing
-from oc_ds_converter.ra_processor import RaProcessor
-from typing import Dict, List, Tuple, Optional, Type, Callable
-from pathlib import Path
-
-warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
-
-
-class DataciteProcessing(RaProcessor):
-    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_dc: str = None, testing: bool = True, storage_manager: Optional[StorageManager] = None, citing=True):
-        super(DataciteProcessing, self).__init__(orcid_index, doi_csv)
-        # self.preprocessor = DatacitePreProcessing(inp_dir, out_dir, interval, filter)
-        if storage_manager is None:
-            self.storage_manager = SqliteStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self.temporary_manager = InMemoryStorageManager('../memory.json')
-
-        self._needed_info = ["relationType", "relatedIdentifierType", "relatedIdentifier"]
-        self._filter = ["references", "isreferencedby", "cites", "iscitedby"]
-
-        self.RIS_types_map = {'abst': 'abstract',
-  'news': 'newspaper article',
-  'slide': 'presentation',
-  'book': 'book',
-  'data': 'dataset',
-  'thes': 'dissertation',
-  'jour': 'journal article',
-  'mgzn': 'journal article',
-  'gen': 'other',
-  'advs': 'other',
-  'video': 'other',
-  'unpb': 'other',
-  'ctlg': 'other',
-  'art': 'other',
-  'case': 'other',
-  'icomm': 'other',
-  'inpr': 'other',
-  'map': 'other',
-  'mpct': 'other',
-  'music': 'other',
-  'pamp': 'other',
-  'pat': 'other',
-  'pcomm': 'other',
-  'catalog': 'other',
-  'elec': 'other',
-  'hear': 'other',
-  'stat': 'other',
-  'bill': 'other',
-  'unbill': 'other',
-  'cpaper': 'proceedings article',
-  'rprt': 'report',
-  'chap': 'book chapter',
-  'ser': 'book series',
-  'jfull': 'journal',
-  'conf': 'proceedings',
-  'comp': 'computer program',
-  'sound': 'audio document'}
-        self.BIBTEX_types_map = {'book': 'book',
-  'mastersthesis': 'dissertation',
-  'phdthesis': 'dissertation',
-  'article': 'journal article',
-  'misc': 'other',
-  'unpublished': 'other',
-  'manual': 'other',
-  'booklet': 'other',
-  'inproceedings': 'proceedings article',
-  'techreport': 'report',
-  'inbook': 'book chapter',
-  'incollection': 'book part',
-  'proceedings': 'proceedings'}
-        self.CITEPROC_types_map = {'book': 'book',
-  'dataset': 'dataset',
-  'thesis': 'dissertation',
-  'article-journal': 'journal article',
-  'article': 'other',
-  'graphic': 'other',
-  'post-weblog': 'web content',
-  'paper-conference': 'proceedings article',
-  'report': 'report',
-  'chapter': 'book chapter',
-  'song': 'audio document'}
-        self.SCHEMAORG_types_map = {'book': 'book',
-  'dataset': 'dataset',
-  'thesis': 'dissertation',
-  'scholarlyarticle': 'journal article',
-  'article': 'journal article',
-  'creativework': 'other',
-  'event': 'other',
-  'service': 'other',
-  'mediaobject': 'other',
-  'review': 'other',
-  'collection': 'other',
-  'imageobject': 'other',
-  'blogposting': 'web content',
-  'report': 'report',
-  'chapter': 'book chapter',
-  'periodical': 'journal',
-  'publicationissue': 'journal issue',
-  'publicationvolume': 'journal volume',
-  'softwaresourcecode': 'computer program',
-  'audioobject': 'audio document'}
-        self.RESOURCETYPEGENERAL_types_map = {'book': 'book',
-  'dataset': 'dataset',
-  'dissertation': 'dissertation',
-  'journalarticle': 'journal article',
-  'text': 'other',
-  'other': 'other',
-  'datapaper': 'other',
-  'audiovisual': 'other',
-  'interactiveresource': 'other',
-  'physicalobject': 'other',
-  'event': 'other',
-  'service': 'other',
-  'collection': 'other',
-  'image': 'other',
-  'model': 'other',
-  'peerreview': 'peer review',
-  'conferencepaper': 'proceedings article',
-  'report': 'report',
-  'bookchapter': 'book chapter',
-  'journal': 'journal',
-  'conferenceproceeding': 'proceedings',
-  'standard': 'standard',
-  'outputmanagementplan': 'data management plan',
-  'preprint': 'preprint',
-  'software': 'computer program',
-  'sound': 'audio document',
-  'workflow': 'workflow'}
-
-    # def input_preprocessing(self):
-    # self.preprocessor.split_input()
-
-        self.doi_m = DOIManager(storage_manager=self.storage_manager)
-        self.orcid_m = ORCIDManager(storage_manager=self.storage_manager)
-        self.issn_m = ISSNManager()
-        self.isbn_m = ISBNManager()
-        self.venue_id_man_dict = {"issn": self.issn_m, "isbn": self.isbn_m}
-        # Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
-        # main storage_manager  only once the full file is processed. Checks must be done both on tmp and in
-        # storage_manager, so that in case the process breaks while processing a file which does not complete (so
-        # without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
-        # a storage_manager db would be considered to have been processed and thus would be ignored by the process
-        # and lost.
-
-        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
-        self.tmp_orcid_m = ORCIDManager(storage_manager=self.temporary_manager)
-        self.venue_tmp_id_man_dict = {"issn": self.issn_m, "isbn": self.isbn_m}
-
-        if testing:
-            self.BR_redis = fakeredis.FakeStrictRedis()
-            self.RA_redis = fakeredis.FakeStrictRedis()
-
-        else:
-            self.BR_redis = RedisDataSource("DB-META-BR")
-            self.RA_redis = RedisDataSource("DB-META-RA")
-
-        self._redis_values_ra = []
-        self._redis_values_br = []
-
-        if not publishers_filepath_dc:
-            self.publishers_filepath = None
-        else:
-            self.publishers_filepath = publishers_filepath_dc
-
-            if os.path.exists(self.publishers_filepath):
-                pfp = dict()
-                csv_headers = ("id", "name", "prefix")
-                if self.publishers_filepath.endswith(".csv"):
-                    with open(self.publishers_filepath, encoding="utf8") as f:
-                        csv_reader = csv.DictReader(f, csv_headers)
-                        for row in csv_reader:
-                            pfp[row["prefix"]] = {"name": row["name"], "crossref_member": row["id"]}
-                    self.publishers_filepath = self.publishers_filepath.replace(".csv", ".json")
-                elif self.publishers_filepath.endswith(".json"):
-                    with open(self.publishers_filepath, encoding="utf8") as f:
-                        pfp = json.load(f)
-                self.publishers_mapping = pfp
-    #added
-    def update_redis_values(self, br, ra):
-        self._redis_values_br = br
-        self._redis_values_ra = ra
-
-    #added
-    def validated_as(self, id_dict):
-        # Check if the validity was already retrieved and thus
-        # a) if it is now saved either in the in-memory database, which only concerns data validated
-        # during the current file processing;
-        # b) or if it is now saved in the storage_manager database, which only concerns data validated
-        # during the previous files processing.
-        # In memory db is checked first because the dimension is smaller and the check is faster and
-        # Because we assume that it is more likely to find the same ids in close positions, e.g.: same
-        # citing id in several citations with different cited ids.
-
-        schema = id_dict["schema"].strip().lower()
-        id = id_dict["identifier"]
-
-        if schema != "orcid":
-            validity_value = self.tmp_doi_m.validated_as_id(id)
-            if validity_value is None:
-                validity_value = self.doi_m.validated_as_id(id)
-            return validity_value
-        else:
-            validity_value = self.tmp_orcid_m.validated_as_id(id)
-            if validity_value is None:
-                validity_value = self.orcid_m.validated_as_id(id)
-            return validity_value
-
-    #added(probably unuseful)
-
-    def get_id_manager(self, schema_or_id, id_man_dict):
-        """Given as input the string of a schema (e.g.:'pmid') and a dictionary mapping strings of
-        the schemas to their id managers, the method returns the correct id manager. Note that each
-        instance of the Preprocessing class needs its own instances of the id managers, in order to
-        avoid conflicts while validating data"""
-        if ":" in schema_or_id:
-            split_id_prefix = schema_or_id.split(":")
-            schema = split_id_prefix[0]
-        else:
-            schema = schema_or_id
-        id_man = id_man_dict.get(schema)
-        return id_man
-
-    #added (probably unuseful)
-    def normalise_any_id(self, id_with_prefix):
-        id_man = self.doi_m
-        id_no_pref = ":".join(id_with_prefix.split(":")[1:])
-        norm_id_w_pref = id_man.normalise(id_no_pref, include_prefix=True)
-        return norm_id_w_pref
-
-    #added
-    def dict_to_cache(self, dict_to_be_saved, path):
-        path = Path(path)
-        parent_dir_path = path.parent.absolute()
-        if not os.path.exists(parent_dir_path):
-            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
-        with open(path, "w", encoding="utf-8") as fd:
-            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
-
-    #no modified(look at the part of the venues)
-    def csv_creator(self, item: dict) -> dict:
-        row = dict()
-        doi = str(item['id'])
-        if (doi and self.doi_set and doi in self.doi_set) or (doi and not self.doi_set):
-            norm_id = self.doi_m.normalise(doi, include_prefix=True)
-            # create empty row
-            keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
-                    'publisher', 'editor']
-            for k in keys:
-                row[k] = ''
-
-            attributes = item['attributes']
-
-            # row['type']
-            if attributes.get('types') is not None:
-                types_dict = attributes['types']
-                for k, v in types_dict.items():
-                    if k.lower() == 'ris':
-                        if type(v) is str:
-                            norm_v = v.strip().lower()
-                            if norm_v in self.RIS_types_map.keys():
-                                row['type'] = self.RIS_types_map[norm_v]
-                                break
-                    if k.lower() == 'bibtex':
-                        if type(v) is str:
-                            norm_v = v.strip().lower()
-                            if norm_v in self.BIBTEX_types_map.keys():
-                                row['type'] = self.BIBTEX_types_map[norm_v]
-                                break
-                    if k.lower() == 'schemaorg':
-                        if type(v) is str:
-                            norm_v = v.strip().lower()
-                            if norm_v in self.SCHEMAORG_types_map.keys():
-                                row['type'] = self.SCHEMAORG_types_map[norm_v]
-                                break
-                    if k.lower() == 'citeproc':
-                        if type(v) is str:
-                            norm_v = v.strip().lower()
-                            if norm_v in self.CITEPROC_types_map.keys():
-                                row['type'] = self.CITEPROC_types_map[norm_v]
-                                break
-                    if k.lower() == 'resourcetypegeneral':
-                        if type(v) is str:
-                            norm_v = v.strip().lower()
-                            if norm_v in self.RESOURCETYPEGENERAL_types_map.keys():
-                                row['type'] = self.RESOURCETYPEGENERAL_types_map[norm_v]
-                                break
-
-
-            # row['id']
-            ids_list = list()
-            ids_list.append(norm_id)
-
-            if attributes.get('identifiers'):
-                for other_id in attributes.get('identifiers'):
-                    if other_id.get('identifier') and other_id.get('identifierType'):
-                        o_id_type = other_id.get('identifierType')
-                        o_id = other_id.get('identifier')
-
-
-                        if o_id_type == 'ISBN':
-                            if row['type'] in {'book', 'dissertation', 'edited book', 'monograph', 'reference book', 'report',
-                                               'standard'}:
-                                self.id_worker(o_id, ids_list, self.isbn_worker)
-
-                        elif o_id_type == 'ISSN':
-                            if row['type'] in {'book series', 'book set', 'journal', 'proceedings series', 'series',
-                                               'standard series', 'report series'}:
-                                self.id_worker(o_id, ids_list, self.issn_worker)
-
-
-            row['id'] = ' '.join(ids_list)
-
-            # row['title']
-            pub_title = ""
-            if attributes.get("titles"):
-                for title in attributes.get("titles"):
-                    if title.get("title"):
-                        p_title = title.get("title")
-                        soup = BeautifulSoup(p_title, 'html.parser')
-                        title_soup = soup.get_text().replace('\n', '')
-                        title_soup_space_replaced = ' '.join(title_soup.split())
-                        title_soup_strip = title_soup_space_replaced.strip()
-                        clean_tit = html.unescape(title_soup_strip)
-                        pub_title = clean_tit if clean_tit else p_title
-
-            row['title'] = pub_title
-
-            agent_list_authors_only = self.add_authors_to_agent_list(attributes, [])
-            agents_list = self.add_editors_to_agent_list(attributes, agent_list_authors_only)
-
-            authors_strings_list, editors_string_list = self.get_agents_strings_list(doi, agents_list)
-
-            # row['author']
-            if 'creators' in attributes:
-                row['author'] = '; '.join(authors_strings_list)
-
-
-            # row['pub_date']
-            cur_date = ""
-            dates = attributes.get("dates")
-            if dates:
-                for date in dates:
-                    if date.get("dateType") == "Issued":
-                        cur_date = date.get("date")
-                        break
-
-            if cur_date == "":
-                if attributes.get("publicationYear"):
-                    cur_date = str(attributes.get("publicationYear"))
-
-            row['pub_date'] = cur_date
-
-            # row['venue']
-            row['venue'] = self.get_venue_name(attributes, row)
-
-            issue = ""
-            volume = ""
-
-            container = attributes.get("container")
-            if container and container.get("identifierType") == "ISSN" or container.get(
-                    "identifierType") == "ISBN":
-                if container.get("issue"):
-                    issue = container.get("issue")
-                if container.get("volume"):
-                    volume = container.get("volume")
-
-            if not issue or not volume:
-                relatedIdentifiers = attributes.get("relatedIdentifiers")
-                if relatedIdentifiers:
-                    for related in relatedIdentifiers:
-                        if related.get("relationType"):
-                            if related.get("relationType").lower() == "ispartof":
-                                if related.get("relatedIdentifierType") == "ISSN" or related.get("relatedIdentifierType") == "ISBN":
-                                    if not issue and related.get("issue"):
-                                        issue = related.get("issue")
-                                    if not volume and related.get("volume"):
-                                        volume = related.get("volume")
-            # row['volume']
-            row['volume'] = volume
-
-            # row['issue']
-            row['issue'] = issue
-
-            # row['page']
-            row['page'] = self.get_datacite_pages(attributes)
-
-            # row['publisher']
-            row['publisher'] = self.get_publisher_name(doi, attributes)
-
-            # row['editor']
-            if attributes.get("contributors"):
-                editors = [contributor for contributor in attributes.get("contributors") if
-                           contributor.get("contributorType") == "Editor"]
-                if editors:
-                    row['editor'] = '; '.join(editors_string_list)
-            try:
-                return self.normalise_unicode(row)
-            except TypeError:
-                print(row)
-                raise(TypeError)
-
-    #added
-    def to_validated_id_list(self, norm_id):
-        valid_id_list = []
-        if norm_id in self._redis_values_br:
-            self.tmp_doi_m.storage_manager.set_value(norm_id,True)  # In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-            # preso in considerazione negli step successivi
-            valid_id_list.append(norm_id)
-        # if the id is not in redis db, validate it before appending
-        elif self.tmp_doi_m.is_valid(norm_id):  # In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
-            # preso in considerazione negli step successivi
-            valid_id_list.append(norm_id)
-        return valid_id_list
-
-    #no modified
-    def get_datacite_pages(self, item: dict) -> str:
-        '''
-        This function returns the pages interval.
-
-        :params item: the item's dictionary
-        :type item: dict
-        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
-        '''
-        container_pages_list = list()
-        related_pages_list = list()
-        container = item.get("container")
-        if container:
-            if container.get("identifierType") == "ISSN" or container.get("identifierType") == "ISBN":
-                if container.get("firstPage"):
-                    container_pages_list.append(container.get("firstPage"))
-                if container.get("lastPage"):
-                    container_pages_list.append(container.get("lastPage"))
-
-        relatedIdentifiers = item.get("relatedIdentifiers")
-        if relatedIdentifiers:
-            for related in relatedIdentifiers:
-                if related.get("relationType"):
-                    if related.get("relationType").lower() == "ispartof":
-                        if related.get("relatedIdentifierType") == "ISSN" or related.get("relatedIdentifierType") == "ISBN":
-                            if related.get("firstPage"):
-                                related_pages_list.append(related.get("firstPage"))
-                            if related.get("lastPage"):
-                                related_pages_list.append(related.get("lastPage"))
-
-        page_list = related_pages_list if len(related_pages_list)> len(container_pages_list) else container_pages_list
-        return self.get_pages(page_list)
-
-    #no modified
-    def get_publisher_name(self, doi: str, item: dict) -> str:
-        '''
-        This function aims to return a publisher's name and id. If a mapping was provided,
-        it is used to find the publisher's standardized name from its id or DOI prefix.
-
-        :params doi: the item's DOI
-        :type doi: str
-        :params item: the item's dictionary
-        :type item: dict
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output is only the name. Finally, if there is no publisher, the output is an empty string.
-        '''
-        publisher = item.get("publisher")
-        if type(publisher) is str:
-            if publisher.lower().strip() == "(:unav)":
-                publisher = ""
-
-        data = {
-            'publisher': publisher,
-            'prefix': doi.split('/')[0]
-        }
-
-        publisher = data['publisher']
-        prefix = data['prefix']
-
-        if self.publishers_mapping:
-            member_dict = next(
-                    ({member: data} for member, data in self.publishers_mapping.items() if prefix in data['prefixes']),
-                    None)
-            if member_dict:
-                member = list(member_dict.keys())[0]
-                name_and_id = f"{member_dict[member]['name']} [datacite:{member}]"
-            else:
-                name_and_id = publisher
-        else:
-            name_and_id = publisher
-
-        return name_and_id
-
-    #no modified
-
-    def get_venue_name(self, item: dict, row: dict) -> str:
-        '''
-        This method deals with generating the venue's name, followed by id in square brackets, separated by spaces.
-        HTML tags are deleted and HTML entities escaped. In addition, any ISBN and ISSN are validated.
-        Finally, the square brackets in the venue name are replaced by round brackets to avoid conflicts with the ids enclosures.
-
-        :params item: the item's dictionary
-        :type item: dict
-        :params row: a CSV row
-        :type row: dict
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'Nutrition & Food Science
-         [issn:0034-6659]'. If the id does not exist, the output is only the name. Finally, if there is no venue,
-         the output is an empty string.
-         '''
-
-        cont_title = ""
-        venids_list = list()
-
-        # container
-        container = item.get("container")
-        if container:
-            # TITLE
-            if container.get("title"):
-                cont_title = (container["title"].lower()).replace('\n', '')
-                ven_soup = BeautifulSoup(cont_title, 'html.parser')
-                ventit = html.unescape(ven_soup.get_text())
-                ambiguous_brackets = re.search('\[\s*((?:[^\s]+:[^\s]+)?(?:\s+[^\s]+:[^\s]+)*)\s*\]', ventit)
-                if ambiguous_brackets:
-                    match = ambiguous_brackets.group(1)
-                    open_bracket = ventit.find(match) - 1
-                    close_bracket = ventit.find(match) + len(match)
-                    ventit = ventit[:open_bracket] + '(' + ventit[open_bracket + 1:]
-                    ventit = ventit[:close_bracket] + ')' + ventit[close_bracket + 1:]
-                    cont_title = ventit
-
-            # IDS
-            if container.get("identifierType") == "ISBN":
-                if row['type'] in {'book chapter', 'book part', 'book section', 'book track', 'reference entry'}:
-                    self.id_worker(container.get("identifier"), venids_list, self.isbn_worker)
-
-            if container.get("identifierType") == "ISSN":
-                if row['type'] in {'book', 'data file', 'dataset', 'edited book', 'journal article', 'journal volume',
-                                   'journal issue', 'monograph', 'proceedings', 'peer review', 'reference book',
-                                   'reference entry', 'report'}:
-                    self.id_worker(container.get("identifier"), venids_list, self.issn_worker)
-                elif row['type'] == 'report series':
-                    if container.get("title"):
-                        if container.get("title"):
-                            self.id_worker(container.get("identifier"), venids_list, self.issn_worker)
-
-
-        if not venids_list:
-            relatedIdentifiers = item.get("relatedIdentifiers")
-            if relatedIdentifiers:
-                for related in relatedIdentifiers:
-                    if related.get("relationType"):
-                        if related.get("relationType").lower() == "ispartof":
-                            if related.get("relatedIdentifierType") == "ISBN":
-                                if row['type'] in {'book chapter', 'book part', 'book section', 'book track',
-                                                   'reference entry'}:
-                                    self.id_worker(related.get("relatedIdentifier"), venids_list, self.isbn_worker)
-                            if related.get("relatedIdentifierType") == "ISSN":
-                                if row['type'] in {'book', 'data file', 'dataset', 'edited book', 'journal article',
-                                                   'journal volume',
-                                                   'journal issue', 'monograph', 'proceedings', 'peer review',
-                                                   'reference book',
-                                                   'reference entry', 'report'}:
-                                    self.id_worker(related.get("relatedIdentifier"), venids_list, self.issn_worker)
-                                elif row['type'] == 'report series':
-                                    if related.get("title"):
-                                        if related.get("title"):
-                                            self.id_worker(related.get("relatedIdentifier"), venids_list, self.issn_worker)
-
-        if venids_list:
-            name_and_id = cont_title + ' [' + ' '.join(venids_list) + ']' if cont_title else '[' + ' '.join(venids_list) + ']'
-        else:
-            name_and_id = cont_title
-
-        return name_and_id
-
-    #added the call to find_datacite_orcid
-    def add_editors_to_agent_list(self, item: dict, ag_list: list) -> list:
-        '''
-        This function returns the the agents list updated with the editors dictionaries, in the correct format.
-
-        :params item: the item's dictionary (attributes), ag_list: the
-        :type item: dict, ag_list: list
-
-        :returns: listthe agents list updated with the editors dictionaries, in the correct format.
-        '''
-        agent_list = ag_list
-        if item.get("contributors"):
-            editors = [contributor for contributor in item.get("contributors") if
-                       contributor.get("contributorType") == "Editor"]
-            for ed in editors:
-                agent = {}
-                agent["role"] = "editor"
-                if ed.get('name'):
-                    agent["name"] = ed.get("name")
-                if ed.get("nameType") == "Personal" or ("familyName" in ed or "givenName" in ed):
-                    agent["family"] = ed.get("familyName")
-                    agent["given"] = ed.get("givenName")
-                    if ed.get("nameIdentifiers"):
-                        orcid_ids = [x.get("nameIdentifier") for x in ed.get("nameIdentifiers") if
-                                     x.get("nameIdentifierScheme") == "ORCID"]
-                        if orcid_ids:
-                            orcid_id = self.find_datacite_orcid(orcid_ids)
-                            if orcid_id:
-                                agent["orcid"] = orcid_id
-
-                missing_names = [x for x in ["family", "given", "name"] if x not in agent]
-                for mn in missing_names:
-                    agent[mn] = ""
-                agent_list.append(agent)
-        return agent_list
-
-    # added the call to find_datacite_orcid
-    def add_authors_to_agent_list(self, item: dict, ag_list: list) -> list:
-        '''
-        This function returns the agents list updated with the authors dictionaries, in the correct format.
-
-        :params item: the item's dictionary (attributes), ag_list: the
-        :type item: dict, ag_list: list
-
-        :returns: list the agents list updated with the authors dictionaries, in the correct format.
-        '''
-        agent_list = ag_list
-        if item.get("creators"):
-            creators = item.get("creators")
-            for c in creators:
-                agent = {}
-                agent["role"] = "author"
-                if c.get("name"):
-                    agent["name"] = c.get("name")
-                if c.get("nameType") == "Personal" or ("familyName" in c or "givenName" in c):
-                    agent["family"] = c.get("familyName")
-                    agent["given"] = c.get("givenName")
-                    if c.get("nameIdentifiers"):
-                        orcid_ids = [x.get("nameIdentifier") for x in c.get("nameIdentifiers") if
-                                     x.get("nameIdentifierScheme") == "ORCID"]
-                        if orcid_ids:
-                            orcid_id = self.find_datacite_orcid(orcid_ids)
-                            if orcid_id:
-                                agent["orcid"] = orcid_id
-                missing_names = [x for x in ["family", "given", "name"] if x not in agent]
-                for mn in missing_names:
-                    agent[mn] = ""
-                agent_list.append(agent)
-        return agent_list
-
-    #added
-    def find_datacite_orcid(self, all_author_ids):
-        orcid = ""
-        if all_author_ids:
-            for identifier in all_author_ids:
-                norm_orcid = self.orcid_m.normalise(identifier, include_prefix = True)
-                ## Check orcid presence in memory and storage before validating the id
-                validity_value_orcid = self.validated_as({"identifier": norm_orcid, "schema": "orcid"})
-                if validity_value_orcid is True:
-                    orcid = norm_orcid
-                elif validity_value_orcid is None:
-                    #if self.RA_redis.get(norm_orcid):
-                    if norm_orcid in self._redis_values_ra:
-                        orcid = norm_orcid
-                    # if the id is not in redis db, validate it before appending
-                    elif self.tmp_orcid_m.is_valid(norm_orcid):
-                        orcid = norm_orcid
-        return orcid
-    # added
-    def memory_to_storage(self):
-        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
-        self.storage_manager.set_multi_value(kv_in_memory)
-        self.temporary_manager.delete_storage()
-
-    # added (division in first and second iteration)
-    def extract_all_ids(self, citation, is_first_iteration: bool):
-
-        if is_first_iteration:
-            all_br = set()
-            all_ra = set()
-
-            subject_id = citation['id']
-            norm_id = self.doi_m.normalise(subject_id, include_prefix=True)
-            if norm_id:
-                # if it was possible to normalise the id according to one of the schemas accepted in oc, add
-                # the id to the set of retrieved br ids for the citation.
-                all_br.add(norm_id)
-
-            attributes = citation.get("attributes")
-            if attributes:
-                creators = attributes.get("creators")
-                if creators:
-                    for c in creators:
-                        c_ids = c.get("nameIdentifiers")
-                        if c_ids:
-                            norm_c_orcids = {self.orcid_m.normalise(x.get("nameIdentifier"), include_prefix=True) for x in c.get("nameIdentifiers") if
-                                         x.get("nameIdentifierScheme") == "ORCID"}
-                            if norm_c_orcids:
-                                # if it was possible to normalise any id according to orcid schema, add
-                                # the norm_orcids to the set of retrieved ra ids for the citation.
-                                all_ra.update(norm_c_orcids)
-
-                if attributes.get("contributors"):
-                    editors = [contributor for contributor in citation .get("contributors") if
-                               contributor.get("contributorType") == "Editor"]
-                    for ed in editors:
-                        if ed.get("nameIdentifiers"):
-                            norm_ed_orcids = {self.orcid_m.normalise(x.get("nameIdentifier"), include_prefix=True) for x in ed.get("nameIdentifiers") if
-                                                x.get("nameIdentifierScheme") == "ORCID"}
-                            if norm_ed_orcids:
-                                all_ra.update(norm_ed_orcids)
-
-            all_br = list(all_br)
-            for x in all_br:
-                if x is None:
-                    all_br.remove(x)
-            all_ra = list(all_ra)
-            for y in all_ra:
-                if y is None:
-                    all_ra.remove(y)
-            return all_br, all_ra
-
-        #all the objects doi
-        else:
-            all_br = set()
-            attributes = citation["attributes"]
-            rel_ids = attributes.get("relatedIdentifiers")
-            if rel_ids:
-                for ref in rel_ids:
-                    if all(elem in ref for elem in self._needed_info):
-                        relatedIdentifierType = (str(ref["relatedIdentifierType"])).lower()
-                        relationType = str(ref["relationType"]).lower()
-                        if relatedIdentifierType == "doi":
-                            if relationType in self._filter:
-                                rel_id = self.doi_m.normalise(ref["relatedIdentifier"], include_prefix=True)
-                                if rel_id:
-                                    all_br.add(rel_id)
-            all_br = list(all_br)
-            return all_br
-
-
-    #added
-    def get_reids_validity_list(self, id_list, redis_db):
-        if redis_db == "ra":
-            valid_ra_ids = []
-            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
-            validity_list_ra = self.RA_redis.mget(id_list)
-            for i, e in enumerate(id_list):
-                if validity_list_ra[i]:
-                    valid_ra_ids.append(e)
-            return valid_ra_ids
-
-        elif redis_db == "br":
-            valid_br_ids = []
-            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
-            validity_list_br = self.BR_redis.mget(id_list)
-            for i, e in enumerate(id_list):
-                if validity_list_br[i]:
-                    valid_br_ids.append(e)
-            return valid_br_ids
-        else:
-            raise ValueError("redis_db must be either 'ra' for responsible agents ids "
-                             "or 'br' for bibliographic resources ids")
+import gzip
+import csv
+import json
+from os import makedirs
+import os
+import os.path
+from oc_ds_converter.oc_idmanager.arxiv import ArXivManager
+from oc_ds_converter.oc_idmanager.doi import DOIManager
+from oc_ds_converter.oc_idmanager.pmid import PMIDManager
+from oc_ds_converter.oc_idmanager.pmcid import PMCIDManager
+from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
+
+from datetime import datetime
+from argparse import ArgumentParser
+import html
+import json
+import os
+import pathlib
+import re
+import warnings
+from os.path import exists
+from pathlib import Path
+from typing import Dict, List, Tuple, Optional, Type, Callable
+
+import fakeredis
+from bs4 import BeautifulSoup
+from oc_ds_converter.datasource.redis import RedisDataSource
+from re import search, match, sub
+from oc_ds_converter.lib.cleaner import Cleaner
+from oc_ds_converter.lib.master_of_regex import *
+from oc_ds_converter.pubmed.get_publishers import ExtractPublisherDOI
+from oc_ds_converter.ra_processor import RaProcessor
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+
+warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
+
+
+class OpenaireProcessing(RaProcessor):
+    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_openaire: str = None, testing:bool = True, storage_manager:Optional[StorageManager] = None):
+        super(OpenaireProcessing, self).__init__(orcid_index, doi_csv)
+        if storage_manager is None:
+            self.storage_manager = SqliteStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self.temporary_manager = InMemoryStorageManager('../memory.json')
+
+        self.types_dict = {
+            "Article": "journal article",
+            "Part of book or chapter of book": "book chapter",
+            "Preprint": "other",
+            "Other literature type": "other",
+            "Conference object": "proceedings",
+            "Doctoral thesis": "dissertation",
+            "Book": "book",
+            "Thesis": "dissertation",
+            "Research": "other",
+            "Master thesis": "dissertation",
+            "Report": "report",
+            "Review": "other",
+            "Contribution for newspaper or weekly magazine": "other",
+            "Journal": "journal",
+            "Presentation": "other",
+            "Software Paper": "other",
+            "External research report": "report",
+            "Data Paper": "other",
+            "Project deliverable": "other",
+            "Bachelor thesis": "dissertation",
+            "Project proposal": "other",
+            "Newsletter": "other",
+            "Data Management Plan": "data management plan",
+            "Software": "computer program",
+            "Dataset": "dataset",
+            "Audiovisual": "dataset",
+            "Image": "dataset",
+            "Other dataset type": "dataset",
+            "Film": "dataset",
+            "UNKNOWN": "other",
+            "Other ORP type": "other",
+            "InteractiveResource": "other",
+            "PhysicalObject": "other",
+            "Collection": "other",
+            "Patent": "other",
+            "Project milestone": "other",
+            "Clinical Trial": "other",
+            "Bioentity": "other",
+            "Sound": "other",
+        }
+        self.doi_m = DOIManager(storage_manager=self.storage_manager)
+        self.pmid_m = PMIDManager(storage_manager=self.storage_manager)
+        self.pmc_m = PMCIDManager(storage_manager=self.storage_manager)
+        self.arxiv_m = ArXivManager(storage_manager=self.storage_manager)
+
+        self.orcid_m = ORCIDManager(storage_manager=self.storage_manager)
+
+        self._id_man_dict = {"doi":self.doi_m, "pmid": self.pmid_m, "pmcid": self.pmc_m,"pmc": self.pmc_m, "arxiv":self.arxiv_m}
+
+        # Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
+        # main storage_manager  only once the full file is processed. Checks must be done both on tmp and in
+        # storage_manager, so that in case the process breaks while processing a file which does not complete (so
+        # without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
+        # a storage_manager db would be considered to have been processed and thus would be ignored by the process
+        # and lost.
+
+        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
+        self.tmp_pmid_m = PMIDManager(storage_manager=self.temporary_manager)
+        self.tmp_pmc_m = PMCIDManager(storage_manager=self.temporary_manager)
+        self.tmp_arxiv_m = ArXivManager(storage_manager=self.temporary_manager)
+
+        self.tmp_orcid_m = ORCIDManager(storage_manager=self.temporary_manager)
+
+        self.tmp_id_man_dict = {"doi": self.tmp_doi_m, "pmid": self.tmp_pmid_m, "pmcid": self.tmp_pmc_m, "pmc": self.tmp_pmc_m,
+                             "arxiv": self.tmp_arxiv_m}
+
+
+        self._doi_prefixes_publishers_dict = {
+        "10.48550":{"publisher":"arxiv", "priority":1},
+        "doi:10.48550":{"publisher":"arxiv", "priority":1},
+        "10.6084":{"publisher":"figshare","priority":1},
+        "doi:10.6084":{"publisher":"figshare","priority":1},
+        "10.1184":{"publisher": "Carnegie Mellon University", "priority":2},
+        "doi:10.1184":{"publisher": "Carnegie Mellon University", "priority":2},
+        "10.25384":{"publisher":"sage", "priority":2},
+        "doi:10.25384":{"publisher":"sage", "priority":2},
+        "10.5281":{"publisher":"zenodo", "priority":3},
+        "doi:10.5281":{"publisher":"zenodo", "priority":3},
+        "10.5061":{"publisher":"dryad", "priority":4},
+        "doi:10.5061":{"publisher":"dryad", "priority":4},
+        "10.17605":{"publisher":"psyarxiv", "priority":5},
+        "doi:10.17605":{"publisher":"psyarxiv", "priority":5},
+        "10.31234": {"publisher":"psyarxiv", "priority":6},
+        "doi:10.31234": {"publisher":"psyarxiv", "priority":6},
+        }
+
+        if testing:
+            self.BR_redis = fakeredis.FakeStrictRedis()
+            self.RA_redis = fakeredis.FakeStrictRedis()
+
+        else:
+            self.BR_redis = RedisDataSource("DB-META-BR")
+            self.RA_redis = RedisDataSource("DB-META-RA")
+
+        self._redis_values_ra = []
+        self._redis_values_br = []
+
+
+        if not publishers_filepath_openaire:
+
+            if not exists(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files")):
+                os.makedirs(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files"))
+            self.publishers_filepath = os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files",
+                                                  "prefix_publishers.json")
+        else:
+            self.publishers_filepath = publishers_filepath_openaire
+
+        if os.path.exists(self.publishers_filepath):
+            pfp = dict()
+            csv_headers = ("id", "name", "prefix")
+            if self.publishers_filepath.endswith(".csv"):
+                with open(self.publishers_filepath, encoding="utf8") as f:
+                    csv_reader = csv.DictReader(f, csv_headers)
+                    for row in csv_reader:
+                        pfp[row["prefix"]] = {"name": row["name"], "crossref_member": row["id"]}
+                self.publishers_filepath = self.publishers_filepath.replace(".csv", ".json")
+            elif self.publishers_filepath.endswith(".json"):
+                with open(self.publishers_filepath, encoding="utf8") as f:
+                    pfp = json.load(f)
+
+            if pfp:
+                self.publisher_manager = ExtractPublisherDOI(pfp)
+            else:
+                self.publisher_manager = ExtractPublisherDOI({})
+        else:
+            self.publisher_manager = ExtractPublisherDOI({})
+            with open(self.publishers_filepath, "w", encoding="utf8") as fdp:
+                json.dump({}, fdp, ensure_ascii=False, indent=4)
+
+    def update_redis_values(self, br, ra):
+        self._redis_values_br = br
+        self._redis_values_ra = ra
+
+    def validated_as(self, id_dict):
+        # Check if the validity was already retrieved and thus
+        # a) if it is now saved either in the in-memory database, which only concerns data validated
+        # during the current file processing;
+        # b) or if it is now saved in the storage_manager database, which only concerns data validated
+        # during the previous files processing.
+        # In memory db is checked first because the dimension is smaller and the check is faster and
+        # Because we assume that it is more likely to find the same ids in close positions, e.g.: same
+        # citing id in several citations with different cited ids.
+
+        schema = id_dict["schema"].strip().lower()
+        id = id_dict["identifier"]
+
+        if schema != "orcid":
+            tmp_id_m = self.get_id_manager(schema, self.tmp_id_man_dict)
+            validity_value = tmp_id_m.validated_as_id(id)
+
+            if validity_value is None:
+                id_m = self.get_id_manager(schema, self._id_man_dict)
+                validity_value = id_m.validated_as_id(id)
+            return validity_value
+
+        else:
+            validity_value = self.tmp_orcid_m.validated_as_id(id)
+            if validity_value is None:
+                validity_value = self.orcid_m.validated_as_id(id)
+            return validity_value
+
+    def get_id_manager(self, schema_or_id, id_man_dict):
+        """Given as input the string of a schema (e.g.:'pmid') and a dictionary mapping strings of
+        the schemas to their id managers, the method returns the correct id manager. Note that each
+        instance of the Preprocessing class needs its own instances of the id managers, in order to
+        avoid conflicts while validating data"""
+        if ":" in schema_or_id:
+            split_id_prefix = schema_or_id.split(":")
+            schema = split_id_prefix[0]
+        else:
+            schema = schema_or_id
+        id_man = id_man_dict.get(schema)
+        return id_man
+
+    def normalise_any_id(self, id_with_prefix):
+        id_man = self.get_id_manager(id_with_prefix, self._id_man_dict)
+        id_no_pref = ":".join(id_with_prefix.split(":")[1:])
+        norm_id_w_pref = id_man.normalise(id_no_pref, include_prefix=True)
+        return norm_id_w_pref
+
+    def get_norm_ids(self, entity):
+        norm_ids = []
+        for e in entity:
+            e_schema = e.get("schema").strip().lower()
+            if e_schema in self._id_man_dict:
+                e_id = self._id_man_dict[e_schema].normalise(e["identifier"], include_prefix=True)
+                if e_id:
+                    dict_to_append = {"schema": e_schema, "identifier": e_id}
+                    if dict_to_append not in norm_ids:
+                        norm_ids.append(dict_to_append)
+        return norm_ids
+
+    def dict_to_cache(self, dict_to_be_saved, path):
+        path = Path(path)
+        parent_dir_path = path.parent.absolute()
+        if not os.path.exists(parent_dir_path):
+            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
+        with open(path, "w", encoding="utf-8") as fd:
+            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
+
+    def csv_creator(self, item: dict) -> dict:
+        #redis_br = item["redis_validity_lists"][0]
+        #redis_ra = item["redis_validity_lists"][1]
+
+        #self.update_redis_values(redis_br, redis_ra)
+
+        row = dict()
+        
+        doi = []
+        
+        keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
+                'publisher', 'editor']
+        for k in keys:
+            row[k] = ''
+
+        attributes = item
+        # row['type'] √
+        att_type = attributes.get("objectSubType")
+        if att_type:
+            map_type = self.types_dict.get(att_type)
+            if not map_type:
+                map_type = "other"
+        else:
+            map_type = "other"
+        row['type'] = map_type
+
+        # row['id']
+        att_identifier_dict_of_lists = attributes.get("identifier")
+        valid_ids_list = self.to_validated_id_list(att_identifier_dict_of_lists)
+
+        # Keep a doi for retrieving information related to its prefix (i.e.: publisher, RA..) only in the cases
+        # where there is only one doi to refer to or where all the dois have the same prefix.
+        if valid_ids_list:
+            for id in valid_ids_list:
+                if id.startswith("doi:"):
+                    doi.append(id[len("doi:"):])
+            row['id'] = ' '.join(valid_ids_list)
+        else:
+            return {}
+
+
+        # row['title'] √
+        pub_title = ""
+        att_title = attributes.get("title")
+        if att_title:
+            p_title = att_title
+            soup = BeautifulSoup(p_title, 'html.parser')
+            title_soup = soup.get_text().replace('\n', '')
+            title_soup_space_replaced = ' '.join(title_soup.split())
+            title_soup_strip = title_soup_space_replaced.strip()
+            clean_tit = html.unescape(title_soup_strip)
+            pub_title = clean_tit if clean_tit else p_title
+        
+        row['title'] = pub_title
+
+        # row['author'] √
+        agents_list = self.add_authors_to_agent_list(attributes, [])
+        pref_dois = [x for x in doi if x.split("/")[0] not in self._doi_prefixes_publishers_dict]
+        if doi:
+            best_doi = pref_dois[0] if pref_dois else doi[0]
+        else:
+            best_doi = ""
+        authors_strings_list, editors_string_list = self.get_agents_strings_list(best_doi, agents_list)
+        row['author'] = '; '.join(authors_strings_list)
+
+        # row['pub_date'] √
+        dates = attributes.get("publicationDate")
+        row['pub_date'] = str(dates) if dates else ""
+
+        # row['venue']
+        row['venue'] = ""
+
+        # row['volume']
+        row['volume'] = ""
+
+        # row['issue']
+        row['issue'] = ""
+
+        # row['page']
+        row['page'] = ""
+
+        # row['publisher']  √
+        att_publ = attributes.get("publisher")
+        publ = ""
+        if att_publ:
+            publ = att_publ[0]
+        publishers = self.get_publisher_name(doi, publ)
+                    
+        row['publisher'] = publishers
+
+        # row['editor']
+        row['editor'] = ""
+
+        try:
+            return self.normalise_unicode(row)
+
+        except TypeError:
+            print(row)
+            raise(TypeError)
+
+    def get_publisher_name(self, doi_list: list, item: dict) -> str:
+        '''
+        This function aims to return a publisher's name and id. If a mapping was provided,
+        it is used to find the publisher's standardized name from its id or DOI prefix.
+
+        :params doi: the item's DOI
+        :type doi_list: list
+        :params item: the item's dictionary
+        :type item: dict
+        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output is only the name. Finally, if there is no publisher, the output is an empty string.
+        '''
+        if not item or not isinstance(item, dict):
+            return ""
+        elif "name" not in item:
+            return ""
+
+        publisher = item.get("name") if item.get("name") else ""
+
+        if publisher and doi_list:
+            for doi in doi_list:
+                prefix = doi.split('/')[0] if doi else ""
+                if prefix:
+                    if prefix in self.publisher_manager._prefix_to_data_dict:
+                        prefix_data = self.publisher_manager.extract_publishers_v(doi, enable_extraagencies=False,get_all_prefix_data=True, skip_update=True)
+                        if prefix_data:
+                            member = prefix_data.get("crossref_member") if prefix_data.get("crossref_member") not in {"not found", None} else ""
+                            retrieved_publisher_name = prefix_data.get("name") if prefix_data.get("name") not in {"unidentified", None} else ""
+                            if isinstance(retrieved_publisher_name, str):
+                                if publisher.lower().strip() == retrieved_publisher_name.lower().strip():
+                                    return f'{publisher} [crossref:{member}]' if member else publisher
+
+        return publisher
+
+    def manage_arxiv_single_id(self, id_dict_list):
+        result_dict_list = []
+        arxiv_id = ""
+        is_arxiv = False
+        ent = id_dict_list[0]
+        schema = ent.get("schema")
+        if isinstance(schema, str):
+            schema = schema.strip().lower()
+            if schema == "doi":
+                id = ent.get("identifier")
+                splitted_pref = id.split('/')[0]
+                pref = re.findall("(10.\d{4,9})", splitted_pref)[0]
+                if pref == "10.48550":
+                    if id.startswith("doi:"):
+                        id = id[len("doi:"):]
+                    id_no_pref = id.replace(pref,"")
+
+                    arxiv_id = self._id_man_dict["arxiv"].normalise(id_no_pref, include_prefix=True)
+                    if not arxiv_id:
+                        return None
+                    else:
+                        is_arxiv = True
+            elif schema == "arxiv":
+                id = ent.get("identifier")
+                arxiv_id = self._id_man_dict["arxiv"].normalise(id, include_prefix=True)
+                if not arxiv_id:
+                    return None
+                else:
+                    is_arxiv = True
+            else:
+                return id_dict_list
+        if is_arxiv:
+            result_dict_list = [{"schema": "arxiv", "identifier": arxiv_id}]
+        if not result_dict_list:
+            return id_dict_list
+
+        return result_dict_list
+
+    def manage_doi_prefixes_priorities(self, id_dict_list):
+        result_id_dict_list= []
+        priority_prefixes = [k for k,v in self._doi_prefixes_publishers_dict.items() if v.get("priority")==1]
+        arxiv_or_figshare_dois = [x for x in id_dict_list if x.get("identifier").split("/")[0] in priority_prefixes]
+        if len(arxiv_or_figshare_dois) == 1:
+            id_dict = arxiv_or_figshare_dois[0]
+            is_arxiv = self._doi_prefixes_publishers_dict[id_dict.get("identifier").split("/")[0]].get("publisher") == "arxiv"
+            has_version = search("v\d+", id_dict.get("identifier"))
+            if has_version: # It is necessarily a figshare doi (ARXIV have version only in arxiv id and not in arxiv dois)
+                #√
+                return arxiv_or_figshare_dois
+            else:
+                if not is_arxiv:
+                    upd_id = id_dict.get("identifier") + "v1"
+                    upd_dict = {k:v for k,v in id_dict.items() if k!= "identifier"}
+                    upd_dict["identifier"] = upd_id
+                    result_id_dict_list.append(upd_dict)
+                    # √
+                    return result_id_dict_list
+                else:
+                    # √
+                    return self.manage_arxiv_single_id([id_dict])
+
+        elif len(arxiv_or_figshare_dois) > 1:
+            versioned_arxiv_or_figshare_dois = [x for x in arxiv_or_figshare_dois if search("v\d+", x.get("identifier"))]
+            if versioned_arxiv_or_figshare_dois:
+                # √
+                return versioned_arxiv_or_figshare_dois
+            else:
+                for id_dict in arxiv_or_figshare_dois:
+                    if self._doi_prefixes_publishers_dict[id_dict.get("identifier").split("/")[0]].get("publisher") == "arxiv":
+                        # in order to avoid multiple ids of the same schema for the same entity without a reasonable expl.
+                        # √
+                        return self.manage_arxiv_single_id([id_dict])
+
+                for id_dict in arxiv_or_figshare_dois:
+                    if self._doi_prefixes_publishers_dict[id_dict.get("identifier").split("/")[0]].get("publisher") == "figshare":
+                        version = "v1"
+                        upd_dict = {k:v for k,v in id_dict.items() if k != "identifier"}
+                        upd_id = id_dict.get("identifier") + version
+                        upd_dict["identifier"] = upd_id
+                        result_id_dict_list.append(upd_dict)
+                        # √
+                        return result_id_dict_list
+        else:
+            zenodo_ids_list = [x for x in id_dict_list if self._doi_prefixes_publishers_dict[x.get("identifier").split("/")[0]].get("publisher") == "zenodo"]
+            if len(zenodo_ids_list) >= 2:
+                list_of_id_n_str = [x["identifier"].replace("doi:", "").replace("10.5281/zenodo.", "") for x in zenodo_ids_list]
+                list_of_id_n_int = []
+                for n in list_of_id_n_str:
+                    try:
+                        int_n = int(n)
+                        list_of_id_n_int.append(int_n)
+                    except:
+                        pass
+                if list_of_id_n_int:
+                    last_assigned_id = str(max(list_of_id_n_int))
+                    for id_dict in zenodo_ids_list:
+                        if id_dict.get("identifier").replace("doi:", "").replace("10.5281/zenodo.", "") == last_assigned_id:
+                            result_id_dict_list.append(id_dict)
+                            # √
+                            return result_id_dict_list
+            else:
+                prefix_set = {x.get("identifier").split("/")[0] for x in id_dict_list}
+                priorities = [self._doi_prefixes_publishers_dict[p]["priority"] for p in prefix_set]
+                max_priority = min(priorities)
+
+                prefixes_w_max_priority = {k for k,v in self._doi_prefixes_publishers_dict.items() if v["priority"] == max_priority}
+
+                for id_dict in id_dict_list:
+                    if id_dict.get("identifier").split("/")[0] in prefixes_w_max_priority:
+                        norm_id = self.doi_m.normalise(id_dict["identifier"], include_prefix=True)
+                        #if self.BR_redis.get(norm_id):
+                        if norm_id in self._redis_values_br:
+                            result_id_dict_list.append(id_dict)
+                            return result_id_dict_list
+                        # if the id is not in redis db, validate it before appending
+                        elif self.tmp_doi_m.is_valid(norm_id):
+                            result_id_dict_list.append(id_dict)
+                            return result_id_dict_list
+
+                if not result_id_dict_list:
+
+                    while id_dict_list and max_priority < 7:
+
+                        id_dict_list = [x for x in id_dict_list if x["identifier"].split("/")[0] not in prefixes_w_max_priority]
+                        max_priority += 1
+                        prefixes_w_max_priority = {k for k, v in self._doi_prefixes_publishers_dict.items() if
+                                                   v["priority"] == max_priority}
+
+                        for id_dict in id_dict_list:
+                            if id_dict.get("identifier").split("/")[0] in prefixes_w_max_priority:
+                                norm_id = self.doi_m.normalise(id_dict["identifier"], include_prefix=True)
+                                #if self.BR_redis.get(norm_id):
+                                if norm_id in self._redis_values_br:
+                                    result_id_dict_list.append(id_dict)
+                                    return result_id_dict_list
+                                # if the id is not in redis db, validate it before appending
+                                elif self.tmp_doi_m.is_valid(norm_id):
+                                    result_id_dict_list.append(id_dict)
+                                    return result_id_dict_list
+
+        return result_id_dict_list
+
+    def to_validated_id_list(self, id_dict_of_list):
+        """this method takes in input a list of id dictionaries and returns a list valid and existent ids with prefixes.
+        For each id, a first validation try is made by checking its presence in META db. If the id is not in META db yet,
+        a second attempt is made by using the specific id-schema API"""
+        valid_id_set = set([x["identifier"] for x in id_dict_of_list["valid"]])
+        to_be_processed_input = id_dict_of_list["to_be_val"]
+        to_be_processed_id_dict_list = []
+        # If there is only an id, check whether it is either an arxiv id or an arxiv doi. In this cases, if there is a
+        # versioned arxiv id, it is kept as such. Otherwise both the arxiv doi and the not versioned arxiv id are replaced
+        # with the v1 version of the arxiv id. If it is not possible to retrieve an arxiv id from the only id which is
+        # either declared as an arxiv id or starts with the arxiv doi prefix, return None and interrupt the process
+        if len(valid_id_set) == 0:
+            if len(to_be_processed_input) == 1:
+                single_id_dict_list = self.manage_arxiv_single_id(to_be_processed_input)
+                if single_id_dict_list:
+                    to_be_processed_id_dict_list = single_id_dict_list
+                else:
+                    return
+            elif len(to_be_processed_input)> 1:
+                second_selection_list = [x for x in to_be_processed_input if x.get("schema") == "pmid" or (x.get("schema") =="doi" and x.get("identifier").split('/')[0] not in self._doi_prefixes_publishers_dict)]
+                if second_selection_list:
+                    to_be_processed_id_dict_list = second_selection_list
+                else:
+                    third_selection = [x for x in to_be_processed_input if x.get("schema") == "pmc" or x.get("schema") == "pmcid"]
+                    if third_selection:
+                        to_be_processed_id_dict_list = third_selection
+                    else:
+                        fourth_selection = [x for x in to_be_processed_input if x.get("schema") == "arxiv"]
+                        if fourth_selection:
+                            to_be_processed_id_dict_list = fourth_selection
+                        else:
+                            fifth_selection = [x for x in to_be_processed_input if x.get("schema") == "doi" and x.get("identifier").split('/')[0] in self._doi_prefixes_publishers_dict]
+                            if fifth_selection:
+                                to_be_processed_id_dict_list = self.manage_doi_prefixes_priorities(fifth_selection)
+
+            else:
+                return None
+        else:
+            to_be_processed_id_dict_list = [x for x in to_be_processed_input if x.get("schema") == "pmid" or (x.get("schema") == "doi" and x.get("identifier").split('/')[0] not in self._doi_prefixes_publishers_dict)]
+
+        if to_be_processed_id_dict_list:
+            for ent in to_be_processed_id_dict_list:
+                schema = ent.get("schema")
+                norm_id = ent.get("identifier")
+                tmp_id_man = self.get_id_manager(schema, self.tmp_id_man_dict)
+                if schema in {"pmid", "pmcid", "pmc", "arxiv", "doi"}:
+                    #if self.BR_redis.get(norm_id):
+                    if norm_id in self._redis_values_br:
+                        tmp_id_man.storage_manager.set_value(norm_id, True) #In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                        # preso in considerazione negli step successivi
+                        valid_id_set.add(norm_id)
+                    # if the id is not in redis db, validate it before appending
+                    elif tmp_id_man.is_valid(norm_id):#In questo modo l'id presente in redis viene inserito anche nello storage e risulta già
+                        # preso in considerazione negli step successivi
+                        valid_id_set.add(norm_id)
+
+        valid_id_list = list(valid_id_set)
+        return valid_id_list
+
+    def add_authors_to_agent_list(self, item: dict, ag_list: list) -> list:
+        '''
+        This function returns the the agents list updated with the authors dictionaries, in the correct format.
+
+        :params item: the item's dictionary (attributes), ag_list: the agent list
+        :type item: dict, ag_list: list
+
+        :returns: list the agents list updated with the authors dictionaries, in the correct format.
+        '''
+
+        agent_list = ag_list
+        if item.get("creator"):
+            for author in item.get("creator"):
+                agent = {}
+                agent["role"] = "author"
+                agent["name"] = author.get("name") if author.get("name") else ""
+                missing_names = [x for x in ["family", "given"] if x not in agent]
+                for mn in missing_names:
+                    agent[mn] = ""
+                all_ids = author.get("identifiers")
+                orcid_id = self.find_openaire_orcid(all_ids)
+                if orcid_id:
+                    agent["orcid"] = orcid_id
+                agent_list.append(agent)
+        
+        return agent_list
+
+    def find_openaire_orcid(self, all_author_ids):
+        orcid = ""
+        if all_author_ids:
+            for id in all_author_ids:
+                schema = id.get("schema")
+                identifier = id.get("identifier")
+                if isinstance(schema, str):
+                    if schema.lower().strip() == "orcid":
+                        if isinstance(identifier, str):
+                            norm_orcid = self.orcid_m.normalise(identifier, include_prefix =True)
+                            ## Check orcid presence in memory and storage before validating the id
+                            validity_value_orcid = self.validated_as({"identifier":norm_orcid, "schema": schema})
+                            if validity_value_orcid is True:
+                                orcid = norm_orcid
+                            elif validity_value_orcid is None:
+                                #if self.RA_redis.get(norm_orcid):
+                                if norm_orcid in self._redis_values_ra:
+                                    orcid = norm_orcid
+                                # if the id is not in redis db, validate it before appending
+                                elif self.tmp_orcid_m.is_valid(norm_orcid):
+                                    orcid = norm_orcid
+
+
+        return orcid
+
+    def memory_to_storage(self):
+        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
+        self.storage_manager.set_multi_value(kv_in_memory)
+        self.temporary_manager.delete_storage()
+
+    def extract_all_ids(self, citation):
+        all_br = set()
+        all_ra = set()
+
+        d1 = citation["source"]
+        d2 = citation["target"]
+
+        source_and_target = [d1, d2]
+
+        #for both source and target entity
+        for d in source_and_target:
+            # get all the br ids
+            br_ids_dicts = d["identifier"]
+            #and use the correct id manager to normalise
+            for br_id in br_ids_dicts:
+                schema = br_id.get("schema").strip().lower()
+                if schema in self._id_man_dict:
+                    norm_id = self._id_man_dict[schema].normalise(br_id["identifier"], include_prefix=True)
+                    if norm_id:
+                        # if it was possible to normalise the id according to one of the schemas accepted in oc, add
+                        # the id to the set of retrieved br ids for the citation.
+                        all_br.add(norm_id)
+            creators = d.get("creator")
+            if creators:
+                for c in creators:
+                    c_ids = c.get("identifiers")
+                    if c_ids:
+                        norm_orcids = {self.orcid_m.normalise(x.get("identifier"), include_prefix=True) for x in c_ids if x.get("schema") in {"ORCID", "orcid"}}
+                        if norm_orcids:
+                            # if it was possible to normalise any id according to orcid schema, add
+                            # the norm_orcids to the set of retrieved ra ids for the citation.
+                            all_ra.update(norm_orcids)
+        all_br = list(all_br)
+        all_ra = list(all_ra)
+        return all_br, all_ra
+
+    def get_reids_validity_list(self, id_list, redis_db):
+        if redis_db == "ra":
+            valid_ra_ids = []
+            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
+            validity_list_ra = self.RA_redis.mget(id_list)
+            for i, e in enumerate(id_list):
+                if validity_list_ra[i]:
+                    valid_ra_ids.append(e)
+            return valid_ra_ids
+
+        elif redis_db == "br":
+            valid_br_ids = []
+            # DO NOT UPDATED (REDIS RETRIEVAL METHOD HERE)
+            validity_list_br = self.BR_redis.mget(id_list)
+            for i, e in enumerate(id_list):
+                if validity_list_br[i]:
+                    valid_br_ids.append(e)
+            return valid_br_ids
+        else:
+            raise ValueError("redis_db must be either 'ra' for responsible agents ids "
+                             "or 'br' for bibliographic resources ids")
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/datasource/datasource.py` & `oc_ds_converter-1.0.1/oc_ds_converter/datasource/datasource.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!python
-# Copyright (c) 2022 The OpenCitations Index Authors.
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-from abc import ABCMeta, abstractmethod
-
-
-class DataSource(metaclass=ABCMeta):
-    def __init__(self, service):
-        self._service = service
-
-    def new(self):
-        return {"date": None, "valid": False, "issn": [], "orcid": []}
-
-    @abstractmethod
-    def get(self, resource_id):
-        pass
-
-    @abstractmethod
-    def mget(self, resources_id):
-        pass
-
-    @abstractmethod
-    def set(self, resource_id, value):
-        pass
-
-    @abstractmethod
-    def mset(self, resources):
+#!python
+# Copyright (c) 2022 The OpenCitations Index Authors.
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+from abc import ABCMeta, abstractmethod
+
+
+class DataSource(metaclass=ABCMeta):
+    def __init__(self, service):
+        self._service = service
+
+    def new(self):
+        return {"date": None, "valid": False, "issn": [], "orcid": []}
+
+    @abstractmethod
+    def get(self, resource_id):
+        pass
+
+    @abstractmethod
+    def mget(self, resources_id):
+        pass
+
+    @abstractmethod
+    def set(self, resource_id, value):
+        pass
+
+    @abstractmethod
+    def mset(self, resources):
         pass
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/datasource/redis.py` & `oc_ds_converter-1.0.1/oc_ds_converter/datasource/redis.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!python
-# Copyright (c) 2022 The OpenCitations Index Authors.
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-import configparser
-import json
-import os
-from os.path import join
-
-import redis
-
-from oc_ds_converter.datasource.datasource import DataSource
-
-
-class RedisDataSource(DataSource):
-    def __init__(self, service, config_filepath: str = 'config.ini'):
-        super().__init__(service)
-        config = configparser.ConfigParser(allow_no_value=True)
-        cur_path = os.path.dirname(os.path.abspath(__file__))
-        conf_file = config_filepath if config_filepath != 'config.ini' else join(cur_path, config_filepath)
-        config.read(conf_file)
-        if service == "DB-META-RA":
-            self._r =  redis.Redis(
-                            host='127.0.0.1',
-                            port=int(config.get('redis', 'port')),
-                            db=(config.get('database 0', 'db')),
-                            password=None,
-                            decode_responses=True
-                        )
-        elif service == "DB-META-BR":
-            self._r = redis.Redis(
-                    host='127.0.0.1',
-                    port=int(config.get('redis', 'port')),
-                    db=(config.get('database 1', 'db')),
-                    password=None,
-                    decode_responses=True
-                )
-        elif service == "PROCESS-DB":
-            self._r =  redis.Redis(
-                            host='127.0.0.1',
-                            port=int(config.get('redis', 'port')),
-                            db=(config.get('database 2', 'db')),
-                            password=None,
-                            decode_responses=True
-                        )
-
-        else:
-            raise ValueError
-
-    def get(self, resource_id):
-        redis_data = self._r.get(resource_id)
-        if redis_data != None:
-            if isinstance(redis_data, str) or isinstance(redis_data, int):
-                return redis_data
-            else:
-                return json.loads(redis_data)
-        else:
-            return None
-
-    def mget(self, resources_id):
-        if resources_id:
-            return [x if x and isinstance(x, (int,str,bool)) else json.loads(x) if x and isinstance(x, bytes) else None for x in self._r.mget(resources_id)]
-        else:
-            return[]
-        # return {
-        #     resources_id[i]: json.loads(v) if not v is None else None
-        #     for i, v in enumerate(self._r.mget(resources_id))
-        # }
-
-    def flushall(self):
-        self._r.flushall()
-
-    def delete(self, resource_id):
-        self._r.delete(resource_id)
-
-    def scan_iter(self, match="*"):
-        return self._r.scan_iter(match=match)
-
-    def set(self, resource_id, value):
-        return self._r.set(resource_id, json.dumps(value))
-
-    def mset(self, resources):
-        if resources:
+#!python
+# Copyright (c) 2022 The OpenCitations Index Authors.
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+import configparser
+import json
+import os
+from os.path import join
+
+import redis
+
+from oc_ds_converter.datasource.datasource import DataSource
+
+
+class RedisDataSource(DataSource):
+    def __init__(self, service, config_filepath: str = 'config.ini'):
+        super().__init__(service)
+        config = configparser.ConfigParser(allow_no_value=True)
+        cur_path = os.path.dirname(os.path.abspath(__file__))
+        conf_file = config_filepath if config_filepath != 'config.ini' else join(cur_path, config_filepath)
+        config.read(conf_file)
+        if service == "DB-META-RA":
+            self._r =  redis.Redis(
+                            host='127.0.0.1',
+                            port=int(config.get('redis', 'port')),
+                            db=(config.get('database 0', 'db')),
+                            password=None,
+                            decode_responses=True
+                        )
+        elif service == "DB-META-BR":
+            self._r = redis.Redis(
+                    host='127.0.0.1',
+                    port=int(config.get('redis', 'port')),
+                    db=(config.get('database 1', 'db')),
+                    password=None,
+                    decode_responses=True
+                )
+        elif service == "PROCESS-DB":
+            self._r =  redis.Redis(
+                            host='127.0.0.1',
+                            port=int(config.get('redis', 'port')),
+                            db=(config.get('database 2', 'db')),
+                            password=None,
+                            decode_responses=True
+                        )
+
+        else:
+            raise ValueError
+
+    def get(self, resource_id):
+        redis_data = self._r.get(resource_id)
+        if redis_data != None:
+            if isinstance(redis_data, str) or isinstance(redis_data, int):
+                return redis_data
+            else:
+                return json.loads(redis_data)
+        else:
+            return None
+
+    def mget(self, resources_id):
+        if resources_id:
+            return [x if x and isinstance(x, (int,str,bool)) else json.loads(x) if x and isinstance(x, bytes) else None for x in self._r.mget(resources_id)]
+        else:
+            return[]
+        # return {
+        #     resources_id[i]: json.loads(v) if not v is None else None
+        #     for i, v in enumerate(self._r.mget(resources_id))
+        # }
+
+    def flushall(self):
+        self._r.flushall()
+
+    def delete(self, resource_id):
+        self._r.delete(resource_id)
+
+    def scan_iter(self, match="*"):
+        return self._r.scan_iter(match=match)
+
+    def set(self, resource_id, value):
+        return self._r.set(resource_id, json.dumps(value))
+
+    def mset(self, resources):
+        if resources:
             return self._r.mset({k: v for k, v in resources.items()})
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/jalc/jalc_processing.py` & `oc_ds_converter-1.0.1/oc_ds_converter/jalc/jalc_processing.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from __future__ import annotations
-
-import csv
-import pathlib
-from os.path import exists
-from oc_ds_converter.pubmed.get_publishers import ExtractPublisherDOI
-
-from oc_ds_converter.oc_idmanager.doi import DOIManager
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.jid import JIDManager
-
-import os
-import os.path
-import json
-import re
-import warnings
-from pathlib import Path
-from typing import Optional
-
-import fakeredis
-from oc_ds_converter.datasource.redis import RedisDataSource
-from oc_ds_converter.ra_processor import RaProcessor
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-
-warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
-
-
-class JalcProcessing(RaProcessor):
-
-    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_jalc: str = None, testing: bool = True, storage_manager: Optional[StorageManager] = None, citing=True):
-        """This class is responsible for producing CSV tables to be used as input for the META process
-        aimed at ingesting data from the sources."""
-        super(JalcProcessing, self).__init__(orcid_index, doi_csv)
-        self.citing = citing
-        if storage_manager is None:
-            self.storage_manager = SqliteStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self.temporary_manager = InMemoryStorageManager('../memory.json')
-
-        self.doi_m = DOIManager(storage_manager=self.storage_manager)
-        self.issn_m = ISSNManager()
-        self.jid_m = JIDManager(storage_manager=self.storage_manager)
-
-        self.venue_id_man_dict = {"issn":self.issn_m, "jid":self.jid_m}
-
-        '''Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
-        main storage_manager only once a full file is processed. Checks must be done both on tmp and in
-        storage_manager, so that in case the process breaks while processing a file which does not complete (so
-        without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
-        a storage_manager db would be considered to have been processed and thus would be ignored by the process
-        and lost.'''
-
-        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
-        self.tmp_jid_m = JIDManager(storage_manager=self.temporary_manager)
-
-        self.venue_tmp_id_man_dict = {"issn":self.issn_m, "jid":self.tmp_jid_m}
-
-
-        if testing:
-            self.BR_redis = fakeredis.FakeStrictRedis()
-
-        else:
-            self.BR_redis = RedisDataSource("DB-META-BR")
-
-        self._redis_values_br = []
-
-        if not publishers_filepath_jalc:
-            self.publishers_filepath = None
-        else:
-            self.publishers_filepath = publishers_filepath_jalc
-
-            if os.path.exists(self.publishers_filepath):
-                pfp = dict()
-                csv_headers = ("id", "name", "prefix")
-                if self.publishers_filepath.endswith(".csv"):
-                    with open(self.publishers_filepath, encoding="utf8") as f:
-                        csv_reader = csv.DictReader(f, csv_headers)
-                        for row in csv_reader:
-                            pfp[row["prefix"]] = {"name": row["name"], "crossref_member": row["id"]}
-                    self.publishers_filepath = self.publishers_filepath.replace(".csv", ".json")
-                elif self.publishers_filepath.endswith(".json"):
-                    with open(self.publishers_filepath, encoding="utf8") as f:
-                        pfp = json.load(f)
-                self.publishers_mapping = pfp
-
-    def update_redis_values(self, br):
-        self._redis_values_br = br
-
-    def validated_as(self, id):
-        """Check if the validity was already retrieved and thus
-        a) if it is now saved either in the in-memory database, which only concerns data validated
-         during the current file processing;
-        b) or if it is now saved in the storage_manager database, which only concerns data validated
-        during the previous files processing.
-        In memory db is checked first because the dimension is smaller and the check is faster and
-        because we assume that it is more likely to find the same ids in close positions, e.g.: same
-        citing id in several citations with different cited ids.
-        In conclusion, if the id is found with this method, it means that this has been found in the dump we are processing"""
-        validity_value = self.tmp_doi_m.validated_as_id(id)
-        if validity_value is None:
-            validity_value = self.doi_m.validated_as_id(id)
-        return validity_value
-
-
-    def get_id_manager(self, schema_or_id, id_man_dict):
-        """Given as input the string of a schema (e.g.:'jid') and a dictionary mapping strings of
-        the schemas to their id managers, the method returns the correct id manager. Note that each
-        instance of the Preprocessing class needs its own instances of the id managers, in order to
-        avoid conflicts while validating data"""
-        if ":" in schema_or_id:
-            split_id_prefix = schema_or_id.split(":")
-            schema = split_id_prefix[0]
-        else:
-            schema = schema_or_id
-        id_man = id_man_dict.get(schema)
-        return id_man
-
-    def dict_to_cache(self, dict_to_be_saved, path):
-        path = Path(path)
-        parent_dir_path = path.parent.absolute()
-        if not os.path.exists(parent_dir_path):
-            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
-        with open(path, "w", encoding="utf-8") as fd:
-            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
-
-    def csv_creator(self, item:dict) -> dict:
-        """This is the method that actually creates the csv table for Meta process given an entity dictionary"""
-        doi = item["doi"]
-        if (doi and self.doi_set and doi in self.doi_set) or (doi and not self.doi_set):
-            norm_id = self.doi_m.normalise(doi, include_prefix=True)
-            title = self.get_ja(item['title_list'])[0]['title'] if 'title_list' in item else ''
-            authors_list = self.get_authors(item)
-            authors_string_list, editors_string_list = self.get_agents_strings_list(doi, authors_list)
-            issue = item['issue'] if 'issue' in item else ''
-            volume = item['volume'] if 'volume' in item else ''
-            publisher = self.get_publisher_name(item)
-
-            metadata = {
-                'id': norm_id,
-                'title': title,
-                'author': '; '.join(authors_string_list),
-                'issue': issue,
-                'volume': volume,
-                'venue': self.get_venue(item),
-                'pub_date': self.get_pub_date(item),
-                'page': self.get_jalc_pages(item),
-                'type': self.get_type(item),
-                'publisher': publisher,
-                'editor': ''
-            }
-            return self.normalise_unicode(metadata)
-
-        
-    @classmethod
-    def get_ja(cls, field: list) -> list:
-        """This method accepts as parameter a list containing dictionaries with the key "lang".
-        If a metadata is originally furnished both in the original language and in the english translation,
-        the method returns the japanese version, otherwise the english translation is returned."""
-        if all('lang' in item for item in field):
-            ja = [item for item in field if item['lang'] == 'ja']
-            ja = list(filter(lambda x: x['type'] != 'before' if 'type' in x else x, ja))
-            if ja:
-                return ja
-            en = [item for item in field if item['lang'] == 'en']
-            en = list(filter(lambda x: x['type'] != 'before' if 'type' in x else x, en))
-            if en:
-                return en
-        return field
-
-    def get_jalc_pages(self, item: dict) -> str:
-        first_page = item['first_page'] if 'first_page' in item else ''
-        last_page = item['last_page'] if 'last_page' in item else ''
-        page_list = list()
-        if first_page:
-            page_list.append(first_page)
-        if last_page:
-            page_list.append(last_page)
-        return self.get_pages(page_list)
-
-
-    def get_publisher_name(self, item: dict) -> str:
-        """This method acts differently for citing and cited entities.
-        If it processes a citing entity it simply returns a string with the name of the publisher if it has been provided in the input dictionary, giving priority to the japanese name.
-        If there is no publisher, the output is an empty string.
-        When it processes a cited entity, if a file containing a mapping of publishers' prefixes, names and crossref ids is provided, it extracts the prefix from the doi of the cited publication and checks if it is present in the mapping.
-        If yes, it returns the linked publisher's name, otherwise an empty string. """
-        if self.citing:
-            publisher = self.get_ja(item['publisher_list'])[0]['publisher_name'] if 'publisher_list' in item else ''
-        elif not self.citing and self.publishers_mapping:
-            publisher=''
-            doi = item['doi']
-            prefix = doi.split('/')[0] if doi else ""
-            if prefix:
-                if prefix in self.publishers_mapping:
-                    name = self.publishers_mapping[prefix]["name"]
-                    member = self.publishers_mapping[prefix]["crossref_member"]
-                    publisher = f'{name} [crossref:{member}]' if member else name
-        else:
-            publisher = ''
-        return publisher
-
-
-    def get_authors(self, data: dict) -> list:
-        authors = list()
-        if data.get("creator_list"):
-            creators = data.get("creator_list")
-            for c in creators:
-                agent = {"role": "author"}
-                names = c['names'] if 'names' in c else ''
-                ja_name = self.get_ja(names)[0]
-                last_name = ja_name['last_name'] if 'last_name' in ja_name else ''
-                first_name = ja_name['first_name'] if 'first_name' in ja_name else ''
-                full_name = ''
-                if last_name:
-                    full_name += last_name
-                    if first_name:
-                        full_name += f', {first_name}'
-                agent["name"] = full_name
-                agent["family"] = last_name
-                agent["given"] = first_name
-                authors.append(agent)
-        return authors
-
-    def get_venue(self, data: dict) -> str:
-        venue_name = ''
-        journal_ids = []
-        if 'journal_title_name_list' in data:
-            candidate_venues = self.get_ja(data['journal_title_name_list'])
-            if candidate_venues:
-                full_venue = [item for item in candidate_venues if 'type' in item if item['type'] == 'full']
-                if full_venue:
-                    venue_name = full_venue[0]['journal_title_name']
-                elif candidate_venues:
-                    venue_name = candidate_venues[0]['journal_title_name']
-        if 'journal_id_list' in data:
-            for v in data['journal_id_list']:
-                if isinstance(v, dict):
-                    if v.get("journal_id"):
-                        if v.get("type").lower().strip() in ["issn", "jid"]:
-                            schema = v.get("type").lower().strip()
-                            venue_id = v.get("journal_id")
-                            tmp_id_man = self.get_id_manager(schema, self.venue_tmp_id_man_dict)
-                            if tmp_id_man:
-                                norm_id = tmp_id_man.normalise(venue_id, include_prefix=True)
-                                journal_ids.append(norm_id)
-        return f"{venue_name} [{' '.join(journal_ids)}]" if journal_ids else venue_name
-
-
-    @classmethod
-    def get_type(cls, data:dict) -> str:
-        if data.get('content_type'):
-            content_type = data['content_type']
-            if content_type == 'JA':
-                br_type = 'journal article'
-            elif content_type == 'BK':
-                br_type = 'book'
-            elif content_type == 'RD':
-                br_type = 'dataset'
-            elif content_type == 'EL':
-                br_type = 'other'
-            elif content_type == 'GD':
-                br_type = 'other'
-            return br_type
-        else:
-            return ''
-    
-    @classmethod
-    def get_pub_date(cls, data) -> str:
-        pub_date_dict = data['publication_date'] if 'publication_date' in data else ''
-        pub_date_list = list()
-        year = pub_date_dict['publication_year'] if 'publication_year' in pub_date_dict else ''
-        if year:
-            pub_date_list.append(year)
-            month = pub_date_dict['publication_month'] if 'publication_month' in pub_date_dict else ''
-            if month:
-                pub_date_list.append(month)
-                day = pub_date_dict['publication_day'] if 'publication_day' in pub_date_dict else ''
-                if day:
-                    pub_date_list.append(day)
-        return '-'.join(pub_date_list)
-
-
-    def to_validated_id_list(self, norm_id):
-        """this method takes in input a normalized DOI identifier and the information of validity and returns a list valid and existent ids with prefixes.
-        For each id, a first validation try is made by checking its presence in META db. If the id is not in META db yet,
-        a second attempt is made by using the specific id-schema API"""
-
-        valid_id_list = []
-        if norm_id in self._redis_values_br:
-            self.tmp_doi_m.storage_manager.set_value(norm_id, True)
-            valid_id_list.append(norm_id)
-        # if the id is not in redis db, validate it before appending
-        elif self.tmp_doi_m.is_valid(norm_id):
-            valid_id_list.append(norm_id)
-        return valid_id_list
-
-    def memory_to_storage(self):
-        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
-        self.storage_manager.set_multi_value(kv_in_memory)
-        self.temporary_manager.delete_storage()
-
-    def extract_all_ids(self, citation, is_first_iteration: bool):
-        """Given an entity dictionary, this method extracts all the DOIs.
-        If the parameter "is_first_iteration" is True, just the DOI of the citing entity is retrieved, while
-        if it is False, all the DOIs of cited entities are extracted."""
-        '''if is_first_iteration:
-            list_id_citing = list()
-            d1_br = citation["data"]["doi"]
-            norm_id = self.doi_m.normalise(d1_br, include_prefix=True)
-            if norm_id:
-                list_id_citing.append(norm_id)
-                #for citing entities the validation is not necessary, so we add the normalized doi as valid to the temporary storage manager
-                #self.tmp_doi_m.storage_manager.set_value(norm_id, True)
-            return list_id_citing'''
-
-        if not is_first_iteration:
-            all_br = list()
-            d2_br = [x["doi"] for x in citation["data"]["citation_list"] if x.get("doi")]
-            for d in d2_br:
-                norm_id = self.doi_m.normalise(d, include_prefix=True)
-                if norm_id:
-                    all_br.append(norm_id)
-            return all_br
-
-    def get_reids_validity_list(self, id_list):
-        valid_br_ids = []
-        validity_list_br = self.BR_redis.mget(id_list)
-        for i, e in enumerate(id_list):
-            if validity_list_br[i]:
-                valid_br_ids.append(e)
-        return valid_br_ids
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from __future__ import annotations
+
+import csv
+import pathlib
+from os.path import exists
+from oc_ds_converter.pubmed.get_publishers import ExtractPublisherDOI
+
+from oc_ds_converter.oc_idmanager.doi import DOIManager
+from oc_ds_converter.oc_idmanager.issn import ISSNManager
+from oc_ds_converter.oc_idmanager.jid import JIDManager
+
+import os
+import os.path
+import json
+import re
+import warnings
+from pathlib import Path
+from typing import Optional
+
+import fakeredis
+from oc_ds_converter.datasource.redis import RedisDataSource
+from oc_ds_converter.ra_processor import RaProcessor
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+
+warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
+
+
+class JalcProcessing(RaProcessor):
+
+    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_jalc: str = None, testing: bool = True, storage_manager: Optional[StorageManager] = None, citing=True):
+        """This class is responsible for producing CSV tables to be used as input for the META process
+        aimed at ingesting data from the sources."""
+        super(JalcProcessing, self).__init__(orcid_index, doi_csv)
+        self.citing = citing
+        if storage_manager is None:
+            self.storage_manager = SqliteStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self.temporary_manager = InMemoryStorageManager('../memory.json')
+
+        self.doi_m = DOIManager(storage_manager=self.storage_manager)
+        self.issn_m = ISSNManager()
+        self.jid_m = JIDManager(storage_manager=self.storage_manager)
+
+        self.venue_id_man_dict = {"issn":self.issn_m, "jid":self.jid_m}
+
+        '''Temporary storage managers : all data must be stored in tmp storage manager and passed all together to the
+        main storage_manager only once a full file is processed. Checks must be done both on tmp and in
+        storage_manager, so that in case the process breaks while processing a file which does not complete (so
+        without writing the final file) all the data concerning the ids are not stored. Otherwise, the ids saved in
+        a storage_manager db would be considered to have been processed and thus would be ignored by the process
+        and lost.'''
+
+        self.tmp_doi_m = DOIManager(storage_manager=self.temporary_manager)
+        self.tmp_jid_m = JIDManager(storage_manager=self.temporary_manager)
+
+        self.venue_tmp_id_man_dict = {"issn":self.issn_m, "jid":self.tmp_jid_m}
+
+
+        if testing:
+            self.BR_redis = fakeredis.FakeStrictRedis()
+
+        else:
+            self.BR_redis = RedisDataSource("DB-META-BR")
+
+        self._redis_values_br = []
+
+        if not publishers_filepath_jalc:
+            self.publishers_filepath = None
+        else:
+            self.publishers_filepath = publishers_filepath_jalc
+
+            if os.path.exists(self.publishers_filepath):
+                pfp = dict()
+                csv_headers = ("id", "name", "prefix")
+                if self.publishers_filepath.endswith(".csv"):
+                    with open(self.publishers_filepath, encoding="utf8") as f:
+                        csv_reader = csv.DictReader(f, csv_headers)
+                        for row in csv_reader:
+                            pfp[row["prefix"]] = {"name": row["name"], "crossref_member": row["id"]}
+                    self.publishers_filepath = self.publishers_filepath.replace(".csv", ".json")
+                elif self.publishers_filepath.endswith(".json"):
+                    with open(self.publishers_filepath, encoding="utf8") as f:
+                        pfp = json.load(f)
+                self.publishers_mapping = pfp
+
+    def update_redis_values(self, br):
+        self._redis_values_br = br
+
+    def validated_as(self, id):
+        """Check if the validity was already retrieved and thus
+        a) if it is now saved either in the in-memory database, which only concerns data validated
+         during the current file processing;
+        b) or if it is now saved in the storage_manager database, which only concerns data validated
+        during the previous files processing.
+        In memory db is checked first because the dimension is smaller and the check is faster and
+        because we assume that it is more likely to find the same ids in close positions, e.g.: same
+        citing id in several citations with different cited ids.
+        In conclusion, if the id is found with this method, it means that this has been found in the dump we are processing"""
+        validity_value = self.tmp_doi_m.validated_as_id(id)
+        if validity_value is None:
+            validity_value = self.doi_m.validated_as_id(id)
+        return validity_value
+
+
+    def get_id_manager(self, schema_or_id, id_man_dict):
+        """Given as input the string of a schema (e.g.:'jid') and a dictionary mapping strings of
+        the schemas to their id managers, the method returns the correct id manager. Note that each
+        instance of the Preprocessing class needs its own instances of the id managers, in order to
+        avoid conflicts while validating data"""
+        if ":" in schema_or_id:
+            split_id_prefix = schema_or_id.split(":")
+            schema = split_id_prefix[0]
+        else:
+            schema = schema_or_id
+        id_man = id_man_dict.get(schema)
+        return id_man
+
+    def dict_to_cache(self, dict_to_be_saved, path):
+        path = Path(path)
+        parent_dir_path = path.parent.absolute()
+        if not os.path.exists(parent_dir_path):
+            Path(parent_dir_path).mkdir(parents=True, exist_ok=True)
+        with open(path, "w", encoding="utf-8") as fd:
+            json.dump(dict_to_be_saved, fd, ensure_ascii=False, indent=4)
+
+    def csv_creator(self, item:dict) -> dict:
+        """This is the method that actually creates the csv table for Meta process given an entity dictionary"""
+        doi = item["doi"]
+        if (doi and self.doi_set and doi in self.doi_set) or (doi and not self.doi_set):
+            norm_id = self.doi_m.normalise(doi, include_prefix=True)
+            title = self.get_ja(item['title_list'])[0]['title'] if 'title_list' in item else ''
+            authors_list = self.get_authors(item)
+            authors_string_list, editors_string_list = self.get_agents_strings_list(doi, authors_list)
+            issue = item['issue'] if 'issue' in item else ''
+            volume = item['volume'] if 'volume' in item else ''
+            publisher = self.get_publisher_name(item)
+
+            metadata = {
+                'id': norm_id,
+                'title': title,
+                'author': '; '.join(authors_string_list),
+                'issue': issue,
+                'volume': volume,
+                'venue': self.get_venue(item),
+                'pub_date': self.get_pub_date(item),
+                'page': self.get_jalc_pages(item),
+                'type': self.get_type(item),
+                'publisher': publisher,
+                'editor': ''
+            }
+            return self.normalise_unicode(metadata)
+
+        
+    @classmethod
+    def get_ja(cls, field: list) -> list:
+        """This method accepts as parameter a list containing dictionaries with the key "lang".
+        If a metadata is originally furnished both in the original language and in the english translation,
+        the method returns the japanese version, otherwise the english translation is returned."""
+        if all('lang' in item for item in field):
+            ja = [item for item in field if item['lang'] == 'ja']
+            ja = list(filter(lambda x: x['type'] != 'before' if 'type' in x else x, ja))
+            if ja:
+                return ja
+            en = [item for item in field if item['lang'] == 'en']
+            en = list(filter(lambda x: x['type'] != 'before' if 'type' in x else x, en))
+            if en:
+                return en
+        return field
+
+    def get_jalc_pages(self, item: dict) -> str:
+        first_page = item['first_page'] if 'first_page' in item else ''
+        last_page = item['last_page'] if 'last_page' in item else ''
+        page_list = list()
+        if first_page:
+            page_list.append(first_page)
+        if last_page:
+            page_list.append(last_page)
+        return self.get_pages(page_list)
+
+
+    def get_publisher_name(self, item: dict) -> str:
+        """This method acts differently for citing and cited entities.
+        If it processes a citing entity it simply returns a string with the name of the publisher if it has been provided in the input dictionary, giving priority to the japanese name.
+        If there is no publisher, the output is an empty string.
+        When it processes a cited entity, if a file containing a mapping of publishers' prefixes, names and crossref ids is provided, it extracts the prefix from the doi of the cited publication and checks if it is present in the mapping.
+        If yes, it returns the linked publisher's name, otherwise an empty string. """
+        if self.citing:
+            publisher = self.get_ja(item['publisher_list'])[0]['publisher_name'] if 'publisher_list' in item else ''
+        elif not self.citing and self.publishers_mapping:
+            publisher=''
+            doi = item['doi']
+            prefix = doi.split('/')[0] if doi else ""
+            if prefix:
+                if prefix in self.publishers_mapping:
+                    name = self.publishers_mapping[prefix]["name"]
+                    member = self.publishers_mapping[prefix]["crossref_member"]
+                    publisher = f'{name} [crossref:{member}]' if member else name
+        else:
+            publisher = ''
+        return publisher
+
+
+    def get_authors(self, data: dict) -> list:
+        authors = list()
+        if data.get("creator_list"):
+            creators = data.get("creator_list")
+            for c in creators:
+                agent = {"role": "author"}
+                names = c['names'] if 'names' in c else ''
+                ja_name = self.get_ja(names)[0]
+                last_name = ja_name['last_name'] if 'last_name' in ja_name else ''
+                first_name = ja_name['first_name'] if 'first_name' in ja_name else ''
+                full_name = ''
+                if last_name:
+                    full_name += last_name
+                    if first_name:
+                        full_name += f', {first_name}'
+                agent["name"] = full_name
+                agent["family"] = last_name
+                agent["given"] = first_name
+                authors.append(agent)
+        return authors
+
+    def get_venue(self, data: dict) -> str:
+        venue_name = ''
+        journal_ids = []
+        if 'journal_title_name_list' in data:
+            candidate_venues = self.get_ja(data['journal_title_name_list'])
+            if candidate_venues:
+                full_venue = [item for item in candidate_venues if 'type' in item if item['type'] == 'full']
+                if full_venue:
+                    venue_name = full_venue[0]['journal_title_name']
+                elif candidate_venues:
+                    venue_name = candidate_venues[0]['journal_title_name']
+        if 'journal_id_list' in data:
+            for v in data['journal_id_list']:
+                if isinstance(v, dict):
+                    if v.get("journal_id"):
+                        if v.get("type").lower().strip() in ["issn", "jid"]:
+                            schema = v.get("type").lower().strip()
+                            venue_id = v.get("journal_id")
+                            tmp_id_man = self.get_id_manager(schema, self.venue_tmp_id_man_dict)
+                            if tmp_id_man:
+                                norm_id = tmp_id_man.normalise(venue_id, include_prefix=True)
+                                journal_ids.append(norm_id)
+        return f"{venue_name} [{' '.join(journal_ids)}]" if journal_ids else venue_name
+
+
+    @classmethod
+    def get_type(cls, data:dict) -> str:
+        if data.get('content_type'):
+            content_type = data['content_type']
+            if content_type == 'JA':
+                br_type = 'journal article'
+            elif content_type == 'BK':
+                br_type = 'book'
+            elif content_type == 'RD':
+                br_type = 'dataset'
+            elif content_type == 'EL':
+                br_type = 'other'
+            elif content_type == 'GD':
+                br_type = 'other'
+            return br_type
+        else:
+            return ''
+    
+    @classmethod
+    def get_pub_date(cls, data) -> str:
+        pub_date_dict = data['publication_date'] if 'publication_date' in data else ''
+        pub_date_list = list()
+        year = pub_date_dict['publication_year'] if 'publication_year' in pub_date_dict else ''
+        if year:
+            pub_date_list.append(year)
+            month = pub_date_dict['publication_month'] if 'publication_month' in pub_date_dict else ''
+            if month:
+                pub_date_list.append(month)
+                day = pub_date_dict['publication_day'] if 'publication_day' in pub_date_dict else ''
+                if day:
+                    pub_date_list.append(day)
+        return '-'.join(pub_date_list)
+
+
+    def to_validated_id_list(self, norm_id):
+        """this method takes in input a normalized DOI identifier and the information of validity and returns a list valid and existent ids with prefixes.
+        For each id, a first validation try is made by checking its presence in META db. If the id is not in META db yet,
+        a second attempt is made by using the specific id-schema API"""
+
+        valid_id_list = []
+        if norm_id in self._redis_values_br:
+            self.tmp_doi_m.storage_manager.set_value(norm_id, True)
+            valid_id_list.append(norm_id)
+        # if the id is not in redis db, validate it before appending
+        elif self.tmp_doi_m.is_valid(norm_id):
+            valid_id_list.append(norm_id)
+        return valid_id_list
+
+    def memory_to_storage(self):
+        kv_in_memory = self.temporary_manager.get_validity_list_of_tuples()
+        self.storage_manager.set_multi_value(kv_in_memory)
+        self.temporary_manager.delete_storage()
+
+    def extract_all_ids(self, citation, is_first_iteration: bool):
+        """Given an entity dictionary, this method extracts all the DOIs.
+        If the parameter "is_first_iteration" is True, just the DOI of the citing entity is retrieved, while
+        if it is False, all the DOIs of cited entities are extracted."""
+        '''if is_first_iteration:
+            list_id_citing = list()
+            d1_br = citation["data"]["doi"]
+            norm_id = self.doi_m.normalise(d1_br, include_prefix=True)
+            if norm_id:
+                list_id_citing.append(norm_id)
+                #for citing entities the validation is not necessary, so we add the normalized doi as valid to the temporary storage manager
+                #self.tmp_doi_m.storage_manager.set_value(norm_id, True)
+            return list_id_citing'''
+
+        if not is_first_iteration:
+            all_br = list()
+            d2_br = [x["doi"] for x in citation["data"]["citation_list"] if x.get("doi")]
+            for d in d2_br:
+                norm_id = self.doi_m.normalise(d, include_prefix=True)
+                if norm_id:
+                    all_br.append(norm_id)
+            return all_br
+
+    def get_reids_validity_list(self, id_list):
+        valid_br_ids = []
+        validity_list_br = self.BR_redis.mget(id_list)
+        for i, e in enumerate(id_list):
+            if validity_list_br[i]:
+                valid_br_ids.append(e)
+        return valid_br_ids
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/lib/__init__.py` & `oc_ds_converter-1.0.1/oc_ds_converter/lib/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2019 Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
-# Copyright 2021 Simone Persiani <iosonopersia@gmail.com>
-# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2019 Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
+# Copyright 2021 Simone Persiani <iosonopersia@gmail.com>
+# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/lib/cleaner.py` & `oc_ds_converter-1.0.1/oc_ds_converter/lib/cleaner.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,400 +1,400 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2019 Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
-# Copyright 2021 Simone Persiani <iosonopersia@gmail.com>
-# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import html
-import re
-from datetime import datetime
-from typing import Tuple, Union
-
-from dateutil.parser import parse
-from oc_ds_converter.oc_idmanager import DOIManager, ISBNManager, ISSNManager, ORCIDManager
-
-from oc_ds_converter.lib.master_of_regex import *
-from oc_ds_converter.lib.master_of_regex import (invalid_vi_patterns,
-                                                 issues_valid_patterns,
-                                                 volumes_valid_patterns)
-
-
-class Cleaner:
-    def __init__(self, string:str):
-        '''
-        :params string: the string to be cleaned.
-        :type string: str
-        '''
-        self.string = string
-
-    def normalize_hyphens(self) -> str:
-        '''
-        It replaces any hyphen, dash and minus sign with a hyphen-minus character.
-        This is done for pages, IDs and dates.
-
-        .. list-table:: Comparison between the various characters similar to hyphen-minus
-            :widths: 25 25 50
-            :header-rows: 1
-
-            * - UTF-8
-                - SIGN
-                - NAME
-            * - U+002D
-                - -
-                - Hyphen-minus
-            * - U+00AD
-                - ­
-                - Soft hyphen
-            * - U+06D4
-                - ۔
-                - Arabic Full Stop
-            * - U+2010
-                - ‐
-                - Hyphen
-            * - U+2011
-                - −
-                - Non-breaking Hyphen
-            * - U+2012
-                - –
-                - Figure Dash
-            * - U+2013
-                - –
-                - En-Dash
-            * - U+2014
-                - —
-                - Em-Dash
-            * - U+2043
-                - ⁃
-                - Hyphen Bullet
-            * - U+2212
-                - −
-                - Minus Sign
-            * - U+2796
-                - ➖
-                - Heavy Minus Sign
-            * - U+2CBA
-                - Ⲻ
-                - Coptic Capital Letter Dialect-p Ni
-            * - U+FE58
-                - ﹘
-                - Small Em Dash
-
-        :returns: str -- the string with normalized hyphens
-        '''
-        string = self.string
-        wrong_characters = {'\u00AD', '\u06D4', '\u2010', '\u2011', '\u2012', '\u2013', '\u2014', '\u2043', '\u2212', '\u2796', '\u2CBA', '\uFE58'}
-        for c in wrong_characters:
-            string = string.replace(c, '\u002D')
-        if 'isbn:' in string:
-            string.replace(u'\u002D', '')
-        return string
-    
-    def normalize_spaces(self) -> str:
-        '''
-        It replaces any ambiguous spaces with a space.
-
-        .. list-table:: List of the various characters similar to the space
-            :widths: 25 25 50
-            :header-rows: 1
-
-            * - UTF-8
-                - NAME
-            * - U+0020
-                - Space
-            * - U+0009
-                - Character Tabulation
-            * - U+00A0
-                - No-break space
-            * - U+200B
-                - Zero width space
-            * - U+202F
-                - Narrow no-break space
-            * - U+2003
-                - Em Space
-            * - U+2005
-                - Four-Per-Em Space
-            * - U+2009
-                - Thin Space
-
-        :returns: str -- the string with normalized spaces
-        '''
-        string = self.string
-        wrong_characters = {'\u0009', '\u00A0', '&nbsp;', '\u200B', '\u202F', '\u2003', '\u2005', '\u2009'}
-        for c in wrong_characters:
-            string = string.replace(c, '\u0020')
-        return string
-
-    def clean_title(self) -> str:
-        '''
-        Concerning titles of bibliographic resources ('venue' and 'title' columns), 
-        every word in the title is capitalized except for those that have capitals within them 
-        (probably acronyms, e.g. 'FaBiO and CiTO'). This exception, however, does not include entirely capitalized titles. 
-        Finally, null characters and spaces are removed.
-
-        :returns: str -- The cleaned title
-        '''
-        title = self.string
-        if title.isupper():
-            title = title.lower()
-        words = title.split()
-        for i, w in enumerate(words):
-            if not any(x.isupper() for x in w):
-                words[i] = w.title()
-        new_title = ' '.join(words)
-        return new_title
-
-    def __date_parse_hack(self, date:str) -> datetime:
-        dt = parse(date, default=datetime(2001, 1, 1))
-        dt2 = parse(date, default=datetime(2002, 2, 2))
-
-        if dt.year == dt2.year and dt.month == dt2.month and dt.day == dt2.day:
-            clean_date = parse(date).strftime('%Y-%m-%d')
-        elif dt.year == dt2.year and dt.month == dt2.month:
-            clean_date = parse(date).strftime('%Y-%m')
-        elif dt.year == dt2.year:
-            clean_date = parse(date).strftime('%Y')
-        else:
-            clean_date = ''
-        return clean_date
-
-    def clean_date(self) -> str:
-        '''
-        It tries to parse a date-string into a datetime object, 
-        considering both the validity of the format (YYYYY-MM-DD) and the value (e.g. 30 February is not a valid date). 
-        For example, a date 2020-02-30 will become 2020-02, because the day is invalid. 
-        On the other hand, 2020-27-12 will become 2020 since the day
-        and month are invalid. 
-        If the year is not valid (e.g.year >9999) data would be totally discarded.
-
-        :returns: str -- The cleaned date or an empty string
-        '''
-        date = self.string
-        try:
-            date = self.__date_parse_hack(date)
-        except ValueError:
-            try:
-                # e.g. 2021-12-17
-                if len(date) == 10:
-                    try:
-                        # Maybe only the day is invalid, try year-month
-                        new_date = date[:-3]
-                        date = self.__date_parse_hack(new_date)
-                    except ValueError:
-                        try:
-                            # Maybe only the month is invalid, try year
-                            new_date = date[:-6]
-                            date = self.__date_parse_hack(new_date)
-                        except ValueError:
-                            date = ''
-                # e.g. 2021-12
-                elif len(date) == 7:
-                    # Maybe only the month is invalid, try year
-                    try:
-                        new_date = date[:-3]
-                        date = self.__date_parse_hack(new_date)
-                    except ValueError:
-                        date = ''
-                else:
-                    date = ''
-            except ValueError:
-                date = ''
-        return date
-
-    def clean_name(self) -> str:
-        '''
-        The first letter of each element of the name is capitalized and superfluous spaces are removed.
-
-        :returns: str -- The cleaned name
-        '''
-        name = self.string
-        if ',' in name:
-            split_name = re.split(comma_and_spaces, name)
-            first_name = split_name[1].split()
-            for i, w in enumerate(first_name):
-                first_name[i] = Cleaner(w).clean_title()
-            new_first_name = ' '.join(first_name)
-            surname = split_name[0].split()
-            for i, w in enumerate(surname):
-                surname[i] = Cleaner(w).clean_title()
-            new_surname = ' '.join(surname)
-            if new_surname:
-                new_name = new_surname + ', ' + new_first_name
-            else:
-                new_name = ''
-        else:
-            split_name = name.split()
-            for i, w in enumerate(split_name):
-                split_name[i] = Cleaner(w).clean_title()
-            new_name = ' '.join(split_name)
-        return new_name
-        
-    def remove_unwanted_characters(self) -> str:
-        '''
-        This method helps remove unwanted characters from authors' names. 
-        Such characters are all characters other than letters, numbers, space, '&', apostroph, or dots that are not preceded by letters. 
-        Numbers and '&' are significant if the author is an organization and not a person.
-        Finally, hyphens are normalized, Unicode encodings decoded, and extra spaces removed.
-
-        :returns: str -- The cleaned name
-        '''
-        unwanted_characters = {'[', ']', '{', '}', '(', ')', '?', ';', ','}
-        clean_string = str()
-        for i, c in enumerate(self.string):
-            if c == '.':
-                if self.string[i-1].isalpha():
-                    clean_string += c
-            elif c not in unwanted_characters:
-                clean_string += c
-        clean_string = ' '.join(clean_string.split()).strip()
-        clean_string = html.unescape(clean_string)
-        clean_string = Cleaner(clean_string).normalize_hyphens()
-        return clean_string
-    
-    @staticmethod
-    def clean_ra_list(ra_list:list) -> list:
-        '''
-        This method removes responsible agents reported as 'Not Available'.
-
-        :returns: list -- The cleaned responsible agents' list
-        '''
-        new_ra_list = list()
-        for ra in ra_list:
-            if ',' in ra:
-                split_name = re.split(comma_and_spaces, ra)
-                first_name = split_name[1] if split_name[1].lower() != 'not available' else ''
-                given_name = split_name[0] if split_name[0].lower() != 'not available' else ''
-                if given_name:
-                    if first_name:
-                        new_ra_list.append(ra)
-                    else:
-                        new_ra_list.append(f'{given_name}, ')
-                else:
-                    continue
-            else:
-                if ra.lower() != 'not available':
-                    new_ra_list.append(ra)
-        return new_ra_list
-        
-    
-    def normalize_id(self, valid_dois_cache:dict=dict()) -> Union[str, None]:
-        '''
-        This function verifies and normalizes identifiers whose schema corresponds to a DOI, an ISSN, an ISBN or an ORCID.
-
-        :returns: Union[str, None] -- The normalized identifier if it is valid, None otherwise
-        '''
-        identifier = self.string.split(':', 1)
-        schema = identifier[0].lower()
-        value = identifier[1]
-        use_api_service = True if valid_dois_cache else False
-        validator = 'is_valid' if use_api_service else 'check_digit'
-        if schema == 'doi':
-            doi_manager = DOIManager(data=valid_dois_cache, use_api_service=use_api_service)
-            valid_id = doi_manager.normalise(value, include_prefix=True) if getattr(doi_manager, validator)(value) else None
-        elif schema == 'isbn':
-            isbn_manager = ISBNManager()
-            valid_id = isbn_manager.normalise(value, include_prefix=True) if getattr(isbn_manager, validator)(value) else None
-        elif schema == 'issn':
-            if value == '0000-0000':
-                valid_id = None
-            else:
-                issn_manager = ISSNManager()
-                valid_id = issn_manager.normalise(value, include_prefix=True) if getattr(issn_manager, validator)(value) else None
-        elif schema == 'orcid':
-            orcid_manager = ORCIDManager()
-            valid_id = orcid_manager.normalise(value, include_prefix=True) if getattr(orcid_manager, validator)(value) else None
-        else:
-            valid_id = f'{schema}:{value}'
-        return valid_id
-
-    @classmethod
-    def clean_volume_and_issue(cls, row:dict) -> None:
-        output = {'volume': '', 'issue': '', 'pub_date': ''}
-        for field in {'volume', 'issue'}:
-            vi = row[field]
-            vi = Cleaner(vi).normalize_hyphens()
-            vi = Cleaner(vi).normalize_spaces().strip()
-            vi = html.unescape(vi)
-            for pattern, strategy in invalid_vi_patterns.items():
-                pattern = f'^{pattern}$'
-                capturing_groups = re.search(pattern, vi, re.IGNORECASE)
-                if capturing_groups:
-                    if strategy == 'del':
-                        row[field] = ''
-                    elif strategy == 'do_nothing':
-                        row[field] = vi
-                    elif strategy == 's)':
-                        row[field] = f'{vi}s)'
-                    else:
-                        row[field] = ''
-                        whatever, volume, issue, pub_date = cls.fix_invalid_vi(capturing_groups, strategy)
-                        row[field] = whatever if whatever else row[field]
-                        output['volume'] = volume if volume else ''
-                        output['issue'] = issue if issue else ''
-                        output['pub_date'] = pub_date if pub_date else ''
-        row['volume'] = output['volume'] if not row['volume'] else row['volume']
-        row['issue'] = output['issue'] if not row['issue'] else row['issue']
-        row['pub_date'] = output['pub_date'] if not row['pub_date'] else row['pub_date']
-        switch_vi = {'volume': '', 'issue': ''}
-        for field in {'volume', 'issue'}:
-            vi = row[field]
-            for pattern in volumes_valid_patterns:
-                pattern = f'^{pattern}$'
-                if re.search(pattern, vi, re.IGNORECASE):
-                    if field == 'issue':
-                        switch_vi['volume'] = vi
-            for pattern in issues_valid_patterns:
-                pattern = f'^{pattern}$'
-                if re.search(pattern, vi, re.IGNORECASE):
-                    if field == 'volume':
-                        switch_vi['issue'] = vi
-        if switch_vi['volume'] and switch_vi['issue']:
-            row['volume'] = switch_vi['volume']
-            row['issue'] = switch_vi['issue']
-        elif switch_vi['volume'] and not row['volume']:
-            row['volume'] = switch_vi['volume']
-            row['issue'] = ''
-            row['type'] = 'journal volume' if row['type'] == 'journal issue' else row['type']
-        elif switch_vi['issue'] and not row['issue']:
-            row['issue'] = switch_vi['issue']
-            row['volume'] = ''
-            row['type'] = 'journal issue' if row['type'] == 'journal volume' else row['type']
-    
-    @staticmethod
-    def fix_invalid_vi(capturing_groups:re.Match, strategy:str) -> Tuple[str, str, str, str]:
-        vol_group = 1 if 'vol_iss' in strategy else 2
-        iss_group = 1 if 'iss_vol' in strategy else 2
-        whatever = None
-        volume = None
-        issue = None
-        pub_date = None
-        if 'vol' in strategy and 'iss' in strategy:
-            volume = capturing_groups.group(vol_group)
-            issue = capturing_groups.group(iss_group)
-            if 'year' in strategy:
-                pub_date = capturing_groups.group(3)
-        elif strategy == 'all':
-            whatever = capturing_groups.group(1)
-        elif strategy == 'sep':
-            first = capturing_groups.group(1)
-            second = capturing_groups.group(2)
-            whatever = f'{first}-{second}'
-        return whatever, volume, issue, pub_date
-
-    def remove_ascii(self):
-        unwanted_chars = '\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f\x7f\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'
-        clean_string = ''.join([' ' if c in unwanted_chars else c for c in self.string])
-        clean_string = ' '.join(clean_string.split())
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2019 Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2019-2020 Fabio Mariani <fabio.mariani555@gmail.com>
+# Copyright 2021 Simone Persiani <iosonopersia@gmail.com>
+# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import html
+import re
+from datetime import datetime
+from typing import Tuple, Union
+
+from dateutil.parser import parse
+from oc_ds_converter.oc_idmanager import DOIManager, ISBNManager, ISSNManager, ORCIDManager
+
+from oc_ds_converter.lib.master_of_regex import *
+from oc_ds_converter.lib.master_of_regex import (invalid_vi_patterns,
+                                                 issues_valid_patterns,
+                                                 volumes_valid_patterns)
+
+
+class Cleaner:
+    def __init__(self, string:str):
+        '''
+        :params string: the string to be cleaned.
+        :type string: str
+        '''
+        self.string = string
+
+    def normalize_hyphens(self) -> str:
+        '''
+        It replaces any hyphen, dash and minus sign with a hyphen-minus character.
+        This is done for pages, IDs and dates.
+
+        .. list-table:: Comparison between the various characters similar to hyphen-minus
+            :widths: 25 25 50
+            :header-rows: 1
+
+            * - UTF-8
+                - SIGN
+                - NAME
+            * - U+002D
+                - -
+                - Hyphen-minus
+            * - U+00AD
+                - ­
+                - Soft hyphen
+            * - U+06D4
+                - ۔
+                - Arabic Full Stop
+            * - U+2010
+                - ‐
+                - Hyphen
+            * - U+2011
+                - −
+                - Non-breaking Hyphen
+            * - U+2012
+                - –
+                - Figure Dash
+            * - U+2013
+                - –
+                - En-Dash
+            * - U+2014
+                - —
+                - Em-Dash
+            * - U+2043
+                - ⁃
+                - Hyphen Bullet
+            * - U+2212
+                - −
+                - Minus Sign
+            * - U+2796
+                - ➖
+                - Heavy Minus Sign
+            * - U+2CBA
+                - Ⲻ
+                - Coptic Capital Letter Dialect-p Ni
+            * - U+FE58
+                - ﹘
+                - Small Em Dash
+
+        :returns: str -- the string with normalized hyphens
+        '''
+        string = self.string
+        wrong_characters = {'\u00AD', '\u06D4', '\u2010', '\u2011', '\u2012', '\u2013', '\u2014', '\u2043', '\u2212', '\u2796', '\u2CBA', '\uFE58'}
+        for c in wrong_characters:
+            string = string.replace(c, '\u002D')
+        if 'isbn:' in string:
+            string.replace(u'\u002D', '')
+        return string
+    
+    def normalize_spaces(self) -> str:
+        '''
+        It replaces any ambiguous spaces with a space.
+
+        .. list-table:: List of the various characters similar to the space
+            :widths: 25 25 50
+            :header-rows: 1
+
+            * - UTF-8
+                - NAME
+            * - U+0020
+                - Space
+            * - U+0009
+                - Character Tabulation
+            * - U+00A0
+                - No-break space
+            * - U+200B
+                - Zero width space
+            * - U+202F
+                - Narrow no-break space
+            * - U+2003
+                - Em Space
+            * - U+2005
+                - Four-Per-Em Space
+            * - U+2009
+                - Thin Space
+
+        :returns: str -- the string with normalized spaces
+        '''
+        string = self.string
+        wrong_characters = {'\u0009', '\u00A0', '&nbsp;', '\u200B', '\u202F', '\u2003', '\u2005', '\u2009'}
+        for c in wrong_characters:
+            string = string.replace(c, '\u0020')
+        return string
+
+    def clean_title(self) -> str:
+        '''
+        Concerning titles of bibliographic resources ('venue' and 'title' columns), 
+        every word in the title is capitalized except for those that have capitals within them 
+        (probably acronyms, e.g. 'FaBiO and CiTO'). This exception, however, does not include entirely capitalized titles. 
+        Finally, null characters and spaces are removed.
+
+        :returns: str -- The cleaned title
+        '''
+        title = self.string
+        if title.isupper():
+            title = title.lower()
+        words = title.split()
+        for i, w in enumerate(words):
+            if not any(x.isupper() for x in w):
+                words[i] = w.title()
+        new_title = ' '.join(words)
+        return new_title
+
+    def __date_parse_hack(self, date:str) -> datetime:
+        dt = parse(date, default=datetime(2001, 1, 1))
+        dt2 = parse(date, default=datetime(2002, 2, 2))
+
+        if dt.year == dt2.year and dt.month == dt2.month and dt.day == dt2.day:
+            clean_date = parse(date).strftime('%Y-%m-%d')
+        elif dt.year == dt2.year and dt.month == dt2.month:
+            clean_date = parse(date).strftime('%Y-%m')
+        elif dt.year == dt2.year:
+            clean_date = parse(date).strftime('%Y')
+        else:
+            clean_date = ''
+        return clean_date
+
+    def clean_date(self) -> str:
+        '''
+        It tries to parse a date-string into a datetime object, 
+        considering both the validity of the format (YYYYY-MM-DD) and the value (e.g. 30 February is not a valid date). 
+        For example, a date 2020-02-30 will become 2020-02, because the day is invalid. 
+        On the other hand, 2020-27-12 will become 2020 since the day
+        and month are invalid. 
+        If the year is not valid (e.g.year >9999) data would be totally discarded.
+
+        :returns: str -- The cleaned date or an empty string
+        '''
+        date = self.string
+        try:
+            date = self.__date_parse_hack(date)
+        except ValueError:
+            try:
+                # e.g. 2021-12-17
+                if len(date) == 10:
+                    try:
+                        # Maybe only the day is invalid, try year-month
+                        new_date = date[:-3]
+                        date = self.__date_parse_hack(new_date)
+                    except ValueError:
+                        try:
+                            # Maybe only the month is invalid, try year
+                            new_date = date[:-6]
+                            date = self.__date_parse_hack(new_date)
+                        except ValueError:
+                            date = ''
+                # e.g. 2021-12
+                elif len(date) == 7:
+                    # Maybe only the month is invalid, try year
+                    try:
+                        new_date = date[:-3]
+                        date = self.__date_parse_hack(new_date)
+                    except ValueError:
+                        date = ''
+                else:
+                    date = ''
+            except ValueError:
+                date = ''
+        return date
+
+    def clean_name(self) -> str:
+        '''
+        The first letter of each element of the name is capitalized and superfluous spaces are removed.
+
+        :returns: str -- The cleaned name
+        '''
+        name = self.string
+        if ',' in name:
+            split_name = re.split(comma_and_spaces, name)
+            first_name = split_name[1].split()
+            for i, w in enumerate(first_name):
+                first_name[i] = Cleaner(w).clean_title()
+            new_first_name = ' '.join(first_name)
+            surname = split_name[0].split()
+            for i, w in enumerate(surname):
+                surname[i] = Cleaner(w).clean_title()
+            new_surname = ' '.join(surname)
+            if new_surname:
+                new_name = new_surname + ', ' + new_first_name
+            else:
+                new_name = ''
+        else:
+            split_name = name.split()
+            for i, w in enumerate(split_name):
+                split_name[i] = Cleaner(w).clean_title()
+            new_name = ' '.join(split_name)
+        return new_name
+        
+    def remove_unwanted_characters(self) -> str:
+        '''
+        This method helps remove unwanted characters from authors' names. 
+        Such characters are all characters other than letters, numbers, space, '&', apostroph, or dots that are not preceded by letters. 
+        Numbers and '&' are significant if the author is an organization and not a person.
+        Finally, hyphens are normalized, Unicode encodings decoded, and extra spaces removed.
+
+        :returns: str -- The cleaned name
+        '''
+        unwanted_characters = {'[', ']', '{', '}', '(', ')', '?', ';', ','}
+        clean_string = str()
+        for i, c in enumerate(self.string):
+            if c == '.':
+                if self.string[i-1].isalpha():
+                    clean_string += c
+            elif c not in unwanted_characters:
+                clean_string += c
+        clean_string = ' '.join(clean_string.split()).strip()
+        clean_string = html.unescape(clean_string)
+        clean_string = Cleaner(clean_string).normalize_hyphens()
+        return clean_string
+    
+    @staticmethod
+    def clean_ra_list(ra_list:list) -> list:
+        '''
+        This method removes responsible agents reported as 'Not Available'.
+
+        :returns: list -- The cleaned responsible agents' list
+        '''
+        new_ra_list = list()
+        for ra in ra_list:
+            if ',' in ra:
+                split_name = re.split(comma_and_spaces, ra)
+                first_name = split_name[1] if split_name[1].lower() != 'not available' else ''
+                given_name = split_name[0] if split_name[0].lower() != 'not available' else ''
+                if given_name:
+                    if first_name:
+                        new_ra_list.append(ra)
+                    else:
+                        new_ra_list.append(f'{given_name}, ')
+                else:
+                    continue
+            else:
+                if ra.lower() != 'not available':
+                    new_ra_list.append(ra)
+        return new_ra_list
+        
+    
+    def normalize_id(self, valid_dois_cache:dict=dict()) -> Union[str, None]:
+        '''
+        This function verifies and normalizes identifiers whose schema corresponds to a DOI, an ISSN, an ISBN or an ORCID.
+
+        :returns: Union[str, None] -- The normalized identifier if it is valid, None otherwise
+        '''
+        identifier = self.string.split(':', 1)
+        schema = identifier[0].lower()
+        value = identifier[1]
+        use_api_service = True if valid_dois_cache else False
+        validator = 'is_valid' if use_api_service else 'check_digit'
+        if schema == 'doi':
+            doi_manager = DOIManager(data=valid_dois_cache, use_api_service=use_api_service)
+            valid_id = doi_manager.normalise(value, include_prefix=True) if getattr(doi_manager, validator)(value) else None
+        elif schema == 'isbn':
+            isbn_manager = ISBNManager()
+            valid_id = isbn_manager.normalise(value, include_prefix=True) if getattr(isbn_manager, validator)(value) else None
+        elif schema == 'issn':
+            if value == '0000-0000':
+                valid_id = None
+            else:
+                issn_manager = ISSNManager()
+                valid_id = issn_manager.normalise(value, include_prefix=True) if getattr(issn_manager, validator)(value) else None
+        elif schema == 'orcid':
+            orcid_manager = ORCIDManager()
+            valid_id = orcid_manager.normalise(value, include_prefix=True) if getattr(orcid_manager, validator)(value) else None
+        else:
+            valid_id = f'{schema}:{value}'
+        return valid_id
+
+    @classmethod
+    def clean_volume_and_issue(cls, row:dict) -> None:
+        output = {'volume': '', 'issue': '', 'pub_date': ''}
+        for field in {'volume', 'issue'}:
+            vi = row[field]
+            vi = Cleaner(vi).normalize_hyphens()
+            vi = Cleaner(vi).normalize_spaces().strip()
+            vi = html.unescape(vi)
+            for pattern, strategy in invalid_vi_patterns.items():
+                pattern = f'^{pattern}$'
+                capturing_groups = re.search(pattern, vi, re.IGNORECASE)
+                if capturing_groups:
+                    if strategy == 'del':
+                        row[field] = ''
+                    elif strategy == 'do_nothing':
+                        row[field] = vi
+                    elif strategy == 's)':
+                        row[field] = f'{vi}s)'
+                    else:
+                        row[field] = ''
+                        whatever, volume, issue, pub_date = cls.fix_invalid_vi(capturing_groups, strategy)
+                        row[field] = whatever if whatever else row[field]
+                        output['volume'] = volume if volume else ''
+                        output['issue'] = issue if issue else ''
+                        output['pub_date'] = pub_date if pub_date else ''
+        row['volume'] = output['volume'] if not row['volume'] else row['volume']
+        row['issue'] = output['issue'] if not row['issue'] else row['issue']
+        row['pub_date'] = output['pub_date'] if not row['pub_date'] else row['pub_date']
+        switch_vi = {'volume': '', 'issue': ''}
+        for field in {'volume', 'issue'}:
+            vi = row[field]
+            for pattern in volumes_valid_patterns:
+                pattern = f'^{pattern}$'
+                if re.search(pattern, vi, re.IGNORECASE):
+                    if field == 'issue':
+                        switch_vi['volume'] = vi
+            for pattern in issues_valid_patterns:
+                pattern = f'^{pattern}$'
+                if re.search(pattern, vi, re.IGNORECASE):
+                    if field == 'volume':
+                        switch_vi['issue'] = vi
+        if switch_vi['volume'] and switch_vi['issue']:
+            row['volume'] = switch_vi['volume']
+            row['issue'] = switch_vi['issue']
+        elif switch_vi['volume'] and not row['volume']:
+            row['volume'] = switch_vi['volume']
+            row['issue'] = ''
+            row['type'] = 'journal volume' if row['type'] == 'journal issue' else row['type']
+        elif switch_vi['issue'] and not row['issue']:
+            row['issue'] = switch_vi['issue']
+            row['volume'] = ''
+            row['type'] = 'journal issue' if row['type'] == 'journal volume' else row['type']
+    
+    @staticmethod
+    def fix_invalid_vi(capturing_groups:re.Match, strategy:str) -> Tuple[str, str, str, str]:
+        vol_group = 1 if 'vol_iss' in strategy else 2
+        iss_group = 1 if 'iss_vol' in strategy else 2
+        whatever = None
+        volume = None
+        issue = None
+        pub_date = None
+        if 'vol' in strategy and 'iss' in strategy:
+            volume = capturing_groups.group(vol_group)
+            issue = capturing_groups.group(iss_group)
+            if 'year' in strategy:
+                pub_date = capturing_groups.group(3)
+        elif strategy == 'all':
+            whatever = capturing_groups.group(1)
+        elif strategy == 'sep':
+            first = capturing_groups.group(1)
+            second = capturing_groups.group(2)
+            whatever = f'{first}-{second}'
+        return whatever, volume, issue, pub_date
+
+    def remove_ascii(self):
+        unwanted_chars = '\x00\x01\x02\x03\x04\x05\x06\x07\x08\t\n\x0b\x0c\r\x0e\x0f\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f\x7f\x80\x81\x82\x83\x84\x85\x86\x87\x88\x89\x8a\x8b\x8c\x8d\x8e\x8f\x90\x91\x92\x93\x94\x95\x96\x97\x98\x99\x9a\x9b\x9c\x9d\x9e\x9f\xa0\xa1\xa2\xa3\xa4\xa5\xa6\xa7\xa8\xa9\xaa\xab\xac\xad\xae\xaf\xb0\xb1\xb2\xb3\xb4\xb5\xb6\xb7\xb8\xb9\xba\xbb\xbc\xbd\xbe\xbf\xc0\xc1\xc2\xc3\xc4\xc5\xc6\xc7\xc8\xc9\xca\xcb\xcc\xcd\xce\xcf\xd0\xd1\xd2\xd3\xd4\xd5\xd6\xd7\xd8\xd9\xda\xdb\xdc\xdd\xde\xdf\xe0\xe1\xe2\xe3\xe4\xe5\xe6\xe7\xe8\xe9\xea\xeb\xec\xed\xee\xef\xf0\xf1\xf2\xf3\xf4\xf5\xf6\xf7\xf8\xf9\xfa\xfb\xfc\xfd\xfe\xff'
+        clean_string = ''.join([' ' if c in unwanted_chars else c for c in self.string])
+        clean_string = ' '.join(clean_string.split())
         return clean_string
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/lib/csvmanager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/lib/csvmanager.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright (c) 2019, Silvio Peroni <essepuntato@gmail.com>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-from csv import DictReader, writer
-from io import StringIO
-from os import mkdir, sep, walk
-from os.path import exists, isdir, join
-from typing import Dict
-
-
-class CSVManager(object):
-    '''
-    This class is able to load a simple CSV composed by two fields, 'id' and
-    'value', and then to index all its items in a structured form so as to be
-    easily queried. In addition, it allows one to store new information in the CSV,
-    if needed.
-    '''
-    def __init__(self, output_path:str=None, line_threshold=10000, low_memory:bool=False):
-        self.output_path = output_path
-        self.data:Dict[str, set] = {}
-        self.data_to_store = list()
-        if output_path is not None:
-            self.existing_files = self.__get_existing_files()
-            if low_memory:
-                self.__load_all_csv_files(self.existing_files, fun=self.__low_memory_load, line_threshold=line_threshold)
-            else:
-                self.__load_csv()
-    
-    def __get_existing_files(self) -> list:
-        files_to_process = []
-        if exists(self.output_path):
-            for cur_dir, _, cur_files in walk(self.output_path):
-                for cur_file in cur_files:
-                    if cur_file.endswith('.csv'):
-                        files_to_process.append(cur_dir + sep + cur_file)
-        else:
-            mkdir(self.output_path)
-        return files_to_process
-
-    @staticmethod
-    def load_csv_column_as_set(file_or_dir_path:str, key:str, line_threshold:int=10000):
-        result = set()
-        if exists(file_or_dir_path):
-            file_to_process = []
-            if isdir(file_or_dir_path):
-                for cur_dir, _, cur_files in walk(file_or_dir_path):
-                    for cur_file in cur_files:
-                        if cur_file.endswith('.csv'):
-                            file_to_process.append(cur_dir + sep + cur_file)
-            else:
-                file_to_process.append(file_or_dir_path)
-            for item in CSVManager.__load_all_csv_files(file_to_process, CSVManager.__load_csv_by_key, line_threshold=line_threshold, key=key):
-                result.update(item)
-        return result
-    
-    @staticmethod
-    def __load_csv_by_key(csv_string, key):
-        result = set()
-        csv_metadata = DictReader(StringIO(csv_string), delimiter=',')
-        for row in csv_metadata:
-            result.add(row[key])
-        return result
-
-    @staticmethod
-    def __load_all_csv_files(file_to_process, fun, line_threshold, **params):
-        result = []
-        header = None
-        for csv_path in file_to_process:
-            with open(csv_path, encoding='utf-8') as f:
-                csv_content = ''
-                for idx, line in enumerate(f.readlines()):
-                    if header is None:
-                        header = line
-                        csv_content = header
-                    else:
-                        if idx % line_threshold == 0:
-                            result.append(fun(csv_content, **params))
-                            csv_content = header
-                        csv_content += line
-            result.append(fun(csv_content, **params))
-        return result
-    
-    def dump_data(self, file_name:str) -> None:
-        path = join(self.output_path, file_name)
-        if not exists(path):
-            with open(path, 'w', encoding='utf-8', newline='') as f:
-                f.write('"id","value"\n')
-        with open(path, 'a', encoding='utf-8', newline='') as f:
-            csv_writer = writer(f, delimiter=',')
-            for el in self.data_to_store:
-                csv_writer.writerow([el[0].replace('"', '""'), el[1].replace('"', '""')])
-        self.data_to_store = list()
-
-    def get_value(self, id_string):
-        '''
-        It returns the set of values associated to the input 'id_string',
-        or None if 'id_string' is not included in the CSV.
-        '''
-        if id_string in self.data:
-            return set(self.data[id_string])
-
-    def add_value(self, id_string, value):
-        '''
-        It adds the value specified in the set of values associated to 'id_string'.
-        If the object was created with the option of storing also the data in a CSV
-        ('store_new' = True, default behaviour), then it also add new data in the CSV.
-        '''
-        self.data.setdefault(id_string, set())
-        if value not in self.data[id_string]:
-            self.data[id_string].add(value)
-            self.data_to_store.append([id_string, value])
-
-    def __load_csv(self):
-        for file in self.existing_files:
-            with open(file, 'r', encoding='utf-8') as f:
-                reader = DictReader(f)
-                for row in reader:
-                    self.data.setdefault(row['id'], set())
-                    self.data[row['id']].add(row['value'])
-    
-    def __low_memory_load(self, csv_string:str):
-        csv_metadata = DictReader(StringIO(csv_string), delimiter=',')
-        for row in csv_metadata:
-            cur_id = row['id']
-            if cur_id not in self.data:
-                self.data[cur_id] = set()
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright (c) 2019, Silvio Peroni <essepuntato@gmail.com>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+from csv import DictReader, writer
+from io import StringIO
+from os import mkdir, sep, walk
+from os.path import exists, isdir, join
+from typing import Dict
+
+
+class CSVManager(object):
+    '''
+    This class is able to load a simple CSV composed by two fields, 'id' and
+    'value', and then to index all its items in a structured form so as to be
+    easily queried. In addition, it allows one to store new information in the CSV,
+    if needed.
+    '''
+    def __init__(self, output_path:str=None, line_threshold=10000, low_memory:bool=False):
+        self.output_path = output_path
+        self.data:Dict[str, set] = {}
+        self.data_to_store = list()
+        if output_path is not None:
+            self.existing_files = self.__get_existing_files()
+            if low_memory:
+                self.__load_all_csv_files(self.existing_files, fun=self.__low_memory_load, line_threshold=line_threshold)
+            else:
+                self.__load_csv()
+    
+    def __get_existing_files(self) -> list:
+        files_to_process = []
+        if exists(self.output_path):
+            for cur_dir, _, cur_files in walk(self.output_path):
+                for cur_file in cur_files:
+                    if cur_file.endswith('.csv'):
+                        files_to_process.append(cur_dir + sep + cur_file)
+        else:
+            mkdir(self.output_path)
+        return files_to_process
+
+    @staticmethod
+    def load_csv_column_as_set(file_or_dir_path:str, key:str, line_threshold:int=10000):
+        result = set()
+        if exists(file_or_dir_path):
+            file_to_process = []
+            if isdir(file_or_dir_path):
+                for cur_dir, _, cur_files in walk(file_or_dir_path):
+                    for cur_file in cur_files:
+                        if cur_file.endswith('.csv'):
+                            file_to_process.append(cur_dir + sep + cur_file)
+            else:
+                file_to_process.append(file_or_dir_path)
+            for item in CSVManager.__load_all_csv_files(file_to_process, CSVManager.__load_csv_by_key, line_threshold=line_threshold, key=key):
+                result.update(item)
+        return result
+    
+    @staticmethod
+    def __load_csv_by_key(csv_string, key):
+        result = set()
+        csv_metadata = DictReader(StringIO(csv_string), delimiter=',')
+        for row in csv_metadata:
+            result.add(row[key])
+        return result
+
+    @staticmethod
+    def __load_all_csv_files(file_to_process, fun, line_threshold, **params):
+        result = []
+        header = None
+        for csv_path in file_to_process:
+            with open(csv_path, encoding='utf-8') as f:
+                csv_content = ''
+                for idx, line in enumerate(f.readlines()):
+                    if header is None:
+                        header = line
+                        csv_content = header
+                    else:
+                        if idx % line_threshold == 0:
+                            result.append(fun(csv_content, **params))
+                            csv_content = header
+                        csv_content += line
+            result.append(fun(csv_content, **params))
+        return result
+    
+    def dump_data(self, file_name:str) -> None:
+        path = join(self.output_path, file_name)
+        if not exists(path):
+            with open(path, 'w', encoding='utf-8', newline='') as f:
+                f.write('"id","value"\n')
+        with open(path, 'a', encoding='utf-8', newline='') as f:
+            csv_writer = writer(f, delimiter=',')
+            for el in self.data_to_store:
+                csv_writer.writerow([el[0].replace('"', '""'), el[1].replace('"', '""')])
+        self.data_to_store = list()
+
+    def get_value(self, id_string):
+        '''
+        It returns the set of values associated to the input 'id_string',
+        or None if 'id_string' is not included in the CSV.
+        '''
+        if id_string in self.data:
+            return set(self.data[id_string])
+
+    def add_value(self, id_string, value):
+        '''
+        It adds the value specified in the set of values associated to 'id_string'.
+        If the object was created with the option of storing also the data in a CSV
+        ('store_new' = True, default behaviour), then it also add new data in the CSV.
+        '''
+        self.data.setdefault(id_string, set())
+        if value not in self.data[id_string]:
+            self.data[id_string].add(value)
+            self.data_to_store.append([id_string, value])
+
+    def __load_csv(self):
+        for file in self.existing_files:
+            with open(file, 'r', encoding='utf-8') as f:
+                reader = DictReader(f)
+                for row in reader:
+                    self.data.setdefault(row['id'], set())
+                    self.data[row['id']].add(row['value'])
+    
+    def __low_memory_load(self, csv_string:str):
+        csv_metadata = DictReader(StringIO(csv_string), delimiter=',')
+        for row in csv_metadata:
+            cur_id = row['id']
+            if cur_id not in self.data:
+                self.data[cur_id] = set()
             self.data[cur_id].add(row['value'])
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/lib/file_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/lib/file_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright (c) 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from __future__ import annotations
-
-import csv
-import json
-import os
-import sys
-from contextlib import contextmanager
-from datetime import datetime
-from pathlib import Path
-from time import sleep
-from typing import Dict, List, Set
-from zipfile import ZIP_DEFLATED, ZipFile
-
-from _collections_abc import dict_keys
-from bs4 import BeautifulSoup
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-from oc_ds_converter.lib.cleaner import Cleaner
-
-
-def get_csv_data(filepath:str) -> List[Dict[str, str]]:
-    if not os.path.splitext(filepath)[1].endswith('.csv'):
-        return list()
-    field_size_changed = False
-    cur_field_size = 128
-    data = list()
-    while not data:
-        try:
-            with open(filepath, 'r', encoding='utf8') as data_initial:
-                valid_data = (Cleaner(line).normalize_spaces().replace('\0','') for line in data_initial)
-                data = list(csv.DictReader(valid_data, delimiter=','))
-        except csv.Error:
-            cur_field_size *= 2
-            csv.field_size_limit(cur_field_size)
-            field_size_changed = True
-    if field_size_changed:
-        csv.field_size_limit(128)
-    return data
-
-def pathoo(path):
-    if not os.path.isdir(os.path.dirname(path)):
-        os.makedirs(os.path.dirname(path))
-
-def write_csv(path:str, datalist:List[dict], fieldnames:list|dict_keys|None=None, method:str='w') -> None:
-    if datalist:
-        fieldnames = datalist[0].keys() if fieldnames is None else fieldnames
-        pathoo(path)
-        file_exists = os.path.isfile(path)
-        with open(path, method, newline='', encoding='utf-8') as output_file:
-            dict_writer = csv.DictWriter(f=output_file, fieldnames=fieldnames, delimiter=',', quotechar='"', quoting=csv.QUOTE_NONNUMERIC)
-            if method == 'w' or (method == 'a' and not file_exists):
-                dict_writer.writeheader()
-            dict_writer.writerows(datalist)
-
-def normalize_path(path:str) -> str:
-    normal_path = path.replace('\\', '/').replace('/', os.sep)
-    return normal_path
-
-def init_cache(cache_filepath:str|None) -> Set[str]:
-    completed = set()
-    if cache_filepath:
-        if not os.path.exists(cache_filepath):
-            pathoo(cache_filepath)
-        else:
-            with open(cache_filepath, 'r', encoding='utf-8') as cache_file:
-                completed = {line.rstrip('\n') for line in cache_file}
-    return completed
-
-@contextmanager
-def suppress_stdout():
-    with open(os.devnull, 'w') as devnull: #pragma: no cover
-        old_stdout = sys.stdout
-        sys.stdout = devnull
-        try:  
-            yield
-        finally:
-            sys.stdout = old_stdout
-
-def sort_files(files_to_be_processed:list) -> list:
-    if all(filename.replace('.csv', '').isdigit() for filename in files_to_be_processed):
-        files_to_be_processed = sorted(files_to_be_processed, key=lambda filename: int(filename.replace('.csv', '')))
-    elif all(filename.split('_')[-1].replace('.csv', '').isdigit() for filename in files_to_be_processed):
-        files_to_be_processed = sorted(files_to_be_processed, key=lambda filename: int(filename.split('_')[-1].replace('.csv', '')))
-    return files_to_be_processed
-
-def zipdir(path, ziph):
-    for root, _, files in os.walk(path):
-        for file in files:
-            ziph.write(os.path.join(root, file),
-                       os.path.relpath(os.path.join(root, file),
-                                       os.path.join(path, '..')))
-
-def zipit(dir_list:list, zip_name:str) -> None:
-    zipf = ZipFile(file=zip_name, mode='w', compression=ZIP_DEFLATED, allowZip64=True)
-    for dir in dir_list:
-        zipdir(dir, zipf)
-    zipf.close()
-
-def zip_files_in_dir(src_dir:str, dst_dir:str, replace_files:bool=False) -> None:
-    '''
-    This method zips files individually in all directories starting from a specified root directory. 
-    In other words, this function does not zip the entire folder but individual files 
-    while maintaining the folder hierarchy in the specified output directory.
-
-    :params src_dir: the source directory
-    :type src_dir: str
-    :params dst_dir: the destination directory
-    :type dst_dir: str
-    :params replace_files: True if you want to replace the original unzipped files with their zipped versions. The dafult value is False
-    :type replace_files: bool
-    :returns: None
-    '''
-    for dirpath, _, filenames in os.walk(src_dir):
-        for filename in filenames:
-            src_path = os.path.join(dirpath, filename)
-            dst_path = os.path.join(
-                dst_dir, 
-                str(Path(src_path).parent)
-                    .replace(f'{src_dir}{os.sep}', ''))
-            if not os.path.exists(dst_path):
-                os.makedirs(dst_path)
-            _, ext = os.path.splitext(filename)
-            zip_path = os.path.join(dst_path, filename).replace(ext, '.zip')
-            with ZipFile(file=zip_path, mode='w', compression=ZIP_DEFLATED, allowZip64=True) as zipf:
-                zipf.write(src_path, arcname=filename)
-            if replace_files:
-                os.remove(src_path)
-
-def unzip_files_in_dir(src_dir:str, dst_dir:str, replace_files:bool=False) -> None:
-    '''
-    This method unzips zipped files individually in all directories starting from a specified root directory. 
-    In other words, this function does not unzip the entire folder but individual files 
-    while maintaining the folder hierarchy in the specified output directory.
-
-    :params src_dir: the source directory
-    :type src_dir: str
-    :params dst_dir: the destination directory
-    :type dst_dir: str
-    :params replace_files: True if you want to replace the original zipped files with their unzipped versions, defaults to [False]
-    :type replace_files: bool
-    :returns: None
-    '''
-    for dirpath, _, filenames in os.walk(src_dir):
-        for filename in filenames:
-            if os.path.splitext(filename)[1] == '.zip':
-                src_path = os.path.join(dirpath, filename)
-                dst_path = os.path.join(
-                    dst_dir, 
-                    str(Path(src_path).parent)
-                        .replace(f'{src_dir}{os.sep}', ''))
-                if not os.path.exists(dst_path):
-                    os.makedirs(dst_path)
-                with ZipFile(file=os.path.join(dst_path, filename), mode='r') as zipf:
-                    zipf.extractall(dst_path)
-                if replace_files:
-                    os.remove(src_path)
-
-def read_zipped_json(filepath:str) -> dict|None:
-    '''
-    This method reads a zipped json file.
-
-    :params filepath: the zipped json file path
-    :type src_dir: str
-    :returns: dict -- It returns the json file as a dictionary
-    '''
-    with ZipFile(filepath, 'r') as zipf:
-        for filename in zipf.namelist(): 
-            with zipf.open(filename) as f:
-                json_data = f.read()
-                json_dict = json.loads(json_data.decode("utf-8"))
-                return json_dict
-
-def call_api(url:str, headers:str, r_format:str="json") -> dict|None:
-    tentative = 3
-    while tentative:
-        tentative -= 1
-        try:
-            r = get(url, headers=headers, timeout=30)
-            if r.status_code == 200:
-                r.encoding = "utf-8"
-                return json.loads(r.text) if r_format == "json" else BeautifulSoup(r.text, 'xml')
-            elif r.status_code == 404:
-                return None
-        except ReadTimeout:
-            # Do nothing, just try again
-            pass
-        except ConnectionError:
-            # Sleep 5 seconds, then try again
-            sleep(5)
-    return None
-
-def rm_tmp_csv_files(base_dir:str) -> None:
-    for filename in os.listdir(base_dir):
-        number = filename.split('_')[0]
-        date = datetime.strptime(filename.split('_')[1].replace('.csv', ''), '%Y-%m-%dT%H-%M-%S')
-        for other_filename in os.listdir(base_dir):
-            other_number = other_filename.split('_')[0]
-            other_date = datetime.strptime(other_filename.split('_')[1].replace('.csv', ''), '%Y-%m-%dT%H-%M-%S')
-            if number == other_number and filename != other_filename:
-                if date < other_date:
-                    os.remove(os.path.join(base_dir, filename))
-                elif other_date < date:
-                    os.remove(os.path.join(base_dir, other_filename))
-
-def chunks(lst:list, n:int) -> List[list]:
-    '''Yield successive n-sized chunks from lst.'''
-    for i in range(0, len(lst), n):
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright (c) 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from __future__ import annotations
+
+import csv
+import json
+import os
+import sys
+from contextlib import contextmanager
+from datetime import datetime
+from pathlib import Path
+from time import sleep
+from typing import Dict, List, Set
+from zipfile import ZIP_DEFLATED, ZipFile
+
+from _collections_abc import dict_keys
+from bs4 import BeautifulSoup
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+from oc_ds_converter.lib.cleaner import Cleaner
+
+
+def get_csv_data(filepath:str) -> List[Dict[str, str]]:
+    if not os.path.splitext(filepath)[1].endswith('.csv'):
+        return list()
+    field_size_changed = False
+    cur_field_size = 128
+    data = list()
+    while not data:
+        try:
+            with open(filepath, 'r', encoding='utf8') as data_initial:
+                valid_data = (Cleaner(line).normalize_spaces().replace('\0','') for line in data_initial)
+                data = list(csv.DictReader(valid_data, delimiter=','))
+        except csv.Error:
+            cur_field_size *= 2
+            csv.field_size_limit(cur_field_size)
+            field_size_changed = True
+    if field_size_changed:
+        csv.field_size_limit(128)
+    return data
+
+def pathoo(path):
+    if not os.path.isdir(os.path.dirname(path)):
+        os.makedirs(os.path.dirname(path))
+
+def write_csv(path:str, datalist:List[dict], fieldnames:list|dict_keys|None=None, method:str='w') -> None:
+    if datalist:
+        fieldnames = datalist[0].keys() if fieldnames is None else fieldnames
+        pathoo(path)
+        file_exists = os.path.isfile(path)
+        with open(path, method, newline='', encoding='utf-8') as output_file:
+            dict_writer = csv.DictWriter(f=output_file, fieldnames=fieldnames, delimiter=',', quotechar='"', quoting=csv.QUOTE_NONNUMERIC)
+            if method == 'w' or (method == 'a' and not file_exists):
+                dict_writer.writeheader()
+            dict_writer.writerows(datalist)
+
+def normalize_path(path:str) -> str:
+    normal_path = path.replace('\\', '/').replace('/', os.sep)
+    return normal_path
+
+def init_cache(cache_filepath:str|None) -> Set[str]:
+    completed = set()
+    if cache_filepath:
+        if not os.path.exists(cache_filepath):
+            pathoo(cache_filepath)
+        else:
+            with open(cache_filepath, 'r', encoding='utf-8') as cache_file:
+                completed = {line.rstrip('\n') for line in cache_file}
+    return completed
+
+@contextmanager
+def suppress_stdout():
+    with open(os.devnull, 'w') as devnull: #pragma: no cover
+        old_stdout = sys.stdout
+        sys.stdout = devnull
+        try:  
+            yield
+        finally:
+            sys.stdout = old_stdout
+
+def sort_files(files_to_be_processed:list) -> list:
+    if all(filename.replace('.csv', '').isdigit() for filename in files_to_be_processed):
+        files_to_be_processed = sorted(files_to_be_processed, key=lambda filename: int(filename.replace('.csv', '')))
+    elif all(filename.split('_')[-1].replace('.csv', '').isdigit() for filename in files_to_be_processed):
+        files_to_be_processed = sorted(files_to_be_processed, key=lambda filename: int(filename.split('_')[-1].replace('.csv', '')))
+    return files_to_be_processed
+
+def zipdir(path, ziph):
+    for root, _, files in os.walk(path):
+        for file in files:
+            ziph.write(os.path.join(root, file),
+                       os.path.relpath(os.path.join(root, file),
+                                       os.path.join(path, '..')))
+
+def zipit(dir_list:list, zip_name:str) -> None:
+    zipf = ZipFile(file=zip_name, mode='w', compression=ZIP_DEFLATED, allowZip64=True)
+    for dir in dir_list:
+        zipdir(dir, zipf)
+    zipf.close()
+
+def zip_files_in_dir(src_dir:str, dst_dir:str, replace_files:bool=False) -> None:
+    '''
+    This method zips files individually in all directories starting from a specified root directory. 
+    In other words, this function does not zip the entire folder but individual files 
+    while maintaining the folder hierarchy in the specified output directory.
+
+    :params src_dir: the source directory
+    :type src_dir: str
+    :params dst_dir: the destination directory
+    :type dst_dir: str
+    :params replace_files: True if you want to replace the original unzipped files with their zipped versions. The dafult value is False
+    :type replace_files: bool
+    :returns: None
+    '''
+    for dirpath, _, filenames in os.walk(src_dir):
+        for filename in filenames:
+            src_path = os.path.join(dirpath, filename)
+            dst_path = os.path.join(
+                dst_dir, 
+                str(Path(src_path).parent)
+                    .replace(f'{src_dir}{os.sep}', ''))
+            if not os.path.exists(dst_path):
+                os.makedirs(dst_path)
+            _, ext = os.path.splitext(filename)
+            zip_path = os.path.join(dst_path, filename).replace(ext, '.zip')
+            with ZipFile(file=zip_path, mode='w', compression=ZIP_DEFLATED, allowZip64=True) as zipf:
+                zipf.write(src_path, arcname=filename)
+            if replace_files:
+                os.remove(src_path)
+
+def unzip_files_in_dir(src_dir:str, dst_dir:str, replace_files:bool=False) -> None:
+    '''
+    This method unzips zipped files individually in all directories starting from a specified root directory. 
+    In other words, this function does not unzip the entire folder but individual files 
+    while maintaining the folder hierarchy in the specified output directory.
+
+    :params src_dir: the source directory
+    :type src_dir: str
+    :params dst_dir: the destination directory
+    :type dst_dir: str
+    :params replace_files: True if you want to replace the original zipped files with their unzipped versions, defaults to [False]
+    :type replace_files: bool
+    :returns: None
+    '''
+    for dirpath, _, filenames in os.walk(src_dir):
+        for filename in filenames:
+            if os.path.splitext(filename)[1] == '.zip':
+                src_path = os.path.join(dirpath, filename)
+                dst_path = os.path.join(
+                    dst_dir, 
+                    str(Path(src_path).parent)
+                        .replace(f'{src_dir}{os.sep}', ''))
+                if not os.path.exists(dst_path):
+                    os.makedirs(dst_path)
+                with ZipFile(file=os.path.join(dst_path, filename), mode='r') as zipf:
+                    zipf.extractall(dst_path)
+                if replace_files:
+                    os.remove(src_path)
+
+def read_zipped_json(filepath:str) -> dict|None:
+    '''
+    This method reads a zipped json file.
+
+    :params filepath: the zipped json file path
+    :type src_dir: str
+    :returns: dict -- It returns the json file as a dictionary
+    '''
+    with ZipFile(filepath, 'r') as zipf:
+        for filename in zipf.namelist(): 
+            with zipf.open(filename) as f:
+                json_data = f.read()
+                json_dict = json.loads(json_data.decode("utf-8"))
+                return json_dict
+
+def call_api(url:str, headers:str, r_format:str="json") -> dict|None:
+    tentative = 3
+    while tentative:
+        tentative -= 1
+        try:
+            r = get(url, headers=headers, timeout=30)
+            if r.status_code == 200:
+                r.encoding = "utf-8"
+                return json.loads(r.text) if r_format == "json" else BeautifulSoup(r.text, 'xml')
+            elif r.status_code == 404:
+                return None
+        except ReadTimeout:
+            # Do nothing, just try again
+            pass
+        except ConnectionError:
+            # Sleep 5 seconds, then try again
+            sleep(5)
+    return None
+
+def rm_tmp_csv_files(base_dir:str) -> None:
+    for filename in os.listdir(base_dir):
+        number = filename.split('_')[0]
+        date = datetime.strptime(filename.split('_')[1].replace('.csv', ''), '%Y-%m-%dT%H-%M-%S')
+        for other_filename in os.listdir(base_dir):
+            other_number = other_filename.split('_')[0]
+            other_date = datetime.strptime(other_filename.split('_')[1].replace('.csv', ''), '%Y-%m-%dT%H-%M-%S')
+            if number == other_number and filename != other_filename:
+                if date < other_date:
+                    os.remove(os.path.join(base_dir, filename))
+                elif other_date < date:
+                    os.remove(os.path.join(base_dir, other_filename))
+
+def chunks(lst:list, n:int) -> List[list]:
+    '''Yield successive n-sized chunks from lst.'''
+    for i in range(0, len(lst), n):
         yield lst[i:i + n]
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/lib/master_of_regex.py` & `oc_ds_converter-1.0.1/oc_ds_converter/lib/master_of_regex.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-'''
-Split by ';' outside '[]' (any spaces before and after ';').
-'''
-semicolon_in_people_field = '\s*;\s*(?=[^\]]*(?:\[|$))'
-
-'''
-It gets string inside '[]' ignoring any space between (ex: [ TARGET  ] --> TARGET).
-An id schema must be present, followed by a colon.
-Before the colon, there must be any character that is not a square bracket 
-to prevent that in strings like 'Boezaart, Andr[eacute] [omid:123]' the id captured is '[eacute] [omid:123]'.
-Alternatively, empty square brackets containing one or more spaces also represent a valid match.
-'''
-ids_inside_square_brackets = '\[\s*((?:[^\s]+:[^\s]+)?(?:\s+[^\s]+:[^\s]+)*)\s*\]'
-
-'''
-It gets the name and ids in two capturing groups.
-As for ids, it gets the string inside '[]' ignoring any space between (ex: [ TARGET  ] --> TARGET).
-An id schema must be present, followed by a colon.
-'''
-name_and_ids = f'\s*(.*?)\s*{ids_inside_square_brackets}'
-
-'''
-It captures a colon preceded and followed by zero or more spaces.
-'''
-colon_and_spaces = '\s*:\s*'
-
-'''
-It captures a colon preceded and followed by zero or more spaces.
-'''
-comma_and_spaces = '\s*,\s*'
-
-'''
-It captures one or more spaces.
-'''
-one_or_more_spaces = '\s+'
-
-'''
-It captures any pages range separator.
-'''
-pages_separator = '[^A-Za-z\d]+(?=[A-Za-z\d]+)'
-
-'''
-It captures an ORCID
-'''
-orcid_pattern = '([0-9]{4}-){3}[0-9]{3}[0-9X]'
-
-'''
-A series of patterns useful to clean invalid "volume" and "issue" fields
-'''
-good_sep = '\-'
-bad_sep = '&\/_,\.:+;\(\[\|'
-separators = good_sep + bad_sep
-alphabets = 'a-zà-öø-ÿ\u0430-я\u0391-ω' # basic latin, latin-1 supplement, cyrillic, greek
-vi_pattern = f'((?:[{alphabets}]*\d[{alphabets}\d]*|[ivxlcdm]+)(?:\s?(?:[{separators}]|and|\()\s?[{alphabets}\d]+\)?)*?)'
-numero = '(?:№|no?(?!v)\.?|n[º°]\.?|n[uú]m(?:[eé]ro)?|number)'
-year_pattern = '(\d{4})'
-valid_vi_patterns = [
-    vi_pattern,
-    f'[‹<\()]?[{alphabets}]+?([{separators}\s]?[{alphabets}])*[\)›>]?',
-    f'[{alphabets}{separators}\s]+{vi_pattern}',
-    f"[{alphabets}\d\-'/]*\d[{alphabets}\d\-'/]*(,?\s[{alphabets}\d\-'/]+)+",
-    f'\(?s(uppl([eéi]ment(ary|um)?))?\)?\s?(part)?\s?(s?{vi_pattern})?',
-    f'({vi_pattern}_)?({vi_pattern}\s)?[\(_]?supp?(plement|pl)?l?[\s\._]*({vi_pattern}|[{alphabets}])?\)?\.?',
-    f'{vi_pattern}*,?\s?part[\s_]{vi_pattern}(\sof\s{vi_pattern})?(,\sno?\.\s?{vi_pattern})?',
-    f'{vi_pattern}*[_\s]?pt?[_\s\.]{vi_pattern}',
-    '(ed|pt|d)\sinside(d|r)',
-    'p(ublish\s)?a(head\sof\s)?p(rint)?',
-    '預刊文章',
-    '[\u0621-\u064A]+',
-    f'\[{year_pattern}\]\s(\d\s)?[{alphabets}]+',
-    f'{vi_pattern}\s\[\+CDROM\]',
-    f'{vi_pattern}[{separators}\s]?\({vi_pattern}\)(\s{vi_pattern})?',
-    f'([{alphabets}]+\.)?[{alphabets}]+\.?',
-    f'[{alphabets}]+-\d+',
-    f'[{alphabets}]+(_[{alphabets}]+)+',
-    f'{numero}:?\s?{vi_pattern}(,?\s({year_pattern}|\({vi_pattern}\)))?',
-    'historica\svol\.\s\d+(,\d+(-\d+)?)?',
-    '\d+\(\d+\)\d{2,4}',
-    f'(\[{year_pattern}\]\s)?(\d+\s)?vl?r(\s\([a-z]+\))?',
-    f'\({vi_pattern}\/{vi_pattern}\)\s[{alphabets}]+(-[{alphabets}]+)?'
-]
-volumes_valid_patterns = [
-    'original\sseries,\svolume\s\d+',
-    f'(vol(ume)?|tome|cilt)\s?[{separators}]?\s?{vi_pattern}'
-]
-issues_valid_patterns = [
-    f'issue[\.,]?\s{vi_pattern}',
-    f'({vi_pattern}\s)?e?sp?e?(ecial)?[\s_\-\.](issue)?(_number_)?[\s_-]?({vi_pattern})?(["“][{alphabets}\s]+?["”])?',
-    f'ö(zel)?(\ss(ayı)?|\(special\))?(\s?{vi_pattern})?',
-    f'({numero}[{separators}\s]?)?hors[{separators}\s]série[{separators}\s]{vi_pattern}',
-    '특별호',
-    f'([{alphabets}]+\s{year_pattern}\s)?\(?(jan(uary)?|feb(ruary)?|mar(ch)?|apr(il)?|may|jun(e)?|jul(y)?|aug(ust)?|sep(tember)?|oct(ober)?|(nov|dec)(ember)?|spring|summer|autumn|winter)(\s{year_pattern})?\)?',
-    f'{vi_pattern},\spart\s{vi_pattern}\sof\s{vi_pattern}',
-    f'sayı[{separators}\s]\s?{vi_pattern}',
-    f'issues?\s{vi_pattern},\s(supplement|part)\s{vi_pattern}',
-    f'issues?\s{vi_pattern}\.?\spp\.\s[a-z\d]+[^a-z\d]+[a-z\d]+'
-]
-invalid_vi_patterns = {
-    f'.*?(?:vol\.?(?:ume)?|tome)(?:[{separators}]?\s?){vi_pattern}[\-&\/_,\.:+;\(\)\[\]|\s]*(?:{numero}|issues?)[{separators}|\s]*(?:sp[eé]cial\s)?{vi_pattern}': 'vol_iss',
-    f'{vi_pattern},\s?{numero}\s?{vi_pattern}': 'vol_iss',
-    f'tập\s?{vi_pattern},?\s?số\s?{vi_pattern}': 'vol_iss',
-    f'issues?\s{vi_pattern}\svol\.?(?:ume)?\s{vi_pattern}(?:.*?{year_pattern}.*?)?': 'iss_vol_year',
-    f"{vi_pattern}\s?\({vi_pattern}'{year_pattern}\)": 'vol_iss_year',
-    f'cilt[{separators}\s]\s?{vi_pattern}[{separators}\s]sayı[{separators}\s]\s?{vi_pattern}(?:[{separators}\s]\s?temmuz\s{year_pattern})?': 'vol_iss_year',
-    '&na;|n\/a|not\savailable': 'del',
-    '[\:\-\.`ё/]': 'del',
-    f'\${{[{alphabets}]+(\.[{alphabets}]+)?}}': 'del',
-    f"[&\/_,:+;\|`'#]\s*{vi_pattern}": 'all',
-    f'[\->+]{vi_pattern}': 'do_nothing',
-    f"{vi_pattern}[\.+]": "do_nothing",
-    f"{numero}?[{separators}]?\s?{vi_pattern}[&\/_,:;\|`'\(\[\{{]": 'all',
-    f'{vi_pattern}\(\)': 'all',
-    f'n[�?]+{vi_pattern}': 'all',
-    f'{vi_pattern}(?:â\x80[\x92\x93\x94]|�+|â|\?+){vi_pattern}': 'sep',
-    f'{vi_pattern}\s?\(first\sserie': 's)'
+'''
+Split by ';' outside '[]' (any spaces before and after ';').
+'''
+semicolon_in_people_field = '\s*;\s*(?=[^\]]*(?:\[|$))'
+
+'''
+It gets string inside '[]' ignoring any space between (ex: [ TARGET  ] --> TARGET).
+An id schema must be present, followed by a colon.
+Before the colon, there must be any character that is not a square bracket 
+to prevent that in strings like 'Boezaart, Andr[eacute] [omid:123]' the id captured is '[eacute] [omid:123]'.
+Alternatively, empty square brackets containing one or more spaces also represent a valid match.
+'''
+ids_inside_square_brackets = '\[\s*((?:[^\s]+:[^\s]+)?(?:\s+[^\s]+:[^\s]+)*)\s*\]'
+
+'''
+It gets the name and ids in two capturing groups.
+As for ids, it gets the string inside '[]' ignoring any space between (ex: [ TARGET  ] --> TARGET).
+An id schema must be present, followed by a colon.
+'''
+name_and_ids = f'\s*(.*?)\s*{ids_inside_square_brackets}'
+
+'''
+It captures a colon preceded and followed by zero or more spaces.
+'''
+colon_and_spaces = '\s*:\s*'
+
+'''
+It captures a colon preceded and followed by zero or more spaces.
+'''
+comma_and_spaces = '\s*,\s*'
+
+'''
+It captures one or more spaces.
+'''
+one_or_more_spaces = '\s+'
+
+'''
+It captures any pages range separator.
+'''
+pages_separator = '[^A-Za-z\d]+(?=[A-Za-z\d]+)'
+
+'''
+It captures an ORCID
+'''
+orcid_pattern = '([0-9]{4}-){3}[0-9]{3}[0-9X]'
+
+'''
+A series of patterns useful to clean invalid "volume" and "issue" fields
+'''
+good_sep = '\-'
+bad_sep = '&\/_,\.:+;\(\[\|'
+separators = good_sep + bad_sep
+alphabets = 'a-zà-öø-ÿ\u0430-я\u0391-ω' # basic latin, latin-1 supplement, cyrillic, greek
+vi_pattern = f'((?:[{alphabets}]*\d[{alphabets}\d]*|[ivxlcdm]+)(?:\s?(?:[{separators}]|and|\()\s?[{alphabets}\d]+\)?)*?)'
+numero = '(?:№|no?(?!v)\.?|n[º°]\.?|n[uú]m(?:[eé]ro)?|number)'
+year_pattern = '(\d{4})'
+valid_vi_patterns = [
+    vi_pattern,
+    f'[‹<\()]?[{alphabets}]+?([{separators}\s]?[{alphabets}])*[\)›>]?',
+    f'[{alphabets}{separators}\s]+{vi_pattern}',
+    f"[{alphabets}\d\-'/]*\d[{alphabets}\d\-'/]*(,?\s[{alphabets}\d\-'/]+)+",
+    f'\(?s(uppl([eéi]ment(ary|um)?))?\)?\s?(part)?\s?(s?{vi_pattern})?',
+    f'({vi_pattern}_)?({vi_pattern}\s)?[\(_]?supp?(plement|pl)?l?[\s\._]*({vi_pattern}|[{alphabets}])?\)?\.?',
+    f'{vi_pattern}*,?\s?part[\s_]{vi_pattern}(\sof\s{vi_pattern})?(,\sno?\.\s?{vi_pattern})?',
+    f'{vi_pattern}*[_\s]?pt?[_\s\.]{vi_pattern}',
+    '(ed|pt|d)\sinside(d|r)',
+    'p(ublish\s)?a(head\sof\s)?p(rint)?',
+    '預刊文章',
+    '[\u0621-\u064A]+',
+    f'\[{year_pattern}\]\s(\d\s)?[{alphabets}]+',
+    f'{vi_pattern}\s\[\+CDROM\]',
+    f'{vi_pattern}[{separators}\s]?\({vi_pattern}\)(\s{vi_pattern})?',
+    f'([{alphabets}]+\.)?[{alphabets}]+\.?',
+    f'[{alphabets}]+-\d+',
+    f'[{alphabets}]+(_[{alphabets}]+)+',
+    f'{numero}:?\s?{vi_pattern}(,?\s({year_pattern}|\({vi_pattern}\)))?',
+    'historica\svol\.\s\d+(,\d+(-\d+)?)?',
+    '\d+\(\d+\)\d{2,4}',
+    f'(\[{year_pattern}\]\s)?(\d+\s)?vl?r(\s\([a-z]+\))?',
+    f'\({vi_pattern}\/{vi_pattern}\)\s[{alphabets}]+(-[{alphabets}]+)?'
+]
+volumes_valid_patterns = [
+    'original\sseries,\svolume\s\d+',
+    f'(vol(ume)?|tome|cilt)\s?[{separators}]?\s?{vi_pattern}'
+]
+issues_valid_patterns = [
+    f'issue[\.,]?\s{vi_pattern}',
+    f'({vi_pattern}\s)?e?sp?e?(ecial)?[\s_\-\.](issue)?(_number_)?[\s_-]?({vi_pattern})?(["“][{alphabets}\s]+?["”])?',
+    f'ö(zel)?(\ss(ayı)?|\(special\))?(\s?{vi_pattern})?',
+    f'({numero}[{separators}\s]?)?hors[{separators}\s]série[{separators}\s]{vi_pattern}',
+    '특별호',
+    f'([{alphabets}]+\s{year_pattern}\s)?\(?(jan(uary)?|feb(ruary)?|mar(ch)?|apr(il)?|may|jun(e)?|jul(y)?|aug(ust)?|sep(tember)?|oct(ober)?|(nov|dec)(ember)?|spring|summer|autumn|winter)(\s{year_pattern})?\)?',
+    f'{vi_pattern},\spart\s{vi_pattern}\sof\s{vi_pattern}',
+    f'sayı[{separators}\s]\s?{vi_pattern}',
+    f'issues?\s{vi_pattern},\s(supplement|part)\s{vi_pattern}',
+    f'issues?\s{vi_pattern}\.?\spp\.\s[a-z\d]+[^a-z\d]+[a-z\d]+'
+]
+invalid_vi_patterns = {
+    f'.*?(?:vol\.?(?:ume)?|tome)(?:[{separators}]?\s?){vi_pattern}[\-&\/_,\.:+;\(\)\[\]|\s]*(?:{numero}|issues?)[{separators}|\s]*(?:sp[eé]cial\s)?{vi_pattern}': 'vol_iss',
+    f'{vi_pattern},\s?{numero}\s?{vi_pattern}': 'vol_iss',
+    f'tập\s?{vi_pattern},?\s?số\s?{vi_pattern}': 'vol_iss',
+    f'issues?\s{vi_pattern}\svol\.?(?:ume)?\s{vi_pattern}(?:.*?{year_pattern}.*?)?': 'iss_vol_year',
+    f"{vi_pattern}\s?\({vi_pattern}'{year_pattern}\)": 'vol_iss_year',
+    f'cilt[{separators}\s]\s?{vi_pattern}[{separators}\s]sayı[{separators}\s]\s?{vi_pattern}(?:[{separators}\s]\s?temmuz\s{year_pattern})?': 'vol_iss_year',
+    '&na;|n\/a|not\savailable': 'del',
+    '[\:\-\.`ё/]': 'del',
+    f'\${{[{alphabets}]+(\.[{alphabets}]+)?}}': 'del',
+    f"[&\/_,:+;\|`'#]\s*{vi_pattern}": 'all',
+    f'[\->+]{vi_pattern}': 'do_nothing',
+    f"{vi_pattern}[\.+]": "do_nothing",
+    f"{numero}?[{separators}]?\s?{vi_pattern}[&\/_,:;\|`'\(\[\{{]": 'all',
+    f'{vi_pattern}\(\)': 'all',
+    f'n[�?]+{vi_pattern}': 'all',
+    f'{vi_pattern}(?:â\x80[\x92\x93\x94]|�+|â|\?+){vi_pattern}': 'sep',
+    f'{vi_pattern}\s?\(first\sserie': 's)'
 }
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/medra/medra_processing.py` & `oc_ds_converter-1.0.1/oc_ds_converter/medra/medra_processing.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,262 +1,262 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-from datetime import datetime
-from typing import List, Tuple
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager import DOIManager, ORCIDManager
-from oc_ds_converter.lib.csvmanager import CSVManager
-
-from oc_ds_converter.ra_processor import RaProcessor
-
-
-class MedraProcessing(RaProcessor):
-    def __init__(self, orcid_index:str=None, doi_csv:str=None):
-        self.doi_set = CSVManager.load_csv_column_as_set(doi_csv, 'id') if doi_csv else None
-        orcid_index = orcid_index if orcid_index else None
-        self.orcid_index = CSVManager(orcid_index)
-        self._om = ORCIDManager()
-    
-    def csv_creator(self, xml_soup:BeautifulSoup) -> dict:
-        try:
-            br_type = self.get_br_type(xml_soup)
-        except UnboundLocalError:
-            print(xml_soup)
-            raise(UnboundLocalError)
-        metadata: dict = getattr(self, f"extract_from_{br_type.replace(' ', '_')}")(xml_soup)
-        return self.normalise_unicode(metadata)
-    
-    def extract_from_book(self, xml_soup:BeautifulSoup) -> dict:
-        ids = [self.get_id(xml_soup)]
-        ids.extend(self.get_isbn(xml_soup))
-        title = xml_soup.find('Title').find('TitleText').get_text()
-        authors, editors = self.get_contributors(xml_soup)
-        return {
-            'id': ' '.join(ids),
-            'title': title,
-            'author': '; '.join(authors),
-            'issue': '',
-            'volume': '',
-            'venue': '',
-            'pub_date': self.get_pub_date(xml_soup),
-            'pages': '',
-            'type': 'book',
-            'publisher': self.get_publisher(xml_soup),
-            'editor': '; '.join(editors)
-        }
-
-    def extract_from_book_chapter(self, xml_soup:BeautifulSoup) -> dict:
-        venue_ids = self.get_isbn(xml_soup)
-        monographic_work = xml_soup.find('MonographicWork')
-        content_item = xml_soup.find('ContentItem')
-        title_chapter = content_item.find('Title').find('TitleText').get_text()
-        title_book = monographic_work.find('Title').find('TitleText').get_text()
-        authors, editors = self.get_contributors(content_item)
-        venue_name = title_book if title_book != title_chapter else ''
-        return {
-            'id': self.get_id(xml_soup),
-            'title': title_chapter,
-            'author': '; '.join(authors),
-            'issue': '',
-            'volume': '',
-            'venue': self.build_venue_string(venue_name, venue_ids),
-            'pub_date': self.get_pub_date(xml_soup),
-            'pages': '',
-            'type': 'book chapter',
-            'publisher': self.get_publisher(xml_soup),
-            'editor': '; '.join(editors)
-        }
-
-    def extract_from_journal_article(self, xml_soup:BeautifulSoup) -> dict:
-        serial_publication = xml_soup.find('SerialPublication')
-        serial_work = serial_publication.find('SerialWork')
-        publisher_name = self.get_publisher(serial_work)
-        journal_issue = xml_soup.find('JournalIssue')
-        volume = journal_issue.find('JournalVolumeNumber')
-        volume = volume.get_text() if volume else ''
-        issue = journal_issue.find('JournalIssueNumber')
-        issue = issue.get_text() if issue else ''
-        content_item = xml_soup.find('ContentItem')
-        title = content_item.find('Title').find('TitleText').get_text()
-        authors, editors = self.get_contributors(xml_soup)
-        venue_name, venue_ids = self.get_venue(xml_soup)
-        return {
-            'id': self.get_id(xml_soup),
-            'title': title,
-            'author': '; '.join(authors),
-            'issue': issue,
-            'volume': volume,
-            'venue': self.build_venue_string(venue_name, venue_ids),
-            'pub_date': self.get_pub_date(content_item),
-            'pages': self.get_pages(content_item),
-            'type': 'journal article',
-            'publisher': publisher_name,
-            'editor': '; '.join(editors)
-        }
-    
-    def build_venue_string(self, venue_name, venue_ids):
-        if venue_name and venue_ids:
-            venue = f"{venue_name} [{' '.join(venue_ids)}]"
-        elif venue_name and not venue_ids:
-            venue = venue_name
-        elif venue_ids and not venue_name:
-            venue = f"[{' '.join(venue_ids)}]"
-        elif not venue_ids and not venue_name:
-            venue = ''
-        return venue
-
-    def extract_from_series(self, xml_soup:BeautifulSoup) -> dict:
-        venue_name, venue_ids = self.get_venue(xml_soup)
-        ids = [self.get_id(xml_soup)]
-        ids.extend(venue_ids)
-        return {
-            'id': ' '.join(ids),
-            'title': venue_name,
-            'author': '',
-            'issue': '',
-            'volume': '',
-            'venue': '',
-            'pub_date': self.get_pub_date(xml_soup),
-            'pages': '',
-            'type': 'series',
-            'publisher': self.get_publisher(xml_soup.find('SerialPublication').find('SerialWork')),
-            'editor': ''
-        }
-    
-    def get_id(self, context:BeautifulSoup) -> str:
-        doi_manager = DOIManager(use_api_service=False)
-        return doi_manager.normalise(context.find('DOI').get_text(), include_prefix=True)
-    
-    def get_isbn(self, context:BeautifulSoup) -> str:
-        product_identifiers: List[BeautifulSoup] = context.findAll('ProductIdentifier')
-        isbn_list = list()
-        if product_identifiers:
-            for product_identifier in product_identifiers:
-                if product_identifier.find('ProductIDType').get_text() in {'02', '15'}:
-                    self.isbn_worker(product_identifier.find('IDValue').get_text(), isbn_list)
-        return isbn_list
-    
-    def get_contributors(self, context:BeautifulSoup) -> Tuple[list, list]:
-        contributors:List[BeautifulSoup] = context.findAll('Contributor')
-        authors = list(); editors = list()
-        contributor_roles = {'A': authors, 'B': editors}
-        for i, contributor in enumerate(contributors):
-            contributor_role = contributor.find('ContributorRole').get_text()[0]
-            person_name_inverted = contributor.find('PersonNameInverted')
-            corporate_name = contributor.find('CorporateName')
-            person_name = contributor.find('PersonName')
-            names_before_key = contributor.find('NamesBeforeKey')
-            key_names = contributor.find('KeyNames')
-            unnamed_persons = contributor.find('UnnamedPersons')
-            if person_name_inverted:
-                author = person_name_inverted.get_text()
-            elif names_before_key and key_names:
-                author = f'{key_names.get_text()}, {names_before_key.get_text()}'
-            elif key_names and not names_before_key:
-                author = f'{key_names.get_text()},'
-            elif corporate_name:
-                author = corporate_name.get_text()
-            elif person_name:
-                author = person_name.get_text()
-            elif unnamed_persons:
-                continue
-            else:
-                raise(ValueError('No author name'))
-            is_there_name_id = contributor.find('NameIdentifier')
-            sequence_number = contributor.find('SequenceNumber')
-            sequence_number = int(sequence_number.get_text()) if sequence_number else i
-            if is_there_name_id:
-                name_id = self._om.normalise(is_there_name_id.find('IDValue').get_text(), include_prefix=True)
-                author += f' [{name_id}]'
-            contributor_roles[contributor_role].append((sequence_number, author))
-        contributor_roles = {k:[ra[1] for ra in sorted(v, key=lambda x:x[0])] for k,v in contributor_roles.items()}
-        return contributor_roles['A'], contributor_roles['B']
-    
-    def get_pub_date(self, context:BeautifulSoup) -> str:
-        raw_date = context.find('PublicationDate')
-        if not raw_date:
-            raw_date = context.find('Date')
-        if not raw_date:
-            return ''
-        raw_date = raw_date.get_text()
-        try:
-            clean_date = datetime.strptime(raw_date, '%Y%m%d').strftime('%Y-%m-%d')
-        except ValueError:
-            try:
-                clean_date = datetime.strptime(raw_date, '%Y%m').strftime('%Y-%m')
-            except ValueError:
-                clean_date = datetime.strptime(raw_date, '%Y').strftime('%Y')
-        return clean_date
-
-    def get_pages(self, context:BeautifulSoup) -> str:
-        page_run = context.find('PageRun')
-        if page_run:
-            starting_page = page_run.find('FirstPageNumber')
-            ending_page = page_run.find('LastPageNumber')
-            starting_page = starting_page.get_text() if starting_page else None
-            ending_page = ending_page.get_text() if ending_page else None
-            if starting_page and '-' in starting_page:
-                starting_page = f'"{starting_page}"'
-            if ending_page and '-' in ending_page:
-                ending_page = f'"{ending_page}"'
-            pages = f'{starting_page}-{ending_page}' if starting_page and ending_page else starting_page if starting_page else ''
-        else:
-            pages = ''
-        return pages
-    
-    def get_publisher(self, context:BeautifulSoup) -> str:
-        publisher = context.find('Publisher')
-        if publisher:
-            publisher_name = publisher.find('PublisherName')
-            if publisher:
-                return publisher_name.get_text()
-        return ''
-    
-    def get_venue(self, context:BeautifulSoup) -> str:
-        serial_publication = context.find('SerialPublication')
-        serial_work = serial_publication.find('SerialWork')
-        serial_work_titles:List[BeautifulSoup] = serial_work.findAll('Title')
-        venue_name = None
-        for serial_work_title in serial_work_titles:
-            if serial_work_title.find('TitleType').get_text() == '01':
-                venue_name = serial_work_title.find('TitleText').get_text()
-            elif serial_work_title.find('TitleType').get_text() == '05':
-                venue_name = serial_work_title.find('TitleText').get_text()
-        serial_versions:List[BeautifulSoup] = serial_publication.findAll('SerialVersion')
-        venue_ids = list()
-        for serial_version in serial_versions:
-            product_id_type = serial_version.find('ProductIDType')
-            if serial_version.find('ProductForm').get_text() in {'JD', 'JB'} and product_id_type:
-                if product_id_type.get_text() == '07':
-                    id_value = serial_version.find('IDValue').get_text()
-                    id_value = id_value + 'X' if len(id_value) == 7 else id_value
-                    self.issn_worker(id_value, venue_ids)
-        return venue_name, venue_ids
-    
-    @classmethod
-    def get_br_type(cls, xml_soup:BeautifulSoup) -> str:
-        if xml_soup.find('DOIMonographicProduct') or xml_soup.find('DOIMonographicWork'):
-            br_type = 'book'
-        elif xml_soup.find('DOIMonographChapterWork') or xml_soup.find('DOIMonographChapterVersion'):
-            br_type = 'book chapter'
-        elif xml_soup.find('DOISerialArticleWork') or xml_soup.find('DOISerialArticleVersion'):
-            br_type = 'journal article'
-        elif xml_soup.find('DOISerialIssueWork'):
-            br_type = 'journal issue'
-        elif xml_soup.find('DOISerialTitleWork'):
-            br_type = 'series'
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+from datetime import datetime
+from typing import List, Tuple
+
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager import DOIManager, ORCIDManager
+from oc_ds_converter.lib.csvmanager import CSVManager
+
+from oc_ds_converter.ra_processor import RaProcessor
+
+
+class MedraProcessing(RaProcessor):
+    def __init__(self, orcid_index:str=None, doi_csv:str=None):
+        self.doi_set = CSVManager.load_csv_column_as_set(doi_csv, 'id') if doi_csv else None
+        orcid_index = orcid_index if orcid_index else None
+        self.orcid_index = CSVManager(orcid_index)
+        self._om = ORCIDManager()
+    
+    def csv_creator(self, xml_soup:BeautifulSoup) -> dict:
+        try:
+            br_type = self.get_br_type(xml_soup)
+        except UnboundLocalError:
+            print(xml_soup)
+            raise(UnboundLocalError)
+        metadata: dict = getattr(self, f"extract_from_{br_type.replace(' ', '_')}")(xml_soup)
+        return self.normalise_unicode(metadata)
+    
+    def extract_from_book(self, xml_soup:BeautifulSoup) -> dict:
+        ids = [self.get_id(xml_soup)]
+        ids.extend(self.get_isbn(xml_soup))
+        title = xml_soup.find('Title').find('TitleText').get_text()
+        authors, editors = self.get_contributors(xml_soup)
+        return {
+            'id': ' '.join(ids),
+            'title': title,
+            'author': '; '.join(authors),
+            'issue': '',
+            'volume': '',
+            'venue': '',
+            'pub_date': self.get_pub_date(xml_soup),
+            'pages': '',
+            'type': 'book',
+            'publisher': self.get_publisher(xml_soup),
+            'editor': '; '.join(editors)
+        }
+
+    def extract_from_book_chapter(self, xml_soup:BeautifulSoup) -> dict:
+        venue_ids = self.get_isbn(xml_soup)
+        monographic_work = xml_soup.find('MonographicWork')
+        content_item = xml_soup.find('ContentItem')
+        title_chapter = content_item.find('Title').find('TitleText').get_text()
+        title_book = monographic_work.find('Title').find('TitleText').get_text()
+        authors, editors = self.get_contributors(content_item)
+        venue_name = title_book if title_book != title_chapter else ''
+        return {
+            'id': self.get_id(xml_soup),
+            'title': title_chapter,
+            'author': '; '.join(authors),
+            'issue': '',
+            'volume': '',
+            'venue': self.build_venue_string(venue_name, venue_ids),
+            'pub_date': self.get_pub_date(xml_soup),
+            'pages': '',
+            'type': 'book chapter',
+            'publisher': self.get_publisher(xml_soup),
+            'editor': '; '.join(editors)
+        }
+
+    def extract_from_journal_article(self, xml_soup:BeautifulSoup) -> dict:
+        serial_publication = xml_soup.find('SerialPublication')
+        serial_work = serial_publication.find('SerialWork')
+        publisher_name = self.get_publisher(serial_work)
+        journal_issue = xml_soup.find('JournalIssue')
+        volume = journal_issue.find('JournalVolumeNumber')
+        volume = volume.get_text() if volume else ''
+        issue = journal_issue.find('JournalIssueNumber')
+        issue = issue.get_text() if issue else ''
+        content_item = xml_soup.find('ContentItem')
+        title = content_item.find('Title').find('TitleText').get_text()
+        authors, editors = self.get_contributors(xml_soup)
+        venue_name, venue_ids = self.get_venue(xml_soup)
+        return {
+            'id': self.get_id(xml_soup),
+            'title': title,
+            'author': '; '.join(authors),
+            'issue': issue,
+            'volume': volume,
+            'venue': self.build_venue_string(venue_name, venue_ids),
+            'pub_date': self.get_pub_date(content_item),
+            'pages': self.get_pages(content_item),
+            'type': 'journal article',
+            'publisher': publisher_name,
+            'editor': '; '.join(editors)
+        }
+    
+    def build_venue_string(self, venue_name, venue_ids):
+        if venue_name and venue_ids:
+            venue = f"{venue_name} [{' '.join(venue_ids)}]"
+        elif venue_name and not venue_ids:
+            venue = venue_name
+        elif venue_ids and not venue_name:
+            venue = f"[{' '.join(venue_ids)}]"
+        elif not venue_ids and not venue_name:
+            venue = ''
+        return venue
+
+    def extract_from_series(self, xml_soup:BeautifulSoup) -> dict:
+        venue_name, venue_ids = self.get_venue(xml_soup)
+        ids = [self.get_id(xml_soup)]
+        ids.extend(venue_ids)
+        return {
+            'id': ' '.join(ids),
+            'title': venue_name,
+            'author': '',
+            'issue': '',
+            'volume': '',
+            'venue': '',
+            'pub_date': self.get_pub_date(xml_soup),
+            'pages': '',
+            'type': 'series',
+            'publisher': self.get_publisher(xml_soup.find('SerialPublication').find('SerialWork')),
+            'editor': ''
+        }
+    
+    def get_id(self, context:BeautifulSoup) -> str:
+        doi_manager = DOIManager(use_api_service=False)
+        return doi_manager.normalise(context.find('DOI').get_text(), include_prefix=True)
+    
+    def get_isbn(self, context:BeautifulSoup) -> str:
+        product_identifiers: List[BeautifulSoup] = context.findAll('ProductIdentifier')
+        isbn_list = list()
+        if product_identifiers:
+            for product_identifier in product_identifiers:
+                if product_identifier.find('ProductIDType').get_text() in {'02', '15'}:
+                    self.isbn_worker(product_identifier.find('IDValue').get_text(), isbn_list)
+        return isbn_list
+    
+    def get_contributors(self, context:BeautifulSoup) -> Tuple[list, list]:
+        contributors:List[BeautifulSoup] = context.findAll('Contributor')
+        authors = list(); editors = list()
+        contributor_roles = {'A': authors, 'B': editors}
+        for i, contributor in enumerate(contributors):
+            contributor_role = contributor.find('ContributorRole').get_text()[0]
+            person_name_inverted = contributor.find('PersonNameInverted')
+            corporate_name = contributor.find('CorporateName')
+            person_name = contributor.find('PersonName')
+            names_before_key = contributor.find('NamesBeforeKey')
+            key_names = contributor.find('KeyNames')
+            unnamed_persons = contributor.find('UnnamedPersons')
+            if person_name_inverted:
+                author = person_name_inverted.get_text()
+            elif names_before_key and key_names:
+                author = f'{key_names.get_text()}, {names_before_key.get_text()}'
+            elif key_names and not names_before_key:
+                author = f'{key_names.get_text()},'
+            elif corporate_name:
+                author = corporate_name.get_text()
+            elif person_name:
+                author = person_name.get_text()
+            elif unnamed_persons:
+                continue
+            else:
+                raise(ValueError('No author name'))
+            is_there_name_id = contributor.find('NameIdentifier')
+            sequence_number = contributor.find('SequenceNumber')
+            sequence_number = int(sequence_number.get_text()) if sequence_number else i
+            if is_there_name_id:
+                name_id = self._om.normalise(is_there_name_id.find('IDValue').get_text(), include_prefix=True)
+                author += f' [{name_id}]'
+            contributor_roles[contributor_role].append((sequence_number, author))
+        contributor_roles = {k:[ra[1] for ra in sorted(v, key=lambda x:x[0])] for k,v in contributor_roles.items()}
+        return contributor_roles['A'], contributor_roles['B']
+    
+    def get_pub_date(self, context:BeautifulSoup) -> str:
+        raw_date = context.find('PublicationDate')
+        if not raw_date:
+            raw_date = context.find('Date')
+        if not raw_date:
+            return ''
+        raw_date = raw_date.get_text()
+        try:
+            clean_date = datetime.strptime(raw_date, '%Y%m%d').strftime('%Y-%m-%d')
+        except ValueError:
+            try:
+                clean_date = datetime.strptime(raw_date, '%Y%m').strftime('%Y-%m')
+            except ValueError:
+                clean_date = datetime.strptime(raw_date, '%Y').strftime('%Y')
+        return clean_date
+
+    def get_pages(self, context:BeautifulSoup) -> str:
+        page_run = context.find('PageRun')
+        if page_run:
+            starting_page = page_run.find('FirstPageNumber')
+            ending_page = page_run.find('LastPageNumber')
+            starting_page = starting_page.get_text() if starting_page else None
+            ending_page = ending_page.get_text() if ending_page else None
+            if starting_page and '-' in starting_page:
+                starting_page = f'"{starting_page}"'
+            if ending_page and '-' in ending_page:
+                ending_page = f'"{ending_page}"'
+            pages = f'{starting_page}-{ending_page}' if starting_page and ending_page else starting_page if starting_page else ''
+        else:
+            pages = ''
+        return pages
+    
+    def get_publisher(self, context:BeautifulSoup) -> str:
+        publisher = context.find('Publisher')
+        if publisher:
+            publisher_name = publisher.find('PublisherName')
+            if publisher:
+                return publisher_name.get_text()
+        return ''
+    
+    def get_venue(self, context:BeautifulSoup) -> str:
+        serial_publication = context.find('SerialPublication')
+        serial_work = serial_publication.find('SerialWork')
+        serial_work_titles:List[BeautifulSoup] = serial_work.findAll('Title')
+        venue_name = None
+        for serial_work_title in serial_work_titles:
+            if serial_work_title.find('TitleType').get_text() == '01':
+                venue_name = serial_work_title.find('TitleText').get_text()
+            elif serial_work_title.find('TitleType').get_text() == '05':
+                venue_name = serial_work_title.find('TitleText').get_text()
+        serial_versions:List[BeautifulSoup] = serial_publication.findAll('SerialVersion')
+        venue_ids = list()
+        for serial_version in serial_versions:
+            product_id_type = serial_version.find('ProductIDType')
+            if serial_version.find('ProductForm').get_text() in {'JD', 'JB'} and product_id_type:
+                if product_id_type.get_text() == '07':
+                    id_value = serial_version.find('IDValue').get_text()
+                    id_value = id_value + 'X' if len(id_value) == 7 else id_value
+                    self.issn_worker(id_value, venue_ids)
+        return venue_name, venue_ids
+    
+    @classmethod
+    def get_br_type(cls, xml_soup:BeautifulSoup) -> str:
+        if xml_soup.find('DOIMonographicProduct') or xml_soup.find('DOIMonographicWork'):
+            br_type = 'book'
+        elif xml_soup.find('DOIMonographChapterWork') or xml_soup.find('DOIMonographChapterVersion'):
+            br_type = 'book chapter'
+        elif xml_soup.find('DOISerialArticleWork') or xml_soup.find('DOISerialArticleVersion'):
+            br_type = 'journal article'
+        elif xml_soup.find('DOISerialIssueWork'):
+            br_type = 'journal issue'
+        elif xml_soup.find('DOISerialTitleWork'):
+            br_type = 'series'
         return br_type
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/metadata_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/metadata_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-#!python
-# Copyright 2022, Arianna Moretti <arianna.moretti4@unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import importlib
-from urllib.parse import quote
-
-from oc_ds_converter.oc_idmanager.isbn import ISBNManager
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
-
-
-class MetadataManager():
-    def __init__(self, metadata_provider:str, api_response:dict, orcid_doi_filepath:str):
-        self.metadata_provider = metadata_provider
-        self.api_response = api_response
-        self.orcid_doi_filepath = orcid_doi_filepath
-        self._issnm = ISSNManager()
-        self._isbnm = ISBNManager()
-        self._om = ORCIDManager()
-        from oc_ds_converter.oc_idmanager.doi import DOIManager
-        self.doi_manager = DOIManager()
-        self._have_api = ['crossref', 'datacite', 'medra', 'jalc']
-
-    def extract_metadata(self) -> None:
-        metadata = {'ra': self.metadata_provider}
-        if self.metadata_provider is None or self.api_response is None:
-            return metadata
-        if self.metadata_provider == 'unknown':
-            return self.extract_from_unknown()
-        elif self.metadata_provider in self._have_api:
-            module = importlib.import_module(f'oc_ds_converter.{self.metadata_provider}.{self.metadata_provider}_processing')
-            class_ = getattr(module, f'{self.metadata_provider.title()}Processing')
-            metadata_processor = class_(orcid_index=self.orcid_doi_filepath)
-            api_response = self.api_response['data'] if self.metadata_provider == 'datacite' else self.api_response
-            metadata.update(getattr(metadata_processor, 'csv_creator')(api_response))                
-        return metadata
-
-    def extract_from_unknown(self) -> None:
-        metadata = dict()
-        api_response: dict = self.api_response[0]
-        if api_response.get('status') == 'Error':
-            metadata['ra'] = 'unknown'
-            return metadata
-        elif api_response.get('status') == 'DOI does not exist':
-            metadata['ra'] = 'invalid'
-            return metadata
-        registration_agency = self.api_response[0]['RA'].lower()
-        metadata['ra'] = registration_agency
-        doi = self.api_response[0]['DOI']
-        api_registration_agency = getattr(self.doi_manager, f'_api_{registration_agency}')
-        if api_registration_agency:
-            from oc_ds_converter.lib.file_manager import call_api
-            url = api_registration_agency + quote(doi)
-            r_format = 'xml' if registration_agency == 'medra' else 'json'
-            extra_api_result = call_api(url=url, headers=self.doi_manager._headers, r_format=r_format)
-            self.metadata_provider = registration_agency
-            self.api_response = extra_api_result
-            try:
-                metadata.update(self.extract_metadata())
-            except Exception as e:
-                print(doi, registration_agency)
-                print(e)
-                raise(Exception)
+#!python
+# Copyright 2022, Arianna Moretti <arianna.moretti4@unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import importlib
+from urllib.parse import quote
+
+from oc_ds_converter.oc_idmanager.isbn import ISBNManager
+from oc_ds_converter.oc_idmanager.issn import ISSNManager
+from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
+
+
+class MetadataManager():
+    def __init__(self, metadata_provider:str, api_response:dict, orcid_doi_filepath:str):
+        self.metadata_provider = metadata_provider
+        self.api_response = api_response
+        self.orcid_doi_filepath = orcid_doi_filepath
+        self._issnm = ISSNManager()
+        self._isbnm = ISBNManager()
+        self._om = ORCIDManager()
+        from oc_ds_converter.oc_idmanager.doi import DOIManager
+        self.doi_manager = DOIManager()
+        self._have_api = ['crossref', 'datacite', 'medra', 'jalc']
+
+    def extract_metadata(self) -> None:
+        metadata = {'ra': self.metadata_provider}
+        if self.metadata_provider is None or self.api_response is None:
+            return metadata
+        if self.metadata_provider == 'unknown':
+            return self.extract_from_unknown()
+        elif self.metadata_provider in self._have_api:
+            module = importlib.import_module(f'oc_ds_converter.{self.metadata_provider}.{self.metadata_provider}_processing')
+            class_ = getattr(module, f'{self.metadata_provider.title()}Processing')
+            metadata_processor = class_(orcid_index=self.orcid_doi_filepath)
+            api_response = self.api_response['data'] if self.metadata_provider == 'datacite' else self.api_response
+            metadata.update(getattr(metadata_processor, 'csv_creator')(api_response))                
+        return metadata
+
+    def extract_from_unknown(self) -> None:
+        metadata = dict()
+        api_response: dict = self.api_response[0]
+        if api_response.get('status') == 'Error':
+            metadata['ra'] = 'unknown'
+            return metadata
+        elif api_response.get('status') == 'DOI does not exist':
+            metadata['ra'] = 'invalid'
+            return metadata
+        registration_agency = self.api_response[0]['RA'].lower()
+        metadata['ra'] = registration_agency
+        doi = self.api_response[0]['DOI']
+        api_registration_agency = getattr(self.doi_manager, f'_api_{registration_agency}')
+        if api_registration_agency:
+            from oc_ds_converter.lib.file_manager import call_api
+            url = api_registration_agency + quote(doi)
+            r_format = 'xml' if registration_agency == 'medra' else 'json'
+            extra_api_result = call_api(url=url, headers=self.doi_manager._headers, r_format=r_format)
+            self.metadata_provider = registration_agency
+            self.api_response = extra_api_result
+            try:
+                metadata.update(self.extract_metadata())
+            except Exception as e:
+                print(doi, registration_agency)
+                print(e)
+                raise(Exception)
         return metadata
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/arxiv.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/arxiv.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from re import compile, match, search
-from time import sleep
-from urllib.parse import quote, unquote
-
-import xmltodict
-from oc_ds_converter.oc_idmanager import *
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Optional, Type, Callable
-
-
-class ArXivManager(IdentifierManager):
-    """This class implements an identifier manager for arxiv identifier"""
-
-    def __init__(self, use_api_service=True, storage_manager:Optional[StorageManager] = None):
-        """arxiv manager constructor."""
-        super(ArXivManager,self).__init__()
-        self._use_api_service = use_api_service
-        if storage_manager is None:
-            self.storage_manager = InMemoryStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self._p = "arxiv:"
-        self._api = f'https://export.arxiv.org/api/query?search_query=all:'
-        self._api_v = f'https://arxiv.org/abs/'
-        self._headers = {
-            "User-Agent": "Identifier Manager / OpenCitations Indexes "
-                          "(http://opencitations.net; mailto:contact@opencitations.net)"
-        }
-
-
-    def validated_as_id(self, id_string):
-        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
-        if isinstance(arxiv_vaidation_value, bool):
-            return arxiv_vaidation_value
-        else:
-            return None
-
-    def is_valid(self, id_string, get_extra_info=False):
-        """Check if an arxiv is valid.
-
-        Args:
-            id_string (str): the arxiv to check
-
-        Returns:
-            bool: true if the arxiv is valid, false otherwise.
-        """
-
-        arxiv = self.normalise(id_string, include_prefix=True)
-        if not arxiv:
-            return False
-        else:
-            arxiv_vaidation_value = self.storage_manager.get_value(arxiv)
-            if isinstance(arxiv_vaidation_value, bool):
-
-                if get_extra_info:
-                    return arxiv_vaidation_value, {"id":arxiv, "valid":arxiv_vaidation_value}
-                return arxiv_vaidation_value
-            else:
-                if get_extra_info:
-                    info = self.exists(arxiv, get_extra_info=True)
-                    self.storage_manager.set_full_value(arxiv,info[1])
-                    return (info[0] and self.syntax_ok(arxiv)), info[1]
-                validity_check = self.exists(arxiv) and self.syntax_ok(arxiv)
-                self.storage_manager.set_value(arxiv, validity_check)
-
-                return validity_check
-
-    def normalise(self, id_string, include_prefix=False):
-        """It returns the arxiv normalized.
-
-        Args:
-            id_string (str): the arxiv to normalize.
-            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
-
-        Returns:
-            str: the normalized arxiv
-        """
-        regex = compile(r'[^0-9v.]')
-        regexdot = compile(r'\.+')
-        reg_api = compile(r'(https?://export\.arxiv\.org/api/query\?search_query=all:)')
-        reg_v_api = compile(r'(https?://arxiv\.org/abs/)')
-        reg_v_extrachar = compile(r'\/?ar[Xx]iv\.?')
-
-        if id_string:
-            id_string = str(id_string).strip().lower()
-
-            if id_string.startswith(self._p):
-                skip_char = len(self._p)
-                id_string = id_string[skip_char:]
-
-            id_string = regexdot.sub('.', id_string)
-            id_string = reg_v_api.sub('', id_string)
-            id_string = reg_api.sub('', id_string)
-            id_string = regex.sub('', id_string)
-            id_string = reg_v_extrachar.sub('', id_string)
-
-            # First parameter is the replacement, second parameter is your input string
-
-            try:
-                id_string = unquote(id_string)
-                arxiv_string = search("(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)", id_string).group(0)
-
-                return "%s%s" % (self._p if include_prefix else "", arxiv_string)
-            except:
-                try:
-                    id_string = unquote(id_string)
-                    arxiv_string = search("(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)?", id_string).group(0)
-                    return "%s%s" % (self._p if include_prefix else "", arxiv_string+"v1")
-                except:
-                    return None
-
-        else:
-            return None
-
-    def syntax_ok(self, id_string):
-        if not id_string.startswith(self._p):
-            id_string = self._p + id_string
-        return True if match("arxiv:(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)?$", id_string) else False
-
-
-    def exists(self, arxiv_full, get_extra_info=False, allow_extra_api=None):
-        """
-        Returns True if the id exists, False otherwise. Not all child class check id existence because of API policies
-        Args:
-            arxiv_full (str): the arxiv string for the api request
-        Returns:
-            bool: True if the arxiv exists (is registered), False otherwise.
-        """
-        valid_bool = True
-        if self._use_api_service:
-            arxiv_full_norm = self.normalise(arxiv_full, include_prefix=False)
-            if arxiv_full_norm:
-                version = ""
-                arxiv_string_match = search("(v\d+)$", arxiv_full_norm)
-                if arxiv_string_match:
-                    version = arxiv_string_match[1]
-
-                if version and version != "v1":
-                    api = self._api_v
-                else:
-                    if version == "v1":
-                        # v1 always exists, and the base API is more efficient,
-                        # so we just check the existence of the base ARXIV id
-                        arxiv_full_norm = arxiv_full_norm[:-2]
-
-                    api = self._api
-
-
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(
-                            api + quote(arxiv_full_norm),
-                            headers=self._headers,
-                            timeout=30,
-                        )
-                        if r.status_code == 200:
-                            if not version or version =="v1":
-                                #data = r.decode('utf-8').text
-                                xml_re = r.text
-                                obj = xmltodict.parse(f'{xml_re}')
-                                feed = obj.get("feed")
-                                results = feed.get("opensearch:totalResults")
-                                try:
-                                    results_n = int(results.get("#text"))
-                                except:
-                                    results_n = 0
-
-                                if results_n >0:
-                                    if get_extra_info:
-                                        return True, self.extra_info(obj)
-                                    return True
-                                else:
-                                    if get_extra_info:
-                                        return False, {"valid": False}
-                                    return False
-                            else:
-                                if get_extra_info:
-                                    return True, {"valid": True}
-                                return True
-                        else:
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-                valid_bool = False
-            else:
-                if get_extra_info:
-                    return False, {"valid": False}
-                return False
-        if get_extra_info:
-            return valid_bool, {"valid": valid_bool}
-        return valid_bool
-
-
-    def extra_info(self, api_response, choose_api=None, info_dict:dict={}):
-        result = {}
-        result["valid"] = True
-        # to be implemented
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from re import compile, match, search
+from time import sleep
+from urllib.parse import quote, unquote
+
+import xmltodict
+from oc_ds_converter.oc_idmanager import *
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+from typing import Optional, Type, Callable
+
+
+class ArXivManager(IdentifierManager):
+    """This class implements an identifier manager for arxiv identifier"""
+
+    def __init__(self, use_api_service=True, storage_manager:Optional[StorageManager] = None):
+        """arxiv manager constructor."""
+        super(ArXivManager,self).__init__()
+        self._use_api_service = use_api_service
+        if storage_manager is None:
+            self.storage_manager = InMemoryStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self._p = "arxiv:"
+        self._api = f'https://export.arxiv.org/api/query?search_query=all:'
+        self._api_v = f'https://arxiv.org/abs/'
+        self._headers = {
+            "User-Agent": "Identifier Manager / OpenCitations Indexes "
+                          "(http://opencitations.net; mailto:contact@opencitations.net)"
+        }
+
+
+    def validated_as_id(self, id_string):
+        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
+        if isinstance(arxiv_vaidation_value, bool):
+            return arxiv_vaidation_value
+        else:
+            return None
+
+    def is_valid(self, id_string, get_extra_info=False):
+        """Check if an arxiv is valid.
+
+        Args:
+            id_string (str): the arxiv to check
+
+        Returns:
+            bool: true if the arxiv is valid, false otherwise.
+        """
+
+        arxiv = self.normalise(id_string, include_prefix=True)
+        if not arxiv:
+            return False
+        else:
+            arxiv_vaidation_value = self.storage_manager.get_value(arxiv)
+            if isinstance(arxiv_vaidation_value, bool):
+
+                if get_extra_info:
+                    return arxiv_vaidation_value, {"id":arxiv, "valid":arxiv_vaidation_value}
+                return arxiv_vaidation_value
+            else:
+                if get_extra_info:
+                    info = self.exists(arxiv, get_extra_info=True)
+                    self.storage_manager.set_full_value(arxiv,info[1])
+                    return (info[0] and self.syntax_ok(arxiv)), info[1]
+                validity_check = self.exists(arxiv) and self.syntax_ok(arxiv)
+                self.storage_manager.set_value(arxiv, validity_check)
+
+                return validity_check
+
+    def normalise(self, id_string, include_prefix=False):
+        """It returns the arxiv normalized.
+
+        Args:
+            id_string (str): the arxiv to normalize.
+            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
+
+        Returns:
+            str: the normalized arxiv
+        """
+        regex = compile(r'[^0-9v.]')
+        regexdot = compile(r'\.+')
+        reg_api = compile(r'(https?://export\.arxiv\.org/api/query\?search_query=all:)')
+        reg_v_api = compile(r'(https?://arxiv\.org/abs/)')
+        reg_v_extrachar = compile(r'\/?ar[Xx]iv\.?')
+
+        if id_string:
+            id_string = str(id_string).strip().lower()
+
+            if id_string.startswith(self._p):
+                skip_char = len(self._p)
+                id_string = id_string[skip_char:]
+
+            id_string = regexdot.sub('.', id_string)
+            id_string = reg_v_api.sub('', id_string)
+            id_string = reg_api.sub('', id_string)
+            id_string = regex.sub('', id_string)
+            id_string = reg_v_extrachar.sub('', id_string)
+
+            # First parameter is the replacement, second parameter is your input string
+
+            try:
+                id_string = unquote(id_string)
+                arxiv_string = search("(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)", id_string).group(0)
+
+                return "%s%s" % (self._p if include_prefix else "", arxiv_string)
+            except:
+                try:
+                    id_string = unquote(id_string)
+                    arxiv_string = search("(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)?", id_string).group(0)
+                    return "%s%s" % (self._p if include_prefix else "", arxiv_string+"v1")
+                except:
+                    return None
+
+        else:
+            return None
+
+    def syntax_ok(self, id_string):
+        if not id_string.startswith(self._p):
+            id_string = self._p + id_string
+        return True if match("arxiv:(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)?$", id_string) else False
+
+
+    def exists(self, arxiv_full, get_extra_info=False, allow_extra_api=None):
+        """
+        Returns True if the id exists, False otherwise. Not all child class check id existence because of API policies
+        Args:
+            arxiv_full (str): the arxiv string for the api request
+        Returns:
+            bool: True if the arxiv exists (is registered), False otherwise.
+        """
+        valid_bool = True
+        if self._use_api_service:
+            arxiv_full_norm = self.normalise(arxiv_full, include_prefix=False)
+            if arxiv_full_norm:
+                version = ""
+                arxiv_string_match = search("(v\d+)$", arxiv_full_norm)
+                if arxiv_string_match:
+                    version = arxiv_string_match[1]
+
+                if version and version != "v1":
+                    api = self._api_v
+                else:
+                    if version == "v1":
+                        # v1 always exists, and the base API is more efficient,
+                        # so we just check the existence of the base ARXIV id
+                        arxiv_full_norm = arxiv_full_norm[:-2]
+
+                    api = self._api
+
+
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(
+                            api + quote(arxiv_full_norm),
+                            headers=self._headers,
+                            timeout=30,
+                        )
+                        if r.status_code == 200:
+                            if not version or version =="v1":
+                                #data = r.decode('utf-8').text
+                                xml_re = r.text
+                                obj = xmltodict.parse(f'{xml_re}')
+                                feed = obj.get("feed")
+                                results = feed.get("opensearch:totalResults")
+                                try:
+                                    results_n = int(results.get("#text"))
+                                except:
+                                    results_n = 0
+
+                                if results_n >0:
+                                    if get_extra_info:
+                                        return True, self.extra_info(obj)
+                                    return True
+                                else:
+                                    if get_extra_info:
+                                        return False, {"valid": False}
+                                    return False
+                            else:
+                                if get_extra_info:
+                                    return True, {"valid": True}
+                                return True
+                        else:
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool = False
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+
+    def extra_info(self, api_response, choose_api=None, info_dict:dict={}):
+        result = {}
+        result["valid"] = True
+        # to be implemented
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/base.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/base.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from abc import ABCMeta, abstractmethod
-
-
-class IdentifierManager(metaclass=ABCMeta):
-    """This is the interface that must be implemented by any identifier manager
-    for a particular identifier scheme. It provides the signatures of the methods
-    for checking the validity of an identifier and for normalising it."""
-
-    def __init__(self, **params):
-        """Identifier manager constructor."""
-        for key in params:
-            setattr(self, key, params[key])
-
-        self._headers = {
-            "User-Agent": "Identifier Manager / OpenCitations Indexes "
-            "(http://opencitations.net; mailto:contact@opencitations.net)"
-        }
-
-    def is_valid(self, id_string, get_extra_info=False):
-        """Returns true if the id is valid, false otherwise.
-
-        Args:
-            id_string (str): id to check
-            get_extra_info (bool, optional): True to get a dictionary with additional info about the id
-        Returns:
-            bool: True if the id is valid, False otherwise.
-            dict : a dictionary with additional information, if required (get_extra_info=True)
-
-        """
-        return True
-
-    def validated_as_id(self, id_string):
-        return None
-
-    @abstractmethod
-    def normalise(self, id_string, include_prefix=False):
-        """Returns the id normalized.
-
-        Args:
-            id_string (str): the id to normalize
-            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
-        Returns:
-            str: normalized id
-        """
-        pass
-
-    def check_digit(self, id_string):
-        """Returns True, if the check digit on the id_string passes (this does not mean that the id is also registered).
-        Not all id types have a check digit
-
-        Args:
-            id_string (str): the id to check
-        Returns:
-            bool: true if id_string passes the check digit of the specific id type
-        """
-        return True
-
-    def syntax_ok(self, id_string):
-        """  Returns True if the syntax of the id string is correct, False otherwise.
-
-        Args:
-            id_string (str): the id string to check
-        Returns:
-            bool: True if the id syntax is correct, False otherwise.
-        """
-        return True
-
-    def exists(self, id_string, get_extra_info=False, allow_extra_api=None):
-        """  Returns True if the id exists, False otherwise.
-        Not all child classes check id existence because of API policies
-
-        Args:
-            id_string (str): the id string for the api request
-            get_extra_info (bool, optional): True to get a dictionary with additional info about the id
-            allow_extra_api (list or None, optional): This optional list is supposed to contain the strings of
-                the names of the enabled APIs to call in case the primary one does not provide all the
-                required information. The default value assigned to this parameter is None, and in case
-                the list is not defined, only the primary API is used to retrieve information.
-        Returns:
-            bool: True if the id exists (is registered), False otherwise.
-            dict : a dictionary with additional information, if required
-        """
-        return True
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        """  Returns a dictionary with extra info about the id, if available.
-        Not all child classes check id existence because of API policies
-
-        Args:
-            api_response (json or string): the api response of the api request
-            choose_api (string or None, optional): the string of the name of the API from whose response
-                the information is to be extracted. The default value is None, and the default
-                behavior in case no string is defined is trying to extract the required extra
-                information from an API response provided by the primary API only. When this
-                method is called by the method exists, the value of the choose_api parameter
-                is supposed to be either one of the strings in the allow_extra_api list or None.
-            info_dict (dict, optional): a dictionary (empty by default) containing pre-processed
-                information, so to avoid retrieving the same data twice from different APIs.
-        Returns:
-            dict: A dictionary with additional information about the id, if provided by the API.
-        """
-        return {"value": True}
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from abc import ABCMeta, abstractmethod
+
+
+class IdentifierManager(metaclass=ABCMeta):
+    """This is the interface that must be implemented by any identifier manager
+    for a particular identifier scheme. It provides the signatures of the methods
+    for checking the validity of an identifier and for normalising it."""
+
+    def __init__(self, **params):
+        """Identifier manager constructor."""
+        for key in params:
+            setattr(self, key, params[key])
+
+        self._headers = {
+            "User-Agent": "Identifier Manager / OpenCitations Indexes "
+            "(http://opencitations.net; mailto:contact@opencitations.net)"
+        }
+
+    def is_valid(self, id_string, get_extra_info=False):
+        """Returns true if the id is valid, false otherwise.
+
+        Args:
+            id_string (str): id to check
+            get_extra_info (bool, optional): True to get a dictionary with additional info about the id
+        Returns:
+            bool: True if the id is valid, False otherwise.
+            dict : a dictionary with additional information, if required (get_extra_info=True)
+
+        """
+        return True
+
+    def validated_as_id(self, id_string):
+        return None
+
+    @abstractmethod
+    def normalise(self, id_string, include_prefix=False):
+        """Returns the id normalized.
+
+        Args:
+            id_string (str): the id to normalize
+            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
+        Returns:
+            str: normalized id
+        """
+        pass
+
+    def check_digit(self, id_string):
+        """Returns True, if the check digit on the id_string passes (this does not mean that the id is also registered).
+        Not all id types have a check digit
+
+        Args:
+            id_string (str): the id to check
+        Returns:
+            bool: true if id_string passes the check digit of the specific id type
+        """
+        return True
+
+    def syntax_ok(self, id_string):
+        """  Returns True if the syntax of the id string is correct, False otherwise.
+
+        Args:
+            id_string (str): the id string to check
+        Returns:
+            bool: True if the id syntax is correct, False otherwise.
+        """
+        return True
+
+    def exists(self, id_string, get_extra_info=False, allow_extra_api=None):
+        """  Returns True if the id exists, False otherwise.
+        Not all child classes check id existence because of API policies
+
+        Args:
+            id_string (str): the id string for the api request
+            get_extra_info (bool, optional): True to get a dictionary with additional info about the id
+            allow_extra_api (list or None, optional): This optional list is supposed to contain the strings of
+                the names of the enabled APIs to call in case the primary one does not provide all the
+                required information. The default value assigned to this parameter is None, and in case
+                the list is not defined, only the primary API is used to retrieve information.
+        Returns:
+            bool: True if the id exists (is registered), False otherwise.
+            dict : a dictionary with additional information, if required
+        """
+        return True
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        """  Returns a dictionary with extra info about the id, if available.
+        Not all child classes check id existence because of API policies
+
+        Args:
+            api_response (json or string): the api response of the api request
+            choose_api (string or None, optional): the string of the name of the API from whose response
+                the information is to be extracted. The default value is None, and the default
+                behavior in case no string is defined is trying to extract the required extra
+                information from an API response provided by the primary API only. When this
+                method is called by the method exists, the value of the choose_api parameter
+                is supposed to be either one of the strings in the allow_extra_api list or None.
+            info_dict (dict, optional): a dictionary (empty by default) containing pre-processed
+                information, so to avoid retrieving the same data twice from different APIs.
+        Returns:
+            dict: A dictionary with additional information about the id, if provided by the API.
+        """
+        return {"value": True}
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/doi.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/pmcid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,164 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from __future__ import annotations
-
-import re
-from re import match, sub
-from urllib.parse import quote, unquote
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from oc_ds_converter.oc_idmanager.isbn import ISBNManager
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
-from oc_ds_converter.oc_idmanager.support import call_api
-
-from oc_ds_converter.metadata_manager import MetadataManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Optional, Type
-
-
-class DOIManager(IdentifierManager):
-    """This class implements an identifier manager for doi identifier"""
-
-    def __init__(self, use_api_service=True, storage_manager:Optional[StorageManager] = None):
-        """DOI manager constructor."""
-        super(DOIManager,self).__init__()
-        if storage_manager is None:
-            self.storage_manager = InMemoryStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self._api = "https://doi.org/api/handles/"
-        self._api_airiti = ""
-        self._api_cnki = ""
-        self._api_crossref = "https://api.crossref.org/works/"
-        self._api_datacite = "https://api.datacite.org/dois/"
-        self._api_istic = ""
-        self._api_jalc = "https://api.japanlinkcenter.org/dois/"
-        self._api_kisti = ""
-        self._api_medra = "https://api.medra.org/metadata/"
-        self._api_op = ""
-        self._api_public = ""
-        self._api_unknown = "https://doi.org/ra/"
-        self._use_api_service = use_api_service
-        self._p = "doi:"
-        self._issnm = ISSNManager()
-        self._isbnm = ISBNManager()
-        self._om = ORCIDManager()
-
-    def validated_as_id(self, id_string):
-        doi_vaidation_value = self.storage_manager.get_value(id_string)
-        if isinstance(doi_vaidation_value, bool):
-            return doi_vaidation_value
-        else:
-            return None
-
-    def is_valid(self, id_string, get_extra_info=False):
-        doi = self.normalise(id_string, include_prefix=True)
-        if doi is None:
-            return False
-        else:
-            doi_vaidation_value = self.storage_manager.get_value(doi)
-            if isinstance(doi_vaidation_value, bool):
-                return doi_vaidation_value
-            else:
-                if get_extra_info:
-                    info = self.exists(doi, get_extra_info=True)
-                    self.storage_manager.set_full_value(doi,info[1])
-                    return (info[0] and self.syntax_ok(doi)), info[1]
-                validity_check = self.exists(doi) and self.syntax_ok(doi)
-                self.storage_manager.set_value(doi, validity_check)
-                return validity_check
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            doi_string = sub(
-                "\0+", "", sub("\s+", "", unquote(id_string[id_string.index("10.") :]))
-            )
-            return "%s%s" % (
-                self._p if include_prefix else "",
-                doi_string.lower().strip(),
-            )
-        except:
-            # Any error in processing the DOI will return None
-            return None
-
-    def syntax_ok(self, id_string):
-        if not id_string.startswith(self._p):
-            id_string = self._p+id_string
-        return True if match("^doi:10\.(\d{4,9}|[^\s/]+(\.[^\s/]+)*)/[^\s]+$", id_string, re.IGNORECASE) else False
-
-    def exists(self, doi_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        doi = doi_full
-        if self._use_api_service:
-            doi = self.normalise(doi_full)
-            if doi:
-                json_res = call_api(url=self._api + quote(doi), headers=self._headers)
-                if json_res:
-                    valid_bool = json_res.get("responseCode") == 1
-                    if get_extra_info:
-                        extra_info = {'id': doi, 'valid': valid_bool, 'ra': 'unknown'}
-                        if allow_extra_api is None:
-                            return valid_bool, extra_info
-                        elif valid_bool is True and allow_extra_api:
-                            r_format = "xml" if allow_extra_api == "medra" else "json"
-                            extra_api_result = call_api(url=getattr(self, f'_api_{allow_extra_api}') + quote(doi), headers=self._headers, r_format=r_format)
-                            if extra_api_result:
-                                metadata_manager = MetadataManager(allow_extra_api, json_res)
-                                extra_info.update(metadata_manager.extract_metadata())
-                                return valid_bool, extra_info
-                            else:
-                                return valid_bool, {'id': doi, 'valid': valid_bool, 'ra': 'unknown'}
-                    return valid_bool
-                valid_bool = False
-            else:
-                return (False, {'id': None, 'valid': False, 'ra': 'unknown'}) if get_extra_info else False
-        return (valid_bool, {'id': doi, 'valid': valid_bool, 'ra': 'unknown'}) if get_extra_info else valid_bool
-
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from json import loads
+from re import match, sub
+from time import sleep
+from urllib.parse import quote, unquote
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+from typing import Type, Optional
+
+
+
+class PMCIDManager(IdentifierManager):
+    """This class implements an identifier manager for PMCID identifier"""
+
+    def __init__(self, use_api_service=True, storage_manager: Optional[StorageManager] = None):
+        """PMCID manager constructor."""
+        super(PMCIDManager, self).__init__()
+        self._use_api_service = use_api_service
+        if storage_manager is None:
+            self.storage_manager = InMemoryStorageManager()
+        else:
+            self.storage_manager = storage_manager
+        self._api = "https://www.ncbi.nlm.nih.gov/pmc/utils/idconv/v1.0/"
+        self._use_api_service = use_api_service
+        self._p = "pmcid:"
+
+        # If there's a need to obtain more metadata from a PMCID, consider using Entrez (aka E-Utilities) API (
+        # https://eutils.ncbi.nlm.nih.gov/entrez/eutils/), which of course works with different parameters and
+        # returns different responses.
+        # The ID Converter API only provides alternative IDs (doi, pmid) for the work associated to the queried pmcid.
+
+    def validated_as_id(self, id_string):
+        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
+        if isinstance(arxiv_vaidation_value, bool):
+            return arxiv_vaidation_value
+        else:
+            return None
+
+
+    def is_valid(self, pmcid, get_extra_info=False):
+        pmcid = self.normalise(pmcid, include_prefix=True)
+
+        if pmcid is None:
+            return False
+        else:
+            pmc_vaidation_value = self.storage_manager.get_value(pmcid)
+            if isinstance(pmc_vaidation_value, bool):
+                return pmc_vaidation_value
+            else:
+                if get_extra_info:
+                    info = self.exists(pmcid, get_extra_info=True)
+                    self.storage_manager.set_full_value(pmcid,info[1])
+                    return (info[0] and self.syntax_ok(pmcid)), info[1]
+                validity_check = self.exists(pmcid) and self.syntax_ok(pmcid)
+                self.storage_manager.set_value(pmcid, validity_check)
+
+                return validity_check
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            if id_string.startswith(self._p):
+                id_string = id_string[len(self._p):]
+            else:
+                id_string = id_string
+
+            pmcid_string = sub(
+                "\0+", "", sub("\s+", "", unquote(id_string[id_string.index("PMC"):]))
+            )
+            return "%s%s" % (
+                self._p if include_prefix else "",
+                pmcid_string.strip(),
+            )
+        except:
+            # Any error in processing the DOI will return None
+            return None
+
+    def syntax_ok(self, id_string):
+
+        if not id_string.startswith("pmcid:"):
+            id_string = self._p + id_string
+        return True if match(r"^pmcid:PMC[1-9]\d+(\.\d{1,2})?$", id_string) else False
+
+    def exists(self, pmcid_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self._use_api_service:
+            pmcid = self.normalise(pmcid_full)
+            if pmcid is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        parameters = {
+                            'ids': quote(pmcid),
+                            'format': 'json',
+                            'idtype': 'pmcid'
+                        }
+
+                        r = get(self._api, params=parameters, headers=self._headers, timeout=30)
+                        if r.status_code == 200:
+                            r.encoding = "utf-8"
+                            json_res = loads(r.text)
+                            if get_extra_info:
+                                extra_info_result = {}
+                                try:
+                                    result = True if not json_res['records'][0].get('status') =='error' else False
+                                    extra_info_result['valid'] = result
+                                    extra_info_result['id'] = pmcid
+                                    return result, extra_info_result
+                                except KeyError:
+                                    extra_info_result["valid"] = False
+                                    extra_info_result['id'] = pmcid
+                                    return False, extra_info_result
+                            try:
+                                return True if not json_res['records'][0].get('status') =='error' else False
+
+                            except KeyError:
+                                return False
+
+                        elif 400 <= r.status_code < 500:
+                            if get_extra_info:
+                                return False, {"id":pmcid, "valid": False}
+                            return False
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool = False
+            else:
+                if get_extra_info:
+                    return False, {"id":pmcid, "valid": False}
+                return False
+
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        # to be implemented
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/isbn.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/isbn.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import re
-from re import match, sub
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-
-
-class ISBNManager(IdentifierManager):
-    """This class implements an identifier manager for isbn identifier"""
-    def __init__(self, data={}):
-        """ISBN manager constructor."""
-        self._p = "isbn:"
-        self._data = data
-        super(ISBNManager, self).__init__()
-
-    def is_valid(self, id_string, get_extra_info=False):
-        isbn = self.normalise(id_string, include_prefix=True)
-        if isbn is None:
-            return False
-        else:
-            if isbn not in self._data or self._data[isbn] is None:
-                return (
-                    self.check_digit(isbn)
-                    and self.syntax_ok(isbn)
-                )
-            return self._data[isbn].get("valid")
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            isbn_string = sub("[^X0-9]", "", id_string.upper())
-            return "%s%s" % (self._p if include_prefix else "", isbn_string)
-        except:  # Any error in processing the ISBN will return None
-            return None
-
-    def check_digit(self, isbn):
-        if isbn.startswith(self._p):
-            spl = isbn.find(self._p) + len(self._p)
-            isbn = isbn[spl:]
-
-        isbn = isbn.replace("-", "")
-        isbn = isbn.replace(" ", "")
-        check_digit = False
-        if len(isbn) == 13:
-            total = 0
-            val = 1
-            for x in isbn:
-                if x == "X":
-                    x = 10
-                total += int(x)*val
-                val = 3 if val == 1 else val == 1
-            if (total % 10) == 0:
-                check_digit = True
-        elif len(isbn) == 10:
-            total = 0
-            val = 10
-            for x in isbn:
-                if x == "X":
-                    x = 10
-                total += int(x)*val
-                val -= 1
-            if (total % 11) == 0:
-                check_digit = True
-
-        return check_digit
-
-    def syntax_ok(self, id_string):
-        id_string.replace(" ", "")
-        id_string.replace("-", "")
-        if not id_string.startswith(self._p):
-            id_string = self._p+id_string
-        if len(id_string) - len(self._p) == 13:
-            return True if match("^isbn:97[89][0-9X]{10}$", id_string, re.IGNORECASE) else False
-        elif len(id_string) - len(self._p) == 10:
-            return True if match("^isbn:[0-9X]{10}$", id_string, re.IGNORECASE) else False
-        else:
-            return False
-
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import re
+from re import match, sub
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+
+
+class ISBNManager(IdentifierManager):
+    """This class implements an identifier manager for isbn identifier"""
+    def __init__(self, data={}):
+        """ISBN manager constructor."""
+        self._p = "isbn:"
+        self._data = data
+        super(ISBNManager, self).__init__()
+
+    def is_valid(self, id_string, get_extra_info=False):
+        isbn = self.normalise(id_string, include_prefix=True)
+        if isbn is None:
+            return False
+        else:
+            if isbn not in self._data or self._data[isbn] is None:
+                return (
+                    self.check_digit(isbn)
+                    and self.syntax_ok(isbn)
+                )
+            return self._data[isbn].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            isbn_string = sub("[^X0-9]", "", id_string.upper())
+            return "%s%s" % (self._p if include_prefix else "", isbn_string)
+        except:  # Any error in processing the ISBN will return None
+            return None
+
+    def check_digit(self, isbn):
+        if isbn.startswith(self._p):
+            spl = isbn.find(self._p) + len(self._p)
+            isbn = isbn[spl:]
+
+        isbn = isbn.replace("-", "")
+        isbn = isbn.replace(" ", "")
+        check_digit = False
+        if len(isbn) == 13:
+            total = 0
+            val = 1
+            for x in isbn:
+                if x == "X":
+                    x = 10
+                total += int(x)*val
+                val = 3 if val == 1 else val == 1
+            if (total % 10) == 0:
+                check_digit = True
+        elif len(isbn) == 10:
+            total = 0
+            val = 10
+            for x in isbn:
+                if x == "X":
+                    x = 10
+                total += int(x)*val
+                val -= 1
+            if (total % 11) == 0:
+                check_digit = True
+
+        return check_digit
+
+    def syntax_ok(self, id_string):
+        id_string.replace(" ", "")
+        id_string.replace("-", "")
+        if not id_string.startswith(self._p):
+            id_string = self._p+id_string
+        if len(id_string) - len(self._p) == 13:
+            return True if match("^isbn:97[89][0-9X]{10}$", id_string, re.IGNORECASE) else False
+        elif len(id_string) - len(self._p) == 10:
+            return True if match("^isbn:[0-9X]{10}$", id_string, re.IGNORECASE) else False
+        else:
+            return False
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/issn.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/issn.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import re
-from re import match, sub
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-
-
-class ISSNManager(IdentifierManager):
-    """This class implements an identifier manager for issn identifier"""
-
-    def __init__(self, data={}):
-        """ISSN manager constructor."""
-        super(ISSNManager, self).__init__()
-        self._p = "issn:"
-        self._data = data
-
-    def is_valid(self, id_string, get_extra_info=False):
-        issn = self.normalise(id_string, include_prefix=True)
-        if issn is None:
-            return False
-        else:
-            if issn not in self._data or self._data[issn] is None:
-                return (
-                    self.syntax_ok(issn)
-                    and self.check_digit(issn)
-                )
-            return self._data[issn].get("valid")
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            issn_string = sub("[^X0-9]", "", id_string.upper())
-            return "%s%s-%s" % (
-                self._p if include_prefix else "",
-                issn_string[:4],
-                issn_string[4:8],
-            )
-        except:  # Any error in processing the ISSN will return None
-            return None
-
-    def syntax_ok(self, id_string):
-        if not id_string.startswith(self._p):
-            id_string = self._p+id_string
-        return True if match("^issn:[0-9]{4}-[0-9]{3}[0-9X]$", id_string, re.IGNORECASE) else False
-
-    def check_digit(self,issn):
-        if issn.startswith(self._p):
-            spl = issn.find(self._p) + len(self._p)
-            issn = issn[spl:]
-        issn = issn.replace('-', '')
-        if len(issn) != 8:
-            raise ValueError('ISSN of len 8 or 9 required (e.g. 00000949 or 0000-0949)')
-        ss = sum([int(digit) * f for digit, f in zip(issn, range(8, 1, -1))])
-        _, mod = divmod(ss, 11)
-        checkdigit = 0 if mod == 0 else 11 - mod
-        if checkdigit == 10:
-            checkdigit = 'X'
-        return '{}'.format(checkdigit) == issn[7]
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import re
+from re import match, sub
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+
+
+class ISSNManager(IdentifierManager):
+    """This class implements an identifier manager for issn identifier"""
+
+    def __init__(self, data={}):
+        """ISSN manager constructor."""
+        super(ISSNManager, self).__init__()
+        self._p = "issn:"
+        self._data = data
+
+    def is_valid(self, id_string, get_extra_info=False):
+        issn = self.normalise(id_string, include_prefix=True)
+        if issn is None:
+            return False
+        else:
+            if issn not in self._data or self._data[issn] is None:
+                return (
+                    self.syntax_ok(issn)
+                    and self.check_digit(issn)
+                )
+            return self._data[issn].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            issn_string = sub("[^X0-9]", "", id_string.upper())
+            return "%s%s-%s" % (
+                self._p if include_prefix else "",
+                issn_string[:4],
+                issn_string[4:8],
+            )
+        except:  # Any error in processing the ISSN will return None
+            return None
+
+    def syntax_ok(self, id_string):
+        if not id_string.startswith(self._p):
+            id_string = self._p+id_string
+        return True if match("^issn:[0-9]{4}-[0-9]{3}[0-9X]$", id_string, re.IGNORECASE) else False
+
+    def check_digit(self,issn):
+        if issn.startswith(self._p):
+            spl = issn.find(self._p) + len(self._p)
+            issn = issn[spl:]
+        issn = issn.replace('-', '')
+        if len(issn) != 8:
+            raise ValueError('ISSN of len 8 or 9 required (e.g. 00000949 or 0000-0949)')
+        ss = sum([int(digit) * f for digit, f in zip(issn, range(8, 1, -1))])
+        _, mod = divmod(ss, 11)
+        checkdigit = 0 if mod == 0 else 11 - mod
+        if checkdigit == 10:
+            checkdigit = 'X'
+        return '{}'.format(checkdigit) == issn[7]
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/jid.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/jid.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-import xml.etree.ElementTree as ET
-from re import match, sub
-from time import sleep
-from urllib.parse import quote
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Type, Optional
-
-
-class JIDManager(IdentifierManager):
-    """This class implements an identifier manager for jid identifier"""
-    def __init__(self, use_api_service=True, storage_manager:Optional[StorageManager] = None):
-        """JID manager constructor"""
-        super(JIDManager, self).__init__()
-        self.use_api_service = use_api_service
-        if storage_manager is None:
-            self.storage_manager = InMemoryStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self._p = "jid:"
-        self._api = "https://api.jstage.jst.go.jp/searchapi/"
-        self._api2 = "https://www.jstage.jst.go.jp/browse/"
-        self._headers = {
-            "User-Agent": "Identifier Manager / OpenCitations Indexes "
-                          "(http://opencitations.net; mailto:contact@opencitations.net)"
-        }
-
-    def validated_as_id(self, id_string):
-        jid_validation_value = self.storage_manager.get_value(id_string)
-        if isinstance(jid_validation_value, bool):
-            return jid_validation_value
-        else:
-            return None
-
-    def is_valid(self, jid, get_extra_info=False):
-        """Check if a jid is valid.
-
-            Args:
-                id_string (str): the jid to check
-
-            Returns:
-                bool: true if the jid is valid, false otherwise.
-        """
-        jid = self.normalise(jid, include_prefix=True)
-
-        if jid is None:
-            return False
-        else:
-            jid_validation_value = self.storage_manager.get_value(jid)
-            if isinstance(jid_validation_value, bool):
-                if get_extra_info:
-                        return jid_validation_value, {"id":jid, "valid": jid_validation_value}
-                return jid_validation_value
-            else:
-                if get_extra_info:
-                    info = self.exists(jid, get_extra_info=True)
-                    self.storage_manager.set_full_value(jid, info[1])
-                    return (info[0] and self.syntax_ok(jid)), info[1]
-                validity_check = self.exists(jid) and self.syntax_ok(jid)
-                self.storage_manager.set_value(jid, validity_check)
-
-                return validity_check
-            
-
-    
-    def normalise(self, id_string, include_prefix=False):
-        """It returns the jid normalized.
-
-        Args:
-            id_string (str): the jid to normalize.
-            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
-
-        Returns:
-            str: the normalized jid
-        """
-        try:
-            if id_string.startswith(self._p):
-                jid_string = id_string[len(self._p):]
-            else:
-                jid_string = id_string
-            jid_string = sub("[^/a-z0-9]", "", jid_string.lower())
-            return "%s%s" % (self._p if include_prefix else "", jid_string)
-        except:
-            # Any error in processing the JID will return None
-            return None
-    
-    def syntax_ok(self, id_string):
-        if not id_string.startswith(self._p):
-            id_string = self._p+id_string
-        return True if match("^jid:[a-z]+([12][0-9]{3}){0,1}[a-z]*$", id_string) else False
-
-       
-    
-    def exists(self, jid_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        if self.use_api_service:
-            jid = self.normalise(jid_full)
-            if jid is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(self._api+ "/do?service=2&cdjournal=" + quote(jid), headers=self._headers, timeout=30)
-                        #fromstring() parses XML from a string directly into an Element, which is the root element of the parsed tree
-                        root = ET.fromstring(r.content)
-                        status = root.find(".//{http://www.w3.org/2005/Atom}status").text
-                        if status =="0":
-                            if get_extra_info:
-                                return True, self.extra_info(r.content)
-                            return True
-                        elif status == "ERR_001":
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-                        else:
-                            tentative=3
-                            while tentative:
-                                tentative -=1
-                                try:
-                                    r = get(self._api+ "/do?service=2&cdjournal=" + quote(jid), headers=self._headers, timeout=30)
-                                    # fromstring() parses XML from a string directly into an Element, which is the root element of the parsed tree
-                                    root = ET.fromstring(r.content)
-                                    status = root.find(".//{http://www.w3.org/2005/Atom}status").text
-                                    if status == "0":
-                                        if get_extra_info:
-                                            return True, self.extra_info(r.content)
-                                        return True
-                                    elif status == "ERR_001":
-                                        if get_extra_info:
-                                            return False, {"valid": False}
-                                        return False
-                                except ReadTimeout:
-                                # Do nothing, just try again
-                                    pass
-                                except ConnectionError:
-                                # Sleep 5 seconds, then try again
-                                    sleep(5)
-
-                            # call to the other API
-                            try:
-                                r = get(self._api2 + quote(jid), headers=self._headers, timeout=30)
-                                if r.status_code == 404:
-                                    if get_extra_info:
-                                        return False, {"valid": False}
-                                    return False
-                                elif r.status_code == 200:
-                                    r.encoding = "utf-8"
-                                    soup = BeautifulSoup(r.text, features="lxml")
-                                    txt_obj = str(soup.find(id="page-content"))
-                                    if get_extra_info:
-                                        return True, self.extra_info(txt_obj)
-                                    return True
-                            except ReadTimeout:
-                                # Do nothing, just try again
-                                    pass
-                            except ConnectionError:
-                            # Sleep 5 seconds, then try again
-                                sleep(5)
-
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-
-                valid_bool=False
-
-            else:
-                if get_extra_info:
-                    return False, {"valid": False}
-                return False
-        if get_extra_info:
-            return valid_bool, {"valid": valid_bool}
-        return valid_bool
-    
-    
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-        return result
+import xml.etree.ElementTree as ET
+from re import match, sub
+from time import sleep
+from urllib.parse import quote
+
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+from typing import Type, Optional
+
+
+class JIDManager(IdentifierManager):
+    """This class implements an identifier manager for jid identifier"""
+    def __init__(self, use_api_service=True, storage_manager:Optional[StorageManager] = None):
+        """JID manager constructor"""
+        super(JIDManager, self).__init__()
+        self.use_api_service = use_api_service
+        if storage_manager is None:
+            self.storage_manager = InMemoryStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self._p = "jid:"
+        self._api = "https://api.jstage.jst.go.jp/searchapi/"
+        self._api2 = "https://www.jstage.jst.go.jp/browse/"
+        self._headers = {
+            "User-Agent": "Identifier Manager / OpenCitations Indexes "
+                          "(http://opencitations.net; mailto:contact@opencitations.net)"
+        }
+
+    def validated_as_id(self, id_string):
+        jid_validation_value = self.storage_manager.get_value(id_string)
+        if isinstance(jid_validation_value, bool):
+            return jid_validation_value
+        else:
+            return None
+
+    def is_valid(self, jid, get_extra_info=False):
+        """Check if a jid is valid.
+
+            Args:
+                id_string (str): the jid to check
+
+            Returns:
+                bool: true if the jid is valid, false otherwise.
+        """
+        jid = self.normalise(jid, include_prefix=True)
+
+        if jid is None:
+            return False
+        else:
+            jid_validation_value = self.storage_manager.get_value(jid)
+            if isinstance(jid_validation_value, bool):
+                if get_extra_info:
+                        return jid_validation_value, {"id":jid, "valid": jid_validation_value}
+                return jid_validation_value
+            else:
+                if get_extra_info:
+                    info = self.exists(jid, get_extra_info=True)
+                    self.storage_manager.set_full_value(jid, info[1])
+                    return (info[0] and self.syntax_ok(jid)), info[1]
+                validity_check = self.exists(jid) and self.syntax_ok(jid)
+                self.storage_manager.set_value(jid, validity_check)
+
+                return validity_check
+            
+
+    
+    def normalise(self, id_string, include_prefix=False):
+        """It returns the jid normalized.
+
+        Args:
+            id_string (str): the jid to normalize.
+            include_prefix (bool, optional): indicates if include the prefix. Defaults to False.
+
+        Returns:
+            str: the normalized jid
+        """
+        try:
+            if id_string.startswith(self._p):
+                jid_string = id_string[len(self._p):]
+            else:
+                jid_string = id_string
+            jid_string = sub("[^/a-z0-9]", "", jid_string.lower())
+            return "%s%s" % (self._p if include_prefix else "", jid_string)
+        except:
+            # Any error in processing the JID will return None
+            return None
+    
+    def syntax_ok(self, id_string):
+        if not id_string.startswith(self._p):
+            id_string = self._p+id_string
+        return True if match("^jid:[a-z]+([12][0-9]{3}){0,1}[a-z]*$", id_string) else False
+
+       
+    
+    def exists(self, jid_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self.use_api_service:
+            jid = self.normalise(jid_full)
+            if jid is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(self._api+ "/do?service=2&cdjournal=" + quote(jid), headers=self._headers, timeout=30)
+                        #fromstring() parses XML from a string directly into an Element, which is the root element of the parsed tree
+                        root = ET.fromstring(r.content)
+                        status = root.find(".//{http://www.w3.org/2005/Atom}status").text
+                        if status =="0":
+                            if get_extra_info:
+                                return True, self.extra_info(r.content)
+                            return True
+                        elif status == "ERR_001":
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+                        else:
+                            tentative=3
+                            while tentative:
+                                tentative -=1
+                                try:
+                                    r = get(self._api+ "/do?service=2&cdjournal=" + quote(jid), headers=self._headers, timeout=30)
+                                    # fromstring() parses XML from a string directly into an Element, which is the root element of the parsed tree
+                                    root = ET.fromstring(r.content)
+                                    status = root.find(".//{http://www.w3.org/2005/Atom}status").text
+                                    if status == "0":
+                                        if get_extra_info:
+                                            return True, self.extra_info(r.content)
+                                        return True
+                                    elif status == "ERR_001":
+                                        if get_extra_info:
+                                            return False, {"valid": False}
+                                        return False
+                                except ReadTimeout:
+                                # Do nothing, just try again
+                                    pass
+                                except ConnectionError:
+                                # Sleep 5 seconds, then try again
+                                    sleep(5)
+
+                            # call to the other API
+                            try:
+                                r = get(self._api2 + quote(jid), headers=self._headers, timeout=30)
+                                if r.status_code == 404:
+                                    if get_extra_info:
+                                        return False, {"valid": False}
+                                    return False
+                                elif r.status_code == 200:
+                                    r.encoding = "utf-8"
+                                    soup = BeautifulSoup(r.text, features="lxml")
+                                    txt_obj = str(soup.find(id="page-content"))
+                                    if get_extra_info:
+                                        return True, self.extra_info(txt_obj)
+                                    return True
+                            except ReadTimeout:
+                                # Do nothing, just try again
+                                    pass
+                            except ConnectionError:
+                            # Sleep 5 seconds, then try again
+                                sleep(5)
+
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+
+                valid_bool=False
+
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+    
+    
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/metadata_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/metadata_manager.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-#!python
-# Copyright 2022-2023 Arianna Moretti <arianna.moretti4@unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-import importlib
-from urllib.parse import quote
-
-from oc_ds_converter.oc_idmanager.isbn import ISBNManager
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
-
-
-class MetadataManager():
-    def __init__(self, metadata_provider:str, api_response:dict, orcid_doi_filepath:str):
-        self.metadata_provider = metadata_provider
-        self.api_response = api_response
-        self.orcid_doi_filepath = orcid_doi_filepath
-        self._issnm = ISSNManager()
-        self._isbnm = ISBNManager()
-        self._om = ORCIDManager()
-        from oc_ds_converter.oc_idmanager.doi import DOIManager
-        self.doi_manager = DOIManager()
-        self._have_api = ['crossref', 'datacite', 'medra', 'jalc']
-
-    def extract_metadata(self) -> None:
-        metadata = {'ra': self.metadata_provider}
-        if self.metadata_provider is None or self.api_response is None:
-            return metadata
-        if self.metadata_provider == 'unknown':
-            return self.extract_from_unknown()
-        elif self.metadata_provider in self._have_api:
-            module = importlib.import_module(f'oc_ds_converter.{self.metadata_provider}.{self.metadata_provider}_processing')
-            class_ = getattr(module, f'{self.metadata_provider.title()}Processing')
-            metadata_processor = class_(orcid_index=self.orcid_doi_filepath)
-            api_response = self.api_response['data'] if self.metadata_provider == 'datacite' else self.api_response
-            metadata.update(getattr(metadata_processor, 'csv_creator')(api_response))                
-        return metadata
-
-    def extract_from_unknown(self) -> None:
-        metadata = dict()
-        api_response: dict = self.api_response[0]
-        if api_response.get('status') == 'Error':
-            metadata['ra'] = 'unknown'
-            return metadata
-        elif api_response.get('status') == 'DOI does not exist':
-            metadata['ra'] = 'invalid'
-            return metadata
-        registration_agency = self.api_response[0]['RA'].lower()
-        metadata['ra'] = registration_agency
-        doi = self.api_response[0]['DOI']
-        api_registration_agency = getattr(self.doi_manager, f'_api_{registration_agency}')
-        if api_registration_agency:
-            from oc_ds_converter.lib.file_manager import call_api
-            url = api_registration_agency + quote(doi)
-            r_format = 'xml' if registration_agency == 'medra' else 'json'
-            extra_api_result = call_api(url=url, headers=self.doi_manager._headers, r_format=r_format)
-            self.metadata_provider = registration_agency
-            self.api_response = extra_api_result
-            try:
-                metadata.update(self.extract_metadata())
-            except Exception as e:
-                print(doi, registration_agency)
-                print(e)
-                raise(Exception)
+#!python
+# Copyright 2022-2023 Arianna Moretti <arianna.moretti4@unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+import importlib
+from urllib.parse import quote
+
+from oc_ds_converter.oc_idmanager.isbn import ISBNManager
+from oc_ds_converter.oc_idmanager.issn import ISSNManager
+from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
+
+
+class MetadataManager():
+    def __init__(self, metadata_provider:str, api_response:dict, orcid_doi_filepath:str):
+        self.metadata_provider = metadata_provider
+        self.api_response = api_response
+        self.orcid_doi_filepath = orcid_doi_filepath
+        self._issnm = ISSNManager()
+        self._isbnm = ISBNManager()
+        self._om = ORCIDManager()
+        from oc_ds_converter.oc_idmanager.doi import DOIManager
+        self.doi_manager = DOIManager()
+        self._have_api = ['crossref', 'datacite', 'medra', 'jalc']
+
+    def extract_metadata(self) -> None:
+        metadata = {'ra': self.metadata_provider}
+        if self.metadata_provider is None or self.api_response is None:
+            return metadata
+        if self.metadata_provider == 'unknown':
+            return self.extract_from_unknown()
+        elif self.metadata_provider in self._have_api:
+            module = importlib.import_module(f'oc_ds_converter.{self.metadata_provider}.{self.metadata_provider}_processing')
+            class_ = getattr(module, f'{self.metadata_provider.title()}Processing')
+            metadata_processor = class_(orcid_index=self.orcid_doi_filepath)
+            api_response = self.api_response['data'] if self.metadata_provider == 'datacite' else self.api_response
+            metadata.update(getattr(metadata_processor, 'csv_creator')(api_response))                
+        return metadata
+
+    def extract_from_unknown(self) -> None:
+        metadata = dict()
+        api_response: dict = self.api_response[0]
+        if api_response.get('status') == 'Error':
+            metadata['ra'] = 'unknown'
+            return metadata
+        elif api_response.get('status') == 'DOI does not exist':
+            metadata['ra'] = 'invalid'
+            return metadata
+        registration_agency = self.api_response[0]['RA'].lower()
+        metadata['ra'] = registration_agency
+        doi = self.api_response[0]['DOI']
+        api_registration_agency = getattr(self.doi_manager, f'_api_{registration_agency}')
+        if api_registration_agency:
+            from oc_ds_converter.lib.file_manager import call_api
+            url = api_registration_agency + quote(doi)
+            r_format = 'xml' if registration_agency == 'medra' else 'json'
+            extra_api_result = call_api(url=url, headers=self.doi_manager._headers, r_format=r_format)
+            self.metadata_provider = registration_agency
+            self.api_response = extra_api_result
+            try:
+                metadata.update(self.extract_metadata())
+            except Exception as e:
+                print(doi, registration_agency)
+                print(e)
+                raise(Exception)
         return metadata
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright (c) 2016, Silvio Peroni <essepuntato@gmail.com>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-from __future__ import annotations
-
-from typing import List, Dict
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-import os
-import json
-import urllib.parse
-from pathlib import Path
-
-
-class InMemoryStorageManager(StorageManager):
-    """A concrete implementation of the ``StorageManager`` interface that persistently stores
-    the IDs validity values within a in-memory dictionary, which is eventually saved in a json file."""
-
-    def __init__(self, json_file_path: str =None, **params) -> None:
-        """
-        Constructor of the ``InMemoryStorageManager`` class.
-        """
-        super().__init__(**params)
-        if json_file_path and os.path.exists(json_file_path):
-            self.storage_filepath = json_file_path
-            o_jfp = open(self.storage_filepath, "r")
-            self.id_value_dict = json.load(o_jfp)
-            o_jfp.close()
-        elif json_file_path and not os.path.exists(json_file_path):
-            if not os.path.exists(os.path.abspath(os.path.join(json_file_path, os.pardir))):
-                Path(os.path.abspath(os.path.join(json_file_path, os.pardir))).mkdir(parents=True, exist_ok=True)
-            self.storage_filepath = json_file_path
-            self.id_value_dict = dict()
-            file = open(self.storage_filepath, "w", encoding='utf8')
-            json.dump(self.id_value_dict, file)
-            file.close()
-        else:
-            new_path_dir = os.path.join(os.getcwd(), "storage")
-            if not os.path.exists(new_path_dir):
-                os.makedirs(new_path_dir)
-            filepath = os.path.join(new_path_dir, "id_value.json" )
-            self.id_value_dict = dict()
-            self.storage_filepath = filepath
-            file = open(self.storage_filepath, "w", encoding='utf8')
-            json.dump(self.id_value_dict, file)
-            file.close()
-
-    def set_full_value(self, id: str, value: dict) -> None:
-        """
-        It allows to set the counter value of provenance entities.
-
-        :param value: The new counter value to be set
-        :type value: dict
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id)
-        if not isinstance(value, dict):
-            raise ValueError("value must be dict")
-        if id_name in self.id_value_dict:
-            new_info = {k:v for k,v in value.items() if k not in self.id_value_dict[id_name]}
-            self.id_value_dict[id_name].update(new_info)
-        else:
-            self.id_value_dict[id_name] = value
-
-    def set_value(self, id: str, value: bool) -> None:
-        """
-        It allows to set the counter value of provenance entities.
-
-        :param value: The new counter value to be set
-        :type value: bool
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id)
-
-        if not isinstance(value, bool):
-            raise ValueError("value must be boolean")
-        if id_name in self.id_value_dict:
-            self.id_value_dict[id_name]["valid"] = value
-        else:
-            self.id_value_dict[id_name] = {"valid": value}
-
-    def get_value(self, id: str):
-        """
-        It allows to read the value of the "valid" key of the identifier's dict.
-
-        :param id: The id name
-        :type id: str
-        :return: The requested id value.
-        """
-
-        id_name = str(id)
-        id_in_dict = self.id_value_dict.get(id_name)
-        if id_in_dict:
-            return id_in_dict["valid"]
-        else:
-            return None
-
-    def store_file(self) -> None:
-        """
-        It stores in a file the dictionary with the validation results
-        """
-        file = open(self.storage_filepath, "w", encoding='utf8')
-        json.dump(self.id_value_dict, file, indent=4)
-        file.close()
-
-    def delete_storage(self):
-        self.id_value_dict = dict()
-        if os.path.exists(self.storage_filepath):
-            os.remove(self.storage_filepath)
-
-    def get_all_keys(self):
-        return self.id_value_dict.keys()
-
-    def get_validity_dict(self):
-        return {k: v["valid"] for k, v in self.id_value_dict.items()}
-
-    def get_validity_list_of_tuples(self):
-        return [(k, v["valid"]) for k, v in self.id_value_dict.items()]
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright (c) 2016, Silvio Peroni <essepuntato@gmail.com>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+from __future__ import annotations
+
+from typing import List, Dict
+
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+import os
+import json
+import urllib.parse
+from pathlib import Path
+
+
+class InMemoryStorageManager(StorageManager):
+    """A concrete implementation of the ``StorageManager`` interface that persistently stores
+    the IDs validity values within a in-memory dictionary, which is eventually saved in a json file."""
+
+    def __init__(self, json_file_path: str =None, **params) -> None:
+        """
+        Constructor of the ``InMemoryStorageManager`` class.
+        """
+        super().__init__(**params)
+        if json_file_path and os.path.exists(json_file_path):
+            self.storage_filepath = json_file_path
+            o_jfp = open(self.storage_filepath, "r")
+            self.id_value_dict = json.load(o_jfp)
+            o_jfp.close()
+        elif json_file_path and not os.path.exists(json_file_path):
+            if not os.path.exists(os.path.abspath(os.path.join(json_file_path, os.pardir))):
+                Path(os.path.abspath(os.path.join(json_file_path, os.pardir))).mkdir(parents=True, exist_ok=True)
+            self.storage_filepath = json_file_path
+            self.id_value_dict = dict()
+            file = open(self.storage_filepath, "w", encoding='utf8')
+            json.dump(self.id_value_dict, file)
+            file.close()
+        else:
+            new_path_dir = os.path.join(os.getcwd(), "storage")
+            if not os.path.exists(new_path_dir):
+                os.makedirs(new_path_dir)
+            filepath = os.path.join(new_path_dir, "id_value.json" )
+            self.id_value_dict = dict()
+            self.storage_filepath = filepath
+            file = open(self.storage_filepath, "w", encoding='utf8')
+            json.dump(self.id_value_dict, file)
+            file.close()
+
+    def set_full_value(self, id: str, value: dict) -> None:
+        """
+        It allows to set the counter value of provenance entities.
+
+        :param value: The new counter value to be set
+        :type value: dict
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id)
+        if not isinstance(value, dict):
+            raise ValueError("value must be dict")
+        if id_name in self.id_value_dict:
+            new_info = {k:v for k,v in value.items() if k not in self.id_value_dict[id_name]}
+            self.id_value_dict[id_name].update(new_info)
+        else:
+            self.id_value_dict[id_name] = value
+
+    def set_value(self, id: str, value: bool) -> None:
+        """
+        It allows to set the counter value of provenance entities.
+
+        :param value: The new counter value to be set
+        :type value: bool
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id)
+
+        if not isinstance(value, bool):
+            raise ValueError("value must be boolean")
+        if id_name in self.id_value_dict:
+            self.id_value_dict[id_name]["valid"] = value
+        else:
+            self.id_value_dict[id_name] = {"valid": value}
+
+    def get_value(self, id: str):
+        """
+        It allows to read the value of the "valid" key of the identifier's dict.
+
+        :param id: The id name
+        :type id: str
+        :return: The requested id value.
+        """
+
+        id_name = str(id)
+        id_in_dict = self.id_value_dict.get(id_name)
+        if id_in_dict:
+            return id_in_dict["valid"]
+        else:
+            return None
+
+    def store_file(self) -> None:
+        """
+        It stores in a file the dictionary with the validation results
+        """
+        file = open(self.storage_filepath, "w", encoding='utf8')
+        json.dump(self.id_value_dict, file, indent=4)
+        file.close()
+
+    def delete_storage(self):
+        self.id_value_dict = dict()
+        if os.path.exists(self.storage_filepath):
+            os.remove(self.storage_filepath)
+
+    def get_all_keys(self):
+        return self.id_value_dict.keys()
+
+    def get_validity_dict(self):
+        return {k: v["valid"] for k, v in self.id_value_dict.items()}
+
+    def get_validity_list_of_tuples(self):
+        return [(k, v["valid"]) for k, v in self.id_value_dict.items()]
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.datasource.redis import RedisDataSource
-import fakeredis
-
-class RedisStorageManager(StorageManager):
-    """A concrete implementation of the ``StorageManager`` interface that persistently stores
-    the IDs validity values within a REDIS database."""
-
-    def __init__(self,  testing=True, config_filepath: str = 'config.ini', **params) -> None:
-        """
-        Constructor of the ``RedisStorageManager`` class.
-
-        :param database: The name of the database
-        :type info_dir: str
-        """
-        if testing:
-            self.testing = True
-            self.PROCESS_redis = fakeredis.FakeStrictRedis()
-        else:
-            self.testing = False
-            self.PROCESS_redis = RedisDataSource("PROCESS-DB", config_filepath)
-        super().__init__(**params)
-
-
-    def set_full_value(self, id_name: str, value: dict) -> None:
-        """
-        It allows to set the counter value of provenance entities.
-
-        :param value: The new counter value to be set
-        :type value: dict
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id_name)
-        if not isinstance(value, dict):
-            raise ValueError("value must be dict")
-        if not isinstance(self.get_value(id_name), bool):
-            id_val = True if value.get("valid") else False
-            self.set_value(id_name, id_val)
-
-    def set_value(self, id: str, value: bool) -> None :
-        """
-        It allows to set a value for the validity check of an id.
-
-        :param value: validity value for the validated id
-        :type value: bool
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id)
-        if not isinstance(value, bool):
-            raise ValueError("value must be int boolean")
-        validity = 1 if value else 0
-        self.PROCESS_redis.set(id_name, validity)
-
-
-    def set_multi_value(self, list_of_tuples: list) -> None :
-        """
-        It allows to set a value for the validity check of an id.
-
-        :param list_of_tuples: a list of tuples of ids and booleans (id, value)
-        :type list_of_tuples: list
-        :return: None
-        """
-        redis_dict = dict()
-        for t in list_of_tuples:
-            if t[1] is True:
-                redis_dict[t[0]] = 1
-            else:
-                redis_dict[t[0]] = 0
-        self.PROCESS_redis.mset(redis_dict)
-
-
-    def get_value(self, id: str):
-        """
-        It allows to read the value of the identifier.
-
-        :param id: The id name
-        :type id: str
-        :return: The requested id value (True if valid, False if invalid, None if not found).
-        """
-        id_name = str(id)
-        result = self.PROCESS_redis.get(id_name)
-        if result:
-            result = int(result.decode("utf-8")) if isinstance(result, bytes) else int(result)
-            return True if result == 1 else False
-        return None
-
-    def del_value(self, id: str) -> None:
-        """
-        It allows to delete the identifier from the redis db.
-
-        :param id: The id name
-        :type id: str
-        :return: None
-        """
-        self.PROCESS_redis.delete(id)
-
-
-    def delete_storage(self):
-        self.PROCESS_redis.flushall()
-
-    def get_all_keys(self):
-        result = [x for x in self.PROCESS_redis.scan_iter('*')]
-        if result:
-            if isinstance(result[0], bytes):
-                result = {x.decode("utf-8") for x in result}
-            else:
-                result = set(result)
-        else:
-            result = set()
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.datasource.redis import RedisDataSource
+import fakeredis
+
+class RedisStorageManager(StorageManager):
+    """A concrete implementation of the ``StorageManager`` interface that persistently stores
+    the IDs validity values within a REDIS database."""
+
+    def __init__(self,  testing=True, config_filepath: str = 'config.ini', **params) -> None:
+        """
+        Constructor of the ``RedisStorageManager`` class.
+
+        :param database: The name of the database
+        :type info_dir: str
+        """
+        if testing:
+            self.testing = True
+            self.PROCESS_redis = fakeredis.FakeStrictRedis()
+        else:
+            self.testing = False
+            self.PROCESS_redis = RedisDataSource("PROCESS-DB", config_filepath)
+        super().__init__(**params)
+
+
+    def set_full_value(self, id_name: str, value: dict) -> None:
+        """
+        It allows to set the counter value of provenance entities.
+
+        :param value: The new counter value to be set
+        :type value: dict
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id_name)
+        if not isinstance(value, dict):
+            raise ValueError("value must be dict")
+        if not isinstance(self.get_value(id_name), bool):
+            id_val = True if value.get("valid") else False
+            self.set_value(id_name, id_val)
+
+    def set_value(self, id: str, value: bool) -> None :
+        """
+        It allows to set a value for the validity check of an id.
+
+        :param value: validity value for the validated id
+        :type value: bool
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id)
+        if not isinstance(value, bool):
+            raise ValueError("value must be int boolean")
+        validity = 1 if value else 0
+        self.PROCESS_redis.set(id_name, validity)
+
+
+    def set_multi_value(self, list_of_tuples: list) -> None :
+        """
+        It allows to set a value for the validity check of an id.
+
+        :param list_of_tuples: a list of tuples of ids and booleans (id, value)
+        :type list_of_tuples: list
+        :return: None
+        """
+        redis_dict = dict()
+        for t in list_of_tuples:
+            if t[1] is True:
+                redis_dict[t[0]] = 1
+            else:
+                redis_dict[t[0]] = 0
+        self.PROCESS_redis.mset(redis_dict)
+
+
+    def get_value(self, id: str):
+        """
+        It allows to read the value of the identifier.
+
+        :param id: The id name
+        :type id: str
+        :return: The requested id value (True if valid, False if invalid, None if not found).
+        """
+        id_name = str(id)
+        result = self.PROCESS_redis.get(id_name)
+        if result:
+            result = int(result.decode("utf-8")) if isinstance(result, bytes) else int(result)
+            return True if result == 1 else False
+        return None
+
+    def del_value(self, id: str) -> None:
+        """
+        It allows to delete the identifier from the redis db.
+
+        :param id: The id name
+        :type id: str
+        :return: None
+        """
+        self.PROCESS_redis.delete(id)
+
+
+    def delete_storage(self):
+        self.PROCESS_redis.flushall()
+
+    def get_all_keys(self):
+        result = [x for x in self.PROCESS_redis.scan_iter('*')]
+        if result:
+            if isinstance(result[0], bytes):
+                result = {x.decode("utf-8") for x in result}
+            else:
+                result = set(result)
+        else:
+            result = set()
         return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-import os.path
-import sqlite3
-import pathlib
-import urllib.parse
-from typing import Optional
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-
-
-class SqliteStorageManager(StorageManager):
-    """A concrete implementation of the ``StorageManager`` interface that persistently stores
-    the IDs validity values within a SQLite database."""
-
-    def __init__(self, database:Optional[str] = None, **params) -> None:
-        """
-        Constructor of the ``SqliteStorageManager`` class.
-
-        :param database: The name of the database
-        :type info_dir: str
-        """
-        super().__init__(**params)
-        sqlite3.threadsafety = 3
-        if database and os.path.exists(database):
-            self.con = sqlite3.connect(database=database)
-            self.storage_filepath = database
-        elif database and not os.path.exists(database):
-            if not os.path.exists(os.path.abspath(os.path.join(database, os.pardir))):
-                pathlib.Path(os.path.abspath(os.path.join(database, os.pardir))).mkdir(parents=True, exist_ok=True)
-            self.con = sqlite3.connect(database=database)
-            self.storage_filepath =database
-
-        else:
-            new_path_dir = os.path.join(os.getcwd(), "storage")
-            if not os.path.exists(new_path_dir):
-                os.makedirs(new_path_dir)
-            new_path_db = os.path.join(new_path_dir, "id_valid_dict.db")
-
-            self.con = sqlite3.connect(database=new_path_db)
-            self.storage_filepath =new_path_db
-
-        self.cur = self.con.cursor()
-        self.cur.execute("""CREATE TABLE IF NOT EXISTS info(
-            id TEXT PRIMARY KEY, 
-            value INTEGER)""")
-
-    def set_full_value(self, id_name: str, value: dict) -> None:
-        """
-        It allows to set the counter value of provenance entities.
-
-        :param value: The new counter value to be set
-        :type value: dict
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id)
-        if not isinstance(value, dict):
-            raise ValueError("value must be dict")
-        if not isinstance(self.get_value(id_name), bool):
-            self.set_value(id_name, value["valid"])
-
-    def set_value(self, id: str, value: bool) -> None :
-        """
-        It allows to set a value for the validity check of an id.
-
-        :param value: The new counter value to be set
-        :type value: bool
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        id_name = str(id)
-        if not isinstance(value, bool):
-            raise ValueError("value must be int boolean")
-        validity = 1 if value else 0
-        id_val = (id_name, validity)
-        self.cur.execute(f"INSERT OR REPLACE INTO info VALUES (?,?)", id_val)
-        self.con.commit()
-
-    def set_multi_value(self, list_of_tuples: list) -> None :
-        """
-        It allows to set a value for the validity check of an id.
-
-        :param value: The new counter value to be set
-        :type value: bool
-        :param id: The id string with prefix
-        :type id: str
-        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
-        :return: None
-        """
-        sqlite_list_copy = []
-        for t in list_of_tuples:
-            if t[1] is True:
-                sqlite_list_copy.append((t[0], 1))
-            else:
-                sqlite_list_copy.append((t[0], 0))
-
-        self.cur.executemany(f"INSERT OR REPLACE INTO info VALUES (?,?)", sqlite_list_copy)
-        self.con.commit()
-
-    def get_value(self, id: str):
-        """
-        It allows to read the value of the identifier.
-
-        :param id: The id name
-        :type id: str
-        :return: The requested id value (True if valid, False if invalid, None if not found).
-        """
-        id_name = str(id)
-        result = self.cur.execute(f"SELECT value FROM info WHERE id='{id_name}'")
-        rows = result.fetchall()
-        if len(rows) == 1:
-            value = rows[0][0]
-            return True if value == 1 else False
-        elif len(rows) == 0:
-            return None
-        else:
-            raise(Exception("There is more than one counter for this id. The databse id broken"))
-
-    def delete_storage(self):
-        if os.path.exists(self.storage_filepath):
-            try:
-                self.con.close()
-                os.remove(self.storage_filepath)
-            except:
-                os.remove(self.storage_filepath)
-
-
-    def get_all_keys(self):
-        ids = [id[0] for id in self.cur.execute("SELECT id FROM info")]
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+import os.path
+import sqlite3
+import pathlib
+import urllib.parse
+from typing import Optional
+
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+
+
+class SqliteStorageManager(StorageManager):
+    """A concrete implementation of the ``StorageManager`` interface that persistently stores
+    the IDs validity values within a SQLite database."""
+
+    def __init__(self, database:Optional[str] = None, **params) -> None:
+        """
+        Constructor of the ``SqliteStorageManager`` class.
+
+        :param database: The name of the database
+        :type info_dir: str
+        """
+        super().__init__(**params)
+        sqlite3.threadsafety = 3
+        if database and os.path.exists(database):
+            self.con = sqlite3.connect(database=database)
+            self.storage_filepath = database
+        elif database and not os.path.exists(database):
+            if not os.path.exists(os.path.abspath(os.path.join(database, os.pardir))):
+                pathlib.Path(os.path.abspath(os.path.join(database, os.pardir))).mkdir(parents=True, exist_ok=True)
+            self.con = sqlite3.connect(database=database)
+            self.storage_filepath =database
+
+        else:
+            new_path_dir = os.path.join(os.getcwd(), "storage")
+            if not os.path.exists(new_path_dir):
+                os.makedirs(new_path_dir)
+            new_path_db = os.path.join(new_path_dir, "id_valid_dict.db")
+
+            self.con = sqlite3.connect(database=new_path_db)
+            self.storage_filepath =new_path_db
+
+        self.cur = self.con.cursor()
+        self.cur.execute("""CREATE TABLE IF NOT EXISTS info(
+            id TEXT PRIMARY KEY, 
+            value INTEGER)""")
+
+    def set_full_value(self, id_name: str, value: dict) -> None:
+        """
+        It allows to set the counter value of provenance entities.
+
+        :param value: The new counter value to be set
+        :type value: dict
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id)
+        if not isinstance(value, dict):
+            raise ValueError("value must be dict")
+        if not isinstance(self.get_value(id_name), bool):
+            self.set_value(id_name, value["valid"])
+
+    def set_value(self, id: str, value: bool) -> None :
+        """
+        It allows to set a value for the validity check of an id.
+
+        :param value: The new counter value to be set
+        :type value: bool
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        id_name = str(id)
+        if not isinstance(value, bool):
+            raise ValueError("value must be int boolean")
+        validity = 1 if value else 0
+        id_val = (id_name, validity)
+        self.cur.execute(f"INSERT OR REPLACE INTO info VALUES (?,?)", id_val)
+        self.con.commit()
+
+    def set_multi_value(self, list_of_tuples: list) -> None :
+        """
+        It allows to set a value for the validity check of an id.
+
+        :param value: The new counter value to be set
+        :type value: bool
+        :param id: The id string with prefix
+        :type id: str
+        :raises ValueError: if ``value`` is neither 0 nor 1 (0 is False, 1 is True).
+        :return: None
+        """
+        sqlite_list_copy = []
+        for t in list_of_tuples:
+            if t[1] is True:
+                sqlite_list_copy.append((t[0], 1))
+            else:
+                sqlite_list_copy.append((t[0], 0))
+
+        self.cur.executemany(f"INSERT OR REPLACE INTO info VALUES (?,?)", sqlite_list_copy)
+        self.con.commit()
+
+    def get_value(self, id: str):
+        """
+        It allows to read the value of the identifier.
+
+        :param id: The id name
+        :type id: str
+        :return: The requested id value (True if valid, False if invalid, None if not found).
+        """
+        id_name = str(id)
+        result = self.cur.execute(f"SELECT value FROM info WHERE id='{id_name}'")
+        rows = result.fetchall()
+        if len(rows) == 1:
+            value = rows[0][0]
+            return True if value == 1 else False
+        elif len(rows) == 0:
+            return None
+        else:
+            raise(Exception("There is more than one counter for this id. The databse id broken"))
+
+    def delete_storage(self):
+        if os.path.exists(self.storage_filepath):
+            try:
+                self.con.close()
+                os.remove(self.storage_filepath)
+            except:
+                os.remove(self.storage_filepath)
+
+
+    def get_all_keys(self):
+        ids = [id[0] for id in self.cur.execute("SELECT id FROM info")]
         return ids
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from abc import ABCMeta, abstractmethod
-
-class StorageManager(metaclass=ABCMeta):
-    """This is the interface that must be implemented by any Storage manager
-    for a particular storage approach. It provides the signatures of the methods
-    for string and retrieving data."""
-
-    def __init__(self, **params):
-        self.cur = None
-        self.con = None
-        """Storage manager constructor."""
-        for key in params:
-            setattr(self, key, params[key])
-
-        self._headers = {
-            "User-Agent": "Identifier Manager / OpenCitations Indexes "
-            "(http://opencitations.net; mailto:contact@opencitations.net)"
-        }
-
-    def set_value(self, id, value):
-        pass
-
-    def set_full_value(self, id, value):
-        pass
-
-    def get_value(self, id):
-        pass
-
-    def set_multi_value(self, list_of_tuples):
-        pass
-
-    def delete_storage(self):
-        pass
-
-    def store_file(self):
-        pass
-
-    def get_all_keys(self):
-        pass
-
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from abc import ABCMeta, abstractmethod
+
+class StorageManager(metaclass=ABCMeta):
+    """This is the interface that must be implemented by any Storage manager
+    for a particular storage approach. It provides the signatures of the methods
+    for string and retrieving data."""
+
+    def __init__(self, **params):
+        self.cur = None
+        self.con = None
+        """Storage manager constructor."""
+        for key in params:
+            setattr(self, key, params[key])
+
+        self._headers = {
+            "User-Agent": "Identifier Manager / OpenCitations Indexes "
+            "(http://opencitations.net; mailto:contact@opencitations.net)"
+        }
+
+    def set_value(self, id, value):
+        pass
+
+    def set_full_value(self, id, value):
+        pass
+
+    def get_value(self, id):
+        pass
+
+    def set_multi_value(self, list_of_tuples):
+        pass
+
+    def delete_storage(self):
+        pass
+
+    def store_file(self):
+        pass
+
+    def get_all_keys(self):
+        pass
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/pmid.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/pmid.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,391 +1,391 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import re
-from datetime import datetime
-from re import match, sub
-from time import sleep
-from urllib.parse import quote
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager import *
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Optional, Type
-
-
-
-class PMIDManager(IdentifierManager):
-    """This class implements an identifier manager for pmid identifier"""
-
-    def __init__(self, use_api_service=True,  storage_manager: Optional[StorageManager] = None):
-        """PMID manager constructor."""
-        super(PMIDManager, self).__init__()
-        self._api = "https://pubmed.ncbi.nlm.nih.gov/"
-        self._use_api_service = use_api_service
-        if storage_manager is None:
-            self.storage_manager = InMemoryStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self._p = "pmid:"
-        self._im = ISSNManager()
-        #regex
-        self._doi_regex = r"(?<=^AID\s-\s).*\[doi\]\s*\n"
-        self._pmid_regex = r"(?<=PMID-\s)[1-9]\d*"
-        self._title_regex = r"(?<=^TI\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._author_regex = r"(?<=^FAU\s-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._date_regex = r"DP\s+-\s+(\d{4}(\s?(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec))?(\s?((3[0-1])|([1-2][0-9])|([0]?[1-9])))?)"
-        self._issn_regex = r"(?<=^IS\s{2}-\s)[0-9]{4}-[0-9]{3}[0-9X]"
-        self._journal_regex = r"(?<=^JT\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._volume_regex = r"(?<=^VI\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._issue_regex = r"(?<=^IP\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._page_regex = r"(?<=^PG\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._type_regex = r"(?<=^PT\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._publisher_regex = r"(?<=^PB\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-        self._editor_regex = r"((?<=^FED\s-\s)|(?<=^ED\s{2}-\s))(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
-
-    def validated_as_id(self, id_string):
-        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
-        if isinstance(arxiv_vaidation_value, bool):
-            return arxiv_vaidation_value
-        else:
-            return None
-
-    def is_valid(self, pmid, get_extra_info=False):
-        pmid = self.normalise(pmid, include_prefix=True)
-
-        if not pmid:
-            return False
-        else:
-            pmid_vaidation_value = self.storage_manager.get_value(pmid)
-            if isinstance(pmid_vaidation_value, bool):
-                return pmid_vaidation_value
-            else:
-                if get_extra_info:
-                    info = self.exists(pmid, get_extra_info=True)
-                    self.storage_manager.set_full_value(pmid,info[1])
-                    return (info[0] and self.syntax_ok(pmid)), info[1]
-                validity_check = self.exists(pmid) and self.syntax_ok(pmid)
-                self.storage_manager.set_value(pmid, validity_check)
-
-                return validity_check
-
-
-
-    def normalise(self, id_string, include_prefix=False):
-        id_string = str(id_string)
-        try:
-            pmid_string = sub("^0+", "", sub("\0+", "", (sub("[^\d+]", "", id_string))))
-            return "%s%s" % (self._p if include_prefix else "", pmid_string)
-        except:
-            # Any error in processing the PMID will return None
-            return None
-
-    def syntax_ok(self, id_string):
-        if not id_string.startswith(self._p):
-            id_string = self._p + id_string
-        return True if match("^pmid:[1-9]\d*$", id_string) else False
-
-    def exists(self, pmid_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        pmid = pmid_full
-        pmid_p = "pmid:"+pmid if not pmid.startswith("pmid:") else pmid
-        if self._use_api_service:
-            pmid = self.normalise(pmid_full)
-            pmid_p = self.normalise(pmid_full, include_prefix=True)
-            if pmid is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(
-                            self._api + quote(pmid) + "/?format=pubmed",
-                            headers=self._headers,
-                            timeout=30,
-                        )
-                        if r.status_code == 200:
-                            r.encoding = "utf-8"
-                            soup = BeautifulSoup(r.text, features="lxml")
-                            txt_obj = str(soup.find(id="article-details"))
-                            match_pmid = re.finditer(self._pmid_regex, txt_obj, re.MULTILINE)
-                            for matchNum_pmid, match_p in enumerate(match_pmid, start=1):
-                                m_pmid = match_p.group()
-                                if m_pmid:
-                                    if get_extra_info:
-                                        result = self.extra_info(txt_obj)
-                                        result["id"] = pmid_p
-                                        return True, result
-                                    return True
-                        elif r.status_code == 404:
-                            if get_extra_info:
-                                return False, {"id":pmid_p, "valid": False}
-                            return False
-
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-                valid_bool = False
-            else:
-                if get_extra_info:
-                    return False, {"id":pmid_p, "valid": False}
-                return False
-        if get_extra_info:
-            return valid_bool, {"id":pmid_p, "valid": valid_bool}
-        return valid_bool
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-
-        try:
-            title = ""
-            match_title = re.finditer(self._title_regex, api_response, re.MULTILINE)
-            for matchNum_tit, match_tit in enumerate(match_title, start=1):
-                m_title = match_tit.group()
-                if m_title:
-                    ts = re.sub("\s+", " ", m_title)
-                    t = re.sub("\n", " ", ts)
-                    norm_title = t.strip()
-                    if norm_title is not None:
-                        title = norm_title
-                        break
-        except:
-            title = ""
-
-        result["title"] = title
-
-        try:
-            authors = set()
-            fa_aut = re.finditer(self._author_regex, api_response, re.MULTILINE)
-            for matchNum_aut, match_au in enumerate(fa_aut, start=1):
-                m_aut = match_au.group()
-                if m_aut:
-                    fau = re.sub("\s+", " ", m_aut)
-                    nlfau = re.sub("\n", " ", fau)
-                    norm_fau = nlfau.strip()
-                    if norm_fau is not None:
-                        authors.add(norm_fau)
-            authorsList = list(authors)
-        except:
-            authorsList = []
-
-        result["author"] = authorsList
-
-        try:
-            date = re.search(self._date_regex,
-                api_response,
-                re.IGNORECASE,
-            ).group(1)
-            re_search = re.search(
-                "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s+((3[0-1])|([1-2][0-9])|([0]?[1-9]))",
-                date,
-                re.IGNORECASE,
-            )
-            if re_search is not None:
-                src = re_search.group(0)
-                datetime_object = datetime.strptime(src, "%Y %b %d")
-                pmid_date = datetime.strftime(datetime_object, "%Y-%m-%d")
-            else:
-                re_search = re.search(
-                    "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)",
-                    date,
-                    re.IGNORECASE,
-                )
-                if re_search is not None:
-                    src = re_search.group(0)
-                    datetime_object = datetime.strptime(src, "%Y %b")
-                    pmid_date = datetime.strftime(datetime_object, "%Y-%m")
-                else:
-                    re_search = re.search("(\d{4})", date)
-                    if re_search is not None:
-                        src = re.search("(\d{4})", date).group(0)
-                        datetime_object = datetime.strptime(src, "%Y")
-                        pmid_date = datetime.strftime(datetime_object, "%Y")
-                    else:
-                        pmid_date = ""
-        except:
-            pmid_date = ""
-        result["pub_date"] = pmid_date
-
-        try:
-            issnset = set()
-            fa_issn = re.finditer(self._issn_regex, api_response, re.MULTILINE)
-            for matchNum_issn, match_issn in enumerate(fa_issn, start=1):
-                m_issn = match_issn.group()
-                if m_issn:
-                    norm_issn = self._im.normalise(m_issn, include_prefix=True)
-                    if norm_issn is not None:
-                        issnset.add(norm_issn)
-            issnlist = list(issnset)
-        except:
-            issnlist = []
-
-        # CONTINUA DA QUI
-
-        try:
-            jur_title = ""
-            fa_jur_title = re.finditer(self._journal_regex, api_response, re.MULTILINE)
-            for matchNum_title, match_tit in enumerate(fa_jur_title, start=1):
-                m_title = match_tit.group()
-                if m_title:
-                    s_jt = re.sub("\s+", " ", m_title)
-                    n_jt = re.sub("\n", " ", s_jt)
-                    norm_jour = n_jt.strip()
-                    if norm_jour is not None:
-                        jur_title = norm_jour
-                        break
-        except:
-            jur_title = ""
-
-        result["venue"] = (
-            f'{jur_title} {[x for x in issnlist]}' if jur_title else str(issnlist).replace(",", "")).replace("'", "")
-
-        try:
-            volume = ""
-            fa_volume = re.finditer(self._volume_regex, api_response, re.MULTILINE)
-            for matchNum_volume, match_vol in enumerate(fa_volume, start=1):
-                m_vol = match_vol.group()
-                if m_vol:
-                    vol = re.sub("\s+", " ", m_vol)
-                    norm_volume = vol.strip()
-                    if norm_volume is not None:
-                        volume = norm_volume
-                        break
-        except:
-            volume = ""
-
-        result["volume"] = volume
-
-        try:
-            issue = ""
-            fa_issue = re.finditer(self._issue_regex, api_response, re.MULTILINE)
-            for matchNum_issue, match_issue in enumerate(fa_issue, start=1):
-                m_issue = match_issue.group()
-                if m_issue:
-                    s_issue = re.sub("\s+", " ", m_issue)
-                    n_issue = re.sub("\n", " ", s_issue)
-                    norm_issue = n_issue.strip()
-                    if norm_issue is not None:
-                        issue = norm_issue
-                        break
-        except:
-            issue = ""
-
-        result["issue"] = issue
-
-        try:
-            pag = ""
-            fa_pag = re.finditer(self._page_regex, api_response, re.MULTILINE)
-            for matchNum_pag, match_pag in enumerate(fa_pag, start=1):
-                m_pag = match_pag.group()
-                if m_pag:
-                    s_pg = re.sub("\s+", " ", m_pag)
-                    n_pg = re.sub("\n", " ", s_pg)
-                    norm_pag = n_pg.strip()
-                    if norm_pag is not None:
-                        pag = norm_pag
-                        break
-        except:
-            pag = ""
-
-        result["page"] = pag
-
-        try:
-            pub_types = set()
-            types = re.finditer(self._type_regex, api_response, re.MULTILINE)
-            for matchNum_types, match_types in enumerate(types, start=1):
-                m_type = match_types.group()
-                if m_type:
-                    s_ty = re.sub("\s+", " ", m_type)
-                    b_ty = re.sub("\n", " ", s_ty)
-                    norm_type = b_ty.strip().lower()
-                    if norm_type is not None:
-                        pub_types.add(norm_type)
-            typeslist = list(pub_types)
-        except:
-            typeslist = []
-
-        result["type"] = typeslist
-
-        try:
-            publisher = set()
-            publishers = re.finditer(self._publisher_regex, api_response, re.MULTILINE)
-            for matchNum_publishers, match_publishers in enumerate(publishers, start=1):
-                m_publishers = match_publishers.group()
-                if m_publishers:
-                    s_pbs = re.sub("\s+", " ", m_publishers)
-                    n_pbs = re.sub("\n", " ", s_pbs)
-                    norm_pbs = n_pbs.strip()
-                    if norm_pbs is not None:
-                        publisher.add(norm_pbs)
-            publisherlist = list(publisher)
-        except:
-            publisherlist = []
-
-        result["publisher"] = publisherlist
-
-        try:
-            editor = set()
-            editors = re.finditer(self._editor_regex, api_response, re.MULTILINE)
-            for matchNum_editors, match_editors in enumerate(editors, start=1):
-                m_editors = match_editors.group()
-                if m_editors:
-                    s_ed = re.sub("\s+", " ", m_editors)
-                    n_ed = re.sub("\n", " ", s_ed)
-                    norm_ed = n_ed.strip()
-                    if norm_ed is not None:
-                        editor.add(norm_ed)
-            editorlist = list(editor)
-        except:
-            editorlist = []
-
-        result["editor"] = editorlist
-
-        doi = ""
-        try:
-            map_doi = re.finditer(self._doi_regex, api_response, re.MULTILINE)
-            for matchNum_doi, match_doi in enumerate(map_doi, start=1):
-                m_doi = match_doi.group()
-                if m_doi:
-                    id = re.sub("\s+", " ", m_doi)
-                    n_id = re.sub("\n", " ", id)
-                    n_id_strip = n_id.strip()
-
-                    if n_id_strip.endswith('[doi]'):
-                        n_id_strip = n_id_strip[:-5]
-                    dm = DOIManager()
-                    norm_id = dm.normalise(n_id_strip)
-                    if norm_id is not None:
-                        doi = norm_id
-                        break
-                    else:
-                        doi = ""
-        except:
-            doi = ""
-
-        result["doi"] = doi
-
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import re
+from datetime import datetime
+from re import match, sub
+from time import sleep
+from urllib.parse import quote
+
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager import *
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
+from typing import Optional, Type
+
+
+
+class PMIDManager(IdentifierManager):
+    """This class implements an identifier manager for pmid identifier"""
+
+    def __init__(self, use_api_service=True,  storage_manager: Optional[StorageManager] = None):
+        """PMID manager constructor."""
+        super(PMIDManager, self).__init__()
+        self._api = "https://pubmed.ncbi.nlm.nih.gov/"
+        self._use_api_service = use_api_service
+        if storage_manager is None:
+            self.storage_manager = InMemoryStorageManager()
+        else:
+            self.storage_manager = storage_manager
+
+        self._p = "pmid:"
+        self._im = ISSNManager()
+        #regex
+        self._doi_regex = r"(?<=^AID\s-\s).*\[doi\]\s*\n"
+        self._pmid_regex = r"(?<=PMID-\s)[1-9]\d*"
+        self._title_regex = r"(?<=^TI\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._author_regex = r"(?<=^FAU\s-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._date_regex = r"DP\s+-\s+(\d{4}(\s?(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec))?(\s?((3[0-1])|([1-2][0-9])|([0]?[1-9])))?)"
+        self._issn_regex = r"(?<=^IS\s{2}-\s)[0-9]{4}-[0-9]{3}[0-9X]"
+        self._journal_regex = r"(?<=^JT\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._volume_regex = r"(?<=^VI\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._issue_regex = r"(?<=^IP\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._page_regex = r"(?<=^PG\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._type_regex = r"(?<=^PT\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._publisher_regex = r"(?<=^PB\s{2}-\s)(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+        self._editor_regex = r"((?<=^FED\s-\s)|(?<=^ED\s{2}-\s))(.+?)*(\n\s{6}(.+?)*)*(?=(?:\n[A-Z]{2,4}\s{,2}-\s*|$))"
+
+    def validated_as_id(self, id_string):
+        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
+        if isinstance(arxiv_vaidation_value, bool):
+            return arxiv_vaidation_value
+        else:
+            return None
+
+    def is_valid(self, pmid, get_extra_info=False):
+        pmid = self.normalise(pmid, include_prefix=True)
+
+        if not pmid:
+            return False
+        else:
+            pmid_vaidation_value = self.storage_manager.get_value(pmid)
+            if isinstance(pmid_vaidation_value, bool):
+                return pmid_vaidation_value
+            else:
+                if get_extra_info:
+                    info = self.exists(pmid, get_extra_info=True)
+                    self.storage_manager.set_full_value(pmid,info[1])
+                    return (info[0] and self.syntax_ok(pmid)), info[1]
+                validity_check = self.exists(pmid) and self.syntax_ok(pmid)
+                self.storage_manager.set_value(pmid, validity_check)
+
+                return validity_check
+
+
+
+    def normalise(self, id_string, include_prefix=False):
+        id_string = str(id_string)
+        try:
+            pmid_string = sub("^0+", "", sub("\0+", "", (sub("[^\d+]", "", id_string))))
+            return "%s%s" % (self._p if include_prefix else "", pmid_string)
+        except:
+            # Any error in processing the PMID will return None
+            return None
+
+    def syntax_ok(self, id_string):
+        if not id_string.startswith(self._p):
+            id_string = self._p + id_string
+        return True if match("^pmid:[1-9]\d*$", id_string) else False
+
+    def exists(self, pmid_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        pmid = pmid_full
+        pmid_p = "pmid:"+pmid if not pmid.startswith("pmid:") else pmid
+        if self._use_api_service:
+            pmid = self.normalise(pmid_full)
+            pmid_p = self.normalise(pmid_full, include_prefix=True)
+            if pmid is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(
+                            self._api + quote(pmid) + "/?format=pubmed",
+                            headers=self._headers,
+                            timeout=30,
+                        )
+                        if r.status_code == 200:
+                            r.encoding = "utf-8"
+                            soup = BeautifulSoup(r.text, features="lxml")
+                            txt_obj = str(soup.find(id="article-details"))
+                            match_pmid = re.finditer(self._pmid_regex, txt_obj, re.MULTILINE)
+                            for matchNum_pmid, match_p in enumerate(match_pmid, start=1):
+                                m_pmid = match_p.group()
+                                if m_pmid:
+                                    if get_extra_info:
+                                        result = self.extra_info(txt_obj)
+                                        result["id"] = pmid_p
+                                        return True, result
+                                    return True
+                        elif r.status_code == 404:
+                            if get_extra_info:
+                                return False, {"id":pmid_p, "valid": False}
+                            return False
+
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool = False
+            else:
+                if get_extra_info:
+                    return False, {"id":pmid_p, "valid": False}
+                return False
+        if get_extra_info:
+            return valid_bool, {"id":pmid_p, "valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+
+        try:
+            title = ""
+            match_title = re.finditer(self._title_regex, api_response, re.MULTILINE)
+            for matchNum_tit, match_tit in enumerate(match_title, start=1):
+                m_title = match_tit.group()
+                if m_title:
+                    ts = re.sub("\s+", " ", m_title)
+                    t = re.sub("\n", " ", ts)
+                    norm_title = t.strip()
+                    if norm_title is not None:
+                        title = norm_title
+                        break
+        except:
+            title = ""
+
+        result["title"] = title
+
+        try:
+            authors = set()
+            fa_aut = re.finditer(self._author_regex, api_response, re.MULTILINE)
+            for matchNum_aut, match_au in enumerate(fa_aut, start=1):
+                m_aut = match_au.group()
+                if m_aut:
+                    fau = re.sub("\s+", " ", m_aut)
+                    nlfau = re.sub("\n", " ", fau)
+                    norm_fau = nlfau.strip()
+                    if norm_fau is not None:
+                        authors.add(norm_fau)
+            authorsList = list(authors)
+        except:
+            authorsList = []
+
+        result["author"] = authorsList
+
+        try:
+            date = re.search(self._date_regex,
+                api_response,
+                re.IGNORECASE,
+            ).group(1)
+            re_search = re.search(
+                "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s+((3[0-1])|([1-2][0-9])|([0]?[1-9]))",
+                date,
+                re.IGNORECASE,
+            )
+            if re_search is not None:
+                src = re_search.group(0)
+                datetime_object = datetime.strptime(src, "%Y %b %d")
+                pmid_date = datetime.strftime(datetime_object, "%Y-%m-%d")
+            else:
+                re_search = re.search(
+                    "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)",
+                    date,
+                    re.IGNORECASE,
+                )
+                if re_search is not None:
+                    src = re_search.group(0)
+                    datetime_object = datetime.strptime(src, "%Y %b")
+                    pmid_date = datetime.strftime(datetime_object, "%Y-%m")
+                else:
+                    re_search = re.search("(\d{4})", date)
+                    if re_search is not None:
+                        src = re.search("(\d{4})", date).group(0)
+                        datetime_object = datetime.strptime(src, "%Y")
+                        pmid_date = datetime.strftime(datetime_object, "%Y")
+                    else:
+                        pmid_date = ""
+        except:
+            pmid_date = ""
+        result["pub_date"] = pmid_date
+
+        try:
+            issnset = set()
+            fa_issn = re.finditer(self._issn_regex, api_response, re.MULTILINE)
+            for matchNum_issn, match_issn in enumerate(fa_issn, start=1):
+                m_issn = match_issn.group()
+                if m_issn:
+                    norm_issn = self._im.normalise(m_issn, include_prefix=True)
+                    if norm_issn is not None:
+                        issnset.add(norm_issn)
+            issnlist = list(issnset)
+        except:
+            issnlist = []
+
+        # CONTINUA DA QUI
+
+        try:
+            jur_title = ""
+            fa_jur_title = re.finditer(self._journal_regex, api_response, re.MULTILINE)
+            for matchNum_title, match_tit in enumerate(fa_jur_title, start=1):
+                m_title = match_tit.group()
+                if m_title:
+                    s_jt = re.sub("\s+", " ", m_title)
+                    n_jt = re.sub("\n", " ", s_jt)
+                    norm_jour = n_jt.strip()
+                    if norm_jour is not None:
+                        jur_title = norm_jour
+                        break
+        except:
+            jur_title = ""
+
+        result["venue"] = (
+            f'{jur_title} {[x for x in issnlist]}' if jur_title else str(issnlist).replace(",", "")).replace("'", "")
+
+        try:
+            volume = ""
+            fa_volume = re.finditer(self._volume_regex, api_response, re.MULTILINE)
+            for matchNum_volume, match_vol in enumerate(fa_volume, start=1):
+                m_vol = match_vol.group()
+                if m_vol:
+                    vol = re.sub("\s+", " ", m_vol)
+                    norm_volume = vol.strip()
+                    if norm_volume is not None:
+                        volume = norm_volume
+                        break
+        except:
+            volume = ""
+
+        result["volume"] = volume
+
+        try:
+            issue = ""
+            fa_issue = re.finditer(self._issue_regex, api_response, re.MULTILINE)
+            for matchNum_issue, match_issue in enumerate(fa_issue, start=1):
+                m_issue = match_issue.group()
+                if m_issue:
+                    s_issue = re.sub("\s+", " ", m_issue)
+                    n_issue = re.sub("\n", " ", s_issue)
+                    norm_issue = n_issue.strip()
+                    if norm_issue is not None:
+                        issue = norm_issue
+                        break
+        except:
+            issue = ""
+
+        result["issue"] = issue
+
+        try:
+            pag = ""
+            fa_pag = re.finditer(self._page_regex, api_response, re.MULTILINE)
+            for matchNum_pag, match_pag in enumerate(fa_pag, start=1):
+                m_pag = match_pag.group()
+                if m_pag:
+                    s_pg = re.sub("\s+", " ", m_pag)
+                    n_pg = re.sub("\n", " ", s_pg)
+                    norm_pag = n_pg.strip()
+                    if norm_pag is not None:
+                        pag = norm_pag
+                        break
+        except:
+            pag = ""
+
+        result["page"] = pag
+
+        try:
+            pub_types = set()
+            types = re.finditer(self._type_regex, api_response, re.MULTILINE)
+            for matchNum_types, match_types in enumerate(types, start=1):
+                m_type = match_types.group()
+                if m_type:
+                    s_ty = re.sub("\s+", " ", m_type)
+                    b_ty = re.sub("\n", " ", s_ty)
+                    norm_type = b_ty.strip().lower()
+                    if norm_type is not None:
+                        pub_types.add(norm_type)
+            typeslist = list(pub_types)
+        except:
+            typeslist = []
+
+        result["type"] = typeslist
+
+        try:
+            publisher = set()
+            publishers = re.finditer(self._publisher_regex, api_response, re.MULTILINE)
+            for matchNum_publishers, match_publishers in enumerate(publishers, start=1):
+                m_publishers = match_publishers.group()
+                if m_publishers:
+                    s_pbs = re.sub("\s+", " ", m_publishers)
+                    n_pbs = re.sub("\n", " ", s_pbs)
+                    norm_pbs = n_pbs.strip()
+                    if norm_pbs is not None:
+                        publisher.add(norm_pbs)
+            publisherlist = list(publisher)
+        except:
+            publisherlist = []
+
+        result["publisher"] = publisherlist
+
+        try:
+            editor = set()
+            editors = re.finditer(self._editor_regex, api_response, re.MULTILINE)
+            for matchNum_editors, match_editors in enumerate(editors, start=1):
+                m_editors = match_editors.group()
+                if m_editors:
+                    s_ed = re.sub("\s+", " ", m_editors)
+                    n_ed = re.sub("\n", " ", s_ed)
+                    norm_ed = n_ed.strip()
+                    if norm_ed is not None:
+                        editor.add(norm_ed)
+            editorlist = list(editor)
+        except:
+            editorlist = []
+
+        result["editor"] = editorlist
+
+        doi = ""
+        try:
+            map_doi = re.finditer(self._doi_regex, api_response, re.MULTILINE)
+            for matchNum_doi, match_doi in enumerate(map_doi, start=1):
+                m_doi = match_doi.group()
+                if m_doi:
+                    id = re.sub("\s+", " ", m_doi)
+                    n_id = re.sub("\n", " ", id)
+                    n_id_strip = n_id.strip()
+
+                    if n_id_strip.endswith('[doi]'):
+                        n_id_strip = n_id_strip[:-5]
+                    dm = DOIManager()
+                    norm_id = dm.normalise(n_id_strip)
+                    if norm_id is not None:
+                        doi = norm_id
+                        break
+                    else:
+                        doi = ""
+        except:
+            doi = ""
+
+        result["doi"] = doi
+
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/ror.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/ror.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from json import loads
-from re import match, sub
-from time import sleep
-from urllib.parse import quote, unquote
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-
-class RORManager(IdentifierManager):
-    """This class implements an identifier manager for ROR identifier"""
-
-    def __init__(self, data={}, use_api_service=True):
-        """PMCID manager constructor."""
-        super(RORManager, self).__init__()
-        self._api = "https://api.ror.org/organizations/"
-        self._use_api_service = use_api_service
-        self._p = "ror:"
-        self._data = data
-
-    def is_valid(self, ror_id, get_extra_info=False):
-        ror_id = self.normalise(ror_id, include_prefix=True)
-
-        if ror_id is None:
-            return False
-        else:
-            if ror_id not in self._data or self._data[ror_id] is None:
-                if get_extra_info:
-                    info = self.exists(ror_id, get_extra_info=True)
-                    self._data[ror_id] = info[1]
-                    return (info[0] and self.syntax_ok(ror_id)), info[1]
-                self._data[ror_id] = dict()
-                self._data[ror_id]["valid"] = True if (self.exists(ror_id) and self.syntax_ok(ror_id)) else False
-                return self._data[ror_id].get("valid")
-            if get_extra_info:
-                return self._data[ror_id].get("valid"), self._data[ror_id]
-            return self._data[ror_id].get("valid")
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            if id_string.startswith(self._p):
-                ror_id_string = id_string[len(self._p):]
-            else:
-                ror_id_string = id_string
-            #  normalize + remove protocol and domain name if they are included in the ID
-            ror_id_string = sub("\0+", "", sub("(https://)?ror\\.org/", "", sub('\s+', "", unquote(ror_id_string))))
-
-            return "%s%s" % (
-                self._p if include_prefix else "",
-                ror_id_string.strip(),
-            )
-        except:
-            # Any error in processing the ROR ID will return None
-            return None
-
-    def syntax_ok(self, id_string):
-        if not id_string.startswith("ror:"):
-            id_string = self._p + id_string
-        # the regex admits the identifier with or without the protocol and the domain name
-        return True if match(r"^ror:((https:\/\/)?ror\.org\/)?0[a-hj-km-np-tv-z|0-9]{6}[0-9]{2}$", id_string) else False
-
-    def exists(self, ror_id_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        if self._use_api_service:
-            ror_id = self.normalise(ror_id_full)
-            if ror_id is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(self._api + ror_id, headers=self._headers, timeout=30)
-                        if r.status_code == 200:
-                            r.encoding = "utf-8"
-                            json_res = loads(r.text)
-                            if get_extra_info:
-                                extra_info_result = {}
-                                try:
-                                    result = True if json_res['id'] else False
-                                    extra_info_result['valid'] = result
-                                    return result, extra_info_result
-                                except KeyError:
-                                    extra_info_result["valid"] = False
-                                    return False, extra_info_result
-                            try:
-                                return True if json_res['id'] else False
-                            except KeyError:
-                                return False
-
-                        elif 400 <= r.status_code < 500:
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-                valid_bool = False
-            else:
-                if get_extra_info:
-                    return False, {"valid": False}
-                return False
-
-        if get_extra_info:
-            return valid_bool, {"valid": valid_bool}
-        return valid_bool
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-        # to be implemented
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from json import loads
+from re import match, sub
+from time import sleep
+from urllib.parse import quote, unquote
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+
+class RORManager(IdentifierManager):
+    """This class implements an identifier manager for ROR identifier"""
+
+    def __init__(self, data={}, use_api_service=True):
+        """PMCID manager constructor."""
+        super(RORManager, self).__init__()
+        self._api = "https://api.ror.org/organizations/"
+        self._use_api_service = use_api_service
+        self._p = "ror:"
+        self._data = data
+
+    def is_valid(self, ror_id, get_extra_info=False):
+        ror_id = self.normalise(ror_id, include_prefix=True)
+
+        if ror_id is None:
+            return False
+        else:
+            if ror_id not in self._data or self._data[ror_id] is None:
+                if get_extra_info:
+                    info = self.exists(ror_id, get_extra_info=True)
+                    self._data[ror_id] = info[1]
+                    return (info[0] and self.syntax_ok(ror_id)), info[1]
+                self._data[ror_id] = dict()
+                self._data[ror_id]["valid"] = True if (self.exists(ror_id) and self.syntax_ok(ror_id)) else False
+                return self._data[ror_id].get("valid")
+            if get_extra_info:
+                return self._data[ror_id].get("valid"), self._data[ror_id]
+            return self._data[ror_id].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            if id_string.startswith(self._p):
+                ror_id_string = id_string[len(self._p):]
+            else:
+                ror_id_string = id_string
+            #  normalize + remove protocol and domain name if they are included in the ID
+            ror_id_string = sub("\0+", "", sub("(https://)?ror\\.org/", "", sub('\s+', "", unquote(ror_id_string))))
+
+            return "%s%s" % (
+                self._p if include_prefix else "",
+                ror_id_string.strip(),
+            )
+        except:
+            # Any error in processing the ROR ID will return None
+            return None
+
+    def syntax_ok(self, id_string):
+        if not id_string.startswith("ror:"):
+            id_string = self._p + id_string
+        # the regex admits the identifier with or without the protocol and the domain name
+        return True if match(r"^ror:((https:\/\/)?ror\.org\/)?0[a-hj-km-np-tv-z|0-9]{6}[0-9]{2}$", id_string) else False
+
+    def exists(self, ror_id_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self._use_api_service:
+            ror_id = self.normalise(ror_id_full)
+            if ror_id is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(self._api + ror_id, headers=self._headers, timeout=30)
+                        if r.status_code == 200:
+                            r.encoding = "utf-8"
+                            json_res = loads(r.text)
+                            if get_extra_info:
+                                extra_info_result = {}
+                                try:
+                                    result = True if json_res['id'] else False
+                                    extra_info_result['valid'] = result
+                                    return result, extra_info_result
+                                except KeyError:
+                                    extra_info_result["valid"] = False
+                                    return False, extra_info_result
+                            try:
+                                return True if json_res['id'] else False
+                            except KeyError:
+                                return False
+
+                        elif 400 <= r.status_code < 500:
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool = False
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        # to be implemented
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/support.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/support.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from __future__ import annotations
-
-from json import loads
-from time import sleep
-
-from bs4 import BeautifulSoup
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-
-def call_api(url:str, headers:str, r_format:str="json") -> dict|None:
-    tentative = 3
-    while tentative:
-        tentative -= 1
-        try:
-            r = get(url, headers=headers, timeout=30)
-            if r.status_code == 200:
-                r.encoding = "utf-8"
-                return loads(r.text) if r_format == "json" else BeautifulSoup(r.text, 'xml')
-            elif r.status_code == 404:
-                return None
-        except ReadTimeout:
-            # Do nothing, just try again
-            pass
-        except ConnectionError:
-            # Sleep 5 seconds, then try again
-            sleep(5)
-    return None
-
-def extract_info(api_response:dict, choose_api:str|None=None) -> dict:
-    from oc_ds_converter.oc_idmanager.metadata_manager import MetadataManager
-    info_dict = {'valid': True}
-    metadata_manager = MetadataManager(metadata_provider=choose_api, api_response=api_response)
-    info_dict.update(metadata_manager.extract_metadata())
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from __future__ import annotations
+
+from json import loads
+from time import sleep
+
+from bs4 import BeautifulSoup
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+
+def call_api(url:str, headers:str, r_format:str="json") -> dict|None:
+    tentative = 3
+    while tentative:
+        tentative -= 1
+        try:
+            r = get(url, headers=headers, timeout=30)
+            if r.status_code == 200:
+                r.encoding = "utf-8"
+                return loads(r.text) if r_format == "json" else BeautifulSoup(r.text, 'xml')
+            elif r.status_code == 404:
+                return None
+        except ReadTimeout:
+            # Do nothing, just try again
+            pass
+        except ConnectionError:
+            # Sleep 5 seconds, then try again
+            sleep(5)
+    return None
+
+def extract_info(api_response:dict, choose_api:str|None=None) -> dict:
+    from oc_ds_converter.oc_idmanager.metadata_manager import MetadataManager
+    info_dict = {'valid': True}
+    metadata_manager = MetadataManager(metadata_provider=choose_api, api_response=api_response)
+    info_dict.update(metadata_manager.extract_metadata())
     return info_dict
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/url.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/url.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import urllib.parse
-from time import sleep
-
-import validators
-from oc_ds_converter.oc_idmanager import *
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-
-class URLManager(IdentifierManager):
-    """This class implements an identifier manager for url identifier"""
-
-    def __init__(self, data={}, use_api_service=True):
-        """URL manager constructor."""
-        super(URLManager, self).__init__()
-        self._use_api_service = use_api_service
-        self._p = "url:"
-        self._data = data
-        self._scheme_https = "https://"
-        self._scheme_http = "http://"
-
-    def is_valid(self, url, get_extra_info=False):
-        url = self.normalise(url, include_prefix=True)
-        if url is None:
-            return False
-        else:
-            if url not in self._data or self._data[url] is None:
-                if get_extra_info:
-                    info = self.exists(url, get_extra_info=True)
-                    self._data[url] = info[1]
-                    return (info[0] and self.syntax_ok(url)), info[1]
-                self._data[url] = dict()
-                self._data[url]["valid"] = True if (self.exists(url) and self.syntax_ok(url)) else False
-                return self._data[url].get("valid")
-
-            if get_extra_info:
-                return self._data[url].get("valid"), self._data[url]
-            return self._data[url].get("valid")
-
-    def normalise(self, id_string, include_prefix=False):
-        id_string = str(id_string)
-        url_string = id_string.strip()
-        if url_string.startswith(self._p):
-            url_string = url_string[len(self._p):]
-        if url_string.endswith("/"):
-            url_string = url_string[:-1]
-        if url_string.startswith("https://"):
-            url_string = url_string[len("https://"):]
-        elif url_string.startswith("http://"):
-            url_string = url_string[len("http://"):]
-        if url_string.startswith("www."):
-            url_string = url_string[len("www."):]
-        try:
-            url_string = urllib.parse.quote(url_string, safe="%/:=&?~#+!$,;'@()*[]")
-            return "%s%s" % (self._p if include_prefix else "", url_string)
-        except:
-            # Any error in processing the URL will return None
-            return None
-
-    def syntax_ok(self, id_string):
-        if id_string.startswith(self._p):
-            id_string = id_string[len(self._p):]
-        return True if validators.url(self._scheme_https + id_string) else False
-
-    def exists(self, url_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        if self._use_api_service:
-            url = self.normalise(url_full)
-            if url is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(self._scheme_https + url,
-                            headers=self._headers,
-                            timeout=30,
-                        )
-                        if r.status_code == 200:
-                            if get_extra_info:
-                                return True, {"valid": True}
-                            return True
-                        elif r.status_code == 404:
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-
-                try:
-                    r = get(self._scheme_http + url,
-                            headers=self._headers,
-                            timeout=30,
-                            )
-                    if r.status_code == 200:
-                        if get_extra_info:
-                            return True, {"valid": True}
-                        return True
-                    elif r.status_code == 404:
-                        if get_extra_info:
-                            return False, {"valid": False}
-                        return False
-                except ReadTimeout:
-                    # Do nothing, just try again
-                    pass
-                except ConnectionError:
-                    # Sleep 5 seconds, then try again
-                    sleep(5)
-
-                valid_bool = False
-
-            else:
-                if get_extra_info:
-                    return False, {"valid": False}
-                return False
-        if get_extra_info:
-            return valid_bool, {"valid": valid_bool}
-        return valid_bool
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import urllib.parse
+from time import sleep
+
+import validators
+from oc_ds_converter.oc_idmanager import *
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+
+class URLManager(IdentifierManager):
+    """This class implements an identifier manager for url identifier"""
+
+    def __init__(self, data={}, use_api_service=True):
+        """URL manager constructor."""
+        super(URLManager, self).__init__()
+        self._use_api_service = use_api_service
+        self._p = "url:"
+        self._data = data
+        self._scheme_https = "https://"
+        self._scheme_http = "http://"
+
+    def is_valid(self, url, get_extra_info=False):
+        url = self.normalise(url, include_prefix=True)
+        if url is None:
+            return False
+        else:
+            if url not in self._data or self._data[url] is None:
+                if get_extra_info:
+                    info = self.exists(url, get_extra_info=True)
+                    self._data[url] = info[1]
+                    return (info[0] and self.syntax_ok(url)), info[1]
+                self._data[url] = dict()
+                self._data[url]["valid"] = True if (self.exists(url) and self.syntax_ok(url)) else False
+                return self._data[url].get("valid")
+
+            if get_extra_info:
+                return self._data[url].get("valid"), self._data[url]
+            return self._data[url].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        id_string = str(id_string)
+        url_string = id_string.strip()
+        if url_string.startswith(self._p):
+            url_string = url_string[len(self._p):]
+        if url_string.endswith("/"):
+            url_string = url_string[:-1]
+        if url_string.startswith("https://"):
+            url_string = url_string[len("https://"):]
+        elif url_string.startswith("http://"):
+            url_string = url_string[len("http://"):]
+        if url_string.startswith("www."):
+            url_string = url_string[len("www."):]
+        try:
+            url_string = urllib.parse.quote(url_string, safe="%/:=&?~#+!$,;'@()*[]")
+            return "%s%s" % (self._p if include_prefix else "", url_string)
+        except:
+            # Any error in processing the URL will return None
+            return None
+
+    def syntax_ok(self, id_string):
+        if id_string.startswith(self._p):
+            id_string = id_string[len(self._p):]
+        return True if validators.url(self._scheme_https + id_string) else False
+
+    def exists(self, url_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self._use_api_service:
+            url = self.normalise(url_full)
+            if url is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(self._scheme_https + url,
+                            headers=self._headers,
+                            timeout=30,
+                        )
+                        if r.status_code == 200:
+                            if get_extra_info:
+                                return True, {"valid": True}
+                            return True
+                        elif r.status_code == 404:
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+
+                try:
+                    r = get(self._scheme_http + url,
+                            headers=self._headers,
+                            timeout=30,
+                            )
+                    if r.status_code == 200:
+                        if get_extra_info:
+                            return True, {"valid": True}
+                        return True
+                    elif r.status_code == 404:
+                        if get_extra_info:
+                            return False, {"valid": False}
+                        return False
+                except ReadTimeout:
+                    # Do nothing, just try again
+                    pass
+                except ConnectionError:
+                    # Sleep 5 seconds, then try again
+                    sleep(5)
+
+                valid_bool = False
+
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/viaf.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/wikipedia.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,139 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from json import loads
-from re import match, sub
-from time import sleep
-from urllib.parse import quote, unquote
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.storage_manager import StorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import SqliteStorageManager
-from typing import Type, Optional
-
-
-class ViafManager(IdentifierManager):
-    """This class implements an identifier manager for VIAF identifier"""
-
-    def __init__(self, use_api_service=True, storage_manager: Optional[StorageManager] = None):
-        """VIAF manager constructor."""
-        super(ViafManager, self).__init__()
-        self._use_api_service = use_api_service
-        if storage_manager is None:
-            self.storage_manager = InMemoryStorageManager()
-        else:
-            self.storage_manager = storage_manager
-
-        self._api = "http://www.viaf.org/viaf/"
-        self._use_api_service = use_api_service
-        self._p = "viaf:"
-
-
-    def validated_as_id(self, id_string):
-        arxiv_vaidation_value = self.storage_manager.get_value(id_string)
-        if isinstance(arxiv_vaidation_value, bool):
-            return arxiv_vaidation_value
-        else:
-            return None
-
-    def is_valid(self, viaf_id, get_extra_info=False):
-        viaf = self.normalise(viaf_id, include_prefix=True)
-        if not viaf:
-            return False
-        else:
-            arxiv_vaidation_value = self.storage_manager.get_value(viaf)
-            if isinstance(arxiv_vaidation_value, bool):
-                return arxiv_vaidation_value
-            else:
-                if get_extra_info:
-                    info = self.exists(viaf, get_extra_info=True)
-                    self.storage_manager.set_full_value(viaf,info[1])
-                    return (info[0] and self.syntax_ok(viaf)), info[1]
-                validity_check = self.exists(viaf) and self.syntax_ok(viaf)
-                self.storage_manager.set_value(viaf, validity_check)
-
-                return validity_check
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            if id_string.startswith(self._p):
-                viaf_string = id_string[len(self._p):]
-            else:
-                viaf_string = id_string
-
-            viaf_string = sub("\0+", "", sub("[^0-9]", "", unquote(viaf_string)))
-            return "%s%s" % (
-                self._p if include_prefix else "",
-                viaf_string.strip(),
-            )
-        except:
-            # Any error in processing the VIAF will return None
-            return None
-
-    def syntax_ok(self, id_string):
-
-        if not id_string.startswith("viaf:"):
-            id_string = self._p + id_string
-        return True if match(r"^viaf:[1-9]\d{1,21}$", id_string) else False
-
-    def exists(self, viaf_id_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        viaf_id = viaf_id_full
-        extra_info_result = {"id": viaf_id}
-        if self._use_api_service:
-            viaf_id = self.normalise(viaf_id_full)
-            extra_info_result = {"id": viaf_id}
-            if viaf_id is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(self._api + quote(viaf_id) + '/viaf.json', headers=self._headers, timeout=30)
-                        if r.status_code == 200:
-                            r.encoding = "utf-8"
-                            json_res = loads(r.text)
-                            if get_extra_info:
-                                try:
-                                    result = True if json_res['viafID'] == str(viaf_id) else False
-                                    extra_info_result["valid"] = result
-                                    return result, extra_info_result
-                                except KeyError:
-                                    extra_info_result["valid"] = False
-                                    return False, extra_info_result
-                            try:
-                                return True if json_res['viafID'] == str(viaf_id) else False
-                            except KeyError:
-                                return False
-                        elif 400 <= r.status_code < 500:
-                            if get_extra_info:
-                                extra_info_result["valid"] = False
-                                return False, extra_info_result
-                            return False
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-                valid_bool = False
-            else:
-                if get_extra_info:
-                    extra_info_result["valid"] = False
-                    return False, extra_info_result
-                return False
-
-        if get_extra_info:
-            return valid_bool, extra_info_result
-        return valid_bool
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-        # to be implemented
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from json import loads
+from re import match, sub
+from time import sleep
+from urllib.parse import unquote
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+
+class WikipediaManager(IdentifierManager):
+    """This class implements an identifier manager for wikidata identifier"""
+
+    def __init__(self, data={}, use_api_service=True):
+        """Wikipedia manager constructor."""
+        super(WikipediaManager, self).__init__()
+        self._api = "https://en.wikipedia.org/w/api.php/"
+        self._use_api_service = use_api_service
+        self._p = "wikipedia:"
+        self._data = data
+
+    def is_valid(self, wikipedia_id, get_extra_info=False):
+
+        wikipedia_id = self.normalise(wikipedia_id, include_prefix=True)
+
+        if wikipedia_id is None:
+            return False
+        else:
+            if wikipedia_id not in self._data or self._data[wikipedia_id] is None:
+                if get_extra_info:
+                    info = self.exists(wikipedia_id, get_extra_info=True)
+                    self._data[wikipedia_id] = info[1]
+                    return (info[0] and self.syntax_ok(wikipedia_id)), info[1]
+                self._data[wikipedia_id] = dict()
+                self._data[wikipedia_id]["valid"] = True if (self.exists(wikipedia_id) and self.syntax_ok(
+                    wikipedia_id)) else False
+                return self._data[wikipedia_id].get("valid")
+            if get_extra_info:
+                return self._data[wikipedia_id].get("valid"), self._data[wikipedia_id]
+            return self._data[wikipedia_id].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            if id_string.startswith(self._p):
+                wikipedia_string = id_string[len(self._p):]
+            else:
+                wikipedia_string = id_string
+
+            wikipedia_string = sub("\0+", "", sub("[^0-9]", "", unquote(wikipedia_string)))
+            return "%s%s" % (
+                self._p if include_prefix else "",
+                wikipedia_string.strip(),
+            )
+        except:
+            # Any error in processing the MediaWiki pageID will return None
+            return None
+
+    def syntax_ok(self, id_string):
+
+        if not id_string.startswith("wikipedia:"):
+            id_string = self._p + id_string
+        return True if match("^wikipedia:[1-9][0-9]*$", id_string) else False
+
+    def exists(self, wikipedia_id_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self._use_api_service:
+            wikipedia_id = self.normalise(wikipedia_id_full)
+            if wikipedia_id is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        query_params = {
+                            "action": "query",
+                            "pageids" : wikipedia_id,
+                            "format": "json",
+                            "formatversion": "1",  # format of json output (current version 1; might be replaced w/ v.2)
+                        }
+
+                        r = get(self._api, params=query_params, headers=self._headers, timeout=30)  # controlla
+                        if r.status_code == 200:
+                            r.encoding = "utf-8"
+                            json_res = loads(r.text)
+                            if get_extra_info:
+                                extra_info_result = {}
+                                try:
+                                    result = True if 'title' in json_res['query']['pages'][wikipedia_id].keys() else False
+                                    extra_info_result["valid"] = result
+                                    return result, extra_info_result
+                                except KeyError:
+                                    extra_info_result["valid"] = False
+                                    return False, extra_info_result
+                            try:
+                                return True if 'title' in json_res['query']['pages'][wikipedia_id].keys() else False
+                            except KeyError:
+                                return False
+
+                        elif 400 <= r.status_code < 500:
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool=False
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        # to be implemented
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/oc_idmanager/wikidata.py` & `oc_ds_converter-1.0.1/oc_ds_converter/oc_idmanager/wikidata.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!python
-# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
-# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-from json import loads
-from re import match, sub
-from time import sleep
-from urllib.parse import quote, unquote
-
-from oc_ds_converter.oc_idmanager.base import IdentifierManager
-from requests import ReadTimeout, get
-from requests.exceptions import ConnectionError
-
-
-class WikidataManager(IdentifierManager):
-    """This class implements an identifier manager for wikidata identifier"""
-
-    def __init__(self, data={}, use_api_service=True):
-        """Wikidata manager constructor."""
-        super(WikidataManager, self).__init__()
-        self._api = "https://www.wikidata.org/wiki/Special:EntityData/"
-        self._use_api_service = use_api_service
-        self._p = "wikidata:"
-        self._data = data
-
-    def is_valid(self, wikidata_id, get_extra_info=False):
-        wikidata_id = self.normalise(wikidata_id, include_prefix=True)
-
-        if wikidata_id is None:
-            return False
-        else:
-            if wikidata_id not in self._data or self._data[wikidata_id] is None:
-                if get_extra_info:
-                    info = self.exists(wikidata_id, get_extra_info=True)
-                    self._data[wikidata_id] = info[1]
-                    return (info[0] and self.syntax_ok(wikidata_id)), info[1]
-                self._data[wikidata_id] = dict()
-                self._data[wikidata_id]["valid"] = True if (self.exists(wikidata_id) and self.syntax_ok(wikidata_id)) else False
-                return self._data[wikidata_id].get("valid")
-            if get_extra_info:
-                return self._data[wikidata_id].get("valid"), self._data[wikidata_id]
-            return self._data[wikidata_id].get("valid")
-
-    def normalise(self, id_string, include_prefix=False):
-        try:
-            if id_string.startswith(self._p):
-                wikidata_string = id_string[len(self._p):]
-            else:
-                wikidata_string = id_string
-
-            wikidata_string = sub("\0+", "", sub("[^Q0-9]", "", unquote(wikidata_string).upper()))
-            return "%s%s" % (
-                self._p if include_prefix else "",
-                wikidata_string.strip(),
-            )
-        except:
-            # Any error in processing the Q-ID will return None
-            return None
-
-    def syntax_ok(self, id_string):
-
-        if not id_string.startswith("wikidata:"):
-            id_string = self._p + id_string
-        return True if match("^wikidata:Q[1-9]\\d*$", id_string) else False
-
-    def exists(self, wikidata_id_full, get_extra_info=False, allow_extra_api=None):
-        valid_bool = True
-        if self._use_api_service:
-            wikidata_id = self.normalise(wikidata_id_full)
-            if wikidata_id is not None:
-                tentative = 3
-                while tentative:
-                    tentative -= 1
-                    try:
-                        r = get(self._api + quote(wikidata_id), headers=self._headers, timeout=30)
-                        if r.status_code == 200:
-                            r.encoding = "utf-8"
-                            json_res = loads(r.text)
-                            if get_extra_info:
-                                extra_info_result = {}
-                                try:
-                                    result = True if json_res['entities'][f"{wikidata_id}"]['id'] == str(wikidata_id) else False
-                                    extra_info_result['valid'] = result
-                                    return result, extra_info_result
-                                except KeyError:
-                                    extra_info_result["valid"] = False
-                                    return False, extra_info_result
-                                # return True if json_res['entities'][f"{wikidata_id}"]['id'] == str(
-                                #     wikidata_id) else False, self.extra_info(json_res)
-                            try:
-                                return True if json_res['entities'][f"{wikidata_id}"]['id'] == str(wikidata_id) else False
-                            except KeyError:
-                                return False
-
-                        elif 400 <= r.status_code < 500:
-                            if get_extra_info:
-                                return False, {"valid": False}
-                            return False
-                    except ReadTimeout:
-                        # Do nothing, just try again
-                        pass
-                    except ConnectionError:
-                        # Sleep 5 seconds, then try again
-                        sleep(5)
-                valid_bool = False
-            else:
-                if get_extra_info:
-                    return False, {"valid": False}
-                return False
-
-        if get_extra_info:
-            return valid_bool, {"valid": valid_bool}
-        return valid_bool
-
-    def extra_info(self, api_response, choose_api=None, info_dict={}):
-        result = {}
-        result["valid"] = True
-        # to be implemented
-        return result
+#!python
+# Copyright 2019, Silvio Peroni <essepuntato@gmail.com>
+# Copyright 2022, Giuseppe Grieco <giuseppe.grieco3@unibo.it>, Arianna Moretti <arianna.moretti4@unibo.it>, Elia Rizzetto <elia.rizzetto@studio.unibo.it>, Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+from json import loads
+from re import match, sub
+from time import sleep
+from urllib.parse import quote, unquote
+
+from oc_ds_converter.oc_idmanager.base import IdentifierManager
+from requests import ReadTimeout, get
+from requests.exceptions import ConnectionError
+
+
+class WikidataManager(IdentifierManager):
+    """This class implements an identifier manager for wikidata identifier"""
+
+    def __init__(self, data={}, use_api_service=True):
+        """Wikidata manager constructor."""
+        super(WikidataManager, self).__init__()
+        self._api = "https://www.wikidata.org/wiki/Special:EntityData/"
+        self._use_api_service = use_api_service
+        self._p = "wikidata:"
+        self._data = data
+
+    def is_valid(self, wikidata_id, get_extra_info=False):
+        wikidata_id = self.normalise(wikidata_id, include_prefix=True)
+
+        if wikidata_id is None:
+            return False
+        else:
+            if wikidata_id not in self._data or self._data[wikidata_id] is None:
+                if get_extra_info:
+                    info = self.exists(wikidata_id, get_extra_info=True)
+                    self._data[wikidata_id] = info[1]
+                    return (info[0] and self.syntax_ok(wikidata_id)), info[1]
+                self._data[wikidata_id] = dict()
+                self._data[wikidata_id]["valid"] = True if (self.exists(wikidata_id) and self.syntax_ok(wikidata_id)) else False
+                return self._data[wikidata_id].get("valid")
+            if get_extra_info:
+                return self._data[wikidata_id].get("valid"), self._data[wikidata_id]
+            return self._data[wikidata_id].get("valid")
+
+    def normalise(self, id_string, include_prefix=False):
+        try:
+            if id_string.startswith(self._p):
+                wikidata_string = id_string[len(self._p):]
+            else:
+                wikidata_string = id_string
+
+            wikidata_string = sub("\0+", "", sub("[^Q0-9]", "", unquote(wikidata_string).upper()))
+            return "%s%s" % (
+                self._p if include_prefix else "",
+                wikidata_string.strip(),
+            )
+        except:
+            # Any error in processing the Q-ID will return None
+            return None
+
+    def syntax_ok(self, id_string):
+
+        if not id_string.startswith("wikidata:"):
+            id_string = self._p + id_string
+        return True if match("^wikidata:Q[1-9]\\d*$", id_string) else False
+
+    def exists(self, wikidata_id_full, get_extra_info=False, allow_extra_api=None):
+        valid_bool = True
+        if self._use_api_service:
+            wikidata_id = self.normalise(wikidata_id_full)
+            if wikidata_id is not None:
+                tentative = 3
+                while tentative:
+                    tentative -= 1
+                    try:
+                        r = get(self._api + quote(wikidata_id), headers=self._headers, timeout=30)
+                        if r.status_code == 200:
+                            r.encoding = "utf-8"
+                            json_res = loads(r.text)
+                            if get_extra_info:
+                                extra_info_result = {}
+                                try:
+                                    result = True if json_res['entities'][f"{wikidata_id}"]['id'] == str(wikidata_id) else False
+                                    extra_info_result['valid'] = result
+                                    return result, extra_info_result
+                                except KeyError:
+                                    extra_info_result["valid"] = False
+                                    return False, extra_info_result
+                                # return True if json_res['entities'][f"{wikidata_id}"]['id'] == str(
+                                #     wikidata_id) else False, self.extra_info(json_res)
+                            try:
+                                return True if json_res['entities'][f"{wikidata_id}"]['id'] == str(wikidata_id) else False
+                            except KeyError:
+                                return False
+
+                        elif 400 <= r.status_code < 500:
+                            if get_extra_info:
+                                return False, {"valid": False}
+                            return False
+                    except ReadTimeout:
+                        # Do nothing, just try again
+                        pass
+                    except ConnectionError:
+                        # Sleep 5 seconds, then try again
+                        sleep(5)
+                valid_bool = False
+            else:
+                if get_extra_info:
+                    return False, {"valid": False}
+                return False
+
+        if get_extra_info:
+            return valid_bool, {"valid": valid_bool}
+        return valid_bool
+
+    def extra_info(self, api_response, choose_api=None, info_dict={}):
+        result = {}
+        result["valid"] = True
+        # to be implemented
+        return result
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/base.py` & `oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import os.path
-import pathlib
-import tarfile
-import zipfile
-from abc import ABCMeta, abstractmethod
-from json import load, loads
-from os import makedirs, sep, walk
-from os.path import basename, exists, isdir
-
-import zstandard as zstd
-
-
-class Preprocessing(metaclass=ABCMeta):
-    """This is the interface for implementing preprocessors for specific datasources.
-    It provides the signatures of the methods for preprocessing a dump"""
-
-    def __init__(self, **params):
-        """preprocessor constructor."""
-        for key in params:
-            setattr(self, key, params[key])
-
-    def get_all_files(self, i_dir_or_compr, req_type):
-        result = []
-        targz_fd = None
-
-        if isdir(i_dir_or_compr):
-
-            for cur_dir, cur_subdir, cur_files in walk(i_dir_or_compr):
-                for cur_file in cur_files:
-                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
-                        result.append(os.path.join(cur_dir, cur_file))
-        elif i_dir_or_compr.endswith("tar.gz"):
-            targz_fd = tarfile.open(i_dir_or_compr, "r:gz", encoding="utf-8")
-            for cur_file in targz_fd:
-                if cur_file.name.endswith(req_type) and not basename(cur_file.name).startswith("."):
-                    result.append(cur_file)
-        elif i_dir_or_compr.endswith("zip"):
-            with zipfile.ZipFile(i_dir_or_compr, 'r') as zip_ref:
-                dest_dir = i_dir_or_compr + "decompr_zip_dir"
-                if not exists(dest_dir):
-                    makedirs(dest_dir)
-                zip_ref.extractall(dest_dir)
-            for cur_dir, cur_subdir, cur_files in walk(dest_dir):
-                for cur_file in cur_files:
-                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
-                        result.append(cur_dir + sep + cur_file)
-
-        elif i_dir_or_compr.endswith("zst"):
-            input_file = pathlib.Path(i_dir_or_compr)
-            dest_dir = i_dir_or_compr + "decompr_zst_dir"
-            with open(input_file, 'rb') as compressed:
-                decomp = zstd.ZstdDecompressor()
-                if not exists(dest_dir):
-                    makedirs(dest_dir)
-                output_path = pathlib.Path(dest_dir) / input_file.stem
-                if not exists(output_path):
-                    with open(output_path, 'wb') as destination:
-                        decomp.copy_stream(compressed, destination)
-            for cur_dir, cur_subdir, cur_files in walk(dest_dir):
-                for cur_file in cur_files:
-                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
-                        result.append(cur_dir + sep + cur_file)
-        else:
-            print("It is not possible to process the input path.")
-        return result, targz_fd
-
-    def load_json(self, file, targz_fd, file_idx, len_all_files):
-        result = None
-
-        if targz_fd is None:
-            print("Open file %s of %s" % (file_idx, len_all_files))
-            with open(file, encoding="utf8") as f:
-                result = load(f)
-
-        else:
-            print("Open file %s of %s (in tar.gz archive)" % (file_idx, len_all_files))
-            cur_tar_file = targz_fd.extractfile(file)
-            json_str = cur_tar_file.read()
-
-            # In Python 3.5 it seems that, for some reason, the extractfile method returns an
-            # object 'bytes' that cannot be managed by the function 'load' in the json package.
-            # Thus, to avoid issues, in case an object having type 'bytes' is return, it is
-            # transformed as a string before passing it to the function 'loads'. Please note
-            # that Python 3.9 does not show this behaviour, and it works correctly without
-            # any transformation.
-            if type(json_str) is bytes:
-                json_str = json_str.decode("utf-8")
-
-            result = loads(json_str)
-
-        return result
-
-    @abstractmethod
-    def split_input(self):
-        """ ...
-        """
-        pass
-
-    def filter(self, data):
-        pass
-
-    @abstractmethod
-    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
+import os.path
+import pathlib
+import tarfile
+import zipfile
+from abc import ABCMeta, abstractmethod
+from json import load, loads
+from os import makedirs, sep, walk
+from os.path import basename, exists, isdir
+
+import zstandard as zstd
+
+
+class Preprocessing(metaclass=ABCMeta):
+    """This is the interface for implementing preprocessors for specific datasources.
+    It provides the signatures of the methods for preprocessing a dump"""
+
+    def __init__(self, **params):
+        """preprocessor constructor."""
+        for key in params:
+            setattr(self, key, params[key])
+
+    def get_all_files(self, i_dir_or_compr, req_type):
+        result = []
+        targz_fd = None
+
+        if isdir(i_dir_or_compr):
+
+            for cur_dir, cur_subdir, cur_files in walk(i_dir_or_compr):
+                for cur_file in cur_files:
+                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
+                        result.append(os.path.join(cur_dir, cur_file))
+        elif i_dir_or_compr.endswith("tar.gz"):
+            targz_fd = tarfile.open(i_dir_or_compr, "r:gz", encoding="utf-8")
+            for cur_file in targz_fd:
+                if cur_file.name.endswith(req_type) and not basename(cur_file.name).startswith("."):
+                    result.append(cur_file)
+        elif i_dir_or_compr.endswith("zip"):
+            with zipfile.ZipFile(i_dir_or_compr, 'r') as zip_ref:
+                dest_dir = i_dir_or_compr + "decompr_zip_dir"
+                if not exists(dest_dir):
+                    makedirs(dest_dir)
+                zip_ref.extractall(dest_dir)
+            for cur_dir, cur_subdir, cur_files in walk(dest_dir):
+                for cur_file in cur_files:
+                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
+                        result.append(cur_dir + sep + cur_file)
+
+        elif i_dir_or_compr.endswith("zst"):
+            input_file = pathlib.Path(i_dir_or_compr)
+            dest_dir = i_dir_or_compr + "decompr_zst_dir"
+            with open(input_file, 'rb') as compressed:
+                decomp = zstd.ZstdDecompressor()
+                if not exists(dest_dir):
+                    makedirs(dest_dir)
+                output_path = pathlib.Path(dest_dir) / input_file.stem
+                if not exists(output_path):
+                    with open(output_path, 'wb') as destination:
+                        decomp.copy_stream(compressed, destination)
+            for cur_dir, cur_subdir, cur_files in walk(dest_dir):
+                for cur_file in cur_files:
+                    if cur_file.endswith(req_type) and not basename(cur_file).startswith("."):
+                        result.append(cur_dir + sep + cur_file)
+        else:
+            print("It is not possible to process the input path.")
+        return result, targz_fd
+
+    def load_json(self, file, targz_fd, file_idx, len_all_files):
+        result = None
+
+        if targz_fd is None:
+            print("Open file %s of %s" % (file_idx, len_all_files))
+            with open(file, encoding="utf8") as f:
+                result = load(f)
+
+        else:
+            print("Open file %s of %s (in tar.gz archive)" % (file_idx, len_all_files))
+            cur_tar_file = targz_fd.extractfile(file)
+            json_str = cur_tar_file.read()
+
+            # In Python 3.5 it seems that, for some reason, the extractfile method returns an
+            # object 'bytes' that cannot be managed by the function 'load' in the json package.
+            # Thus, to avoid issues, in case an object having type 'bytes' is return, it is
+            # transformed as a string before passing it to the function 'loads'. Please note
+            # that Python 3.9 does not show this behaviour, and it works correctly without
+            # any transformation.
+            if type(json_str) is bytes:
+                json_str = json_str.decode("utf-8")
+
+            result = loads(json_str)
+
+        return result
+
+    @abstractmethod
+    def split_input(self):
+        """ ...
+        """
+        pass
+
+    def filter(self, data):
+        pass
+
+    @abstractmethod
+    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
         pass
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/datacite.py` & `oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/datacite.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import glob
-import json
-import os
-import os.path
-from os import listdir, makedirs
-from os.path import exists, join
-
-from oc_ds_converter.preprocessing.base import Preprocessing
-from tqdm import tqdm
-
-
-class DatacitePreProcessing(Preprocessing):
-    """This class aims at pre-processing DataCite dumps.
-    In particular, DatacitePreProcessing splits the original nldJSON in many JSON files, each one containing the number of entities specified in input by the user. Further, the class discards those entities that do not provide useful information for meta"""
-
-    def __init__(self, input_dir, output_dir, interval, filter=None, low_memo=True):
-        self._req_type = ".json"
-        self._input_dir = input_dir
-        self._output_dir = output_dir
-        self._needed_info = ["relationType", "relatedIdentifierType", "relatedIdentifier"]
-        if not exists(self._output_dir):
-            makedirs(self._output_dir)
-        self._interval = interval
-        if low_memo:
-            self._low_memo = low_memo
-        else:
-            self._low_memo = True
-        if filter:
-            self._filter = filter
-        else:
-            self._filter = ["references", "isreferencedby", "cites", "iscitedby"]
-        super(DatacitePreProcessing, self).__init__()
-
-    def split_input(self):
-        # restart from the last processed line, in case of previous process interruption
-        out_dir = listdir(self._output_dir)
-        # Checking if the list is empty or not
-        if len(out_dir) != 0:
-            list_of_files = glob.glob(join(self._output_dir, '*.json'))  # * means all if need specific format then *.csv
-            latest_file = max(list_of_files, key=os.path.getctime)
-            with open(latest_file, encoding="utf8") as f:
-                recover_dict = json.load(f)
-                data_list = recover_dict["data"]
-                last_processed_dict = data_list[-1]
-                last_dict_id = last_processed_dict["id"]
-                f.close()
-        else:
-            last_processed_dict = None
-
-        all_files, targz_fd = self.get_all_files(self._input_dir, self._req_type)
-        len_all_files = len(all_files)
-        data = []
-        #pre_count = 0
-        count = 0
-
-        for file_idx, file in enumerate(all_files, 1):
-            if not self._low_memo:
-                f = self.load_json(file, targz_fd, file_idx, len_all_files)
-            else:
-                f = open(file, encoding="utf8")
-            #verificare corretto funzionamento con opzione LOW MEMO = False !!! OPZIONE LOW MEMO FALSE NON VA LETTA COME STRINGA
-            for line in tqdm(f):
-                if self._low_memo:
-                    if last_processed_dict is not None:
-                        if not line.startswith('{"id":"' + last_dict_id+'",') :
-                            #pre_count += 1
-                            continue
-                        else:
-                            last_processed_dict = None
-                            # pre_count += 1
-                            # count = pre_count
-                            continue
-                    else:
-                        pass
-                else:
-                    if last_processed_dict is not None:
-                        if line.get("id") != last_dict_id:
-                            #pre_count += 1
-                            continue
-                        else:
-                            last_processed_dict = None
-                            # pre_count += 1
-                            # count = pre_count
-                            continue
-                    else:
-                        pass
-
-                # count += 1
-                # to be logged: print("Processing entity n.:", n_lines)
-                if self._low_memo:
-                    try:
-                        linedict = json.loads(line)
-                    except:
-                        print(ValueError, line)
-                        continue
-                else:
-                    linedict = line
-                if 'id' not in linedict or 'type' not in linedict:
-                    continue
-                if linedict['type'] != "dois":
-                    continue
-                attributes = linedict["attributes"]
-                rel_ids = attributes.get("relatedIdentifiers")
-
-                if rel_ids:
-                    for ref in rel_ids:
-                        if all(elem in ref for elem in self._needed_info):
-                            relatedIdentifierType = (str(ref["relatedIdentifierType"])).lower()
-                            relationType = str(ref["relationType"]).lower()
-                            if relatedIdentifierType == "doi":
-                                if relationType in self._filter:
-                                    data.append(linedict)
-                                    count += 1
-                                    break
-
-
-                data = self.splitted_to_file(
-                    count, self._interval, self._output_dir, data
-                )
-            f.close()
-
-        if len(data) > 0:
-            count = count + (self._interval - (int(count) % int(self._interval)))
-            data = self.splitted_to_file(count, self._interval, self._output_dir, data)
-
-
-    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
-        if not exists(out_dir):
-            makedirs(out_dir)
-        dict_to_json = dict()
-        if int(cur_n) != 0 and int(cur_n) % int(target_n) == 0:
-            # to be logged: print("Processed lines:", cur_n, ". Reduced csv nr.", cur_n // target_n)
-            filename = "jSonFile_" + str(cur_n // target_n) + self._req_type
-            with (
-                    open(os.path.join(out_dir, filename), "w", encoding="utf8")
-            ) as json_file:
-                dict_to_json["data"] = data
-                json.dump(dict_to_json, json_file)
-                empt_list = []
-            return empt_list
-        else:
-            return data
-
-
+import glob
+import json
+import os
+import os.path
+from os import listdir, makedirs
+from os.path import exists, join
+
+from oc_ds_converter.preprocessing.base import Preprocessing
+from tqdm import tqdm
+
+
+class DatacitePreProcessing(Preprocessing):
+    """This class aims at pre-processing DataCite dumps.
+    In particular, DatacitePreProcessing splits the original nldJSON in many JSON files, each one containing the number of entities specified in input by the user. Further, the class discards those entities that do not provide useful information for meta"""
+
+    def __init__(self, input_dir, output_dir, interval, filter=None, low_memo=True):
+        self._req_type = ".json"
+        self._input_dir = input_dir
+        self._output_dir = output_dir
+        self._needed_info = ["relationType", "relatedIdentifierType", "relatedIdentifier"]
+        if not exists(self._output_dir):
+            makedirs(self._output_dir)
+        self._interval = interval
+        if low_memo:
+            self._low_memo = low_memo
+        else:
+            self._low_memo = True
+        if filter:
+            self._filter = filter
+        else:
+            self._filter = ["references", "isreferencedby", "cites", "iscitedby"]
+        super(DatacitePreProcessing, self).__init__()
+
+    def split_input(self):
+        # restart from the last processed line, in case of previous process interruption
+        out_dir = listdir(self._output_dir)
+        # Checking if the list is empty or not
+        if len(out_dir) != 0:
+            list_of_files = glob.glob(join(self._output_dir, '*.json'))  # * means all if need specific format then *.csv
+            latest_file = max(list_of_files, key=os.path.getctime)
+            with open(latest_file, encoding="utf8") as f:
+                recover_dict = json.load(f)
+                data_list = recover_dict["data"]
+                last_processed_dict = data_list[-1]
+                last_dict_id = last_processed_dict["id"]
+                f.close()
+        else:
+            last_processed_dict = None
+
+        all_files, targz_fd = self.get_all_files(self._input_dir, self._req_type)
+        len_all_files = len(all_files)
+        data = []
+        #pre_count = 0
+        count = 0
+
+        for file_idx, file in enumerate(all_files, 1):
+            if not self._low_memo:
+                f = self.load_json(file, targz_fd, file_idx, len_all_files)
+            else:
+                f = open(file, encoding="utf8")
+            #verificare corretto funzionamento con opzione LOW MEMO = False !!! OPZIONE LOW MEMO FALSE NON VA LETTA COME STRINGA
+            for line in tqdm(f):
+                if self._low_memo:
+                    if last_processed_dict is not None:
+                        if not line.startswith('{"id":"' + last_dict_id+'",') :
+                            #pre_count += 1
+                            continue
+                        else:
+                            last_processed_dict = None
+                            # pre_count += 1
+                            # count = pre_count
+                            continue
+                    else:
+                        pass
+                else:
+                    if last_processed_dict is not None:
+                        if line.get("id") != last_dict_id:
+                            #pre_count += 1
+                            continue
+                        else:
+                            last_processed_dict = None
+                            # pre_count += 1
+                            # count = pre_count
+                            continue
+                    else:
+                        pass
+
+                # count += 1
+                # to be logged: print("Processing entity n.:", n_lines)
+                if self._low_memo:
+                    try:
+                        linedict = json.loads(line)
+                    except:
+                        print(ValueError, line)
+                        continue
+                else:
+                    linedict = line
+                if 'id' not in linedict or 'type' not in linedict:
+                    continue
+                if linedict['type'] != "dois":
+                    continue
+                attributes = linedict["attributes"]
+                rel_ids = attributes.get("relatedIdentifiers")
+
+                if rel_ids:
+                    for ref in rel_ids:
+                        if all(elem in ref for elem in self._needed_info):
+                            relatedIdentifierType = (str(ref["relatedIdentifierType"])).lower()
+                            relationType = str(ref["relationType"]).lower()
+                            if relatedIdentifierType == "doi":
+                                if relationType in self._filter:
+                                    data.append(linedict)
+                                    count += 1
+                                    break
+
+
+                data = self.splitted_to_file(
+                    count, self._interval, self._output_dir, data
+                )
+            f.close()
+
+        if len(data) > 0:
+            count = count + (self._interval - (int(count) % int(self._interval)))
+            data = self.splitted_to_file(count, self._interval, self._output_dir, data)
+
+
+    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
+        if not exists(out_dir):
+            makedirs(out_dir)
+        dict_to_json = dict()
+        if int(cur_n) != 0 and int(cur_n) % int(target_n) == 0:
+            # to be logged: print("Processed lines:", cur_n, ". Reduced csv nr.", cur_n // target_n)
+            filename = "jSonFile_" + str(cur_n // target_n) + self._req_type
+            with (
+                    open(os.path.join(out_dir, filename), "w", encoding="utf8")
+            ) as json_file:
+                dict_to_json["data"] = data
+                json.dump(dict_to_json, json_file)
+                empt_list = []
+            return empt_list
+        else:
+            return data
+
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/jalc.py` & `oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/jalc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-
-import shutil
-from tqdm import tqdm
-from oc_ds_converter.lib.jsonmanager import *
-from oc_ds_converter.lib.file_manager import normalize_path
-from argparse import ArgumentParser
-from pebble import ProcessPool, ProcessFuture
-
-
-def preprocessing(jalc_json_dir:str, output_dir:str, max_workers:int = 1):
-    """This function preprocesses the original JALC zipped dump. The original dump has the following structure:
-    - jalc_dump.zip
-        -jalc_dataset_dir
-            -prefixes.json
-            -prefix1.zip
-                -prefix1_dir
-                    -doiList1.json
-                    -doi1A.json
-                    -doi1B.json
-                    -etc.
-            -prefix2.zip
-                -prefix2_dir
-                    -doiList2.json
-                    -doi2A.json
-                    -etc.
-    The preprocessing in particular removes the intermediate folders (like jalc_dump, prefix1, prefix2 in the example above)
-    and if inside one prefix.zip file are found more than 100 files, the original zip file is divided into the number of
-    json files in it//100 +1. In the case in which a prefix.zip file is divided into more zip files, the doiList.json is copied
-    just in the first subfile."""
-
-    '''In the els_to_be_skipped list are appended all the files found in the input directory starting with
-    "._" and the zip file if the corresponding decompressed directory is found'''
-    els_to_be_skipped = []
-    input_dir_cont = os.listdir(jalc_json_dir)
-    for el in input_dir_cont:# should be one (the input dir contains 1 zip)
-        if el.startswith("._"):
-            # skip elements starting with ._
-            els_to_be_skipped.append(os.path.join(jalc_json_dir, el))
-        else:
-            if el.endswith(".zip"):
-                base_name = el.replace('.zip', '')
-                if [x for x in os.listdir(jalc_json_dir) if x.startswith(base_name) and x.endswith("decompr_zip_dir")]:
-                    els_to_be_skipped.append(os.path.join(jalc_json_dir, el))
-
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
-
-    all_unzipped_files = []
-    '''The elements in the "els_to_be_skipped" list are now taken into account. If inside the list a zip element is found,
-    the corresponding unzipped folder (if found in the input directory) is used to list all the elements inside the original 
-    zipped dump.'''
-    els_to_be_skipped_cont = [x for x in els_to_be_skipped if x.endswith(".zip")]
-    if els_to_be_skipped_cont:
-        for el_to_skip in els_to_be_skipped_cont:
-            if el_to_skip.startswith("._"):
-                continue
-            base_name_el_to_skip = os.path.basename(el_to_skip).replace('.zip', '')
-            for directory in os.listdir(jalc_json_dir):
-                if directory == base_name_el_to_skip + "_decompr_zip_dir":
-                    # if el.startswith(base_name_el_to_skip) and el.endswith("decompr_zip_dir"):
-                    for dir_lev2 in os.listdir(os.path.join(jalc_json_dir, directory)):
-                        all_unzipped_files = [os.path.join(jalc_json_dir, directory, dir_lev2, file) for file in os.listdir(os.path.join(jalc_json_dir, directory, dir_lev2)) if not file.startswith("._")]
-
-    '''If there aren't elements in the "els_to_be_skipped" list all the elements in the original
-    zipped dump are extracted in a folder with the same basename of the original dump + "_decompre_zip_dir".'''
-    if len(all_unzipped_files) == 0:
-        for zip_lev0 in os.listdir(jalc_json_dir):
-            if zip_lev0.endswith("zip") and not zip_lev0.startswith("._"):
-                with zipfile.ZipFile(os.path.join(jalc_json_dir, zip_lev0), 'r') as zip_ref:
-                    dest_dir = os.path.join(jalc_json_dir, zip_lev0).replace('.zip', '') + "_decompr_zip_dir"
-                    if not exists(dest_dir):
-                        makedirs(dest_dir)
-                    zip_ref.extractall(dest_dir)
-                    print(f"Unzipped to {dest_dir}")
-                for cur_dir, cur_subdir, cur_files in walk(dest_dir):
-                    for cur_file in cur_files:
-                        if not basename(cur_file).startswith("."):
-                            all_unzipped_files.append(cur_dir + sep + cur_file)
-
-
-
-    # Filter for zip files (files with ".zip" extension)
-    zip_files = [file for file in all_unzipped_files if file.endswith(".zip")]
-    not_zip_files = [file for file in all_unzipped_files if not file.endswith(".zip")]
-
-    # copy all extra files as they are in the output dir
-    for file in not_zip_files:
-        if os.path.isfile(file):
-            shutil.copy(file, output_dir)
-
-    # parallelization of the process
-    if max_workers == 1:
-        for zip_file in tqdm(zip_files, desc="Processing ZIP Files"):
-            process_zip(zip_file, output_dir)
-
-    else:
-        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
-            for zip_file in tqdm(zip_files, desc="Processing ZIP Files"):
-                future: ProcessFuture = executor.schedule(function=process_zip, args=[zip_file, output_dir])
-
-
-    # At the end of the process, create a ZIP archive of the output_dir and rename it
-    print("Zipping the output directory")
-    shutil.make_archive(output_dir, 'zip', output_dir)
-    print("Removing output directory")
-    shutil.rmtree(output_dir)  # Delete the original directory
-
-
-def process_zip(zip_file, output_dir2):
-
-    if not zip_file.endswith(".zip"):
-        shutil.copy(zip_file, output_dir2)
-
-    else:
-        # manage the resizing
-        # Full path to the zip file
-        zip_file_path = zip_file
-        first_level_path = os.path.dirname(zip_file_path)
-        print("executing", zip_file_path)
-        # Open the zip file for reading
-        with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
-            all_files_in_zip = zip_ref.namelist()
-
-            directories = [entry for entry in all_files_in_zip if entry.endswith('/')]
-            # List the names of files within the zip (the relevant one, the json containing the citation information)
-            file_names = [x for x in all_files_in_zip if x.endswith(".json") and "doiList" not in x and x not in directories]
-            extra_file_names = [x for x in all_files_in_zip if "doiList" in x or x.endswith(".out")]
-
-            if len(file_names) <= 100:
-                print("less than 100")
-                zip_file_name = os.path.basename(zip_file_path).replace(".zip", "")
-                dir_to_zip = os.path.join(output_dir2, zip_file_name)
-                os.makedirs(dir_to_zip, exist_ok=True)
-                for non_zip in extra_file_names:
-                    if not os.path.isdir(non_zip) and 'doiList' in non_zip:
-                        '''We use os.path.basename(file_info.filename) to extract just the filename
-                        without the folder structure. We create a new file in the destination folder 
-                        with the extracted filename and write the content of the file from the ZIP archive into it.'''
-                        file_info = zip_ref.getinfo(non_zip)
-                        extracted_file_path = os.path.join(dir_to_zip, os.path.basename(file_info.filename))
-                        with open(extracted_file_path, 'wb') as extracted_file:
-                            extracted_file.write(zip_ref.read(non_zip))
-                for fs in file_names:
-                    file_info = zip_ref.getinfo(fs)
-                    extracted_file_path = os.path.join(dir_to_zip,
-                                                       os.path.basename(file_info.filename))
-                    with open(extracted_file_path, 'wb') as extracted_file:
-                        extracted_file.write(zip_ref.read(fs))
-
-                # Parent directory
-                parent_directory = os.path.dirname(dir_to_zip)
-                # Name the zip file
-                zip_file_name = dir_to_zip + ".zip"
-                # Full path to the destination zip file
-                zip_file_path = os.path.join(parent_directory, zip_file_name)
-
-                with zipfile.ZipFile(zip_file_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
-                    for foldername, subfolders, filenames in os.walk(dir_to_zip):
-                        for filename in filenames:
-                            file_path = os.path.join(foldername, filename)
-                            relative_path = os.path.relpath(file_path, dir_to_zip)
-                            zipf.write(file_path, relative_path)
-                # After creating the zip, delete the original directory
-                shutil.rmtree(dir_to_zip)
-                print("Just Completed zip:", zip_file_path)
-
-            else:
-                # if there are more than 100 jsons, they should be divided as many zips as the total number of jsons/ 100.
-                # The first of the new sub-zip files should also contain all the extra files which where stored in the original zip
-                print("more than 100: ", len(file_names))
-                zip_basename = zip_file_path.replace(".zip", "").replace(first_level_path, "").replace("/", "").replace(
-                "\\", "")
-                zip_part_counter = 0
-
-                while len(file_names):
-                    # name of the new folder (prefix_0.zip)
-                    zip_basename_w_counter = zip_basename + "_" + str(zip_part_counter)
-                    # path of the new folder where files will be extracted
-                    sliced_out_name = os.path.join(output_dir2, zip_basename_w_counter)
-                    os.makedirs(sliced_out_name, exist_ok=True)
-
-                    # copying in the output folder all the extra files (not json files with information on the bibliographic entities)
-                    if zip_part_counter == 0:
-                        for non_zip in extra_file_names:
-                            if not os.path.isdir(non_zip) and 'doiList' in non_zip:
-                                '''We use os.path.basename(file_info.filename) to extract just the filename
-                                without the folder structure. We create a new file in the destination folder 
-                                with the extracted filename and write the content of the file from the ZIP archive into it.'''
-                                file_info = zip_ref.getinfo(non_zip)
-                                extracted_file_path = os.path.join(sliced_out_name, os.path.basename(file_info.filename))
-                                with open(extracted_file_path, 'wb') as extracted_file:
-                                    extracted_file.write(zip_ref.read(non_zip))
-
-                    if len(file_names) > 100:
-                        print("json to be processed in this zip:", len(file_names))
-
-                        files_slice = file_names[:100]
-                        file_names = file_names[100:]
-                        zip_part_counter +=1
-
-                        for fs in files_slice:
-                            file_info = zip_ref.getinfo(fs)
-                            extracted_file_path = os.path.join(sliced_out_name,
-                                                               os.path.basename(file_info.filename))
-                            with open(extracted_file_path, 'wb') as extracted_file:
-                                extracted_file.write(zip_ref.read(fs))
-                    else:
-                        print("last", len(file_names), "jsons to be processed")
-                        files_slice = file_names
-                        file_names = []
-                        zip_part_counter += 1
-
-                        for fs in files_slice:
-                            file_info = zip_ref.getinfo(fs)
-                            extracted_file_path = os.path.join(sliced_out_name,
-                                                               os.path.basename(file_info.filename))
-                            with open(extracted_file_path, 'wb') as extracted_file:
-                                extracted_file.write(zip_ref.read(fs))
-
-                    # Directory to zip and delete
-                    directory_to_zip = sliced_out_name
-                    # Parent directory
-                    parent_directory = os.path.dirname(directory_to_zip)
-                    # Name the zip file
-                    zip_file_name = directory_to_zip + ".zip"
-                    # Full path to the destination zip file
-                    zip_file_path = os.path.join(parent_directory, zip_file_name)
-                    # create a zip file
-                    with zipfile.ZipFile(zip_file_name, 'w', zipfile.ZIP_DEFLATED) as zipf:
-                        for foldername, subfolders, filenames in os.walk(directory_to_zip):
-                            for filename in filenames:
-                                file_path = os.path.join(foldername, filename)
-                                relative_path = os.path.relpath(file_path, directory_to_zip)
-                                zipf.write(file_path, relative_path)
-                    # After creating the zip, delete the original directory
-                    shutil.rmtree(directory_to_zip)
-                    print("Just Completed zip:", zip_file_path)
-        zip_ref.close()
-
-
-
-if __name__ == '__main__':
-    arg_parser = ArgumentParser('jalc.py', description='''This script does the preprocessing of the initial JALC dump, in particular it splits the original zip files in smaller ones if they contain more than 100 JSON files 
-                                and it modifies the dump's original structure by removing the intermediate directories and bringing it to the following structure: dump.zip -> prefixes.zip -> json files''')
-    arg_parser.add_argument('-ja', '--jalc', dest='jalc_json_dir', required=True, help='Directory that contains the original zipped dump')
-    arg_parser.add_argument('-out', '--output', dest='output_dir', required=True, help='Directory where the files of the original dump will be stored, and the directory will be zipped.')
-    arg_parser.add_argument('-m', '--max_workers', required=False, default=1, type=int, help='Workers number')
-    args = arg_parser.parse_args()
-    jalc_json_dir = args.jalc_json_dir
-    jalc_json_dir = normalize_path(jalc_json_dir)
-    output_dir = args.output_dir
-    output_dir = normalize_path(output_dir)
-    max_workers = args.max_workers
-    preprocessing(jalc_json_dir, output_dir, max_workers)
-
+
+import shutil
+from tqdm import tqdm
+from oc_ds_converter.lib.jsonmanager import *
+from oc_ds_converter.lib.file_manager import normalize_path
+from argparse import ArgumentParser
+from pebble import ProcessPool, ProcessFuture
+
+
+def preprocessing(jalc_json_dir:str, output_dir:str, max_workers:int = 1):
+    """This function preprocesses the original JALC zipped dump. The original dump has the following structure:
+    - jalc_dump.zip
+        -jalc_dataset_dir
+            -prefixes.json
+            -prefix1.zip
+                -prefix1_dir
+                    -doiList1.json
+                    -doi1A.json
+                    -doi1B.json
+                    -etc.
+            -prefix2.zip
+                -prefix2_dir
+                    -doiList2.json
+                    -doi2A.json
+                    -etc.
+    The preprocessing in particular removes the intermediate folders (like jalc_dump, prefix1, prefix2 in the example above)
+    and if inside one prefix.zip file are found more than 100 files, the original zip file is divided into the number of
+    json files in it//100 +1. In the case in which a prefix.zip file is divided into more zip files, the doiList.json is copied
+    just in the first subfile."""
+
+    '''In the els_to_be_skipped list are appended all the files found in the input directory starting with
+    "._" and the zip file if the corresponding decompressed directory is found'''
+    els_to_be_skipped = []
+    input_dir_cont = os.listdir(jalc_json_dir)
+    for el in input_dir_cont:# should be one (the input dir contains 1 zip)
+        if el.startswith("._"):
+            # skip elements starting with ._
+            els_to_be_skipped.append(os.path.join(jalc_json_dir, el))
+        else:
+            if el.endswith(".zip"):
+                base_name = el.replace('.zip', '')
+                if [x for x in os.listdir(jalc_json_dir) if x.startswith(base_name) and x.endswith("decompr_zip_dir")]:
+                    els_to_be_skipped.append(os.path.join(jalc_json_dir, el))
+
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+
+    all_unzipped_files = []
+    '''The elements in the "els_to_be_skipped" list are now taken into account. If inside the list a zip element is found,
+    the corresponding unzipped folder (if found in the input directory) is used to list all the elements inside the original 
+    zipped dump.'''
+    els_to_be_skipped_cont = [x for x in els_to_be_skipped if x.endswith(".zip")]
+    if els_to_be_skipped_cont:
+        for el_to_skip in els_to_be_skipped_cont:
+            if el_to_skip.startswith("._"):
+                continue
+            base_name_el_to_skip = os.path.basename(el_to_skip).replace('.zip', '')
+            for directory in os.listdir(jalc_json_dir):
+                if directory == base_name_el_to_skip + "_decompr_zip_dir":
+                    # if el.startswith(base_name_el_to_skip) and el.endswith("decompr_zip_dir"):
+                    for dir_lev2 in os.listdir(os.path.join(jalc_json_dir, directory)):
+                        all_unzipped_files = [os.path.join(jalc_json_dir, directory, dir_lev2, file) for file in os.listdir(os.path.join(jalc_json_dir, directory, dir_lev2)) if not file.startswith("._")]
+
+    '''If there aren't elements in the "els_to_be_skipped" list all the elements in the original
+    zipped dump are extracted in a folder with the same basename of the original dump + "_decompre_zip_dir".'''
+    if len(all_unzipped_files) == 0:
+        for zip_lev0 in os.listdir(jalc_json_dir):
+            if zip_lev0.endswith("zip") and not zip_lev0.startswith("._"):
+                with zipfile.ZipFile(os.path.join(jalc_json_dir, zip_lev0), 'r') as zip_ref:
+                    dest_dir = os.path.join(jalc_json_dir, zip_lev0).replace('.zip', '') + "_decompr_zip_dir"
+                    if not exists(dest_dir):
+                        makedirs(dest_dir)
+                    zip_ref.extractall(dest_dir)
+                    print(f"Unzipped to {dest_dir}")
+                for cur_dir, cur_subdir, cur_files in walk(dest_dir):
+                    for cur_file in cur_files:
+                        if not basename(cur_file).startswith("."):
+                            all_unzipped_files.append(cur_dir + sep + cur_file)
+
+
+
+    # Filter for zip files (files with ".zip" extension)
+    zip_files = [file for file in all_unzipped_files if file.endswith(".zip")]
+    not_zip_files = [file for file in all_unzipped_files if not file.endswith(".zip")]
+
+    # copy all extra files as they are in the output dir
+    for file in not_zip_files:
+        if os.path.isfile(file):
+            shutil.copy(file, output_dir)
+
+    # parallelization of the process
+    if max_workers == 1:
+        for zip_file in tqdm(zip_files, desc="Processing ZIP Files"):
+            process_zip(zip_file, output_dir)
+
+    else:
+        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
+            for zip_file in tqdm(zip_files, desc="Processing ZIP Files"):
+                future: ProcessFuture = executor.schedule(function=process_zip, args=[zip_file, output_dir])
+
+
+    # At the end of the process, create a ZIP archive of the output_dir and rename it
+    print("Zipping the output directory")
+    shutil.make_archive(output_dir, 'zip', output_dir)
+    print("Removing output directory")
+    shutil.rmtree(output_dir)  # Delete the original directory
+
+
+def process_zip(zip_file, output_dir2):
+
+    if not zip_file.endswith(".zip"):
+        shutil.copy(zip_file, output_dir2)
+
+    else:
+        # manage the resizing
+        # Full path to the zip file
+        zip_file_path = zip_file
+        first_level_path = os.path.dirname(zip_file_path)
+        print("executing", zip_file_path)
+        # Open the zip file for reading
+        with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
+            all_files_in_zip = zip_ref.namelist()
+
+            directories = [entry for entry in all_files_in_zip if entry.endswith('/')]
+            # List the names of files within the zip (the relevant one, the json containing the citation information)
+            file_names = [x for x in all_files_in_zip if x.endswith(".json") and "doiList" not in x and x not in directories]
+            extra_file_names = [x for x in all_files_in_zip if "doiList" in x or x.endswith(".out")]
+
+            if len(file_names) <= 100:
+                print("less than 100")
+                zip_file_name = os.path.basename(zip_file_path).replace(".zip", "")
+                dir_to_zip = os.path.join(output_dir2, zip_file_name)
+                os.makedirs(dir_to_zip, exist_ok=True)
+                for non_zip in extra_file_names:
+                    if not os.path.isdir(non_zip) and 'doiList' in non_zip:
+                        '''We use os.path.basename(file_info.filename) to extract just the filename
+                        without the folder structure. We create a new file in the destination folder 
+                        with the extracted filename and write the content of the file from the ZIP archive into it.'''
+                        file_info = zip_ref.getinfo(non_zip)
+                        extracted_file_path = os.path.join(dir_to_zip, os.path.basename(file_info.filename))
+                        with open(extracted_file_path, 'wb') as extracted_file:
+                            extracted_file.write(zip_ref.read(non_zip))
+                for fs in file_names:
+                    file_info = zip_ref.getinfo(fs)
+                    extracted_file_path = os.path.join(dir_to_zip,
+                                                       os.path.basename(file_info.filename))
+                    with open(extracted_file_path, 'wb') as extracted_file:
+                        extracted_file.write(zip_ref.read(fs))
+
+                # Parent directory
+                parent_directory = os.path.dirname(dir_to_zip)
+                # Name the zip file
+                zip_file_name = dir_to_zip + ".zip"
+                # Full path to the destination zip file
+                zip_file_path = os.path.join(parent_directory, zip_file_name)
+
+                with zipfile.ZipFile(zip_file_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
+                    for foldername, subfolders, filenames in os.walk(dir_to_zip):
+                        for filename in filenames:
+                            file_path = os.path.join(foldername, filename)
+                            relative_path = os.path.relpath(file_path, dir_to_zip)
+                            zipf.write(file_path, relative_path)
+                # After creating the zip, delete the original directory
+                shutil.rmtree(dir_to_zip)
+                #print("Just Completed zip:", zip_file_path)
+
+            else:
+                # if there are more than 100 jsons, they should be divided as many zips as the total number of jsons/ 100.
+                # The first of the new sub-zip files should also contain all the extra files which where stored in the original zip
+                print("more than 100: ", len(file_names))
+                zip_basename = zip_file_path.replace(".zip", "").replace(first_level_path, "").replace("/", "").replace(
+                "\\", "")
+                zip_part_counter = 0
+
+                while len(file_names):
+                    # name of the new folder (prefix_0.zip)
+                    zip_basename_w_counter = zip_basename + "_" + str(zip_part_counter)
+                    # path of the new folder where files will be extracted
+                    sliced_out_name = os.path.join(output_dir2, zip_basename_w_counter)
+                    os.makedirs(sliced_out_name, exist_ok=True)
+
+                    # copying in the output folder all the extra files (not json files with information on the bibliographic entities)
+                    if zip_part_counter == 0:
+                        for non_zip in extra_file_names:
+                            if not os.path.isdir(non_zip) and 'doiList' in non_zip:
+                                '''We use os.path.basename(file_info.filename) to extract just the filename
+                                without the folder structure. We create a new file in the destination folder 
+                                with the extracted filename and write the content of the file from the ZIP archive into it.'''
+                                file_info = zip_ref.getinfo(non_zip)
+                                extracted_file_path = os.path.join(sliced_out_name, os.path.basename(file_info.filename))
+                                with open(extracted_file_path, 'wb') as extracted_file:
+                                    extracted_file.write(zip_ref.read(non_zip))
+
+                    if len(file_names) > 100:
+                        print("json to be processed in this zip:", len(file_names))
+
+                        files_slice = file_names[:100]
+                        file_names = file_names[100:]
+                        zip_part_counter +=1
+
+                        for fs in files_slice:
+                            file_info = zip_ref.getinfo(fs)
+                            extracted_file_path = os.path.join(sliced_out_name,
+                                                               os.path.basename(file_info.filename))
+                            with open(extracted_file_path, 'wb') as extracted_file:
+                                extracted_file.write(zip_ref.read(fs))
+                    else:
+                        print("last", len(file_names), "jsons to be processed")
+                        files_slice = file_names
+                        file_names = []
+                        zip_part_counter += 1
+
+                        for fs in files_slice:
+                            file_info = zip_ref.getinfo(fs)
+                            extracted_file_path = os.path.join(sliced_out_name,
+                                                               os.path.basename(file_info.filename))
+                            with open(extracted_file_path, 'wb') as extracted_file:
+                                extracted_file.write(zip_ref.read(fs))
+
+                    # Directory to zip and delete
+                    directory_to_zip = sliced_out_name
+                    # Parent directory
+                    parent_directory = os.path.dirname(directory_to_zip)
+                    # Name the zip file
+                    zip_file_name = directory_to_zip + ".zip"
+                    # Full path to the destination zip file
+                    zip_file_path = os.path.join(parent_directory, zip_file_name)
+                    # create a zip file
+                    with zipfile.ZipFile(zip_file_name, 'w', zipfile.ZIP_DEFLATED) as zipf:
+                        for foldername, subfolders, filenames in os.walk(directory_to_zip):
+                            for filename in filenames:
+                                file_path = os.path.join(foldername, filename)
+                                relative_path = os.path.relpath(file_path, directory_to_zip)
+                                zipf.write(file_path, relative_path)
+                    # After creating the zip, delete the original directory
+                    shutil.rmtree(directory_to_zip)
+                    #print("Just Completed zip:", zip_file_path)
+        zip_ref.close()
+
+
+
+if __name__ == '__main__':
+    arg_parser = ArgumentParser('jalc.py', description='''This script does the preprocessing of the initial JALC dump, in particular it splits the original zip files in smaller ones if they contain more than 100 JSON files 
+                                and it modifies the dump's original structure by removing the intermediate directories and bringing it to the following structure: dump.zip -> prefixes.zip -> json files''')
+    arg_parser.add_argument('-ja', '--jalc', dest='jalc_json_dir', required=True, help='Directory that contains the original zipped dump')
+    arg_parser.add_argument('-out', '--output', dest='output_dir', required=True, help='Directory where the files of the original dump will be stored, and the directory will be zipped.')
+    arg_parser.add_argument('-m', '--max_workers', required=False, default=1, type=int, help='Workers number')
+    args = arg_parser.parse_args()
+    jalc_json_dir = args.jalc_json_dir
+    jalc_json_dir = normalize_path(jalc_json_dir)
+    output_dir = args.output_dir
+    output_dir = normalize_path(output_dir)
+    max_workers = args.max_workers
+    preprocessing(jalc_json_dir, output_dir, max_workers)
+
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/preprocessing/nih.py` & `oc_ds_converter-1.0.1/oc_ds_converter/preprocessing/nih.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-import csv
-import os.path
-import sys
-from os import makedirs
-from os.path import exists
-
-import pandas as pd
-from oc_ds_converter.preprocessing.base import Preprocessing
-from tqdm import tqdm
-
-
-class NIHPreProcessing(Preprocessing):
-    """This class aims at pre-processing iCite Database Snapshots (NIH Open
-    Citation Collection + ICite Metadata), available at:
-    https://nih.figshare.com/search?q=iCite+Database+Snapshot. In particular,
-    NIHPreProcessing splits the original CSV file in many lighter CSV files,
-    each one containing the number of entities specified in input by the user"""
-    def __init__(self, input_dir, output_dir, interval, filter=None):
-        self._req_type = ".csv"
-        self._input_dir = input_dir
-        self._output_dir = output_dir
-        if not exists(self._output_dir):
-            makedirs(self._output_dir)
-        self._interval = interval
-        if filter:
-            self._filter = filter
-        else:
-            self._filter = ["pmid","doi","title","authors","year","journal", "cited_by","references"]
-        super(NIHPreProcessing, self).__init__()
-
-    def split_input(self):
-        maxInt = sys.maxsize
-        while True:
-            # decrease the maxInt value by factor 10
-            # as long as the OverflowError occurs.
-            try:
-                csv.field_size_limit(maxInt)
-                break
-            except OverflowError:
-                maxInt = int(maxInt / 10)
-
-        all_files = self.get_all_files(self._input_dir, self._req_type)
-        count = 0
-        lines = []
-        headers = self._filter
-        for file_idx, file in enumerate(all_files):
-            if isinstance(file, list):
-                file = file[0]
-            if file:
-                #df = pd.DataFrame()
-                iter_csv = pd.read_csv(file, usecols=self._filter, chunksize=1000, engine='python')
-                try:
-                    for chunk in tqdm(iter_csv):
-                        try:
-                            f = pd.concat([chunk], ignore_index=True)
-                            f.fillna("", inplace=True)
-                            #df = pd.read_csv(file, usecols=self._filter, low_memory=True, dtype={'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': int, 'journal': str, 'is_research_article': bool, 'citation_count':int, 'field_citation_rate': float, 'expected_citations_per_year': float, 'citations_per_year':float, 'relative_citation_ratio': float, 'nih_percentile': int, 'human': float, 'animal': float, 'molecular_cellular': float, 'x_coord':float,	'y_coord': float, 'apt': float, 'is_clinical': bool, 'cited_by_clin': str, 'cited_by': str, 'references':str, 'provisional': str})
-                            #df.fillna("", inplace=True)
-                            f1 = f.values.tolist()
-
-                            for line in tqdm(f1):
-                                try:
-                                    count += 1
-                                    lines.append(line)
-                                    if int(count) != 0 and int(count) % int(self._interval) == 0:
-                                        lines = self.splitted_to_file(
-                                            count, self._interval, self._output_dir, lines, headers
-                                    )
-                                except:
-                                    print("error with line:", line)
-                        except:
-                            print("error with chunk:", chunk)
-                except:
-                    print("error with pd.read_csv")
-
-        if len(lines) > 0:
-            self.splitted_to_file(count, self._interval, self._output_dir, lines, headers)
-
-
-    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
-        if int(cur_n) != 0 and int(cur_n) % int(target_n) == 0:
-            # to be logged: print("Processed lines:", cur_n, ". Reduced csv nr.", cur_n // target_n)
-            filename = "CSVFile_" + str(cur_n // target_n) + self._req_type
-            with (
-                open(os.path.join(out_dir, filename), "w", encoding="utf8", newline="")
-            ) as f_out:
-                writer = csv.writer(f_out)
-                writer.writerow(headers)
-                writer.writerows(data)
-                lines = []
-            return lines
-        else:
-            # to be logged: print("Processed lines:", cur_n)
-            filename = "CSVFile_" + "Rem" + self._req_type
-            with (
-                open(os.path.join(out_dir, filename), "w", encoding="utf8", newline="")
-            ) as f_out:
-                writer = csv.writer(f_out)
-                writer.writerow(headers)
-                writer.writerows(data)
+import csv
+import os.path
+import sys
+from os import makedirs
+from os.path import exists
+
+import pandas as pd
+from oc_ds_converter.preprocessing.base import Preprocessing
+from tqdm import tqdm
+
+
+class NIHPreProcessing(Preprocessing):
+    """This class aims at pre-processing iCite Database Snapshots (NIH Open
+    Citation Collection + ICite Metadata), available at:
+    https://nih.figshare.com/search?q=iCite+Database+Snapshot. In particular,
+    NIHPreProcessing splits the original CSV file in many lighter CSV files,
+    each one containing the number of entities specified in input by the user"""
+    def __init__(self, input_dir, output_dir, interval, filter=None):
+        self._req_type = ".csv"
+        self._input_dir = input_dir
+        self._output_dir = output_dir
+        if not exists(self._output_dir):
+            makedirs(self._output_dir)
+        self._interval = interval
+        if filter:
+            self._filter = filter
+        else:
+            self._filter = ["pmid","doi","title","authors","year","journal", "cited_by","references"]
+        super(NIHPreProcessing, self).__init__()
+
+    def split_input(self):
+        maxInt = sys.maxsize
+        while True:
+            # decrease the maxInt value by factor 10
+            # as long as the OverflowError occurs.
+            try:
+                csv.field_size_limit(maxInt)
+                break
+            except OverflowError:
+                maxInt = int(maxInt / 10)
+
+        all_files = self.get_all_files(self._input_dir, self._req_type)
+        count = 0
+        lines = []
+        headers = self._filter
+        for file_idx, file in enumerate(all_files):
+            if isinstance(file, list):
+                file = file[0]
+            if file:
+                #df = pd.DataFrame()
+                iter_csv = pd.read_csv(file, usecols=self._filter, chunksize=1000, engine='python')
+                try:
+                    for chunk in tqdm(iter_csv):
+                        try:
+                            f = pd.concat([chunk], ignore_index=True)
+                            f.fillna("", inplace=True)
+                            #df = pd.read_csv(file, usecols=self._filter, low_memory=True, dtype={'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': int, 'journal': str, 'is_research_article': bool, 'citation_count':int, 'field_citation_rate': float, 'expected_citations_per_year': float, 'citations_per_year':float, 'relative_citation_ratio': float, 'nih_percentile': int, 'human': float, 'animal': float, 'molecular_cellular': float, 'x_coord':float,	'y_coord': float, 'apt': float, 'is_clinical': bool, 'cited_by_clin': str, 'cited_by': str, 'references':str, 'provisional': str})
+                            #df.fillna("", inplace=True)
+                            f1 = f.values.tolist()
+
+                            for line in tqdm(f1):
+                                try:
+                                    count += 1
+                                    lines.append(line)
+                                    if int(count) != 0 and int(count) % int(self._interval) == 0:
+                                        lines = self.splitted_to_file(
+                                            count, self._interval, self._output_dir, lines, headers
+                                    )
+                                except:
+                                    print("error with line:", line)
+                        except:
+                            print("error with chunk:", chunk)
+                except:
+                    print("error with pd.read_csv")
+
+        if len(lines) > 0:
+            self.splitted_to_file(count, self._interval, self._output_dir, lines, headers)
+
+
+    def splitted_to_file(self, cur_n, target_n, out_dir, data, headers=None):
+        if int(cur_n) != 0 and int(cur_n) % int(target_n) == 0:
+            # to be logged: print("Processed lines:", cur_n, ". Reduced csv nr.", cur_n // target_n)
+            filename = "CSVFile_" + str(cur_n // target_n) + self._req_type
+            with (
+                open(os.path.join(out_dir, filename), "w", encoding="utf8", newline="")
+            ) as f_out:
+                writer = csv.writer(f_out)
+                writer.writerow(headers)
+                writer.writerows(data)
+                lines = []
+            return lines
+        else:
+            # to be logged: print("Processed lines:", cur_n)
+            filename = "CSVFile_" + "Rem" + self._req_type
+            with (
+                open(os.path.join(out_dir, filename), "w", encoding="utf8", newline="")
+            ) as f_out:
+                writer = csv.writer(f_out)
+                writer.writerow(headers)
+                writer.writerows(data)
             return
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/pubmed/finder_nih.py` & `oc_ds_converter-1.0.1/oc_ds_converter/pubmed/finder_nih.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-#!python
-# Copyright (c) 2022 The OpenCitations Index Authors.
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-import re
-from datetime import datetime
-from urllib.parse import quote, unquote
-
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager.issn import ISSNManager
-from oc_ds_converter.oc_idmanager.pmid import PMIDManager
-from requests import get
-
-
-class NIHResourceFinder():
-    """This class implements an api pmid resource finder for NIH"""
-
-    def __init__(self, data={}, use_api_service=True):
-        """National Institute of Health resource finder constructor."""
-        self._api = "https://pubmed.ncbi.nlm.nih.gov/"
-        self._use_api_service = use_api_service
-        self._p = "pmid:"
-        self._data = data
-        self._im = ISSNManager()
-        self._pm = PMIDManager()
-        self._headers = {
-            "User-Agent": "ResourceFinder / OpenCitations Indexes "
-            "(http://opencitations.net; mailto:contact@opencitations.net)"
-        }
-        self._issn_regex = r"(?<=^IS\s{2}-\s)[0-9]{4}-[0-9]{3}[0-9X]"
-        self._jtitle_regex = r"(?<=^JT\s{2}-\s)(.*)(?<!\n)$"
-        self._date_regex = r"DP\s+-\s+(\d{4}(\s?(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec))?(\s?((3[0-1])|([1-2][0-9])|([0]?[1-9])))?)"
-        super(NIHResourceFinder, self).__init__()
-
-    def _get_issn(self, txt_obj):
-        result = set()
-        fa_issn = re.finditer(self._issn_regex, txt_obj, re.MULTILINE)
-        for matchNum_issn, match_issn in enumerate(fa_issn, start=1):
-            m_issn = match_issn.group()
-            if m_issn:
-                norm_issn = self._im.normalise(m_issn, include_prefix=True)
-                if norm_issn is not None:
-                    result.add(norm_issn)
-        return result
-
-    def _get_extended_j_title(self, txt_obj):
-        matches = re.finditer(self._jtitle_regex, txt_obj, re.MULTILINE)
-        for matchNum, match in enumerate(matches, start=1):
-            m = match.group()
-            if m:
-                m = unquote(m.strip())
-                return m
-
-    def _get_date(self, txt_obj):
-        pmid_date = None
-        date = re.search(self._date_regex,
-                         txt_obj,
-                         re.IGNORECASE,
-                         ).group(1)
-        re_search = re.search(
-            "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s+((3[0-1])|([1-2][0-9])|([0]?[1-9]))",
-            date,
-            re.IGNORECASE,
-        )
-        if re_search is not None:
-            src = re_search.group(0)
-            datetime_object = datetime.strptime(src, "%Y %b %d")
-            pmid_date = datetime.strftime(datetime_object, "%Y-%m-%d")
-        else:
-            re_search = re.search(
-                "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)",
-                date,
-                re.IGNORECASE,
-            )
-            if re_search is not None:
-                src = re_search.group(0)
-                datetime_object = datetime.strptime(src, "%Y %b")
-                pmid_date = datetime.strftime(datetime_object, "%Y-%m")
-            else:
-                re_search = re.search("(\d{4})", date)
-                if re_search is not None:
-                    src = re.search("(\d{4})", date).group(0)
-                    datetime_object = datetime.strptime(src, "%Y")
-                    pmid_date = datetime.strftime(datetime_object, "%Y")
-        return pmid_date
-
-
-    def _call_api(self, pmid_full):
-        if self._use_api_service:
-            pmid = self._pm.normalise(pmid_full)
-            r = get(
-                self._api + quote(pmid) + "/?format=pubmed",
-                headers=self._headers,
-                timeout=30,
-            )
-            if r.status_code == 200:
-                r.encoding = "utf-8"
-                soup = BeautifulSoup(r.text, features="lxml")
-                mdata = str(soup.find(id="article-details"))
-                return mdata
+#!python
+# Copyright (c) 2022 The OpenCitations Index Authors.
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+import re
+from datetime import datetime
+from urllib.parse import quote, unquote
+
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager.issn import ISSNManager
+from oc_ds_converter.oc_idmanager.pmid import PMIDManager
+from requests import get
+
+
+class NIHResourceFinder():
+    """This class implements an api pmid resource finder for NIH"""
+
+    def __init__(self, data={}, use_api_service=True):
+        """National Institute of Health resource finder constructor."""
+        self._api = "https://pubmed.ncbi.nlm.nih.gov/"
+        self._use_api_service = use_api_service
+        self._p = "pmid:"
+        self._data = data
+        self._im = ISSNManager()
+        self._pm = PMIDManager()
+        self._headers = {
+            "User-Agent": "ResourceFinder / OpenCitations Indexes "
+            "(http://opencitations.net; mailto:contact@opencitations.net)"
+        }
+        self._issn_regex = r"(?<=^IS\s{2}-\s)[0-9]{4}-[0-9]{3}[0-9X]"
+        self._jtitle_regex = r"(?<=^JT\s{2}-\s)(.*)(?<!\n)$"
+        self._date_regex = r"DP\s+-\s+(\d{4}(\s?(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec))?(\s?((3[0-1])|([1-2][0-9])|([0]?[1-9])))?)"
+        super(NIHResourceFinder, self).__init__()
+
+    def _get_issn(self, txt_obj):
+        result = set()
+        fa_issn = re.finditer(self._issn_regex, txt_obj, re.MULTILINE)
+        for matchNum_issn, match_issn in enumerate(fa_issn, start=1):
+            m_issn = match_issn.group()
+            if m_issn:
+                norm_issn = self._im.normalise(m_issn, include_prefix=True)
+                if norm_issn is not None:
+                    result.add(norm_issn)
+        return result
+
+    def _get_extended_j_title(self, txt_obj):
+        matches = re.finditer(self._jtitle_regex, txt_obj, re.MULTILINE)
+        for matchNum, match in enumerate(matches, start=1):
+            m = match.group()
+            if m:
+                m = unquote(m.strip())
+                return m
+
+    def _get_date(self, txt_obj):
+        pmid_date = None
+        date = re.search(self._date_regex,
+                         txt_obj,
+                         re.IGNORECASE,
+                         ).group(1)
+        re_search = re.search(
+            "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s+((3[0-1])|([1-2][0-9])|([0]?[1-9]))",
+            date,
+            re.IGNORECASE,
+        )
+        if re_search is not None:
+            src = re_search.group(0)
+            datetime_object = datetime.strptime(src, "%Y %b %d")
+            pmid_date = datetime.strftime(datetime_object, "%Y-%m-%d")
+        else:
+            re_search = re.search(
+                "(\d{4})\s+(Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)",
+                date,
+                re.IGNORECASE,
+            )
+            if re_search is not None:
+                src = re_search.group(0)
+                datetime_object = datetime.strptime(src, "%Y %b")
+                pmid_date = datetime.strftime(datetime_object, "%Y-%m")
+            else:
+                re_search = re.search("(\d{4})", date)
+                if re_search is not None:
+                    src = re.search("(\d{4})", date).group(0)
+                    datetime_object = datetime.strptime(src, "%Y")
+                    pmid_date = datetime.strftime(datetime_object, "%Y")
+        return pmid_date
+
+
+    def _call_api(self, pmid_full):
+        if self._use_api_service:
+            pmid = self._pm.normalise(pmid_full)
+            r = get(
+                self._api + quote(pmid) + "/?format=pubmed",
+                headers=self._headers,
+                timeout=30,
+            )
+            if r.status_code == 200:
+                r.encoding = "utf-8"
+                soup = BeautifulSoup(r.text, features="lxml")
+                mdata = str(soup.find(id="article-details"))
+                return mdata
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/pubmed/get_publishers.py` & `oc_ds_converter-1.0.1/oc_ds_converter/pubmed/get_publishers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import re
-
-import requests
-from lxml import etree
-
-
-class ExtractPublisherDOI(object):
-    def __init__(self, pref_info_dict):
-        self.description = "class aimed at extracting publishers' names exploiting the DOI "
-        self.datacite_prefixes = ['10.48550', '10.4230', '10.5281', '10.17863', '10.3929', '10.6084', '10.5451', '10.5445', '10.17615', '10.17877', '10.5167', '10.13140', '10.18154', '10.48350', '10.7892', '10.17605', '10.5283', '10.17169', '10.15488', '10.5169', '10.1184', '10.3204', '10.6073', '10.14288', '10.5061', '10.25384']
-        if pref_info_dict:
-            self._prefix_to_data_dict = pref_info_dict
-        else:
-            self._prefix_to_data_dict = dict()
-
-    def get_registration_agency(self, prefix):
-        req_url = "https://doi.org/ra/"+prefix
-        try:
-            req = requests.get(url=req_url)
-            req_status_code = req.status_code
-            if req_status_code == 200:
-                req_data = req.json()
-                ra = req_data[0].get("RA")
-                if ra:
-                    norm_ra = ra.lower().strip()
-                    if norm_ra:
-                        return norm_ra
-                    else:
-                        return ""
-        except requests.ConnectionError:
-            print("failed to connect to crossref for", prefix)
-            quit()
-        return ""
-
-    def get_last_map_ver(self):
-        return self._prefix_to_data_dict
-
-    def add_prefix_pub_data(self,prefix):
-        if prefix not in self._prefix_to_data_dict.keys():
-            pref_to_publisher = dict()
-            req_url = "https://api.crossref.org/prefixes/" + prefix
-
-            try:
-                req = requests.get(url=req_url)
-                req_status_code = req.status_code
-                if req_status_code == 200:
-                    req_data = req.json()
-                    pref_to_publisher["name"] = req_data["message"]["name"]
-                    extended_member_code = req_data["message"]["member"]
-                    reduced_member_code = (re.findall("(\d+)", extended_member_code))[0]
-                    pref_to_publisher["crossref_member"] = reduced_member_code
-                    pref_to_publisher["from"] = "Crossref"
-                else:
-                    pref_to_publisher["name"] = "unidentified"
-                    pref_to_publisher["crossref_member"] = "not found"
-                    pref_to_publisher["from"] = "not found"
-
-
-                self._prefix_to_data_dict[prefix] = pref_to_publisher
-
-            except requests.ConnectionError:
-                print("failed to connect to crossref for", prefix)
-                quit()
-        return self._prefix_to_data_dict
-
-
-    def search_in_datacite(self,doi):
-        publisher = dict()
-        datacite_req_url = "https://api.datacite.org/dois/" + doi
-
-        try:
-            req = requests.get(url=datacite_req_url)
-
-            req_status_code = req.status_code
-            if req_status_code == 200:
-                req_data = req.json()
-                publisher["name"] = req_data["data"]["attributes"]["publisher"]
-                publisher["prefix"] = doi.split('/')[0]
-
-        except requests.ConnectionError:
-            print("failed to connect to datacite for", doi)
-
-        return publisher
-
-
-    def search_in_medra(self, doi):
-        publisher = dict()
-        medra_req_url = "https://api.medra.org/metadata/" + doi
-
-        try:
-            req = requests.get(url=medra_req_url)
-
-            req_status_code = req.status_code
-            if req_status_code == 200:
-                tree = etree.XML(req.content)
-                publisher_xpath = tree.xpath('//x:PublisherName',
-                                             namespaces={'x': 'http://www.editeur.org/onix/DOIMetadata/2.0'})
-                if len(publisher_xpath) == 0:
-                    return publisher
-                publisher["name"] = publisher_xpath[0].text
-                publisher["prefix"] = doi.split('/')[0]
-
-        except requests.ConnectionError:
-            print("failed to connect to crossref for", doi)
-
-        return publisher
-
-
-    def search_for_cnki(self,doi):
-        publisher = dict()
-        datacite_req_url = "https://doi.org/api/handles/" + doi
-
-        try:
-            req = requests.get(url=datacite_req_url)
-
-            req_status_code = req.status_code
-            if req_status_code == 200:
-                req_data = req.json()
-                if 'values' in req_data.keys() and 'data' in req_data['values'][0].keys():
-                    if 'www.cnki.net' in req_data['values'][0]['data']['value']:
-                        publisher["name"] = 'CNKI Publisher (unspecified)'
-                        publisher["prefix"] = doi.split('/')[0]
-
-        except requests.ConnectionError:
-            print("failed to connect to doi for", doi)
-
-        return publisher
-
-
-    def add_extra_publisher(self, publisher, agency):
-        self._prefix_to_data_dict[publisher["prefix"]] = {
-            'name': publisher['name'],
-            'from': agency
-        }
-
-
-    def search_for_publisher_in_other_agencies(self,doi):
-        publisher = self.search_in_datacite(doi)
-        if 'name' in publisher.keys():
-            self.add_extra_publisher(publisher, 'datacite')
-            return self._prefix_to_data_dict
-        publisher = self.search_in_medra(doi)
-        if 'name' in publisher.keys():
-            self.add_extra_publisher(publisher, 'medra')
-            return self._prefix_to_data_dict
-        publisher = self.search_for_cnki(doi)
-        if 'name' in publisher.keys():
-            self.add_extra_publisher(publisher, 'doi')
-            return self._prefix_to_data_dict
-
-
-    """
-    extract_publishers_valid(row, publisher_data, prefix_to_member_code_dict, external_data_dict) manages the 
-    addition of unprocessed publishers’ dictionaries to publisher_data and the update 
-    of the values related to the number of either valid or invalid addressed or received 
-    citations, in the case a dictionary for a given publisher already exists. 
-    In the case a publisher's prefix doesn't allow its identification in Crossref, we call the function 
-    search_for_publisher_in_other_agencies(row[1], external_data_dict), in order to try to identify it in other services.
-    This very last option is not included for the version for not validated citations. 
-    """
-
-    def extract_publishers_v(self,doi_or_pref, enable_extraagencies=True, get_all_prefix_data=False, skip_update=False):
-        if "/" in doi_or_pref:
-            prefix = re.findall("(10.\d{4,9})", doi_or_pref.split('/')[0])[0]
-        else:
-            prefix = re.findall("(10.\d{4,9})", doi_or_pref)[0]
-        if not skip_update:
-            self._prefix_to_data_dict = self.add_prefix_pub_data(prefix)
-
-        # set enable_extraagencies = False if you just want to use data already in the mapping and Crossref data
-        if not enable_extraagencies:
-            # set get_all_prefix_data = True if you want to retrieve all the info about the prefix and not only
-            # the name of the publisher
-            if get_all_prefix_data:
-                #return self._prefix_to_data_dict[prefix], self._prefix_to_data_dict
-                return self._prefix_to_data_dict[prefix]
-            else:
-                return self._prefix_to_data_dict[prefix]["name"]
-        else:
-            if self._prefix_to_data_dict[prefix]["from"] == "not found":
-                self.search_for_publisher_in_other_agencies(doi_or_pref)
-            if get_all_prefix_data:
-                return self._prefix_to_data_dict[prefix]
-                #return self._prefix_to_data_dict[prefix], self._prefix_to_data_dict
-            else:
-                return self._prefix_to_data_dict[prefix]["name"]
+import re
+
+import requests
+from lxml import etree
+
+
+class ExtractPublisherDOI(object):
+    def __init__(self, pref_info_dict):
+        self.description = "class aimed at extracting publishers' names exploiting the DOI "
+        self.datacite_prefixes = ['10.48550', '10.4230', '10.5281', '10.17863', '10.3929', '10.6084', '10.5451', '10.5445', '10.17615', '10.17877', '10.5167', '10.13140', '10.18154', '10.48350', '10.7892', '10.17605', '10.5283', '10.17169', '10.15488', '10.5169', '10.1184', '10.3204', '10.6073', '10.14288', '10.5061', '10.25384']
+        if pref_info_dict:
+            self._prefix_to_data_dict = pref_info_dict
+        else:
+            self._prefix_to_data_dict = dict()
+
+    def get_registration_agency(self, prefix):
+        req_url = "https://doi.org/ra/"+prefix
+        try:
+            req = requests.get(url=req_url)
+            req_status_code = req.status_code
+            if req_status_code == 200:
+                req_data = req.json()
+                ra = req_data[0].get("RA")
+                if ra:
+                    norm_ra = ra.lower().strip()
+                    if norm_ra:
+                        return norm_ra
+                    else:
+                        return ""
+        except requests.ConnectionError:
+            print("failed to connect to crossref for", prefix)
+            quit()
+        return ""
+
+    def get_last_map_ver(self):
+        return self._prefix_to_data_dict
+
+    def add_prefix_pub_data(self,prefix):
+        if prefix not in self._prefix_to_data_dict.keys():
+            pref_to_publisher = dict()
+            req_url = "https://api.crossref.org/prefixes/" + prefix
+
+            try:
+                req = requests.get(url=req_url)
+                req_status_code = req.status_code
+                if req_status_code == 200:
+                    req_data = req.json()
+                    pref_to_publisher["name"] = req_data["message"]["name"]
+                    extended_member_code = req_data["message"]["member"]
+                    reduced_member_code = (re.findall("(\d+)", extended_member_code))[0]
+                    pref_to_publisher["crossref_member"] = reduced_member_code
+                    pref_to_publisher["from"] = "Crossref"
+                else:
+                    pref_to_publisher["name"] = "unidentified"
+                    pref_to_publisher["crossref_member"] = "not found"
+                    pref_to_publisher["from"] = "not found"
+
+
+                self._prefix_to_data_dict[prefix] = pref_to_publisher
+
+            except requests.ConnectionError:
+                print("failed to connect to crossref for", prefix)
+                quit()
+        return self._prefix_to_data_dict
+
+
+    def search_in_datacite(self,doi):
+        publisher = dict()
+        datacite_req_url = "https://api.datacite.org/dois/" + doi
+
+        try:
+            req = requests.get(url=datacite_req_url)
+
+            req_status_code = req.status_code
+            if req_status_code == 200:
+                req_data = req.json()
+                publisher["name"] = req_data["data"]["attributes"]["publisher"]
+                publisher["prefix"] = doi.split('/')[0]
+
+        except requests.ConnectionError:
+            print("failed to connect to datacite for", doi)
+
+        return publisher
+
+
+    def search_in_medra(self, doi):
+        publisher = dict()
+        medra_req_url = "https://api.medra.org/metadata/" + doi
+
+        try:
+            req = requests.get(url=medra_req_url)
+
+            req_status_code = req.status_code
+            if req_status_code == 200:
+                tree = etree.XML(req.content)
+                publisher_xpath = tree.xpath('//x:PublisherName',
+                                             namespaces={'x': 'http://www.editeur.org/onix/DOIMetadata/2.0'})
+                if len(publisher_xpath) == 0:
+                    return publisher
+                publisher["name"] = publisher_xpath[0].text
+                publisher["prefix"] = doi.split('/')[0]
+
+        except requests.ConnectionError:
+            print("failed to connect to crossref for", doi)
+
+        return publisher
+
+
+    def search_for_cnki(self,doi):
+        publisher = dict()
+        datacite_req_url = "https://doi.org/api/handles/" + doi
+
+        try:
+            req = requests.get(url=datacite_req_url)
+
+            req_status_code = req.status_code
+            if req_status_code == 200:
+                req_data = req.json()
+                if 'values' in req_data.keys() and 'data' in req_data['values'][0].keys():
+                    if 'www.cnki.net' in req_data['values'][0]['data']['value']:
+                        publisher["name"] = 'CNKI Publisher (unspecified)'
+                        publisher["prefix"] = doi.split('/')[0]
+
+        except requests.ConnectionError:
+            print("failed to connect to doi for", doi)
+
+        return publisher
+
+
+    def add_extra_publisher(self, publisher, agency):
+        self._prefix_to_data_dict[publisher["prefix"]] = {
+            'name': publisher['name'],
+            'from': agency
+        }
+
+
+    def search_for_publisher_in_other_agencies(self,doi):
+        publisher = self.search_in_datacite(doi)
+        if 'name' in publisher.keys():
+            self.add_extra_publisher(publisher, 'datacite')
+            return self._prefix_to_data_dict
+        publisher = self.search_in_medra(doi)
+        if 'name' in publisher.keys():
+            self.add_extra_publisher(publisher, 'medra')
+            return self._prefix_to_data_dict
+        publisher = self.search_for_cnki(doi)
+        if 'name' in publisher.keys():
+            self.add_extra_publisher(publisher, 'doi')
+            return self._prefix_to_data_dict
+
+
+    """
+    extract_publishers_valid(row, publisher_data, prefix_to_member_code_dict, external_data_dict) manages the 
+    addition of unprocessed publishers’ dictionaries to publisher_data and the update 
+    of the values related to the number of either valid or invalid addressed or received 
+    citations, in the case a dictionary for a given publisher already exists. 
+    In the case a publisher's prefix doesn't allow its identification in Crossref, we call the function 
+    search_for_publisher_in_other_agencies(row[1], external_data_dict), in order to try to identify it in other services.
+    This very last option is not included for the version for not validated citations. 
+    """
+
+    def extract_publishers_v(self,doi_or_pref, enable_extraagencies=True, get_all_prefix_data=False, skip_update=False):
+        if "/" in doi_or_pref:
+            prefix = re.findall("(10.\d{4,9})", doi_or_pref.split('/')[0])[0]
+        else:
+            prefix = re.findall("(10.\d{4,9})", doi_or_pref)[0]
+        if not skip_update:
+            self._prefix_to_data_dict = self.add_prefix_pub_data(prefix)
+
+        # set enable_extraagencies = False if you just want to use data already in the mapping and Crossref data
+        if not enable_extraagencies:
+            # set get_all_prefix_data = True if you want to retrieve all the info about the prefix and not only
+            # the name of the publisher
+            if get_all_prefix_data:
+                #return self._prefix_to_data_dict[prefix], self._prefix_to_data_dict
+                return self._prefix_to_data_dict[prefix]
+            else:
+                return self._prefix_to_data_dict[prefix]["name"]
+        else:
+            if self._prefix_to_data_dict[prefix]["from"] == "not found":
+                self.search_for_publisher_in_other_agencies(doi_or_pref)
+            if get_all_prefix_data:
+                return self._prefix_to_data_dict[prefix]
+                #return self._prefix_to_data_dict[prefix], self._prefix_to_data_dict
+            else:
+                return self._prefix_to_data_dict[prefix]["name"]
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/pubmed/pubmed_dump_explorer.py` & `oc_ds_converter-1.0.1/oc_ds_converter/pubmed/pubmed_dump_explorer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2023 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import warnings
-
-import pandas as pd
-from tqdm import tqdm
-
-warnings.simplefilter('error', pd.errors.DtypeWarning)
-
-filepath = 'C:/Users/arcangelo.massari2/Downloads/icite_metadata/icite_metadata.csv'
-filter = ["pmid", "doi", "title", "authors", "year", "journal", "references"]
-pmid_found = set()
-duplicated_pmids = list()
-with open(filepath, 'r', encoding='utf8') as f:
-    number_of_rows = sum(1 for _ in f) - 1
-pbar = tqdm(total=number_of_rows)
-dtype={'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': str, 'journal': str, 'references': str}
-pmid_by_doi = dict()
-count_of_multiple_pmid_by_doi = set()
-try:
-    with pd.read_csv(filepath, usecols=filter, chunksize=100000, dtype=dtype) as reader:
-        for chunk in reader:
-            chunk.fillna("", inplace=True)
-            df_dict_list = chunk.to_dict("records")
-            filt_values = [d for d in df_dict_list if (d.get("cited_by") or d.get("references"))]
-            for item in filt_values:
-                pmid = item['pmid']
-                doi = item['doi']
-                if doi:
-                    pmid_by_doi.setdefault(doi, {'pmid': set(), 'title': ''})
-                    pmid_by_doi[doi]['pmid'].add(pmid)
-                    pmid_by_doi[doi]['title'] = item['title']
-                    if len(pmid_by_doi[doi]) > 1:
-                        count_of_multiple_pmid_by_doi.add(doi)
-            pbar.update(len(chunk))
-except pd.errors.DtypeWarning:
-    print(item)
-    raise(pd.errors.DtypeWarning)
-
-pbar.close()
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2023 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import warnings
+
+import pandas as pd
+from tqdm import tqdm
+
+warnings.simplefilter('error', pd.errors.DtypeWarning)
+
+filepath = 'C:/Users/arcangelo.massari2/Downloads/icite_metadata/icite_metadata.csv'
+filter = ["pmid", "doi", "title", "authors", "year", "journal", "references"]
+pmid_found = set()
+duplicated_pmids = list()
+with open(filepath, 'r', encoding='utf8') as f:
+    number_of_rows = sum(1 for _ in f) - 1
+pbar = tqdm(total=number_of_rows)
+dtype={'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': str, 'journal': str, 'references': str}
+pmid_by_doi = dict()
+count_of_multiple_pmid_by_doi = set()
+try:
+    with pd.read_csv(filepath, usecols=filter, chunksize=100000, dtype=dtype) as reader:
+        for chunk in reader:
+            chunk.fillna("", inplace=True)
+            df_dict_list = chunk.to_dict("records")
+            filt_values = [d for d in df_dict_list if (d.get("cited_by") or d.get("references"))]
+            for item in filt_values:
+                pmid = item['pmid']
+                doi = item['doi']
+                if doi:
+                    pmid_by_doi.setdefault(doi, {'pmid': set(), 'title': ''})
+                    pmid_by_doi[doi]['pmid'].add(pmid)
+                    pmid_by_doi[doi]['title'] = item['title']
+                    if len(pmid_by_doi[doi]) > 1:
+                        count_of_multiple_pmid_by_doi.add(doi)
+            pbar.update(len(chunk))
+except pd.errors.DtypeWarning:
+    print(item)
+    raise(pd.errors.DtypeWarning)
+
+pbar.close()
 print(len(count_of_multiple_pmid_by_doi))
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/pubmed/pubmed_processing.py` & `oc_ds_converter-1.0.1/oc_ds_converter/pubmed/pubmed_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,701 +1,741 @@
-import html
-import json
-import os
-import pathlib
-import re
-import warnings
-from os.path import exists
-from typing import Dict, List, Tuple
-
-import fakeredis
-from bs4 import BeautifulSoup
-from oc_ds_converter.oc_idmanager.doi import DOIManager
-from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
-from oc_ds_converter.oc_idmanager.pmid import PMIDManager
-from oc_ds_converter.lib.cleaner import Cleaner
-from oc_ds_converter.lib.master_of_regex import *
-
-from oc_ds_converter.datasource.redis import RedisDataSource
-from oc_ds_converter.pubmed.finder_nih import NIHResourceFinder
-from oc_ds_converter.pubmed.get_publishers import ExtractPublisherDOI
-from oc_ds_converter.ra_processor import RaProcessor
-
-warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
-
-
-class PubmedProcessing(RaProcessor):
-    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_pubmed: str = None, journals_filepath: str = None, testing:bool = True):
-        super(PubmedProcessing, self).__init__(orcid_index, doi_csv)
-        self.nihrf = NIHResourceFinder()
-        self.doi_m = DOIManager()
-        if testing:
-            self.BR_redis= fakeredis.FakeStrictRedis()
-            self.RA_redis= fakeredis.FakeStrictRedis()
-
-        else:
-            self.BR_redis = RedisDataSource("DB-META-BR")
-            self.RA_redis = RedisDataSource("DB-META-RA")
-
-        if not journals_filepath:
-            if not exists(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files")):
-                os.makedirs(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files"))
-            self.journals_filepath = os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files",
-                                                  "issn_jour_ext.json")
-        else:
-            self.journals_filepath = journals_filepath
-
-        self.jour_dict = self.issn_data_recover_poci(self.journals_filepath)
-
-
-        if not publishers_filepath_pubmed:
-            if not exists(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files")):
-                os.makedirs(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files"))
-            self.publishers_filepath = os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files",
-                                                  "prefix_publishers.json")
-        else:
-            self.publishers_filepath = publishers_filepath_pubmed
-
-        self.jour_dict = self.issn_data_recover_poci(self.journals_filepath)
-
-        if os.path.exists(self.publishers_filepath):
-            with open(self.publishers_filepath, "r", encoding="utf8") as fdp:
-                pfp = json.load(fdp)
-                if pfp:
-                    self.publisher_manager = ExtractPublisherDOI(pfp)
-                else:
-                    self.publisher_manager = ExtractPublisherDOI({})
-        else:
-            self.publisher_manager = ExtractPublisherDOI({})
-            with open(self.publishers_filepath, "w", encoding="utf8") as fdp:
-                json.dump({}, fdp, ensure_ascii=False, indent=4)
-
-
-    def issn_data_recover_poci(self, path):
-        journal_issn_dict = dict()
-        if not path:
-            return journal_issn_dict
-        if not os.path.exists(path):
-            return journal_issn_dict
-        else:
-            with open(path, "r", encoding="utf8") as fd:
-                journal_issn_dict = json.load(fd)
-                return journal_issn_dict
-
-
-    def issn_data_to_cache_poci(self, jtitle_issn_dict, path):
-        with open(path, "w", encoding="utf-8") as fd:
-            json.dump(jtitle_issn_dict, fd, ensure_ascii=False, indent=4)
-
-    def prefix_to_publisher_to_cache(self, pref_pub_dict, path):
-        with open(path, "w", encoding="utf-8") as fd:
-            json.dump(pref_pub_dict, fd, ensure_ascii=False, indent=4)
-
-    def csv_creator(self, item: dict) -> dict:
-        row = dict()
-        doi = ""
-        pmid = PMIDManager().normalise(str(item['pmid']))
-        if (pmid and self.doi_set and pmid in self.doi_set) or (pmid and not self.doi_set):
-            # create empty row
-            keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
-                    'publisher', 'editor']
-            for k in keys:
-                row[k] = ''
-
-            attributes = item
-
-            # row['type']
-            row['type'] = 'journal article'
-
-            # row['id']
-            ids_list = list()
-            ids_list.append(str('pmid:' + pmid))
-            if attributes.get('doi'):
-                doi = DOIManager().normalise(attributes.get('doi'), include_prefix=False)
-                if doi:
-                    doi_w_pref = "doi:"+doi
-                    if self.BR_redis.get(doi_w_pref):
-                        ids_list.append(doi_w_pref)
-                    elif self.doi_m.is_valid(doi):
-                        ids_list.append(doi_w_pref)
-                    else:
-                        doi = ''
-
-
-            row['id'] = ' '.join(ids_list)
-
-            # row['title']
-            pub_title = ""
-            if attributes.get("title"):
-                p_title = attributes.get("title")
-                soup = BeautifulSoup(p_title, 'html.parser')
-                title_soup = soup.get_text().replace('\n', '')
-                title_soup_space_replaced = ' '.join(title_soup.split())
-                title_soup_strip = title_soup_space_replaced.strip()
-                clean_tit = html.unescape(title_soup_strip)
-                pub_title = clean_tit if clean_tit else p_title
-
-            row['title'] = pub_title
-
-            agents_list = self.add_authors_to_agent_list(attributes, [])
-            authors_strings_list, editors_string_list = self.get_agents_strings_list(doi, agents_list)
-
-            # row['author']
-            if attributes.get('authors'):
-                row['author'] = '; '.join(authors_strings_list)
-
-            # row['pub_date']
-            dates = attributes.get("year")
-            row['pub_date'] = str(dates) if dates else ""
-
-            # row['venue']
-            row['venue'] = self.get_venue_name(attributes, pmid)
-
-            # row['volume']
-            row['volume'] = ""
-
-            # row['issue']
-            row['issue'] = ""
-
-            # row['page']
-            row['page'] = "" #self.get_pubmed_pages(attributes)
-
-            # row['publisher']
-            if doi:
-                try:
-                    row['publisher'] = self.get_publisher_name(doi)
-                except IndexError:
-                    print(doi, type(doi), row, item)
-                    raise(IndexError)
-            else:
-                row['publisher'] = ""
-
-            # row['editor']
-            row['editor'] = ""
-
-            try:
-                return self.normalise_unicode(row)
-            except TypeError:
-                print(row)
-                raise(TypeError)
-
-    def get_pubmed_pages(self, item: dict) -> str:
-        '''
-        This function returns the pages interval.
-
-        :params item: the item's dictionary
-        :type item: dict
-        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
-        '''
-        page_list = []
-        ''' NO INFO IN DUMP: to be updated with API DATA'''
-        return self.get_pages(page_list)
-
-    def get_publisher_name(self, doi: str) -> str:
-        '''
-        This function aims to return a publisher's name and id. If a mapping was provided,
-        it is used to find the publisher's standardized name from its id or DOI prefix.
-
-        :params doi: the item's DOI
-        :type doi: str
-
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example,
-        'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output
-        is only the name. Finally, if there is no publisher, the output is an empty string.
-        '''
-
-        publisher_name = self.publisher_manager.extract_publishers_v(doi)
-        if publisher_name and publisher_name != "unidentified":
-            return publisher_name
-        else:
-            return ""
-
-    def save_updated_pref_publishers_map(self):
-        upd_dict = self.publisher_manager.get_last_map_ver()
-        self.prefix_to_publisher_to_cache(upd_dict, self.publishers_filepath)
-
-
-    def get_venue_name(self, item: dict, id: str) -> str:
-        '''
-        This method deals with generating the venue's name, followed by id in square brackets, separated by spaces.
-        HTML tags are deleted and HTML entities escaped. In addition, any ISBN and ISSN are validated.
-        Finally, the square brackets in the venue name are replaced by round brackets to avoid conflicts with the ids enclosures.
-
-        :params item: the item's dictionary
-        :type item: dict
-        :params row: a CSV row
-        :type row: dict
-        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'Nutrition & Food Science
-         [issn:0034-6659]'. If the id does not exist, the output is only the name. Finally, if there is no venue,
-         the output is an empty string.
-         '''
-
-        short_n = item.get('journal') if item.get('journal') else ""
-        venids_list = []
-        cont_title = short_n
-        if short_n:
-            if short_n not in self.jour_dict.keys():
-                self.jour_dict[short_n] = {"extended": "", "issn": []}
-            if not self.jour_dict[short_n].get("extended") or not self.jour_dict[short_n].get("issn"):
-                if id:
-                    api_response = self.nihrf._call_api(id)
-                    if api_response:
-                        if not self.jour_dict[short_n].get("extended"):
-                            self.jour_dict[short_n]["extended"] = self.nihrf._get_extended_j_title(api_response)
-                        if not self.jour_dict[short_n].get("issn"):
-                            issn_dict_list_valid = [x for x in self.nihrf._get_issn(api_response) if x]
-                            self.jour_dict[short_n]["issn"] = issn_dict_list_valid
-                    self.issn_data_to_cache_poci(self.jour_dict, self.journals_filepath)
-
-            if short_n in self.jour_dict.keys():
-                jt_data = self.jour_dict.get(short_n)
-                if jt_data.get("issn"):
-                    venids_list = [x for x in jt_data.get("issn") if x.startswith("issn:")]
-                    venids_list_integration = ["issn:"+x for x in jt_data.get("issn") if not x.startswith("issn:")]
-                    venids_list.extend(venids_list_integration)
-                extended_jt = jt_data.get("extended") if jt_data.get("extended") else short_n
-                cont_title = extended_jt
-
-        # use abbreviated journal title if no mapping was provided
-        cont_title = cont_title.replace('\n', '')
-        ven_soup = BeautifulSoup(cont_title, 'html.parser')
-        ventit = html.unescape(ven_soup.get_text())
-        ambiguous_brackets = re.search('\[\s*((?:[^\s]+:[^\s]+)?(?:\s+[^\s]+:[^\s]+)*)\s*\]', ventit)
-        if ambiguous_brackets:
-            match = ambiguous_brackets.group(1)
-            open_bracket = ventit.find(match) - 1
-            close_bracket = ventit.find(match) + len(match)
-            ventit = ventit[:open_bracket] + '(' + ventit[open_bracket + 1:]
-            ventit = ventit[:close_bracket] + ')' + ventit[close_bracket + 1:]
-            cont_title = ventit
-
-            # IDS
-        if venids_list:
-            name_and_id = cont_title + ' [' + ' '.join(venids_list) + ']' if cont_title else '[' + ' '.join(venids_list) + ']'
-        else:
-            name_and_id = cont_title
-
-        return name_and_id
-
-    def add_authors_to_agent_list(self, item: dict, ag_list: list) -> list:
-        '''
-        This function returns the the agents list updated with the authors dictionaries, in the correct format.
-
-        :params item: the item's dictionary (attributes), ag_list: the agent list
-        :type item: dict, ag_list: list
-
-        :returns: listthe agents list updated with the authors dictionaries, in the correct format.
-        '''
-        agent_list = ag_list
-        if item.get("authors"):
-            multi_space = re.compile(r"\s+")
-            authors_string = str(item.get("authors")).strip()
-            authors_split_list = [a.strip() for a in authors_string.split(",") if a]
-            for author in authors_split_list:
-
-                agent = {}
-                agent["role"] = "author"
-                agent["name"] = author
-                missing_names = [x for x in ["family", "given", "name"] if x not in agent]
-                for mn in missing_names:
-                    agent[mn] = ""
-                agent_list.append(agent)
-        return agent_list
-
-    def find_homonyms(self, lst):
-        homonyms_dict = dict()
-        multi_space = re.compile(r"\s+")
-        extend_pattern = r"[a-zA-Z'\-áéíóúäëïöüÄłŁőŐűŰZàáâäãåąčćęèéêëėįìíîïłńòóôöõøùúûüųūÿýżźñçčšžÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽñÑâê]{2,}(?:\s|$)"
-        for d in lst:
-            if d.get('name'):
-                name = d.get('name')
-                author = name.replace(".", " ")
-                author = multi_space.sub(" ", author).strip()
-                re_extended = re.findall(extend_pattern, author)
-                extended = [(s.strip()).lower() for s in re_extended]
-                d_hom_set = set()
-                for i in extended:
-                    dicts_to_check = [dct for dct in lst if dct.get('name') and dct != d]
-                    homonyms = [dct.get('name') for dct in dicts_to_check if
-                                i in [(s.strip()).lower() for s in re.findall(extend_pattern, dct.get('name'))]]
-                    for n in homonyms:
-                        d_hom_set.add(n)
-                if d_hom_set:
-                    homonyms_dict[d.get('name')] = list(d_hom_set)
-
-        return homonyms_dict
-
-    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
-        homonyms_dict = self.find_homonyms(agents_list)
-        hom_w_orcid = set()
-        authors_strings_list = list()
-        editors_string_list = list()
-        dict_orcid = None
-        multi_space = re.compile(r"\s+")
-        inits_pattern = r"([A-Z]|[ÄŐŰÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽÑ]){1}(?:\s|$)"
-        extend_pattern = r"[a-zA-Z'\-áéíóúäëïöüÄłŁőŐűŰZàáâäãåąčćęèéêëėįìíîïłńòóôöõøùúûüųūÿýżźñçčšžÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽñÑâê]{2,}(?:\s|$)"
-
-        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list) and doi:
-            dict_orcid = self.orcid_finder(doi)
-        agents_list = [
-            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None
-            else v for k, v in
-            agent_dict.items()} for agent_dict in agents_list]
-        for agent in agents_list:
-            cur_role = agent['role']
-            f_name = None
-            g_name = None
-            name = None
-            agent_string = None
-            if agent.get('family') and agent.get('given'):
-                f_name = agent['family']
-                g_name = agent['given']
-                agent_string = f_name + ', ' + g_name
-            elif agent.get('name'):
-                name = agent['name']
-                f_name = name.split(",")[0].strip() if "," in name else None
-                g_name = name.split(",")[-1].strip() if "," in name else None
-
-                if f_name and g_name:
-                    agent_string = f_name + ', ' + g_name
-
-
-            if agent_string is None:
-                if agent.get('family') and not agent.get('given'):
-                    if g_name:
-                        agent_string = agent['family'] + ', ' + g_name
-                    else:
-                        agent_string = agent['family'] + ', '
-                elif agent.get('given') and not agent.get('family'):
-                    if f_name:
-                        agent_string = f_name + ', ' + agent['given']
-                    else:
-                        agent_string = ', ' + agent['given']
-                elif agent.get('name'):
-                    agent_string = agent.get('name')
-
-            orcid = None
-            if 'orcid' in agent:
-                if isinstance(agent['orcid'], list):
-                    orcid = str(agent['orcid'][0])
-                else:
-                    orcid = str(agent['orcid'])
-            elif 'ORCID' in agent:
-                if isinstance(agent['ORCID'], list):
-                    orcid = str(agent['ORCID'][0])
-                else:
-                    orcid = str(agent['ORCID'])
-            if orcid:
-                orcid_manager = ORCIDManager(data=dict(), use_api_service=False)
-                orcid = orcid_manager.normalise(orcid, include_prefix=False)
-                orcid = orcid if orcid_manager.check_digit(orcid) else None
-
-            elif dict_orcid and f_name:
-                for ori in dict_orcid:
-                    orc_n: List[str] = dict_orcid[ori].split(', ')
-                    orc_f = orc_n[0].lower()
-                    orc_g = orc_n[1] if len(orc_n) == 2 else None
-                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
-                        if g_name and orc_g:
-                            # If there are several authors with the same surname
-                            if len([person for person in agents_list if 'family' in person if person['family'] if
-                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
-                                        'family'].lower()]) > 1:
-                                # If there are several authors with the same surname and the same given names' initials
-                                if len([person for person in agents_list if 'given' in person if person['given'] if
-                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
-                                    homonyms_list = [person for person in agents_list if 'given' in person if
-                                                     person['given'] if person['given'].lower() == orc_g.lower()]
-                                    # If there are homonyms
-                                    if len(homonyms_list) > 1:
-                                        # If such homonyms have different roles from the current role
-                                        if [person for person in homonyms_list if person['role'] != cur_role]:
-                                            if orc_g.lower() == g_name.lower():
-                                                orcid = ori
-                                    else:
-                                        if orc_g.lower() == g_name.lower():
-                                            orcid = ori
-                                elif orc_g[0].lower() == g_name[0].lower():
-                                    orcid = ori
-                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
-                            elif any([person for person in agents_list if 'given' in person if person['given'] if
-                                      person['given'].lower() == f_name.lower()]):
-                                if orc_g.lower() == g_name.lower():
-                                    orcid = ori
-                            else:
-                                orcid = ori
-                        else:
-                            orcid = ori
-
-            # If the ra name can't be clearly divided in given name and surname
-            elif dict_orcid and name:
-                for ori in dict_orcid:
-                    try_match = True
-                    if name in homonyms_dict.keys():
-                        get_best_affinity = self.compute_affinity(dict_orcid[ori], homonyms_dict.keys())
-                        if name != get_best_affinity:
-                            try_match = False
-                    if try_match:
-                        orc_n: List[str] = dict_orcid[ori].split(', ')
-                        orc_f = orc_n[0].lower()
-                        orc_g = orc_n[1] if len(orc_n) == 2 else None
-
-                        author = name.replace(".", " ")
-                        author = multi_space.sub(" ", author).strip()
-                        re_inits = re.findall(inits_pattern, author)
-                        re_extended = re.findall(extend_pattern, author)
-                        initials = [(x.strip()).lower() for x in re_inits]
-                        extended = [(s.strip()).lower() for s in re_extended]
-                        author_dict = {"initials": initials, "extended": extended}
-
-                        surname_match = True if [x for x in author_dict["extended"] if x in orc_f.split()] else False
-                        if orc_g:
-                            name_match_all = True if [x for x in author_dict["extended"] if x in orc_g.split()] else False
-                            name_match_init = True if [x for x in author_dict["initials"] if any(
-                                        element.startswith(x) and element not in author_dict["extended"] for
-                                                element in orc_g.split())] else False
-                        else:
-                            name_match_all = False
-                            name_match_init = False
-                        matches = (surname_match and (name_match_all or name_match_init))
-
-                        if matches:
-                            # managing cases in which a name string was already retrieved but the one
-                            # provided by the mapping is better
-                            f_name = orc_f
-                            if not g_name:
-                                g_name = orc_g
-                            elif g_name:
-                                if len(g_name.strip()) < len(orc_g.strip()):
-                                    g_name = orc_g
-                            orcid = ori
-
-                    if agent_string is None:
-                        if f_name and g_name:
-                            agent_string = f_name + ', ' + g_name
-                        elif f_name and not g_name:
-                            agent_string = f_name + ', '
-                        elif g_name and not f_name:
-                            agent_string = ', ' + g_name
-                    elif agent_string == agent.get('name') and f_name and g_name:
-                        agent_string = f_name + ', ' + g_name
-
-
-            if agent_string and orcid:
-                agent_string = self.uppercase_initials(agent_string)
-                if agent_string not in hom_w_orcid:
-                    hom_w_orcid.add(agent_string)
-                    agent_string += ' [' + 'orcid:' + str(orcid) + ']'
-
-            if agent_string:
-                agent_string = self.uppercase_initials(agent_string)
-
-                if agent['role'] == 'author':
-                    authors_strings_list.append(agent_string)
-                elif agent['role'] == 'editor':
-                    editors_string_list.append(agent_string)
-
-        return authors_strings_list, editors_string_list
-
-
-    def compute_affinity(self, s, lst):
-        s = s.replace(r"\s+", " ")
-        s = s.replace(r"\n+", " ")
-        name = s.lower()
-        agent = name.replace(".", " ")
-        agent = agent.replace(",", " ")
-        agent = agent.strip()
-        agent_name_parts = agent.split()
-        extended = [x for x in agent_name_parts if len(x) > 1]
-        initials = [x for x in agent_name_parts if len(x) == 1]
-
-        target_agent_dict = {"initials": initials, "extended": extended}
-
-        report_dicts = {}
-        for ag in lst:
-            name = ag.lower()
-            name = name.replace(r"\s+", " ")
-            name = name.replace(r"\n+", " ")
-            agent = name.replace(".", " ")
-            agent = agent.strip()
-            agent_name_parts = agent.split()
-            ag_extended = [x for x in agent_name_parts if len(x) > 1]
-            ag_initials = [x for x in agent_name_parts if len(x) == 1]
-
-            copy_ext_target = [x for x in extended]
-            copy_init_target = [x for x in initials]
-            copy_ag_ext = [x for x in ag_extended]
-            copy_ag_init = [x for x in ag_initials]
-
-            ext_matched = 0
-            init_matched = 0
-
-            for i in ag_extended:
-                if i in copy_ext_target:
-                    ext_matched += 1
-                    copy_ext_target.remove(i)
-                    copy_ag_ext.remove(i)
-
-            for ii in ag_initials:
-                if ii in copy_init_target:
-                    init_matched += 1
-                    copy_init_target.remove(ii)
-                    copy_ag_init.remove(ii)
-
-            # check the remaining unpaired
-            # check first if the extra initials in the ra name can be paired with the remaining extended names
-            init_compatible = 0
-
-            if copy_ag_init and copy_ext_target:
-                remaining_ag_initials = [x for x in copy_ag_init]
-                remaining_tar_extended = [x for x in copy_ext_target]
-
-                for ri in remaining_ag_initials:
-                    if ri in copy_ag_init:
-                        for re in remaining_tar_extended:
-                            if re in copy_ext_target:
-                                if re.startswith(ri):
-                                    copy_ag_init.remove(ri)
-                                    copy_ext_target.remove(re)
-                                    init_compatible += 1
-                                    break
-
-            # check if the remaining initials of the target name are compatible with the remaining extended names of the ra
-            ext_compatible = 0
-
-            if copy_ag_ext and copy_init_target:
-                remaining_tar_initials = [x for x in copy_init_target]
-                remaining_ag_extended = [x for x in copy_ag_ext]
-
-                for ri in remaining_tar_initials:
-                    if ri in copy_init_target:
-                        for re in remaining_ag_extended:
-                            if re in copy_ag_ext:
-                                if re.startswith(ri):
-                                    copy_ag_ext.remove(re)
-                                    copy_init_target.remove(ri)
-                                    ext_compatible += 1
-                                    break
-            ext_not_compatible = len(copy_ag_ext)
-            init_not_compatible = len(copy_ag_init)
-
-            cur_agent_dict = {
-                "ext_matched": ext_matched,
-                "init_matched": init_matched,
-                "ext_compatible": ext_compatible,
-                "init_compatible": init_compatible,
-                "ext_not_compatible": ext_not_compatible,
-                "init_not_compatible": init_not_compatible,
-            }
-
-            report_dicts[ag] = cur_agent_dict
-        best_match_name = self.get_best_match(target_agent_dict, report_dicts)
-        return best_match_name
-
-
-
-    def add_editors_to_agent_list(self, item: dict, ag_list: list) -> list:
-        '''
-        This function returns the the agents list updated with the editors dictionaries, in the correct format.
-
-        :params item: the item's dictionary (attributes), ag_list: the agent list
-        :type item: dict, ag_list: list
-
-        :returns: listthe agents list updated with the authors dictionaries, in the correct format.
-        '''
-
-        agent_list = ag_list
-
-        ''' NO INFO IN DUMP: to be updated with API DATA'''
-        return agent_list
-
-
-
-    def get_best_match(self, target_agent_dict, report_dicts):
-        if max([v.get("ext_matched") for k,v in report_dicts.items()]) == 0:
-            return ""
-        elif max([v.get("ext_matched") for k,v in report_dicts.items()]) == 1:
-            min_comp_dict = {k:v for k,v in report_dicts.items() if v.get("ext_matched") ==1 and (
-                    (v.get("init_matched") >= 1 or v.get("ext_compatible")>=1 or v.get("init_compatible")>=1)
-                    and
-                    (v.get("ext_not_compatible")<= 1 and v.get("init_not_compatible")<= 1)
-            )}
-            if not min_comp_dict:
-                return ""
-
-
-
-        len_target_init = len(target_agent_dict["initials"])
-        len_target_ext = len(target_agent_dict["extended"])
-        if len_target_init + len_target_ext >= 1:
-
-            # Case 1: There is a perfect match with no exceedings: return it
-            complete_matches = {k: v for k, v in report_dicts.items() if
-                                v["ext_matched"] == len_target_ext and v["init_matched"] == len_target_init and v[
-                                    "init_not_compatible"] == 0 and v["ext_not_compatible"] == 0}
-            if complete_matches:
-                for k in complete_matches.keys():
-                    return k
-            # Case 2: There is a complete match with all the extended names and the initials of the target are compatible
-            match_all_extended_comp_ext = {k: v for k, v in report_dicts.items() if v["ext_matched"] == len_target_ext and (
-                        v["init_matched"] + v["ext_compatible"] == len_target_init) and v["init_not_compatible"] == 0 and v[
-                                               "ext_not_compatible"] == 0}
-            if match_all_extended_comp_ext:
-                if len(match_all_extended_comp_ext) == 1:
-                    for k in match_all_extended_comp_ext.keys():
-                        return k
-                else:
-                    return [k for k, v in match_all_extended_comp_ext.items() if
-                            v["init_matched"] == max([v["init_matched"] for v in match_all_extended_comp_ext.values()])][0]
-
-            # Case 3: Get max extended names match + compatible extended/initials
-            max_comp_exc_ext = max([v["ext_matched"] for v in report_dicts.values()])
-            match_max_extended_comp_init = {k: v for k, v in report_dicts.items() if
-                                            v["ext_matched"] == max_comp_exc_ext and (
-                                                        v["ext_matched"] + v["init_compatible"] == len_target_ext) and (
-                                                        v["init_matched"] + v["ext_compatible"] == len_target_init) and v[
-                                                "init_not_compatible"] == 0 and v["ext_not_compatible"] == 0}
-            if match_max_extended_comp_init:
-                if len(match_max_extended_comp_init) == 1:
-                    for k in match_max_extended_comp_init.keys():
-                        return k
-                else:
-                    return [k for k, v in match_max_extended_comp_init.items() if
-                            v["init_matched"] == max([v["init_matched"] for v in match_max_extended_comp_init.values()])][0]
-
-            # Case 4 (suboptimal cases), get best compatibility
-            scores_dict = dict()
-
-            for k, v in report_dicts.items():
-                score = 0
-
-                p_match_ext = 0
-                if len_target_ext:
-                    p_match_ext = v["ext_matched"] / len_target_ext
-                    if p_match_ext < 1:
-                        if v["init_compatible"]:
-                            p_match_ext = (v["init_compatible"] * 0.2 + v["ext_matched"]) / len_target_ext
-
-                p_match_init = 0
-                if len_target_init:
-                    p_match_init = v["init_matched"] / len_target_init
-                    if p_match_init < 1:
-                        if v["ext_compatible"]:
-                            p_match_init = (v["ext_compatible"] * 0.7 + v["init_matched"]) / len_target_init
-
-                total_len_name_parts_target = len_target_ext + len_target_init
-                if v["ext_not_compatible"]:
-                    p_inc_ext = v["ext_not_compatible"] * 0.7 / total_len_name_parts_target
-                else:
-                    p_inc_ext = 0
-                if v["init_not_compatible"]:
-                    p_inc_init = v["init_not_compatible"] * 0.2 / total_len_name_parts_target
-                else:
-                    p_inc_init = 0
-                score = p_match_ext + p_match_init - p_inc_init - p_inc_ext
-                scores_dict[k] = score
-            result = [k for k, v in scores_dict.items() if v == max(scores_dict.values())]
-            if len(result) == 1:
-                return result[0]
-            else:
-                return ""
+import html
+import json
+import os
+import pathlib
+import re
+import warnings
+from os.path import exists
+from typing import Dict, List, Tuple
+
+import fakeredis
+from bs4 import BeautifulSoup
+from oc_ds_converter.oc_idmanager.doi import DOIManager
+from oc_ds_converter.oc_idmanager.orcid import ORCIDManager
+from oc_ds_converter.oc_idmanager.pmid import PMIDManager
+from oc_ds_converter.lib.cleaner import Cleaner
+from oc_ds_converter.lib.master_of_regex import *
+
+from oc_ds_converter.datasource.redis import RedisDataSource
+from oc_ds_converter.pubmed.finder_nih import NIHResourceFinder
+from oc_ds_converter.pubmed.get_publishers import ExtractPublisherDOI
+from oc_ds_converter.ra_processor import RaProcessor
+
+warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
+
+
+class PubmedProcessing(RaProcessor):
+    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath_pubmed: str = None, journals_filepath: str = None, testing:bool = True):
+        super(PubmedProcessing, self).__init__(orcid_index, doi_csv)
+        self.nihrf = NIHResourceFinder()
+        self.doi_m = DOIManager()
+        self.pmid_m = PMIDManager()
+        if testing:
+            self.BR_redis= fakeredis.FakeStrictRedis()
+            self.RA_redis= fakeredis.FakeStrictRedis()
+
+        else:
+            self.BR_redis = RedisDataSource("DB-META-BR")
+            self.RA_redis = RedisDataSource("DB-META-RA")
+
+        if not journals_filepath:
+            if not exists(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files")):
+                os.makedirs(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files"))
+            self.journals_filepath = os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files",
+                                                  "issn_jour_ext.json")
+        else:
+            self.journals_filepath = journals_filepath
+
+        self.jour_dict = self.issn_data_recover_poci(self.journals_filepath)
+
+
+        if not publishers_filepath_pubmed:
+            if not exists(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files")):
+                os.makedirs(os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files"))
+            self.publishers_filepath = os.path.join(pathlib.Path(__file__).parent.resolve(), "support_files",
+                                                  "prefix_publishers.json")
+        else:
+            self.publishers_filepath = publishers_filepath_pubmed
+
+        self.jour_dict = self.issn_data_recover_poci(self.journals_filepath)
+
+        if os.path.exists(self.publishers_filepath):
+            with open(self.publishers_filepath, "r", encoding="utf8") as fdp:
+                pfp = json.load(fdp)
+                if pfp:
+                    self.publisher_manager = ExtractPublisherDOI(pfp)
+                else:
+                    self.publisher_manager = ExtractPublisherDOI({})
+        else:
+            self.publisher_manager = ExtractPublisherDOI({})
+            with open(self.publishers_filepath, "w", encoding="utf8") as fdp:
+                json.dump({}, fdp, ensure_ascii=False, indent=4)
+
+
+    def issn_data_recover_poci(self, path):
+        journal_issn_dict = dict()
+        if not path:
+            return journal_issn_dict
+        if not os.path.exists(path):
+            return journal_issn_dict
+        else:
+            with open(path, "r", encoding="utf8") as fd:
+                journal_issn_dict = json.load(fd)
+                return journal_issn_dict
+
+
+    def issn_data_to_cache_poci(self, jtitle_issn_dict, path):
+        with open(path, "w", encoding="utf-8") as fd:
+            json.dump(jtitle_issn_dict, fd, ensure_ascii=False, indent=4)
+
+    def prefix_to_publisher_to_cache(self, pref_pub_dict, path):
+        with open(path, "w", encoding="utf-8") as fd:
+            json.dump(pref_pub_dict, fd, ensure_ascii=False, indent=4)
+
+    def csv_creator(self, item: dict) -> dict:
+        row = dict()
+        doi = ""
+        pmid = self.pmid_m.normalise(str(item['pmid']))
+        if (pmid and self.doi_set and pmid in self.doi_set) or (pmid and not self.doi_set):
+            # create empty row
+            keys = ['id', 'title', 'author', 'pub_date', 'venue', 'volume', 'issue', 'page', 'type',
+                    'publisher', 'editor']
+            for k in keys:
+                row[k] = ''
+
+            attributes = item
+
+            # row['type']
+            row['type'] = 'journal article'
+
+            # row['id']
+            ids_list = list()
+            ids_list.append(str('pmid:' + pmid))
+            if attributes.get('doi'):
+                doi = DOIManager().normalise(attributes.get('doi'), include_prefix=False)
+                if doi:
+                    doi_w_pref = "doi:"+doi
+                    if self.BR_redis.get(doi_w_pref):
+                        ids_list.append(doi_w_pref)
+                    elif self.doi_m.is_valid(doi):
+                        ids_list.append(doi_w_pref)
+                    else:
+                        doi = ''
+
+
+            row['id'] = ' '.join(ids_list)
+
+            # row['title']
+            pub_title = ""
+            if attributes.get("title"):
+                p_title = attributes.get("title")
+                soup = BeautifulSoup(p_title, 'html.parser')
+                title_soup = soup.get_text().replace('\n', '')
+                title_soup_space_replaced = ' '.join(title_soup.split())
+                title_soup_strip = title_soup_space_replaced.strip()
+                clean_tit = html.unescape(title_soup_strip)
+                pub_title = clean_tit if clean_tit else p_title
+
+            row['title'] = pub_title
+
+            agents_list = self.add_authors_to_agent_list(attributes, [])
+            authors_strings_list, editors_string_list = self.get_agents_strings_list(doi, agents_list)
+
+            # row['author']
+            if attributes.get('authors'):
+                row['author'] = '; '.join(authors_strings_list)
+
+            # row['pub_date']
+            dates = attributes.get("year")
+            row['pub_date'] = str(dates) if dates else ""
+
+            # row['venue']
+            row['venue'] = self.get_venue_name(attributes, pmid)
+
+            # row['volume']
+            row['volume'] = ""
+
+            # row['issue']
+            row['issue'] = ""
+
+            # row['page']
+            row['page'] = "" #self.get_pubmed_pages(attributes)
+
+            # row['publisher']
+            if doi:
+                try:
+                    row['publisher'] = self.get_publisher_name(doi)
+                except IndexError:
+                    print(doi, type(doi), row, item)
+                    raise(IndexError)
+            else:
+                row['publisher'] = ""
+
+            # row['editor']
+            row['editor'] = ""
+
+            try:
+                return self.normalise_unicode(row)
+            except TypeError:
+                print(row)
+                raise(TypeError)
+
+    def get_pubmed_pages(self, item: dict) -> str:
+        '''
+        This function returns the pages interval.
+
+        :params item: the item's dictionary
+        :type item: dict
+        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
+        '''
+        page_list = []
+        ''' NO INFO IN DUMP: to be updated with API DATA'''
+        return self.get_pages(page_list)
+
+    def get_publisher_name(self, doi: str) -> str:
+        '''
+        This function aims to return a publisher's name and id. If a mapping was provided,
+        it is used to find the publisher's standardized name from its id or DOI prefix.
+
+        :params doi: the item's DOI
+        :type doi: str
+
+        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example,
+        'American Medical Association (AMA) [crossref:10]'. If the id does not exist, the output
+        is only the name. Finally, if there is no publisher, the output is an empty string.
+        '''
+
+        publisher_name = self.publisher_manager.extract_publishers_v(doi)
+        if publisher_name and publisher_name != "unidentified":
+            return publisher_name
+        else:
+            return ""
+
+    def save_updated_pref_publishers_map(self):
+        upd_dict = self.publisher_manager.get_last_map_ver()
+        self.prefix_to_publisher_to_cache(upd_dict, self.publishers_filepath)
+
+
+    def get_venue_name(self, item: dict, id: str) -> str:
+        '''
+        This method deals with generating the venue's name, followed by id in square brackets, separated by spaces.
+        HTML tags are deleted and HTML entities escaped. In addition, any ISBN and ISSN are validated.
+        Finally, the square brackets in the venue name are replaced by round brackets to avoid conflicts with the ids enclosures.
+
+        :params item: the item's dictionary
+        :type item: dict
+        :params row: a CSV row
+        :type row: dict
+        :returns: str -- The output is a string in the format 'NAME [SCHEMA:ID]', for example, 'Nutrition & Food Science
+         [issn:0034-6659]'. If the id does not exist, the output is only the name. Finally, if there is no venue,
+         the output is an empty string.
+         '''
+
+        short_n = item.get('journal') if item.get('journal') else ""
+        venids_list = []
+        cont_title = short_n
+        if short_n:
+            if short_n not in self.jour_dict.keys():
+                self.jour_dict[short_n] = {"extended": "", "issn": []}
+            if not self.jour_dict[short_n].get("extended") or not self.jour_dict[short_n].get("issn"):
+                if id:
+                    api_response = self.nihrf._call_api(id)
+                    if api_response:
+                        if not self.jour_dict[short_n].get("extended"):
+                            self.jour_dict[short_n]["extended"] = self.nihrf._get_extended_j_title(api_response)
+                        if not self.jour_dict[short_n].get("issn"):
+                            issn_dict_list_valid = [x for x in self.nihrf._get_issn(api_response) if x]
+                            self.jour_dict[short_n]["issn"] = issn_dict_list_valid
+                    self.issn_data_to_cache_poci(self.jour_dict, self.journals_filepath)
+
+            if short_n in self.jour_dict.keys():
+                jt_data = self.jour_dict.get(short_n)
+                if jt_data.get("issn"):
+                    venids_list = [x for x in jt_data.get("issn") if x.startswith("issn:")]
+                    venids_list_integration = ["issn:"+x for x in jt_data.get("issn") if not x.startswith("issn:")]
+                    venids_list.extend(venids_list_integration)
+                extended_jt = jt_data.get("extended") if jt_data.get("extended") else short_n
+                cont_title = extended_jt
+
+        # use abbreviated journal title if no mapping was provided
+        cont_title = cont_title.replace('\n', '')
+        ven_soup = BeautifulSoup(cont_title, 'html.parser')
+        ventit = html.unescape(ven_soup.get_text())
+        ambiguous_brackets = re.search('\[\s*((?:[^\s]+:[^\s]+)?(?:\s+[^\s]+:[^\s]+)*)\s*\]', ventit)
+        if ambiguous_brackets:
+            match = ambiguous_brackets.group(1)
+            open_bracket = ventit.find(match) - 1
+            close_bracket = ventit.find(match) + len(match)
+            ventit = ventit[:open_bracket] + '(' + ventit[open_bracket + 1:]
+            ventit = ventit[:close_bracket] + ')' + ventit[close_bracket + 1:]
+            cont_title = ventit
+
+            # IDS
+        if venids_list:
+            name_and_id = cont_title + ' [' + ' '.join(venids_list) + ']' if cont_title else '[' + ' '.join(venids_list) + ']'
+        else:
+            name_and_id = cont_title
+
+        return name_and_id
+
+    def add_authors_to_agent_list(self, item: dict, ag_list: list) -> list:
+        '''
+        This function returns the the agents list updated with the authors dictionaries, in the correct format.
+
+        :params item: the item's dictionary (attributes), ag_list: the agent list
+        :type item: dict, ag_list: list
+
+        :returns: listthe agents list updated with the authors dictionaries, in the correct format.
+        '''
+        agent_list = ag_list
+        if item.get("authors"):
+            multi_space = re.compile(r"\s+")
+            authors_string = str(item.get("authors")).strip()
+            authors_split_list = [a.strip() for a in authors_string.split(",") if a]
+            for author in authors_split_list:
+
+                agent = {}
+                agent["role"] = "author"
+                agent["name"] = author
+                missing_names = [x for x in ["family", "given", "name"] if x not in agent]
+                for mn in missing_names:
+                    agent[mn] = ""
+                agent_list.append(agent)
+        return agent_list
+
+    def find_homonyms(self, lst):
+        homonyms_dict = dict()
+        multi_space = re.compile(r"\s+")
+        extend_pattern = r"[a-zA-Z'\-áéíóúäëïöüÄłŁőŐűŰZàáâäãåąčćęèéêëėįìíîïłńòóôöõøùúûüųūÿýżźñçčšžÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽñÑâê]{2,}(?:\s|$)"
+        for d in lst:
+            if d.get('name'):
+                name = d.get('name')
+                author = name.replace(".", " ")
+                author = multi_space.sub(" ", author).strip()
+                re_extended = re.findall(extend_pattern, author)
+                extended = [(s.strip()).lower() for s in re_extended]
+                d_hom_set = set()
+                for i in extended:
+                    dicts_to_check = [dct for dct in lst if dct.get('name') and dct != d]
+                    homonyms = [dct.get('name') for dct in dicts_to_check if
+                                i in [(s.strip()).lower() for s in re.findall(extend_pattern, dct.get('name'))]]
+                    for n in homonyms:
+                        d_hom_set.add(n)
+                if d_hom_set:
+                    homonyms_dict[d.get('name')] = list(d_hom_set)
+
+        return homonyms_dict
+
+    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
+        homonyms_dict = self.find_homonyms(agents_list)
+        hom_w_orcid = set()
+        authors_strings_list = list()
+        editors_string_list = list()
+        dict_orcid = None
+        multi_space = re.compile(r"\s+")
+        inits_pattern = r"([A-Z]|[ÄŐŰÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽÑ]){1}(?:\s|$)"
+        extend_pattern = r"[a-zA-Z'\-áéíóúäëïöüÄłŁőŐűŰZàáâäãåąčćęèéêëėįìíîïłńòóôöõøùúûüųūÿýżźñçčšžÀÁÂÄÃÅĄĆČĖĘÈÉÊËÌÍÎÏĮŁŃÒÓÔÖÕØÙÚÛÜŲŪŸÝŻŹÑßÇŒÆČŠŽñÑâê]{2,}(?:\s|$)"
+
+        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list) and doi:
+            dict_orcid = self.orcid_finder(doi)
+        agents_list = [
+            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None
+            else v for k, v in
+            agent_dict.items()} for agent_dict in agents_list]
+        for agent in agents_list:
+            cur_role = agent['role']
+            f_name = None
+            g_name = None
+            name = None
+            agent_string = None
+            if agent.get('family') and agent.get('given'):
+                f_name = agent['family']
+                g_name = agent['given']
+                agent_string = f_name + ', ' + g_name
+            elif agent.get('name'):
+                name = agent['name']
+                f_name = name.split(",")[0].strip() if "," in name else None
+                g_name = name.split(",")[-1].strip() if "," in name else None
+
+                if f_name and g_name:
+                    agent_string = f_name + ', ' + g_name
+
+
+            if agent_string is None:
+                if agent.get('family') and not agent.get('given'):
+                    if g_name:
+                        agent_string = agent['family'] + ', ' + g_name
+                    else:
+                        agent_string = agent['family'] + ', '
+                elif agent.get('given') and not agent.get('family'):
+                    if f_name:
+                        agent_string = f_name + ', ' + agent['given']
+                    else:
+                        agent_string = ', ' + agent['given']
+                elif agent.get('name'):
+                    agent_string = agent.get('name')
+
+            orcid = None
+            if 'orcid' in agent:
+                if isinstance(agent['orcid'], list):
+                    orcid = str(agent['orcid'][0])
+                else:
+                    orcid = str(agent['orcid'])
+            elif 'ORCID' in agent:
+                if isinstance(agent['ORCID'], list):
+                    orcid = str(agent['ORCID'][0])
+                else:
+                    orcid = str(agent['ORCID'])
+            if orcid:
+                orcid_manager = ORCIDManager(data=dict(), use_api_service=False)
+                orcid = orcid_manager.normalise(orcid, include_prefix=False)
+                orcid = orcid if orcid_manager.check_digit(orcid) else None
+
+            elif dict_orcid and f_name:
+                for ori in dict_orcid:
+                    orc_n: List[str] = dict_orcid[ori].split(', ')
+                    orc_f = orc_n[0].lower()
+                    orc_g = orc_n[1] if len(orc_n) == 2 else None
+                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
+                        if g_name and orc_g:
+                            # If there are several authors with the same surname
+                            if len([person for person in agents_list if 'family' in person if person['family'] if
+                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
+                                        'family'].lower()]) > 1:
+                                # If there are several authors with the same surname and the same given names' initials
+                                if len([person for person in agents_list if 'given' in person if person['given'] if
+                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
+                                    homonyms_list = [person for person in agents_list if 'given' in person if
+                                                     person['given'] if person['given'].lower() == orc_g.lower()]
+                                    # If there are homonyms
+                                    if len(homonyms_list) > 1:
+                                        # If such homonyms have different roles from the current role
+                                        if [person for person in homonyms_list if person['role'] != cur_role]:
+                                            if orc_g.lower() == g_name.lower():
+                                                orcid = ori
+                                    else:
+                                        if orc_g.lower() == g_name.lower():
+                                            orcid = ori
+                                elif orc_g[0].lower() == g_name[0].lower():
+                                    orcid = ori
+                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
+                            elif any([person for person in agents_list if 'given' in person if person['given'] if
+                                      person['given'].lower() == f_name.lower()]):
+                                if orc_g.lower() == g_name.lower():
+                                    orcid = ori
+                            else:
+                                orcid = ori
+                        else:
+                            orcid = ori
+
+            # If the ra name can't be clearly divided in given name and surname
+            elif dict_orcid and name:
+                for ori in dict_orcid:
+                    try_match = True
+                    if name in homonyms_dict.keys():
+                        get_best_affinity = self.compute_affinity(dict_orcid[ori], homonyms_dict.keys())
+                        if name != get_best_affinity:
+                            try_match = False
+                    if try_match:
+                        orc_n: List[str] = dict_orcid[ori].split(', ')
+                        orc_f = orc_n[0].lower()
+                        orc_g = orc_n[1] if len(orc_n) == 2 else None
+
+                        author = name.replace(".", " ")
+                        author = multi_space.sub(" ", author).strip()
+                        re_inits = re.findall(inits_pattern, author)
+                        re_extended = re.findall(extend_pattern, author)
+                        initials = [(x.strip()).lower() for x in re_inits]
+                        extended = [(s.strip()).lower() for s in re_extended]
+                        author_dict = {"initials": initials, "extended": extended}
+
+                        surname_match = True if [x for x in author_dict["extended"] if x in orc_f.split()] else False
+                        if orc_g:
+                            name_match_all = True if [x for x in author_dict["extended"] if x in orc_g.split()] else False
+                            name_match_init = True if [x for x in author_dict["initials"] if any(
+                                        element.startswith(x) and element not in author_dict["extended"] for
+                                                element in orc_g.split())] else False
+                        else:
+                            name_match_all = False
+                            name_match_init = False
+                        matches = (surname_match and (name_match_all or name_match_init))
+
+                        if matches:
+                            # managing cases in which a name string was already retrieved but the one
+                            # provided by the mapping is better
+                            f_name = orc_f
+                            if not g_name:
+                                g_name = orc_g
+                            elif g_name:
+                                if len(g_name.strip()) < len(orc_g.strip()):
+                                    g_name = orc_g
+                            orcid = ori
+
+                    if agent_string is None:
+                        if f_name and g_name:
+                            agent_string = f_name + ', ' + g_name
+                        elif f_name and not g_name:
+                            agent_string = f_name + ', '
+                        elif g_name and not f_name:
+                            agent_string = ', ' + g_name
+                    elif agent_string == agent.get('name') and f_name and g_name:
+                        agent_string = f_name + ', ' + g_name
+
+
+            if agent_string and orcid:
+                agent_string = self.uppercase_initials(agent_string)
+                if agent_string not in hom_w_orcid:
+                    hom_w_orcid.add(agent_string)
+                    agent_string += ' [' + 'orcid:' + str(orcid) + ']'
+
+            if agent_string:
+                agent_string = self.uppercase_initials(agent_string)
+
+                if agent['role'] == 'author':
+                    authors_strings_list.append(agent_string)
+                elif agent['role'] == 'editor':
+                    editors_string_list.append(agent_string)
+
+        return authors_strings_list, editors_string_list
+
+
+    def compute_affinity(self, s, lst):
+        s = s.replace(r"\s+", " ")
+        s = s.replace(r"\n+", " ")
+        name = s.lower()
+        agent = name.replace(".", " ")
+        agent = agent.replace(",", " ")
+        agent = agent.strip()
+        agent_name_parts = agent.split()
+        extended = [x for x in agent_name_parts if len(x) > 1]
+        initials = [x for x in agent_name_parts if len(x) == 1]
+
+        target_agent_dict = {"initials": initials, "extended": extended}
+
+        report_dicts = {}
+        for ag in lst:
+            name = ag.lower()
+            name = name.replace(r"\s+", " ")
+            name = name.replace(r"\n+", " ")
+            agent = name.replace(".", " ")
+            agent = agent.strip()
+            agent_name_parts = agent.split()
+            ag_extended = [x for x in agent_name_parts if len(x) > 1]
+            ag_initials = [x for x in agent_name_parts if len(x) == 1]
+
+            copy_ext_target = [x for x in extended]
+            copy_init_target = [x for x in initials]
+            copy_ag_ext = [x for x in ag_extended]
+            copy_ag_init = [x for x in ag_initials]
+
+            ext_matched = 0
+            init_matched = 0
+
+            for i in ag_extended:
+                if i in copy_ext_target:
+                    ext_matched += 1
+                    copy_ext_target.remove(i)
+                    copy_ag_ext.remove(i)
+
+            for ii in ag_initials:
+                if ii in copy_init_target:
+                    init_matched += 1
+                    copy_init_target.remove(ii)
+                    copy_ag_init.remove(ii)
+
+            # check the remaining unpaired
+            # check first if the extra initials in the ra name can be paired with the remaining extended names
+            init_compatible = 0
+
+            if copy_ag_init and copy_ext_target:
+                remaining_ag_initials = [x for x in copy_ag_init]
+                remaining_tar_extended = [x for x in copy_ext_target]
+
+                for ri in remaining_ag_initials:
+                    if ri in copy_ag_init:
+                        for re in remaining_tar_extended:
+                            if re in copy_ext_target:
+                                if re.startswith(ri):
+                                    copy_ag_init.remove(ri)
+                                    copy_ext_target.remove(re)
+                                    init_compatible += 1
+                                    break
+
+            # check if the remaining initials of the target name are compatible with the remaining extended names of the ra
+            ext_compatible = 0
+
+            if copy_ag_ext and copy_init_target:
+                remaining_tar_initials = [x for x in copy_init_target]
+                remaining_ag_extended = [x for x in copy_ag_ext]
+
+                for ri in remaining_tar_initials:
+                    if ri in copy_init_target:
+                        for re in remaining_ag_extended:
+                            if re in copy_ag_ext:
+                                if re.startswith(ri):
+                                    copy_ag_ext.remove(re)
+                                    copy_init_target.remove(ri)
+                                    ext_compatible += 1
+                                    break
+            ext_not_compatible = len(copy_ag_ext)
+            init_not_compatible = len(copy_ag_init)
+
+            cur_agent_dict = {
+                "ext_matched": ext_matched,
+                "init_matched": init_matched,
+                "ext_compatible": ext_compatible,
+                "init_compatible": init_compatible,
+                "ext_not_compatible": ext_not_compatible,
+                "init_not_compatible": init_not_compatible,
+            }
+
+            report_dicts[ag] = cur_agent_dict
+        best_match_name = self.get_best_match(target_agent_dict, report_dicts)
+        return best_match_name
+
+
+
+    def add_editors_to_agent_list(self, item: dict, ag_list: list) -> list:
+        '''
+        This function returns the the agents list updated with the editors dictionaries, in the correct format.
+
+        :params item: the item's dictionary (attributes), ag_list: the agent list
+        :type item: dict, ag_list: list
+
+        :returns: listthe agents list updated with the authors dictionaries, in the correct format.
+        '''
+
+        agent_list = ag_list
+
+        ''' NO INFO IN DUMP: to be updated with API DATA'''
+        return agent_list
+
+    def get_citing_pmid(self, meta_dict:dict) -> str:
+        citing_pmid = ""
+        id_string = meta_dict.get("id")
+        if id_string:
+            id_list = id_string.split()
+            pmid_list = [x for x in id_list if x.startswith("pmid:")]
+            if len(pmid_list) == 1:
+                citing_pmid = pmid_list[0] # we expect only one pmid for each entity
+        return citing_pmid
+
+    def get_citations(self, validated_pmid, item:dict) -> list:
+        addressed_citations = set()
+
+        citing = validated_pmid
+        if not citing.startswith("pmid:"):
+            try:
+                int_pmid = int(citing)
+                citing = "pmid:" + str(int_pmid)
+            except:
+                return []
+
+        references_string = item.get("references")
+        cited_ids = references_string.split()
+
+        for cited_id in cited_ids:
+            try:
+                id_n = int(cited_id)
+
+                if id_n:
+                    norm_cited = self.pmid_m.normalise(str(id_n), include_prefix=True)
+
+                    if norm_cited:
+                        addressed_citations.add((citing, norm_cited))
+            except:
+                pass
+
+        addressed_citations_list = list(addressed_citations)
+
+        return addressed_citations_list
+
+
+    def get_best_match(self, target_agent_dict, report_dicts):
+        if max([v.get("ext_matched") for k,v in report_dicts.items()]) == 0:
+            return ""
+        elif max([v.get("ext_matched") for k,v in report_dicts.items()]) == 1:
+            min_comp_dict = {k:v for k,v in report_dicts.items() if v.get("ext_matched") ==1 and (
+                    (v.get("init_matched") >= 1 or v.get("ext_compatible")>=1 or v.get("init_compatible")>=1)
+                    and
+                    (v.get("ext_not_compatible")<= 1 and v.get("init_not_compatible")<= 1)
+            )}
+            if not min_comp_dict:
+                return ""
+
+
+
+        len_target_init = len(target_agent_dict["initials"])
+        len_target_ext = len(target_agent_dict["extended"])
+        if len_target_init + len_target_ext >= 1:
+
+            # Case 1: There is a perfect match with no exceedings: return it
+            complete_matches = {k: v for k, v in report_dicts.items() if
+                                v["ext_matched"] == len_target_ext and v["init_matched"] == len_target_init and v[
+                                    "init_not_compatible"] == 0 and v["ext_not_compatible"] == 0}
+            if complete_matches:
+                for k in complete_matches.keys():
+                    return k
+            # Case 2: There is a complete match with all the extended names and the initials of the target are compatible
+            match_all_extended_comp_ext = {k: v for k, v in report_dicts.items() if v["ext_matched"] == len_target_ext and (
+                        v["init_matched"] + v["ext_compatible"] == len_target_init) and v["init_not_compatible"] == 0 and v[
+                                               "ext_not_compatible"] == 0}
+            if match_all_extended_comp_ext:
+                if len(match_all_extended_comp_ext) == 1:
+                    for k in match_all_extended_comp_ext.keys():
+                        return k
+                else:
+                    return [k for k, v in match_all_extended_comp_ext.items() if
+                            v["init_matched"] == max([v["init_matched"] for v in match_all_extended_comp_ext.values()])][0]
+
+            # Case 3: Get max extended names match + compatible extended/initials
+            max_comp_exc_ext = max([v["ext_matched"] for v in report_dicts.values()])
+            match_max_extended_comp_init = {k: v for k, v in report_dicts.items() if
+                                            v["ext_matched"] == max_comp_exc_ext and (
+                                                        v["ext_matched"] + v["init_compatible"] == len_target_ext) and (
+                                                        v["init_matched"] + v["ext_compatible"] == len_target_init) and v[
+                                                "init_not_compatible"] == 0 and v["ext_not_compatible"] == 0}
+            if match_max_extended_comp_init:
+                if len(match_max_extended_comp_init) == 1:
+                    for k in match_max_extended_comp_init.keys():
+                        return k
+                else:
+                    return [k for k, v in match_max_extended_comp_init.items() if
+                            v["init_matched"] == max([v["init_matched"] for v in match_max_extended_comp_init.values()])][0]
+
+            # Case 4 (suboptimal cases), get best compatibility
+            scores_dict = dict()
+
+            for k, v in report_dicts.items():
+                score = 0
+
+                p_match_ext = 0
+                if len_target_ext:
+                    p_match_ext = v["ext_matched"] / len_target_ext
+                    if p_match_ext < 1:
+                        if v["init_compatible"]:
+                            p_match_ext = (v["init_compatible"] * 0.2 + v["ext_matched"]) / len_target_ext
+
+                p_match_init = 0
+                if len_target_init:
+                    p_match_init = v["init_matched"] / len_target_init
+                    if p_match_init < 1:
+                        if v["ext_compatible"]:
+                            p_match_init = (v["ext_compatible"] * 0.7 + v["init_matched"]) / len_target_init
+
+                total_len_name_parts_target = len_target_ext + len_target_init
+                if v["ext_not_compatible"]:
+                    p_inc_ext = v["ext_not_compatible"] * 0.7 / total_len_name_parts_target
+                else:
+                    p_inc_ext = 0
+                if v["init_not_compatible"]:
+                    p_inc_init = v["init_not_compatible"] * 0.2 / total_len_name_parts_target
+                else:
+                    p_inc_init = 0
+                score = p_match_ext + p_match_init - p_inc_init - p_inc_ext
+                scores_dict[k] = score
+            result = [k for k, v in scores_dict.items() if v == max(scores_dict.values())]
+            if len(result) == 1:
+                return result[0]
+            else:
+                return ""
         return ""
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/ra_processor.py` & `oc_ds_converter-1.0.1/oc_ds_converter/ra_processor.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-import os
-import re
-import unicodedata
-from csv import DictReader
-from typing import Dict, List, Tuple
-from zipfile import ZipFile
-
-from oc_ds_converter.oc_idmanager import ISBNManager, ISSNManager, ORCIDManager
-
-from oc_ds_converter.lib.cleaner import Cleaner
-from oc_ds_converter.lib.csvmanager import CSVManager
-from oc_ds_converter.lib.master_of_regex import orcid_pattern
-
-
-class RaProcessor(object):
-    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath: str = None, citing_entities: str = None):
-        self.doi_set = CSVManager.load_csv_column_as_set(doi_csv, 'id') if doi_csv else None
-        self.publishers_mapping = self.load_publishers_mapping(publishers_filepath) if publishers_filepath else None
-        orcid_index = orcid_index if orcid_index else None
-        self.orcid_index = CSVManager(orcid_index)
-        if citing_entities:
-            self.unzip_citing_entities(citing_entities)
-            self.citing_entities_set = CSVManager.load_csv_column_as_set(citing_entities, 'id') if citing_entities else None
-
-    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
-        authors_strings_list = list()
-        editors_string_list = list()
-        dict_orcid = None
-        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list):
-            dict_orcid = self.orcid_finder(doi)
-        agents_list = [
-            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None 
-            else v for k, v in agent_dict.items()} for agent_dict in agents_list]
-
-        for agent in agents_list:
-            cur_role = agent['role']
-            f_name = None
-            g_name = None
-            agent_string = None
-            if agent.get('family') and agent.get('given'):
-                f_name = agent['family']
-                g_name = agent['given']
-                agent_string = f_name + ', ' + g_name
-            elif agent.get('name'):
-                agent_string = agent['name']
-                f_name = agent_string.split(",")[0].strip() if "," in agent_string else None
-                g_name = agent_string.split(",")[-1].strip() if "," in agent_string else None
-
-                if f_name and g_name:
-                    agent_string = f_name + ', ' + g_name
-            if agent_string is None:
-                if agent.get('family') and not agent.get('given'):
-                    if g_name:
-                        agent_string = agent['family'] + ', ' + g_name
-                    else:
-                        agent_string = agent['family'] + ', '
-                elif agent.get('given') and not agent.get('family'):
-                    if f_name:
-                        agent_string = f_name + ', ' + agent['given']
-                    else:
-                        agent_string = ', ' + agent['given']
-            orcid = None
-            if 'orcid' in agent:
-                if isinstance(agent['orcid'], list):
-                    orcid = str(agent['orcid'][0])
-                else:
-                    orcid = str(agent['orcid'])
-            elif 'ORCID' in agent:
-                if isinstance(agent['ORCID'], list):
-                    orcid = str(agent['ORCID'][0])
-                else:
-                    orcid = str(agent['ORCID'])
-            if orcid:
-                orcid_manager = ORCIDManager(use_api_service=False)
-                orcid = orcid_manager.normalise(orcid, include_prefix=False)
-                orcid = orcid if orcid_manager.check_digit(orcid) else None
-            elif dict_orcid and f_name:
-                for ori in dict_orcid:
-                    orc_n: List[str] = dict_orcid[ori].split(', ')
-                    orc_f = orc_n[0].lower()
-                    orc_g = orc_n[1] if len(orc_n) == 2 else None
-                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
-                        if g_name and orc_g:
-                            # If there are several authors with the same surname
-                            if len([person for person in agents_list if 'family' in person if person['family'] if
-                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
-                                        'family'].lower()]) > 1:
-                                # If there are several authors with the same surname and the same given names' initials
-                                if len([person for person in agents_list if 'given' in person if person['given'] if
-                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
-                                    homonyms_list = [person for person in agents_list if 'given' in person if
-                                                     person['given'] if person['given'].lower() == orc_g.lower()]
-                                    # If there are homonyms
-                                    if len(homonyms_list) > 1:
-                                        # If such homonyms have different roles from the current role
-                                        if [person for person in homonyms_list if person['role'] != cur_role]:
-                                            if orc_g.lower() == g_name.lower():
-                                                orcid = ori
-                                    else:
-                                        if orc_g.lower() == g_name.lower():
-                                            orcid = ori
-                                elif orc_g[0].lower() == g_name[0].lower():
-                                    orcid = ori
-                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
-                            elif any([person for person in agents_list if 'given' in person if person['given'] if
-                                      person['given'].lower() == f_name.lower()]):
-                                if orc_g.lower() == g_name.lower():
-                                    orcid = ori
-                            else:
-                                orcid = ori
-                        else:
-                            orcid = ori
-            if agent_string and orcid:
-                agent_string += ' [' + 'orcid:' + str(orcid) + ']'
-            if agent_string:
-                if agent['role'] == 'author':
-                    authors_strings_list.append(agent_string)
-                elif agent['role'] == 'editor':
-                    editors_string_list.append(agent_string)
-        return authors_strings_list, editors_string_list
-
-    def orcid_finder(self, doi: str) -> dict:
-        found = dict()
-        doi = doi.lower()
-        people:  List[str] = self.orcid_index.get_value(doi)
-        if people:
-            for person in people:
-                orcid = re.search(orcid_pattern, person).group(0)
-                name: str = person[:person.find(orcid)-1]
-                found[orcid] = name.strip().lower()
-        return found
-
-    def unzip_citing_entities(self, citing_entities):
-        for dirpath, _, filenames in os.walk(citing_entities):
-            for filename in filenames:
-                if filename.endswith('.zip'):
-                    with ZipFile(os.path.join(citing_entities, filename), mode='r') as zipf:
-                        zipf.extractall(citing_entities)
-                    os.remove(os.path.join(citing_entities, filename))
-
-    def get_pages(self, pages_list:list) -> str:
-        '''
-        This function returns the pages interval. 
-
-        :params pages_list: a list of pages
-        :type item: dict
-        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
-        '''
-        roman_letters = {'I', 'V', 'X', 'L', 'C', 'D', 'M'}
-        clean_pages_list = list()
-        for page in pages_list:
-            # e.g. 583-584 or 1_583-1_584
-            if all(c.isdigit() or c == "_" for c in page):
-                clean_pages_list.append(page)
-            # e.g. G27. It is a born digital document. PeerJ uses this approach, where G27 identifies the whole document, since it has no pages.
-            elif len(pages_list) == 1:
-                clean_pages_list.append(page)
-            # e.g. iv-vii. This syntax is used in the prefaces.
-            elif all(c.upper() in roman_letters for c in page):
-                clean_pages_list.append(page)
-            # 583b-584. It is an error. The b must be removed.
-            elif any(c.isdigit() for c in page):
-                page_without_letters = ''.join([c for c in page if c.isdigit() or c == '_'])
-                clean_pages_list.append(page_without_letters)
-        if clean_pages_list:
-            if len(clean_pages_list) == 1:
-                clean_pages_list.append(clean_pages_list[0])
-            return '-'.join(clean_pages_list)
-        return ''
-    
-    @staticmethod
-    def normalise_unicode(metadata: dict) -> dict:
-        return {k:unicodedata.normalize('NFKC', v) for k, v in metadata.items()}
-
-    @staticmethod
-    def id_worker(field, ids:list, func) -> None:
-        if isinstance(field, list):
-            for i in field:
-                func(str(i), ids)
-        else:
-            id = str(field)
-            func(id, ids)
-
-    @staticmethod
-    def load_publishers_mapping(publishers_filepath: str) -> dict:
-        publishers_mapping: Dict[str, Dict[str, set]] = dict()
-        with open(publishers_filepath, 'r', encoding='utf-8') as f:
-            data = DictReader(f)
-            for row in data:
-                id = row['id']
-                publishers_mapping.setdefault(id, dict())
-                publishers_mapping[id]['name'] = row['name']
-                publishers_mapping[id].setdefault('prefixes', set()).add(row['prefix'])
-        return publishers_mapping
-    
-    @staticmethod
-    def issn_worker(issnid:str, ids:list):
-        issn_manager = ISSNManager()
-        issnid = issn_manager.normalise(issnid, include_prefix=False)
-        if issn_manager.check_digit(issnid) and f'issn:{issnid}' not in ids:
-            ids.append('issn:' + issnid)
-
-    @staticmethod
-    def isbn_worker(isbnid, ids:list):
-        isbn_manager = ISBNManager()
-        isbnid = isbn_manager.normalise(isbnid, include_prefix=False)
-        if isbn_manager.check_digit(isbnid) and f'isbn:{isbnid}' not in ids:
-            ids.append('isbn:' + isbnid)
-
-    @staticmethod
-    def uppercase_initials(inp_str: str):
-        upper_word_list = []
-        words_list = inp_str.split()
-        for w in words_list:
-            upper_word_list.append(w[0].upper() + w[1:]) if len(w)>1 else upper_word_list.append(w[0].upper())
-        upper_str = " ".join(upper_word_list)
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+import os
+import re
+import unicodedata
+from csv import DictReader
+from typing import Dict, List, Tuple
+from zipfile import ZipFile
+
+from oc_ds_converter.oc_idmanager import ISBNManager, ISSNManager, ORCIDManager
+
+from oc_ds_converter.lib.cleaner import Cleaner
+from oc_ds_converter.lib.csvmanager import CSVManager
+from oc_ds_converter.lib.master_of_regex import orcid_pattern
+
+
+class RaProcessor(object):
+    def __init__(self, orcid_index: str = None, doi_csv: str = None, publishers_filepath: str = None, citing_entities: str = None):
+        self.doi_set = CSVManager.load_csv_column_as_set(doi_csv, 'id') if doi_csv else None
+        self.publishers_mapping = self.load_publishers_mapping(publishers_filepath) if publishers_filepath else None
+        orcid_index = orcid_index if orcid_index else None
+        self.orcid_index = CSVManager(orcid_index)
+        if citing_entities:
+            self.unzip_citing_entities(citing_entities)
+            self.citing_entities_set = CSVManager.load_csv_column_as_set(citing_entities, 'id') if citing_entities else None
+
+    def get_agents_strings_list(self, doi: str, agents_list: List[dict]) -> Tuple[list, list]:
+        authors_strings_list = list()
+        editors_string_list = list()
+        dict_orcid = None
+        if not all('orcid' in agent or 'ORCID' in agent for agent in agents_list):
+            dict_orcid = self.orcid_finder(doi)
+        agents_list = [
+            {k: Cleaner(v).remove_unwanted_characters() if k in {'family', 'given', 'name'} and v is not None 
+            else v for k, v in agent_dict.items()} for agent_dict in agents_list]
+
+        for agent in agents_list:
+            cur_role = agent['role']
+            f_name = None
+            g_name = None
+            agent_string = None
+            if agent.get('family') and agent.get('given'):
+                f_name = agent['family']
+                g_name = agent['given']
+                agent_string = f_name + ', ' + g_name
+            elif agent.get('name'):
+                agent_string = agent['name']
+                f_name = agent_string.split(",")[0].strip() if "," in agent_string else None
+                g_name = agent_string.split(",")[-1].strip() if "," in agent_string else None
+
+                if f_name and g_name:
+                    agent_string = f_name + ', ' + g_name
+            if agent_string is None:
+                if agent.get('family') and not agent.get('given'):
+                    if g_name:
+                        agent_string = agent['family'] + ', ' + g_name
+                    else:
+                        agent_string = agent['family'] + ', '
+                elif agent.get('given') and not agent.get('family'):
+                    if f_name:
+                        agent_string = f_name + ', ' + agent['given']
+                    else:
+                        agent_string = ', ' + agent['given']
+            orcid = None
+            if 'orcid' in agent:
+                if isinstance(agent['orcid'], list):
+                    orcid = str(agent['orcid'][0])
+                else:
+                    orcid = str(agent['orcid'])
+            elif 'ORCID' in agent:
+                if isinstance(agent['ORCID'], list):
+                    orcid = str(agent['ORCID'][0])
+                else:
+                    orcid = str(agent['ORCID'])
+            if orcid:
+                orcid_manager = ORCIDManager(use_api_service=False)
+                orcid = orcid_manager.normalise(orcid, include_prefix=False)
+                orcid = orcid if orcid_manager.check_digit(orcid) else None
+            elif dict_orcid and f_name:
+                for ori in dict_orcid:
+                    orc_n: List[str] = dict_orcid[ori].split(', ')
+                    orc_f = orc_n[0].lower()
+                    orc_g = orc_n[1] if len(orc_n) == 2 else None
+                    if f_name.lower() in orc_f.lower() or orc_f.lower() in f_name.lower():
+                        if g_name and orc_g:
+                            # If there are several authors with the same surname
+                            if len([person for person in agents_list if 'family' in person if person['family'] if
+                                    person['family'].lower() in orc_f.lower() or orc_f.lower() in person[
+                                        'family'].lower()]) > 1:
+                                # If there are several authors with the same surname and the same given names' initials
+                                if len([person for person in agents_list if 'given' in person if person['given'] if
+                                        person['given'][0].lower() == orc_g[0].lower()]) > 1:
+                                    homonyms_list = [person for person in agents_list if 'given' in person if
+                                                     person['given'] if person['given'].lower() == orc_g.lower()]
+                                    # If there are homonyms
+                                    if len(homonyms_list) > 1:
+                                        # If such homonyms have different roles from the current role
+                                        if [person for person in homonyms_list if person['role'] != cur_role]:
+                                            if orc_g.lower() == g_name.lower():
+                                                orcid = ori
+                                    else:
+                                        if orc_g.lower() == g_name.lower():
+                                            orcid = ori
+                                elif orc_g[0].lower() == g_name[0].lower():
+                                    orcid = ori
+                            # If there is a person whose given name is equal to the family name of the current person (a common situation for cjk names)
+                            elif any([person for person in agents_list if 'given' in person if person['given'] if
+                                      person['given'].lower() == f_name.lower()]):
+                                if orc_g.lower() == g_name.lower():
+                                    orcid = ori
+                            else:
+                                orcid = ori
+                        else:
+                            orcid = ori
+            if agent_string and orcid:
+                agent_string += ' [' + 'orcid:' + str(orcid) + ']'
+            if agent_string:
+                if agent['role'] == 'author':
+                    authors_strings_list.append(agent_string)
+                elif agent['role'] == 'editor':
+                    editors_string_list.append(agent_string)
+        return authors_strings_list, editors_string_list
+
+    def orcid_finder(self, doi: str) -> dict:
+        found = dict()
+        doi = doi.lower()
+        people:  List[str] = self.orcid_index.get_value(doi)
+        if people:
+            for person in people:
+                orcid = re.search(orcid_pattern, person).group(0)
+                name: str = person[:person.find(orcid)-1]
+                found[orcid] = name.strip().lower()
+        return found
+
+    def unzip_citing_entities(self, citing_entities):
+        for dirpath, _, filenames in os.walk(citing_entities):
+            for filename in filenames:
+                if filename.endswith('.zip'):
+                    with ZipFile(os.path.join(citing_entities, filename), mode='r') as zipf:
+                        zipf.extractall(citing_entities)
+                    os.remove(os.path.join(citing_entities, filename))
+
+    def get_pages(self, pages_list:list) -> str:
+        '''
+        This function returns the pages interval. 
+
+        :params pages_list: a list of pages
+        :type item: dict
+        :returns: str -- The output is a string in the format 'START-END', for example, '583-584'. If there are no pages, the output is an empty string.
+        '''
+        roman_letters = {'I', 'V', 'X', 'L', 'C', 'D', 'M'}
+        clean_pages_list = list()
+        for page in pages_list:
+            # e.g. 583-584 or 1_583-1_584
+            if all(c.isdigit() or c == "_" for c in page):
+                clean_pages_list.append(page)
+            # e.g. G27. It is a born digital document. PeerJ uses this approach, where G27 identifies the whole document, since it has no pages.
+            elif len(pages_list) == 1:
+                clean_pages_list.append(page)
+            # e.g. iv-vii. This syntax is used in the prefaces.
+            elif all(c.upper() in roman_letters for c in page):
+                clean_pages_list.append(page)
+            # 583b-584. It is an error. The b must be removed.
+            elif any(c.isdigit() for c in page):
+                page_without_letters = ''.join([c for c in page if c.isdigit() or c == '_'])
+                clean_pages_list.append(page_without_letters)
+        if clean_pages_list:
+            if len(clean_pages_list) == 1:
+                clean_pages_list.append(clean_pages_list[0])
+            return '-'.join(clean_pages_list)
+        return ''
+    
+    @staticmethod
+    def normalise_unicode(metadata: dict) -> dict:
+        return {k:unicodedata.normalize('NFKC', v) for k, v in metadata.items()}
+
+    @staticmethod
+    def id_worker(field, ids:list, func) -> None:
+        if isinstance(field, list):
+            for i in field:
+                func(str(i), ids)
+        else:
+            id = str(field)
+            func(id, ids)
+
+    @staticmethod
+    def load_publishers_mapping(publishers_filepath: str) -> dict:
+        publishers_mapping: Dict[str, Dict[str, set]] = dict()
+        with open(publishers_filepath, 'r', encoding='utf-8') as f:
+            data = DictReader(f)
+            for row in data:
+                id = row['id']
+                publishers_mapping.setdefault(id, dict())
+                publishers_mapping[id]['name'] = row['name']
+                publishers_mapping[id].setdefault('prefixes', set()).add(row['prefix'])
+        return publishers_mapping
+    
+    @staticmethod
+    def issn_worker(issnid:str, ids:list):
+        issn_manager = ISSNManager()
+        issnid = issn_manager.normalise(issnid, include_prefix=False)
+        if issn_manager.check_digit(issnid) and f'issn:{issnid}' not in ids:
+            ids.append('issn:' + issnid)
+
+    @staticmethod
+    def isbn_worker(isbnid, ids:list):
+        isbn_manager = ISBNManager()
+        isbnid = isbn_manager.normalise(isbnid, include_prefix=False)
+        if isbn_manager.check_digit(isbnid) and f'isbn:{isbnid}' not in ids:
+            ids.append('isbn:' + isbnid)
+
+    @staticmethod
+    def uppercase_initials(inp_str: str):
+        upper_word_list = []
+        words_list = inp_str.split()
+        for w in words_list:
+            upper_word_list.append(w[0].upper() + w[1:]) if len(w)>1 else upper_word_list.append(w[0].upper())
+        upper_str = " ".join(upper_word_list)
         return upper_str
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/run/crossref_process.py` & `oc_ds_converter-1.0.1/oc_ds_converter/run/crossref_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,485 +1,489 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-
-import csv
-import os
-import sys
-import tarfile
-from argparse import ArgumentParser
-from tarfile import TarInfo
-from pathlib import Path
-from filelock import FileLock
-
-import yaml
-from tqdm import tqdm
-from pebble import ProcessFuture, ProcessPool
-
-
-from oc_ds_converter.oc_idmanager.oc_data_storage.redis_manager import \
-    RedisStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import \
-    SqliteStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import \
-    InMemoryStorageManager
-
-from oc_ds_converter.crossref.crossref_processing import *
-from oc_ds_converter.lib.file_manager import normalize_path
-from oc_ds_converter.lib.jsonmanager import *
-
-
-def preprocess(crossref_json_dir:str, publishers_filepath:str, orcid_doi_filepath:str, csv_dir:str, wanted_doi_filepath:str=None, cache:str=None, verbose:bool=False, storage_path:str = None,
-               testing: bool = True, redis_storage_manager: bool = False, max_workers: int = 1) -> None:
-
-
-    if verbose:
-        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
-            what = list()
-            if publishers_filepath:
-                what.append('publishers mapping')
-            if orcid_doi_filepath:
-                what.append('DOI-ORCID index')
-            if wanted_doi_filepath:
-                what.append('wanted DOIs CSV')
-            log = '[INFO: crossref_process] Processing: ' + '; '.join(what)
-            print(log)
-
-    # create output dir if does not exist
-    if not os.path.exists(csv_dir):
-        os.makedirs(csv_dir)
-
-    # create output dir for citation data
-    preprocessed_citations_dir = csv_dir + "_citations"
-    if not os.path.exists(preprocessed_citations_dir):
-        makedirs(preprocessed_citations_dir)
-
-    if verbose:
-        print(f'[INFO: crossref_process] Getting all files from {crossref_json_dir}')
-    all_files, targz_fd = get_all_files_by_type(crossref_json_dir, ".json", cache)
-    if verbose:
-        pbar = tqdm(total=len(all_files))
-
-
-
-    if not redis_storage_manager or max_workers == 1:
-        for filename in all_files:
-            # skip elements starting with ._
-            #if filename.startswith("._"):
-               # continue
-            get_citations_and_metadata(filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath,
-                                       wanted_doi_filepath, publishers_filepath, storage_path,
-                                       redis_storage_manager,
-                                       testing, cache, is_first_iteration=True)
-        for filename in all_files:
-            # skip elements starting with ._
-            #if filename.startswith("._"):
-            #    continue
-            get_citations_and_metadata(filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath,
-                                       wanted_doi_filepath, publishers_filepath, storage_path,
-                                       redis_storage_manager,
-                                       testing, cache, is_first_iteration=False)
-
-    elif redis_storage_manager or max_workers > 1:
-
-        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
-            for filename in all_files:
-                # skip elements starting with ._
-                if filename.startswith("._"):
-                    continue
-
-                future: ProcessFuture = executor.schedule(
-                    function=get_citations_and_metadata,
-                    args=(
-                    filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath, wanted_doi_filepath,
-                    publishers_filepath, storage_path, redis_storage_manager, testing, cache, True))
-
-
-        print("End of FIRST iteration: all the citing entities csv tables should have been produced by now")
-
-        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
-            for filename in all_files:
-                # skip elements starting with ._
-                if filename.startswith("._"):
-                    continue
-
-                future: ProcessFuture = executor.schedule(
-                        function=get_citations_and_metadata,
-                        args=(
-                        filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath, wanted_doi_filepath,
-                        publishers_filepath, storage_path, redis_storage_manager, testing, cache, False))
-
-        print("End of SECOND iteration: all the cited entities csv tables + all the citations tables should have been produced by now")
-
-    # DELETE CACHE AND .LOCK FILE
-    if cache:
-        if os.path.exists(cache):
-            os.remove(cache)
-    lock_file = cache + ".lock"
-    if os.path.exists(lock_file):
-        os.remove(lock_file)
-    pbar.close() if verbose else None
-
-
-def get_citations_and_metadata(file_name, targz_fd, preprocessed_citations_dir: str, csv_dir: str,
-                               orcid_index: str,
-                               doi_csv: str, publishers_filepath: str, storage_path: str,
-                               redis_storage_manager: bool,
-                               testing: bool, cache: str, is_first_iteration:bool):
-    if isinstance(file_name, tarfile.TarInfo):
-        file_tarinfo = file_name
-        file_name = file_name.name
-    storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
-    if cache:
-        if not cache.endswith(".json"):
-            cache = os.path.join(os.getcwd(), "cache.json")
-        else:
-            if not os.path.exists(os.path.abspath(os.path.join(cache, os.pardir))):
-                Path(os.path.abspath(os.path.join(cache, os.pardir))).mkdir(parents=True, exist_ok=True)
-    else:
-        cache = os.path.join(os.getcwd(), "cache.json")
-
-    lock = FileLock(cache + ".lock")
-    cache_dict = dict()
-    file_name = file_name
-    write_new = False
-    if os.path.exists(cache):
-        with lock:
-            with open(cache, "r", encoding="utf-8") as c:
-                try:
-                    cache_dict = json.load(c)
-                except:
-                    write_new = True
-    else:
-        write_new = True
-    if write_new:
-        with lock:
-            with open(cache, "w", encoding="utf-8") as c:
-                json.dump(cache_dict, c)
-
-    # skip if in cache
-    filename = file_name
-    if cache_dict.get("first_iteration"):
-        if is_first_iteration and filename in cache_dict["first_iteration"]:
-            return
-    if cache_dict.get("second_iteration"):
-        if not is_first_iteration and filename in cache_dict["second_iteration"]:
-            return
-
-    if is_first_iteration:
-        crossref_csv = CrossrefProcessing(orcid_index=orcid_index, doi_csv=doi_csv,
-                                      publishers_filepath=publishers_filepath,
-                                      storage_manager=storage_manager, testing=testing, citing=True)
-
-    elif not is_first_iteration:
-        crossref_csv = CrossrefProcessing(orcid_index=orcid_index, doi_csv=doi_csv,
-                                  publishers_filepath=publishers_filepath,
-                                  storage_manager=storage_manager, testing=testing, citing=False)
-    index_citations_to_csv = []
-    data_citing = []
-    data_cited = []
-
-    source_data = load_json(filename, targz_fd)
-    #here I create a list containing all the entities dicts
-    source_dict = source_data['items']
-
-
-    filename = filename.name if isinstance(filename, TarInfo) else filename
-    filename_without_ext = filename.replace('.json', '').replace('.tar', '').replace('.gz', '')
-    filepath = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}.csv')
-    pathoo(filepath)
-
-    filepath_ne = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}')
-    filepath_citations_ne = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}')
-
-    filepath_citations = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}.csv')
-    pathoo(filepath_citations)
-
-    #  √ REDIS UPDATE
-    def get_all_redis_ids_and_save_updates(sli_da, is_first_iteration_par:bool):
-        all_br = []
-        all_ra = []
-
-        # RETRIEVE ALL THE IDENTIFIERS TO BE VALIDATED THAT MAY BE IN REDIS
-        # DOI, ORCID,
-        for entity in sli_da: # for each bibliographical entity in the list
-            if entity and "reference" in entity:
-                # filtering out entities without citations
-                has_doi_references = True if [x for x in entity["reference"] if x.get("DOI")] else False
-                if has_doi_references:
-                    if is_first_iteration_par:
-                        ent_all_br, ent_all_ra = crossref_csv.extract_all_ids(entity, True)
-                    else:
-                        ent_all_br, ent_all_ra = crossref_csv.extract_all_ids(entity, False)
-                    all_br.extend(ent_all_br)
-                    all_ra.extend(all_ra)
-
-        redis_validity_values_br = crossref_csv.get_reids_validity_list(all_br, "br")
-        redis_validity_values_ra = crossref_csv.get_reids_validity_list(all_ra, "ra")
-        crossref_csv.update_redis_values(redis_validity_values_br, redis_validity_values_ra)
-
-    def save_files(ent_list, citation_list, is_first_iteration_par: bool):
-        if ent_list:
-            # Filename of the source json, At first iteration, we will generate a CSV file containing all the
-            # citing entities metadata, at the second iteration we will generate a cited entities metadata file
-            # and the citations csv file
-            if is_first_iteration_par:
-                filename_str = filepath_ne+"_citing.csv"
-            else:
-                filename_str = filepath_ne+"_cited.csv"
-            with open(filename_str, 'w', newline='', encoding='utf-8') as output_file:
-                dict_writer = csv.DictWriter(output_file, ent_list[0].keys(), delimiter=',', quotechar='"',
-                                             quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
-                dict_writer.writeheader()
-                dict_writer.writerows(ent_list)
-            ent_list = []
-        crossref_csv.memory_to_storage()
-
-        if not is_first_iteration_par:
-            if citation_list:
-                filename_cit_str = filepath_citations_ne + ".csv"
-                with open(filename_cit_str, 'w', newline='', encoding='utf-8') as output_file_citations:
-                    dict_writer = csv.DictWriter(output_file_citations, citation_list[0].keys(), delimiter=',',
-                                                 quotechar='"', quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
-                    dict_writer.writeheader()
-                    dict_writer.writerows(citation_list)
-                citation_list = []
-
-        crossref_csv.memory_to_storage()
-        if is_first_iteration_par:
-            task_done(is_first_iteration_par=True)
-        else:
-            task_done(is_first_iteration_par=False)
-        return ent_list, citation_list
-
-    def task_done(is_first_iteration_par: bool) -> None:
-
-        try:
-
-
-            if is_first_iteration_par and "first_iteration" not in cache_dict.keys():
-                cache_dict["first_iteration"] = set()
-
-            if not is_first_iteration_par and "second_iteration" not in cache_dict.keys():
-                cache_dict["second_iteration"] = set()
-
-            for k,v in cache_dict.items():
-                cache_dict[k] = set(v)
-
-            if is_first_iteration_par:
-                cache_dict["first_iteration"].add(Path(file_name).name)
-
-            if not is_first_iteration_par:
-                cache_dict["second_iteration"].add(Path(file_name).name)
-
-
-            with lock:
-                with open(cache, 'r', encoding='utf-8') as aux_file:
-                    cur_cache_dict = json.load(aux_file)
-
-                    for k,v in cur_cache_dict.items():
-                        cur_cache_dict[k] = set(v)
-                        if not cache_dict.get(k) and cur_cache_dict.get(k):
-                            cache_dict[k] = v
-                        elif cache_dict[k] != v:
-                            zip_files_processed_values_list = cache_dict[k]
-                            cur_zip_files_processed_values_list = cur_cache_dict[k]
-
-                            #unione set e poi lista
-                            list_updated = list(cur_zip_files_processed_values_list.union(zip_files_processed_values_list))
-                            cache_dict[k] = list_updated
-
-                    for k,v in cache_dict.items():
-                        if k not in cur_cache_dict:
-                            cur_cache_dict[k] = v
-
-                for k,v in cache_dict.items():
-                    if isinstance(v, set):
-                        cache_dict[k] = list(v)
-
-                with open(cache, 'w', encoding='utf-8') as aux_file:
-                    json.dump(cache_dict, aux_file)
-
-        except Exception as e:
-            print(e)
-
-    if is_first_iteration:
-        get_all_redis_ids_and_save_updates(source_dict, is_first_iteration_par=True)
-        # prima l'ultimo file va processato
-        for entity in tqdm(source_dict):
-            #pbar.update()
-            if entity:
-                #per i citanti la validazione non serve, se è normalizzabile va direttamente alla crezione tabelle Meta
-                norm_source_id = crossref_csv.tmp_doi_m.normalise(entity['DOI'], include_prefix=True)
-
-                # if the id is not in the redis database, it means that it was not processed and that it is not in the csv output tables yet.
-
-                if not crossref_csv.doi_m.storage_manager.get_value(norm_source_id):
-                    # add the id as valid to the temporary storage manager (whose values will be transferred to the redis storage manager at the
-                    # time of the csv files creation process) and create a meta csv row for the entity in this case only
-                    crossref_csv.tmp_doi_m.storage_manager.set_value(norm_source_id, True)
-
-                    if norm_source_id:
-                        source_tab_data = crossref_csv.csv_creator(entity)
-                        if source_tab_data:
-                            processed_source_id = source_tab_data["id"]
-                            if processed_source_id:
-                                data_citing.append(source_tab_data)
-
-        save_files(data_citing, index_citations_to_csv, True)
-
-
-    '''cited entities:
-    - look for the DOI in the temporary manager and in the storage manager:
-        - if found as valid -> do not create the Meta table, but include the cited entity in the citations' tables;
-        - if not found -> look for the doi in Redis server and later call the API if needed -> if the DOI is valid create the
-        table for Meta and include the cited entity in the citations' tables
-        - if found as not valid -> next entity'''
-
-    if not is_first_iteration:
-        get_all_redis_ids_and_save_updates(source_dict, is_first_iteration_par=False)
-        for entity in tqdm(source_dict):
-            if entity and "reference" in entity:
-                # filtering out entities without citations
-                has_doi_references = [x for x in entity["reference"] if x.get("DOI")]
-                if has_doi_references:
-                    norm_source_id = crossref_csv.doi_m.normalise(entity['DOI'], include_prefix=True)
-
-                    cit_list_entities = [x.get("DOI") for x in has_doi_references]
-                    cit_list_entities_dois = [x for x in cit_list_entities if x]
-                    # filtering out entities with citations without dois
-                    if cit_list_entities_dois:
-
-                        valid_target_ids = []
-                        for cited_entity in cit_list_entities_dois:
-
-                            # / START: BR ID VALIDATION
-                            norm_id = crossref_csv.doi_m.normalise(cited_entity, include_prefix=True)
-                            if norm_id:
-                                norm_id_dict_to_val = {"schema":"doi"}
-                                norm_id_dict_to_val["identifier"] = norm_id
-                                stored_validity = crossref_csv.validated_as(norm_id_dict_to_val)
-                                if stored_validity is None:
-                                    norm_id_dict = {"id": norm_id, "schema":"doi"}
-                                    if norm_id in crossref_csv.to_validated_id_list(norm_id_dict):
-                                        cited_entity_dict = {"DOI": norm_id}
-                                        target_tab_data = crossref_csv.csv_creator(cited_entity_dict)
-                                        if target_tab_data:
-                                            processed_target_id = target_tab_data.get("id")
-                                            if processed_target_id:
-                                                data_cited.append(target_tab_data)
-                                                valid_target_ids.append(norm_id)
-                                elif stored_validity is True:
-                                    valid_target_ids.append(norm_id)
-
-                        for target_id in valid_target_ids:
-                            citation = dict()
-                            citation["citing"] = norm_source_id
-                            citation["cited"] = target_id
-                            index_citations_to_csv.append(citation)
-
-        save_files(data_cited, index_citations_to_csv, False)
-
-def get_storage_manager(storage_path: str, redis_storage_manager: bool, testing: bool):
-    if not redis_storage_manager:
-        if storage_path:
-            if not os.path.exists(storage_path):
-            # if parent dir does not exist, it is created
-                if not os.path.exists(os.path.abspath(os.path.join(storage_path, os.pardir))):
-                    Path(os.path.abspath(os.path.join(storage_path, os.pardir))).mkdir(parents=True, exist_ok=True)
-            if storage_path.endswith(".db"):
-                storage_manager = SqliteStorageManager(storage_path)
-            elif storage_path.endswith(".json"):
-                storage_manager = InMemoryStorageManager(storage_path)
-
-        if not storage_path and not redis_storage_manager:
-            new_path_dir = os.path.join(os.getcwd(), "storage")
-            if not os.path.exists(new_path_dir):
-                os.makedirs(new_path_dir)
-            storage_manager = SqliteStorageManager(os.path.join(new_path_dir, "id_valid_dict.db"))
-    elif redis_storage_manager:
-        if testing:
-            storage_manager = RedisStorageManager(testing=True)
-        else:
-            storage_manager = RedisStorageManager(testing=False)
-    return storage_manager
-
-def pathoo(path:str) -> None:
-    if not os.path.exists(os.path.dirname(path)):
-        os.makedirs(os.path.dirname(path))
-
-
-if __name__ == '__main__':
-    arg_parser = ArgumentParser('crossref_process.py', description='This script creates CSV files from Crossref JSON files, enriching them through of a DOI-ORCID index')
-    arg_parser.add_argument('-c', '--config', dest='config', required=False,
-                            help='Configuration file path')
-    required = not any(arg in sys.argv for arg in {'--config', '-c'})
-    arg_parser.add_argument('-cf', '--crossref', dest='crossref_json_dir', required=required,
-                            help='Crossref json files directory')
-    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
-                            help='Directory where CSV will be stored')
-    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
-                            help='CSV file path containing information about publishers (id, name, prefix)')
-    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
-                            help='DOI-ORCID index filepath, to enrich data')
-    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
-                            help='A CSV filepath containing what DOI to process, not mandatory')
-    arg_parser.add_argument('-ca', '--cache', dest='cache', required=False,
-                        help='The cache file path. This file will be deleted at the end of the process')
-    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
-                            help='Show a loading bar, elapsed time and estimated time')
-    arg_parser.add_argument('-sp', '--storage_path', dest='storage_path', required=False,
-                            help='path of the file where to store data concerning validated pids information.'
-                                 'Pay attention to specify a ".db" file in case you chose the SqliteStorageManager'
-                                 'and a ".json" file if you chose InMemoryStorageManager')
-    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
-                            help='parameter to define if the script is to be run in testing mode. Pay attention:'
-                                 'by default the script is run in test modality and thus the data managed by redis, '
-                                 'stored in a specific redis db, are not retrieved nor permanently saved, since an '
-                                 'instance of a FakeRedis class is created and deleted by the end of the process.')
-    arg_parser.add_argument('-r', '--redis_storage_manager', dest='redis_storage_manager', action='store_true',
-                            required=False,
-                            help='parameter to define whether or not to use redis as storage manager. Note that by default the parameter '
-                                 'value is set to false, which means that -unless it is differently stated- the storage manager used is'
-                                 'the one chosen as value of the parameter --storage_manager. The redis db used by the storage manager is the n.2')
-    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=1, type=int,
-                            help='Workers number')
-    args = arg_parser.parse_args()
-    config = args.config
-    settings = None
-    if config:
-        with open(config, encoding='utf-8') as f:
-            settings = yaml.full_load(f)
-    crossref_json_dir = settings['crossref_json_dir'] if settings else args.crossref_json_dir
-    crossref_json_dir = normalize_path(crossref_json_dir)
-    csv_dir = settings['output'] if settings else args.csv_dir
-    csv_dir = normalize_path(csv_dir)
-    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
-    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
-    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
-    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
-    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
-    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
-    cache = settings['cache_filepath'] if settings else args.cache
-    cache = normalize_path(cache) if cache else None
-    verbose = settings['verbose'] if settings else args.verbose
-    storage_path = settings['storage_path'] if settings else args.storage_path
-    storage_path = normalize_path(storage_path) if storage_path else None
-    testing = settings['testing'] if settings else args.testing
-    redis_storage_manager = settings['redis_storage_manager'] if settings else args.redis_storage_manager
-    max_workers = settings['max_workers'] if settings else args.max_workers
-
-    preprocess(crossref_json_dir=crossref_json_dir, publishers_filepath=publishers_filepath, orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir, wanted_doi_filepath=wanted_doi_filepath, cache=cache, verbose=verbose, storage_path=storage_path, testing=testing,
-               redis_storage_manager=redis_storage_manager, max_workers=max_workers)
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright 2021-2022 Arcangelo Massari <arcangelo.massari@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+
+import csv
+import os
+import sys
+import tarfile
+from argparse import ArgumentParser
+from tarfile import TarInfo
+from pathlib import Path
+from filelock import FileLock
+
+import yaml
+from tqdm import tqdm
+from pebble import ProcessFuture, ProcessPool
+
+
+from oc_ds_converter.oc_idmanager.oc_data_storage.redis_manager import \
+    RedisStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import \
+    SqliteStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import \
+    InMemoryStorageManager
+
+from oc_ds_converter.crossref.crossref_processing import *
+from oc_ds_converter.lib.file_manager import normalize_path
+from oc_ds_converter.lib.jsonmanager import *
+
+
+def preprocess(crossref_json_dir:str, publishers_filepath:str, orcid_doi_filepath:str, csv_dir:str, wanted_doi_filepath:str=None, cache:str=None, verbose:bool=False, storage_path:str = None,
+               testing: bool = True, redis_storage_manager: bool = False, max_workers: int = 1) -> None:
+
+
+    if verbose:
+        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
+            what = list()
+            if publishers_filepath:
+                what.append('publishers mapping')
+            if orcid_doi_filepath:
+                what.append('DOI-ORCID index')
+            if wanted_doi_filepath:
+                what.append('wanted DOIs CSV')
+            log = '[INFO: crossref_process] Processing: ' + '; '.join(what)
+            print(log)
+
+    # create output dir if does not exist
+    if not os.path.exists(csv_dir):
+        os.makedirs(csv_dir)
+
+    # create output dir for citation data
+    preprocessed_citations_dir = csv_dir + "_citations"
+    if not os.path.exists(preprocessed_citations_dir):
+        os.makedirs(preprocessed_citations_dir)
+
+    if verbose:
+        print(f'[INFO: crossref_process] Getting all files from {crossref_json_dir}')
+    all_files, targz_fd = get_all_files_by_type(crossref_json_dir, ".json", cache)
+    if verbose:
+        pbar = tqdm(total=len(all_files))
+
+    if not redis_storage_manager or max_workers == 1:
+        for filename in all_files:
+            # skip elements starting with ._
+            #if filename.startswith("._"):
+               # continue
+            get_citations_and_metadata(filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath,
+                                       wanted_doi_filepath, publishers_filepath, storage_path,
+                                       redis_storage_manager,
+                                       testing, cache, is_first_iteration=True)
+        for filename in all_files:
+            # skip elements starting with ._
+            #if filename.startswith("._"):
+            #    continue
+            get_citations_and_metadata(filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath,
+                                       wanted_doi_filepath, publishers_filepath, storage_path,
+                                       redis_storage_manager,
+                                       testing, cache, is_first_iteration=False)
+
+    elif redis_storage_manager or max_workers > 1:
+
+        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
+            for filename in all_files:
+                # skip elements starting with ._
+                if filename.startswith("._"):
+                    continue
+
+                future: ProcessFuture = executor.schedule(
+                    function=get_citations_and_metadata,
+                    args=(
+                    filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath, wanted_doi_filepath,
+                    publishers_filepath, storage_path, redis_storage_manager, testing, cache, True))
+
+
+        print("End of FIRST iteration: all the citing entities csv tables should have been produced by now")
+
+        with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
+            for filename in all_files:
+                # skip elements starting with ._
+                if filename.startswith("._"):
+                    continue
+
+                future: ProcessFuture = executor.schedule(
+                        function=get_citations_and_metadata,
+                        args=(
+                        filename, targz_fd, preprocessed_citations_dir, csv_dir, orcid_doi_filepath, wanted_doi_filepath,
+                        publishers_filepath, storage_path, redis_storage_manager, testing, cache, False))
+
+        print("End of SECOND iteration: all the cited entities csv tables + all the citations tables should have been produced by now")
+
+    # DELETE CACHE AND .LOCK FILE
+    if cache:
+        if os.path.exists(cache):
+            os.remove(cache)
+    lock_file = cache + ".lock"
+
+    if os.path.exists(lock_file):
+        os.remove(lock_file)
+    pbar.close() if verbose else None
+
+    # added to avoid order-releted issues in sequential tests runs
+    if testing:
+        storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
+        storage_manager.delete_storage()
+
+
+def get_citations_and_metadata(file_name, targz_fd, preprocessed_citations_dir: str, csv_dir: str,
+                               orcid_index: str,
+                               doi_csv: str, publishers_filepath: str, storage_path: str,
+                               redis_storage_manager: bool,
+                               testing: bool, cache: str, is_first_iteration:bool):
+    if isinstance(file_name, tarfile.TarInfo):
+        file_tarinfo = file_name
+        file_name = file_name.name
+    storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
+    if cache:
+        if not cache.endswith(".json"):
+            cache = os.path.join(os.getcwd(), "cache.json")
+        else:
+            if not os.path.exists(os.path.abspath(os.path.join(cache, os.pardir))):
+                Path(os.path.abspath(os.path.join(cache, os.pardir))).mkdir(parents=True, exist_ok=True)
+    else:
+        cache = os.path.join(os.getcwd(), "cache.json")
+
+    lock = FileLock(cache + ".lock")
+    cache_dict = dict()
+    file_name = file_name
+    write_new = False
+    if os.path.exists(cache):
+        with lock:
+            with open(cache, "r", encoding="utf-8") as c:
+                try:
+                    cache_dict = json.load(c)
+                except:
+                    write_new = True
+    else:
+        write_new = True
+    if write_new:
+        with lock:
+            with open(cache, "w", encoding="utf-8") as c:
+                json.dump(cache_dict, c)
+
+    # skip if in cache
+    filename = file_name
+    if cache_dict.get("first_iteration"):
+        if is_first_iteration and filename in cache_dict["first_iteration"]:
+            return
+    if cache_dict.get("second_iteration"):
+        if not is_first_iteration and filename in cache_dict["second_iteration"]:
+            return
+
+    if is_first_iteration:
+        crossref_csv = CrossrefProcessing(orcid_index=orcid_index, doi_csv=doi_csv,
+                                      publishers_filepath=publishers_filepath,
+                                      storage_manager=storage_manager, testing=testing, citing=True)
+
+    elif not is_first_iteration:
+        crossref_csv = CrossrefProcessing(orcid_index=orcid_index, doi_csv=doi_csv,
+                                  publishers_filepath=publishers_filepath,
+                                  storage_manager=storage_manager, testing=testing, citing=False)
+    index_citations_to_csv = []
+    data_citing = []
+    data_cited = []
+
+    source_data = load_json(filename, targz_fd)
+    #here I create a list containing all the entities dicts
+    source_dict = source_data['items']
+
+
+    filename = filename.name if isinstance(filename, TarInfo) else filename
+    filename_without_ext = filename.replace('.json', '').replace('.tar', '').replace('.gz', '')
+    filepath = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}.csv')
+    pathoo(filepath)
+
+    filepath_ne = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}')
+    filepath_citations_ne = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}')
+
+    filepath_citations = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}.csv')
+    pathoo(filepath_citations)
+
+    #  √ REDIS UPDATE
+    def get_all_redis_ids_and_save_updates(sli_da, is_first_iteration_par:bool):
+        all_br = []
+        all_ra = []
+
+        # RETRIEVE ALL THE IDENTIFIERS TO BE VALIDATED THAT MAY BE IN REDIS
+        # DOI, ORCID,
+        for entity in sli_da: # for each bibliographical entity in the list
+            if entity and "reference" in entity:
+                # filtering out entities without citations
+                has_doi_references = True if [x for x in entity["reference"] if x.get("DOI")] else False
+                if has_doi_references:
+                    if is_first_iteration_par:
+                        ent_all_br, ent_all_ra = crossref_csv.extract_all_ids(entity, True)
+                    else:
+                        ent_all_br, ent_all_ra = crossref_csv.extract_all_ids(entity, False)
+                    all_br.extend(ent_all_br)
+                    all_ra.extend(all_ra)
+
+        redis_validity_values_br = crossref_csv.get_reids_validity_list(all_br, "br")
+        redis_validity_values_ra = crossref_csv.get_reids_validity_list(all_ra, "ra")
+        crossref_csv.update_redis_values(redis_validity_values_br, redis_validity_values_ra)
+
+    def save_files(ent_list, citation_list, is_first_iteration_par: bool):
+        if ent_list:
+            # Filename of the source json, At first iteration, we will generate a CSV file containing all the
+            # citing entities metadata, at the second iteration we will generate a cited entities metadata file
+            # and the citations csv file
+            if is_first_iteration_par:
+                filename_str = filepath_ne+"_citing.csv"
+            else:
+                filename_str = filepath_ne+"_cited.csv"
+            with open(filename_str, 'w', newline='', encoding='utf-8') as output_file:
+                dict_writer = csv.DictWriter(output_file, ent_list[0].keys(), delimiter=',', quotechar='"',
+                                             quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
+                dict_writer.writeheader()
+                dict_writer.writerows(ent_list)
+            ent_list = []
+        crossref_csv.memory_to_storage()
+
+        if not is_first_iteration_par:
+            if citation_list:
+                filename_cit_str = filepath_citations_ne + ".csv"
+                with open(filename_cit_str, 'w', newline='', encoding='utf-8') as output_file_citations:
+                    dict_writer = csv.DictWriter(output_file_citations, citation_list[0].keys(), delimiter=',',
+                                                 quotechar='"', quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
+                    dict_writer.writeheader()
+                    dict_writer.writerows(citation_list)
+                citation_list = []
+
+        crossref_csv.memory_to_storage()
+        if is_first_iteration_par:
+            task_done(is_first_iteration_par=True)
+        else:
+            task_done(is_first_iteration_par=False)
+        return ent_list, citation_list
+
+    def task_done(is_first_iteration_par: bool) -> None:
+
+        try:
+
+
+            if is_first_iteration_par and "first_iteration" not in cache_dict.keys():
+                cache_dict["first_iteration"] = set()
+
+            if not is_first_iteration_par and "second_iteration" not in cache_dict.keys():
+                cache_dict["second_iteration"] = set()
+
+            for k,v in cache_dict.items():
+                cache_dict[k] = set(v)
+
+            if is_first_iteration_par:
+                cache_dict["first_iteration"].add(Path(file_name).name)
+
+            if not is_first_iteration_par:
+                cache_dict["second_iteration"].add(Path(file_name).name)
+
+
+            with lock:
+                with open(cache, 'r', encoding='utf-8') as aux_file:
+                    cur_cache_dict = json.load(aux_file)
+
+                    for k,v in cur_cache_dict.items():
+                        cur_cache_dict[k] = set(v)
+                        if not cache_dict.get(k) and cur_cache_dict.get(k):
+                            cache_dict[k] = v
+                        elif cache_dict[k] != v:
+                            zip_files_processed_values_list = cache_dict[k]
+                            cur_zip_files_processed_values_list = cur_cache_dict[k]
+
+                            #unione set e poi lista
+                            list_updated = list(cur_zip_files_processed_values_list.union(zip_files_processed_values_list))
+                            cache_dict[k] = list_updated
+
+                    for k,v in cache_dict.items():
+                        if k not in cur_cache_dict:
+                            cur_cache_dict[k] = v
+
+                for k,v in cache_dict.items():
+                    if isinstance(v, set):
+                        cache_dict[k] = list(v)
+
+                with open(cache, 'w', encoding='utf-8') as aux_file:
+                    json.dump(cache_dict, aux_file)
+
+        except Exception as e:
+            print(e)
+
+    if is_first_iteration:
+        get_all_redis_ids_and_save_updates(source_dict, is_first_iteration_par=True)
+        # prima l'ultimo file va processato
+        for entity in tqdm(source_dict):
+            #pbar.update()
+            if entity:
+                #per i citanti la validazione non serve, se è normalizzabile va direttamente alla crezione tabelle Meta
+                norm_source_id = crossref_csv.tmp_doi_m.normalise(entity['DOI'], include_prefix=True)
+
+                # if the id is not in the redis database, it means that it was not processed and that it is not in the csv output tables yet.
+
+                if not crossref_csv.doi_m.storage_manager.get_value(norm_source_id):
+                    # add the id as valid to the temporary storage manager (whose values will be transferred to the redis storage manager at the
+                    # time of the csv files creation process) and create a meta csv row for the entity in this case only
+                    crossref_csv.tmp_doi_m.storage_manager.set_value(norm_source_id, True)
+
+                    if norm_source_id:
+                        source_tab_data = crossref_csv.csv_creator(entity)
+                        if source_tab_data:
+                            processed_source_id = source_tab_data["id"]
+                            if processed_source_id:
+                                data_citing.append(source_tab_data)
+
+        save_files(data_citing, index_citations_to_csv, True)
+
+
+    '''cited entities:
+    - look for the DOI in the temporary manager and in the storage manager:
+        - if found as valid -> do not create the Meta table, but include the cited entity in the citations' tables;
+        - if not found -> look for the doi in Redis server and later call the API if needed -> if the DOI is valid create the
+        table for Meta and include the cited entity in the citations' tables
+        - if found as not valid -> next entity'''
+
+    if not is_first_iteration:
+        get_all_redis_ids_and_save_updates(source_dict, is_first_iteration_par=False)
+        for entity in tqdm(source_dict):
+            if entity and "reference" in entity:
+                # filtering out entities without citations
+                has_doi_references = [x for x in entity["reference"] if x.get("DOI")]
+                if has_doi_references:
+                    norm_source_id = crossref_csv.doi_m.normalise(entity['DOI'], include_prefix=True)
+
+                    cit_list_entities = [x.get("DOI") for x in has_doi_references]
+                    cit_list_entities_dois = [x for x in cit_list_entities if x]
+                    # filtering out entities with citations without dois
+                    if cit_list_entities_dois:
+
+                        valid_target_ids = []
+                        for cited_entity in cit_list_entities_dois:
+
+                            # / START: BR ID VALIDATION
+                            norm_id = crossref_csv.doi_m.normalise(cited_entity, include_prefix=True)
+                            if norm_id:
+                                norm_id_dict_to_val = {"schema":"doi"}
+                                norm_id_dict_to_val["identifier"] = norm_id
+                                stored_validity = crossref_csv.validated_as(norm_id_dict_to_val)
+                                if stored_validity is None:
+                                    norm_id_dict = {"id": norm_id, "schema":"doi"}
+                                    if norm_id in crossref_csv.to_validated_id_list(norm_id_dict):
+                                        cited_entity_dict = {"DOI": norm_id}
+                                        target_tab_data = crossref_csv.csv_creator(cited_entity_dict)
+                                        if target_tab_data:
+                                            processed_target_id = target_tab_data.get("id")
+                                            if processed_target_id:
+                                                data_cited.append(target_tab_data)
+                                                valid_target_ids.append(norm_id)
+                                elif stored_validity is True:
+                                    valid_target_ids.append(norm_id)
+
+                        for target_id in valid_target_ids:
+                            citation = dict()
+                            citation["citing"] = norm_source_id
+                            citation["cited"] = target_id
+                            index_citations_to_csv.append(citation)
+
+        save_files(data_cited, index_citations_to_csv, False)
+
+def get_storage_manager(storage_path: str, redis_storage_manager: bool, testing: bool):
+    if not redis_storage_manager:
+        if storage_path:
+            if not os.path.exists(storage_path):
+            # if parent dir does not exist, it is created
+                if not os.path.exists(os.path.abspath(os.path.join(storage_path, os.pardir))):
+                    Path(os.path.abspath(os.path.join(storage_path, os.pardir))).mkdir(parents=True, exist_ok=True)
+            if storage_path.endswith(".db"):
+                storage_manager = SqliteStorageManager(storage_path)
+            elif storage_path.endswith(".json"):
+                storage_manager = InMemoryStorageManager(storage_path)
+
+        if not storage_path and not redis_storage_manager:
+            new_path_dir = os.path.join(os.getcwd(), "storage")
+            if not os.path.exists(new_path_dir):
+                os.makedirs(new_path_dir)
+            storage_manager = SqliteStorageManager(os.path.join(new_path_dir, "id_valid_dict.db"))
+    elif redis_storage_manager:
+        if testing:
+            storage_manager = RedisStorageManager(testing=True)
+        else:
+            storage_manager = RedisStorageManager(testing=False)
+    return storage_manager
+
+def pathoo(path:str) -> None:
+    if not os.path.exists(os.path.dirname(path)):
+        os.makedirs(os.path.dirname(path))
+
+
+if __name__ == '__main__':
+    arg_parser = ArgumentParser('crossref_process.py', description='This script creates CSV files from Crossref JSON files, enriching them through of a DOI-ORCID index')
+    arg_parser.add_argument('-c', '--config', dest='config', required=False,
+                            help='Configuration file path')
+    required = not any(arg in sys.argv for arg in {'--config', '-c'})
+    arg_parser.add_argument('-cf', '--crossref', dest='crossref_json_dir', required=required,
+                            help='Crossref json files directory')
+    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
+                            help='Directory where CSV will be stored')
+    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
+                            help='CSV file path containing information about publishers (id, name, prefix)')
+    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
+                            help='DOI-ORCID index filepath, to enrich data')
+    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
+                            help='A CSV filepath containing what DOI to process, not mandatory')
+    arg_parser.add_argument('-ca', '--cache', dest='cache', required=False,
+                        help='The cache file path. This file will be deleted at the end of the process')
+    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
+                            help='Show a loading bar, elapsed time and estimated time')
+    arg_parser.add_argument('-sp', '--storage_path', dest='storage_path', required=False,
+                            help='path of the file where to store data concerning validated pids information.'
+                                 'Pay attention to specify a ".db" file in case you chose the SqliteStorageManager'
+                                 'and a ".json" file if you chose InMemoryStorageManager')
+    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
+                            help='parameter to define if the script is to be run in testing mode. Pay attention:'
+                                 'by default the script is run in test modality and thus the data managed by redis, '
+                                 'stored in a specific redis db, are not retrieved nor permanently saved, since an '
+                                 'instance of a FakeRedis class is created and deleted by the end of the process.')
+    arg_parser.add_argument('-r', '--redis_storage_manager', dest='redis_storage_manager', action='store_true',
+                            required=False,
+                            help='parameter to define whether or not to use redis as storage manager. Note that by default the parameter '
+                                 'value is set to false, which means that -unless it is differently stated- the storage manager used is'
+                                 'the one chosen as value of the parameter --storage_manager. The redis db used by the storage manager is the n.2')
+    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=1, type=int,
+                            help='Workers number')
+    args = arg_parser.parse_args()
+    config = args.config
+    settings = None
+    if config:
+        with open(config, encoding='utf-8') as f:
+            settings = yaml.full_load(f)
+    crossref_json_dir = settings['crossref_json_dir'] if settings else args.crossref_json_dir
+    crossref_json_dir = normalize_path(crossref_json_dir)
+    csv_dir = settings['output'] if settings else args.csv_dir
+    csv_dir = normalize_path(csv_dir)
+    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
+    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
+    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
+    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
+    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
+    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
+    cache = settings['cache_filepath'] if settings else args.cache
+    cache = normalize_path(cache) if cache else None
+    verbose = settings['verbose'] if settings else args.verbose
+    storage_path = settings['storage_path'] if settings else args.storage_path
+    storage_path = normalize_path(storage_path) if storage_path else None
+    testing = settings['testing'] if settings else args.testing
+    redis_storage_manager = settings['redis_storage_manager'] if settings else args.redis_storage_manager
+    max_workers = settings['max_workers'] if settings else args.max_workers
+
+    preprocess(crossref_json_dir=crossref_json_dir, publishers_filepath=publishers_filepath, orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir, wanted_doi_filepath=wanted_doi_filepath, cache=cache, verbose=verbose, storage_path=storage_path, testing=testing,
+               redis_storage_manager=redis_storage_manager, max_workers=max_workers)
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/run/openaire_process.py` & `oc_ds_converter-1.0.1/oc_ds_converter/run/openaire_process.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,482 +1,487 @@
-import functools
-import os.path
-import sys
-from tarfile import TarInfo
-
-import yaml
-from oc_ds_converter.lib.file_manager import normalize_path
-from oc_ds_converter.lib.jsonmanager import *
-from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import \
-    InMemoryStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.redis_manager import \
-    RedisStorageManager
-from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import \
-    SqliteStorageManager
-from oc_ds_converter.openaire.openaire_processing import *
-from pebble import ProcessFuture, ProcessPool
-from tqdm import tqdm
-from filelock import Timeout, FileLock
-
-
-def preprocess(
-        openaire_json_dir:str, publishers_filepath:str, orcid_doi_filepath:str, 
-        csv_dir:str, wanted_doi_filepath:str=None, cache:str=None, verbose:bool=False, storage_path:str = None, 
-        testing: bool = True, redis_storage_manager: bool = False, max_workers: int = 1, target=50000) -> None:
-
-    if not testing: # NON CANCELLARE FILES MA PRENDI SOLO IN CONSIDERAZIONE
-        input_dir_cont = os.listdir(openaire_json_dir)
-        els_to_be_removed = []
-        for el in input_dir_cont:
-            if el.startswith("._"):
-                els_to_be_removed.append(os.path.join(openaire_json_dir, el))
-            else:
-                if el.endswith(".tar"):
-                    base_name = el.replace('.tar', '')
-                    if [x for x in os.listdir(openaire_json_dir) if x.startswith(base_name) and x.endswith("decompr_zip_dir")]:
-                        els_to_be_removed.append(os.path.join(openaire_json_dir, el))
-
-        if els_to_be_removed: # Anziché els_to_be_removed +  os.remove(etbr), fare in modo di skippare (es. els_to_be_skipped + skip
-            # in fase di lettura dell'input) questi compressi nel processo
-            # nel caso in cui ci sia già un decompresso equivalente (per evitare di riprocessare inutilmente gli stessi dati)
-            for etbr in els_to_be_removed:
-                os.remove(etbr)
-
-
-
-    # creare cartella di output se non esiste (dove verranno salvati i csv delle tabelle di meta)
-    if not os.path.exists(csv_dir):
-        os.makedirs(csv_dir)
-
-    req_type = ".gz"
-
-    # creare cartella _citations di output se non esiste (dove verranno salvati i csv delle citazioni)
-    preprocessed_citations_dir = csv_dir + "_citations"
-    if not os.path.exists(preprocessed_citations_dir):
-        makedirs(preprocessed_citations_dir)
-    if verbose:
-        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
-            what = list()
-            if publishers_filepath:
-                what.append('publishers mapping')
-            if orcid_doi_filepath:
-                what.append('DOI-ORCID index')
-            if wanted_doi_filepath:
-                what.append('wanted DOIs CSV')
-            log = '[INFO: openaire_process] Processing: ' + '; '.join(what)
-            print(log)
-
-    
-    if verbose:
-        print(f'[INFO: openaire_process] Getting all files from {openaire_json_dir}')
-
-    all_input_tar = os.listdir(openaire_json_dir)
-    for tar in all_input_tar:
-        all_files, targz_fd = get_all_files_by_type(os.path.join(openaire_json_dir, tar), req_type, cache)
-        if not redis_storage_manager or max_workers == 1:
-            for filename in all_files:
-                get_citations_and_metadata(tar, preprocessed_citations_dir, csv_dir, filename, orcid_doi_filepath, wanted_doi_filepath, publishers_filepath, storage_path, redis_storage_manager, testing, cache, target)
-
-
-        elif redis_storage_manager or max_workers > 1:
-            with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
-                for filename in all_files:
-                    future:ProcessFuture = executor.schedule(
-                        function = get_citations_and_metadata,
-                        args=(tar, preprocessed_citations_dir, csv_dir, filename, orcid_doi_filepath, wanted_doi_filepath, publishers_filepath, storage_path, redis_storage_manager, testing, cache, target)
-                    )
-
-
-    if cache:
-        if os.path.exists(cache):
-            os.remove(cache)
-    lock_file = cache + ".lock"
-    if os.path.exists(lock_file):
-        os.remove(lock_file)
-
-
-def get_citations_and_metadata(tar: str, preprocessed_citations_dir: str, csv_dir: str, filename: str, orcid_index: str, doi_csv: str, publishers_filepath_openaire: str, storage_path: str, redis_storage_manager: bool, testing: bool, cache:str, target=50000):
-
-    storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
-
-    if cache:
-        if not cache.endswith(".json"):
-            cache = os.path.join(os.getcwd(), "cache.json")
-        else:
-            if not os.path.exists(os.path.abspath(os.path.join(cache, os.pardir))):
-                Path(os.path.abspath(os.path.join(cache, os.pardir))).mkdir(parents=True, exist_ok=True)
-    else:
-        cache = os.path.join(os.getcwd(), "cache.json")
-
-    last_part_processed = 0
-    lock = FileLock(cache + ".lock")
-    cache_dict = dict()
-    write_new = False
-
-    if os.path.exists(cache):
-        with lock:
-            with open(cache, "r", encoding="utf-8") as c:
-                try:
-                    cache_dict = json.load(c)
-                except:
-                    write_new = True
-    else:
-        write_new = True
-
-    if write_new:
-        with lock:
-            with open(cache, "w", encoding="utf-8") as c:
-                json.dump(cache_dict, c)
-
-    # skip if in cache
-    if tar in cache_dict:
-        if filename in cache_dict[tar]:
-            if cache_dict[tar][filename] == "completed":
-                return
-            else:
-                last_part_processed = cache_dict[tar][filename]
-        else:
-            filename_alt = ''
-            if '/' in filename:
-                filename_alt = filename.replace('/', '\\')
-            elif '\\' in filename:
-                filename_alt = filename.replace('\\', '/')
-            if filename_alt:
-                if filename_alt in cache_dict[tar]:
-                    if cache_dict[tar][filename_alt] == "completed":
-                        return
-                    else:
-                        last_part_processed = cache_dict[tar][filename]
-
-    openaire_csv = OpenaireProcessing(orcid_index=orcid_index, doi_csv=doi_csv, publishers_filepath_openaire=publishers_filepath_openaire, storage_manager=storage_manager, testing=testing)
-
-    index_citations_to_csv = []
-    data = []
-
-    target = target
-
-    skip_rows = target * last_part_processed
-
-    f = gzip.open(filename, 'rb')
-    source_data = f.readlines()
-    pbar = tqdm(total=len(source_data))
-    f.close()
-    filename = filename.name if isinstance(filename, TarInfo) else filename
-    filename_without_ext = filename.replace('.json', '').replace('.tar', '').replace('.gz', '')
-    filepath_ne = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}')
-    filepath_citations_ne = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}')
-
-    filepath = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}.csv')
-    filepath_citations = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}.csv')
-    pathoo(filepath)
-
-    def get_all_redis_ids_and_save_updates(sli_da):
-        all_br = []
-        all_ra = []
-        for entity in sli_da:
-
-            # start check: if line is processable
-            if entity:
-                d = json.loads(entity.decode('utf-8'))
-                if d.get("relationship"):
-                    if d.get("relationship").get("name") == "Cites":
-                        # end check: if line is processable
-
-                        ent_all_br, ent_all_ra = openaire_csv.extract_all_ids(json.loads(entity))
-                        all_br.extend(ent_all_br)
-                        all_ra.extend(ent_all_ra)
-
-        redis_validity_values_br = openaire_csv.get_reids_validity_list(all_br, "br")
-        redis_validity_values_ra = openaire_csv.get_reids_validity_list(all_ra, "ra")
-        openaire_csv.update_redis_values(redis_validity_values_br, redis_validity_values_ra)
-
-    def save_files(ent_list, citation_list, nf, is_last_sf=False):
-        if ent_list:
-            filename_str = filepath_ne+"_"+str(nf) + ".csv"
-            with open(filename_str, 'w', newline='', encoding='utf-8') as output_file:
-                dict_writer = csv.DictWriter(output_file, ent_list[0].keys(), delimiter=',', quotechar='"',
-                                             quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
-                dict_writer.writeheader()
-                dict_writer.writerows(ent_list)
-            ent_list = []
-
-        if citation_list:
-            filename_cit_str = filepath_citations_ne+"_"+str(nf) + ".csv"
-            with open(filename_cit_str, 'w', newline='', encoding='utf-8') as output_file_citations:
-                dict_writer = csv.DictWriter(output_file_citations, citation_list[0].keys(), delimiter=',',
-                                             quotechar='"', quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
-                dict_writer.writeheader()
-                dict_writer.writerows(citation_list)
-            citation_list = []
-
-        openaire_csv.memory_to_storage()
-
-        task_done(nf, is_last=is_last_sf)
-
-        return ent_list, citation_list
-
-    def task_done(file_part_number, is_last=False) -> None:
-        try:
-            if tar not in cache_dict:
-                cache_dict[tar] = dict()
-
-            if not is_last:
-                cache_dict[tar][filename] = file_part_number
-            else:
-                cache_dict[tar][filename] = "completed"
-
-            with lock:
-                with open(cache, 'r', encoding='utf-8') as aux_file:
-                    cur_cache_dict = json.load(aux_file)
-
-                    for k,v in cur_cache_dict.items():
-                        if not cache_dict.get(k) and cur_cache_dict.get(k):
-                            cache_dict[k] = v
-                        elif cache_dict[k] != v:
-                            tar_files_processed_values_dict = cache_dict[k]
-                            cur_tar_files_processed_values_dict = cur_cache_dict[k]
-
-                            for c, w in cur_tar_files_processed_values_dict.items():
-                                if tar_files_processed_values_dict.get(c) == "completed" or cur_tar_files_processed_values_dict.get(c) == "completed":
-                                    cur_tar_files_processed_values_dict[c] = "completed"
-                                elif isinstance(tar_files_processed_values_dict.get(c), int) and isinstance(cur_tar_files_processed_values_dict.get(c), int):
-                                    cur_tar_files_processed_values_dict[c] = max([tar_files_processed_values_dict.get(c), cur_tar_files_processed_values_dict.get(c)])
-                                elif isinstance(tar_files_processed_values_dict.get(c), int) or isinstance(cur_tar_files_processed_values_dict.get(c), int):
-                                    cur_tar_files_processed_values_dict[c] = tar_files_processed_values_dict.get(c) if isinstance(tar_files_processed_values_dict.get(c), int) else cur_tar_files_processed_values_dict.get(c)
-
-                            tar_files_processed_values_dict.update(cur_tar_files_processed_values_dict)
-                            cache_dict[k] = tar_files_processed_values_dict
-
-                    for k,v in cache_dict.items():
-                        if k not in cur_cache_dict:
-                            cur_cache_dict[k] = v
-
-                    for k,v in cur_cache_dict.items():
-                        if k not in cache_dict:
-                            cache_dict[k] = v
-
-                with open(cache, 'w', encoding='utf-8') as aux_file:
-                    json.dump(cache_dict, aux_file)
-
-        except Exception as e:
-            print(e)
-
-
-    start = skip_rows
-    cnt = skip_rows
-    end = start + target
-
-    if len(source_data[start:]) > target:
-        source_data_slice = source_data[start: end]
-    else:
-        source_data_slice = source_data[start:]
-
-    get_all_redis_ids_and_save_updates(source_data_slice)
-
-    for entity in source_data:
-
-        # in case the current entity is the <target>nth entity
-        if cnt == end:
-            start = cnt
-            end = start + target
-            if len(source_data[start:]) > target:
-                source_data_slice = source_data[start: end]
-            else:
-                source_data_slice = source_data[start:]
-
-            # update redis validated id list + save citation and meta file
-            get_all_redis_ids_and_save_updates(source_data_slice)
-            last_part_processed += 1
-            data, index_citations_to_csv = save_files(data, index_citations_to_csv, last_part_processed)
-
-        # real entity process
-        if entity:
-            d = json.loads(entity.decode('utf-8'))
-            if d.get("relationship"):
-                if d.get("relationship").get("name") == "Cites":
-
-                    norm_source_ids = []
-                    norm_target_ids = []
-
-                    any_source_id = ""
-                    any_target_id = ""
-
-                    source_entity = d.get("source")
-                    if source_entity:
-                        norm_source_ids = openaire_csv.get_norm_ids(source_entity['identifier'])
-                        if norm_source_ids:
-                            for e, nsi in enumerate(norm_source_ids):
-                                stored_validity = openaire_csv.validated_as(nsi)
-                                norm_source_ids[e]["valid"] = stored_validity
-
-
-                    target_entity = d.get("target")
-                    if target_entity:
-                        norm_target_ids = openaire_csv.get_norm_ids(target_entity['identifier'])
-                        if norm_target_ids:
-                            for i, nti in enumerate(norm_target_ids):
-                                stored_validity_t = openaire_csv.validated_as(nti)
-                                norm_target_ids[i]["valid"] = stored_validity_t
-
-                    # check that there is a citation we can handle (i.e.: expressed with ids we actually manage)
-                    if norm_source_ids and norm_target_ids:
-
-                        source_entity_upd_ids = {k:v for k,v in source_entity.items() if k != "identifier"}
-                        source_valid_ids = [x for x in norm_source_ids if x["valid"] is True]
-                        source_invalid_ids = [x for x in norm_source_ids if x["valid"] is False]
-                        source_to_be_val_ids = [x for x in norm_source_ids if x["valid"] is None]
-                        source_identifier = {}
-                        source_identifier["valid"] = source_valid_ids
-                        source_identifier["not_valid"] = source_invalid_ids
-                        source_identifier["to_be_val"] = source_to_be_val_ids
-                        source_entity_upd_ids["identifier"] = source_identifier
-                        #source_entity_upd_ids["redis_validity_lists"] = [redis_validity_values_br, redis_validity_values_ra]
-
-                        target_entity_upd_ids = {k:v for k,v in target_entity.items() if k != "identifier"}
-                        target_valid_ids = [x for x in norm_target_ids if x["valid"] is True]
-                        target_invalid_ids = [x for x in norm_target_ids if x["valid"] is False]
-                        target_to_be_val_ids = [x for x in norm_target_ids if x["valid"] is None]
-                        target_identifier = {}
-                        target_identifier["valid"] = target_valid_ids
-                        target_identifier["not_valid"] = target_invalid_ids
-                        target_identifier["to_be_val"] = target_to_be_val_ids
-                        target_entity_upd_ids["identifier"] = target_identifier
-                        #target_entity_upd_ids["redis_validity_lists"] = [redis_validity_values_br, redis_validity_values_ra]
-
-                        # creation of a new row in meta table because there are new ids to be validated.
-                        # "any_source_id" will be chosen among the valid source entity ids, if any
-                        if source_identifier["to_be_val"]:
-                            source_tab_data = openaire_csv.csv_creator(source_entity_upd_ids) #valid_citation_ids_s --> evitare rivalidazione ?
-                            if source_tab_data:
-                                processed_source_ids = source_tab_data["id"].split(" ")
-                                all_citing_valid = processed_source_ids
-                                if all_citing_valid: # It meanst that there is at least one valid id for the citing entity
-                                    any_source_id = all_citing_valid[0]
-                                    data.append(source_tab_data) # Otherwise the row should not be included in meta tables
-
-
-                        # skip creation of a new row in meta table because there is no new id to be validated
-                        # "any_source_id" will be chosen among the valid source entity ids, if any
-                        elif source_identifier["valid"]:
-                            all_citing_valid = source_identifier["valid"]
-                            any_source_id = all_citing_valid[0]["identifier"]
-
-                        # creation of a new row in meta table because there are new ids to be validated.
-                        # "any_target_id" will be chosen among the valid target entity ids, if any
-                        if target_identifier["to_be_val"]:
-                            target_tab_data = openaire_csv.csv_creator(target_entity_upd_ids)
-                            if target_tab_data:
-                                processed_target_ids = target_tab_data["id"].split(" ")
-                                all_cited_valid = processed_target_ids
-                                if all_cited_valid:
-                                    any_target_id = all_cited_valid[0]
-                                    data.append(target_tab_data) # otherwise the row should not be included in meta tables
-
-                        # skip creation of a new row in meta table because there is no new id to be validated
-                        # "any_target_id" will be chosen among the valid source entity ids, if any
-                        elif target_identifier["valid"]:
-                            all_cited_valid = target_identifier["valid"]
-                            any_target_id = all_cited_valid[0]["identifier"]
-
-
-                    if any_source_id and any_target_id:
-                        citation = dict()
-                        citation["citing"] = any_source_id
-                        citation["referenced"] = any_target_id
-                        index_citations_to_csv.append(citation)
-        pbar.update()
-        cnt += 1
-    last_part_processed += 1
-    data, index_citations_to_csv = save_files(data, index_citations_to_csv, last_part_processed, is_last_sf=True)
-    pbar.close()
-
-def get_storage_manager(storage_path: str, redis_storage_manager: bool, testing: bool):
-    if not redis_storage_manager:
-        if storage_path:
-            if not os.path.exists(storage_path):
-            # if parent dir does not exist, it is created
-                if not os.path.exists(os.path.abspath(os.path.join(storage_path, os.pardir))):
-                    Path(os.path.abspath(os.path.join(storage_path, os.pardir))).mkdir(parents=True, exist_ok=True)
-            if storage_path.endswith(".db"):
-                storage_manager = SqliteStorageManager(storage_path)
-            elif storage_path.endswith(".json"):
-                storage_manager = InMemoryStorageManager(storage_path)
-
-        if not storage_path and not redis_storage_manager:
-            new_path_dir = os.path.join(os.getcwd(), "storage")
-            if not os.path.exists(new_path_dir):
-                os.makedirs(new_path_dir)
-            storage_manager = SqliteStorageManager(os.path.join(new_path_dir, "id_valid_dict.db"))
-    elif redis_storage_manager:
-        if testing:
-            storage_manager = RedisStorageManager(testing=True)
-        else:
-            storage_manager = RedisStorageManager(testing=False)
-    return storage_manager
-
-
-def pathoo(path:str) -> None:
-    if not os.path.exists(os.path.dirname(path)):
-        os.makedirs(os.path.dirname(path))
-
-if __name__ == '__main__':
-    arg_parser = ArgumentParser('openaire_process.py', description='This script creates CSV files from Openaire JSON files, enriching them through of a DOI-ORCID index')
-    arg_parser.add_argument('-c', '--config', dest='config', required=False,
-                            help='Configuration file path')
-    required = not any(arg in sys.argv for arg in {'--config', '-c'})
-    arg_parser.add_argument('-cf', '--openaire', dest='openaire_json_dir', required=required,
-                            help='Openaire json files directory')
-    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
-                            help='Directory where CSV will be stored')
-    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
-                            help='CSV file path containing information about publishers (id, name, prefix)')
-    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
-                            help='DOI-ORCID index filepath, to enrich data')
-    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
-                            help='A CSV filepath containing what DOI to process, not mandatory')
-    arg_parser.add_argument('-ca', '--cache', dest='cache', required=False,
-                        help='The cache file path. This file will be deleted at the end of the process')
-    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
-                            help='Show a loading bar, elapsed time and estimated time')
-    arg_parser.add_argument('-sp', '--storage_path', dest='storage_path', required=False,
-                            help='path of the file where to store data concerning validated pids information.'
-                                 'Pay attention to specify a ".db" file in case you chose the SqliteStorageManager'
-                                 'and a ".json" file if you chose InMemoryStorageManager')
-    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
-                            help='parameter to define if the script is to be run in testing mode. Pay attention:'
-                                 'by default the script is run in test modality and thus the data managed by redis, '
-                                 'stored in a specific redis db, are not retrieved nor permanently saved, since an '
-                                 'instance of a FakeRedis class is created and deleted by the end of the process.')
-    arg_parser.add_argument('-r', '--redis_storage_manager', dest='redis_storage_manager', action='store_true', required=False,
-                            help='parameter to define whether or not to use redis as storage manager. Note that by default the parameter '
-                                 'value is set to false, which means that -unless it is differently stated- the storage manager used is'
-                                 'derived by the storage filepath type (i.e.: .db or .json). The redis db used by the storage manager is the n.2')
-    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=1, type=int, help='Workers number')
-    args = arg_parser.parse_args()
-    config = args.config
-    settings = None
-    if config:
-        with open(config, encoding='utf-8') as f:
-            settings = yaml.full_load(f)
-    openaire_json_dir = settings['openaire_json_dir'] if settings else args.openaire_json_dir
-    openaire_json_dir = normalize_path(openaire_json_dir)
-    csv_dir = settings['output'] if settings else args.csv_dir
-    csv_dir = normalize_path(csv_dir)
-    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
-    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
-    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
-    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
-    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
-    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
-    cache = settings['cache_filepath'] if settings else args.cache
-    cache = normalize_path(cache) if cache else None
-    verbose = settings['verbose'] if settings else args.verbose
-    storage_path = settings['storage_path'] if settings else args.storage_path
-    storage_path = normalize_path(storage_path) if storage_path else None
-    testing = settings['testing'] if settings else args.testing
-    redis_storage_manager = settings['redis_storage_manager'] if settings else args.redis_storage_manager
-    max_workers = settings['max_workers'] if settings else args.max_workers
-
-    preprocess(openaire_json_dir=openaire_json_dir, publishers_filepath=publishers_filepath,
-               orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir, wanted_doi_filepath=wanted_doi_filepath, 
-               cache=cache, verbose=verbose, storage_path=storage_path, testing=testing, 
-               redis_storage_manager=redis_storage_manager, max_workers=max_workers)
+import functools
+import os.path
+import sys
+from tarfile import TarInfo
+
+import yaml
+from oc_ds_converter.lib.file_manager import normalize_path
+from oc_ds_converter.lib.jsonmanager import *
+from oc_ds_converter.oc_idmanager.oc_data_storage.in_memory_manager import \
+    InMemoryStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.redis_manager import \
+    RedisStorageManager
+from oc_ds_converter.oc_idmanager.oc_data_storage.sqlite_manager import \
+    SqliteStorageManager
+from oc_ds_converter.openaire.openaire_processing import *
+from pebble import ProcessFuture, ProcessPool
+from tqdm import tqdm
+from filelock import Timeout, FileLock
+
+
+def preprocess(
+        openaire_json_dir:str, publishers_filepath:str, orcid_doi_filepath:str, 
+        csv_dir:str, wanted_doi_filepath:str=None, cache:str=None, verbose:bool=False, storage_path:str = None, 
+        testing: bool = True, redis_storage_manager: bool = False, max_workers: int = 1, target=50000) -> None:
+
+    if not testing: # NON CANCELLARE FILES MA PRENDI SOLO IN CONSIDERAZIONE
+        input_dir_cont = os.listdir(openaire_json_dir)
+        els_to_be_removed = []
+        for el in input_dir_cont:
+            if el.startswith("._"):
+                els_to_be_removed.append(os.path.join(openaire_json_dir, el))
+            else:
+                if el.endswith(".tar"):
+                    base_name = el.replace('.tar', '')
+                    if [x for x in os.listdir(openaire_json_dir) if x.startswith(base_name) and x.endswith("decompr_zip_dir")]:
+                        els_to_be_removed.append(os.path.join(openaire_json_dir, el))
+
+        if els_to_be_removed: # Anziché els_to_be_removed +  os.remove(etbr), fare in modo di skippare (es. els_to_be_skipped + skip
+            # in fase di lettura dell'input) questi compressi nel processo
+            # nel caso in cui ci sia già un decompresso equivalente (per evitare di riprocessare inutilmente gli stessi dati)
+            for etbr in els_to_be_removed:
+                os.remove(etbr)
+
+
+
+    # creare cartella di output se non esiste (dove verranno salvati i csv delle tabelle di meta)
+    if not os.path.exists(csv_dir):
+        os.makedirs(csv_dir)
+
+    req_type = ".gz"
+
+    # creare cartella _citations di output se non esiste (dove verranno salvati i csv delle citazioni)
+    preprocessed_citations_dir = csv_dir + "_citations"
+    if not os.path.exists(preprocessed_citations_dir):
+        makedirs(preprocessed_citations_dir)
+    if verbose:
+        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
+            what = list()
+            if publishers_filepath:
+                what.append('publishers mapping')
+            if orcid_doi_filepath:
+                what.append('DOI-ORCID index')
+            if wanted_doi_filepath:
+                what.append('wanted DOIs CSV')
+            log = '[INFO: openaire_process] Processing: ' + '; '.join(what)
+            print(log)
+
+    
+    if verbose:
+        print(f'[INFO: openaire_process] Getting all files from {openaire_json_dir}')
+
+    all_input_tar = os.listdir(openaire_json_dir)
+    for tar in all_input_tar:
+        all_files, targz_fd = get_all_files_by_type(os.path.join(openaire_json_dir, tar), req_type, cache)
+        if not redis_storage_manager or max_workers == 1:
+            for filename in all_files:
+                get_citations_and_metadata(tar, preprocessed_citations_dir, csv_dir, filename, orcid_doi_filepath, wanted_doi_filepath, publishers_filepath, storage_path, redis_storage_manager, testing, cache, target)
+
+
+        elif redis_storage_manager or max_workers > 1:
+            with ProcessPool(max_workers=max_workers, max_tasks=1) as executor:
+                for filename in all_files:
+                    future:ProcessFuture = executor.schedule(
+                        function = get_citations_and_metadata,
+                        args=(tar, preprocessed_citations_dir, csv_dir, filename, orcid_doi_filepath, wanted_doi_filepath, publishers_filepath, storage_path, redis_storage_manager, testing, cache, target)
+                    )
+
+
+    if cache:
+        if os.path.exists(cache):
+            os.remove(cache)
+    lock_file = cache + ".lock"
+    if os.path.exists(lock_file):
+        os.remove(lock_file)
+
+    # added to avoid order-releted issues in sequential tests runs
+    if testing:
+        storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
+        storage_manager.delete_storage()
+
+
+def get_citations_and_metadata(tar: str, preprocessed_citations_dir: str, csv_dir: str, filename: str, orcid_index: str, doi_csv: str, publishers_filepath_openaire: str, storage_path: str, redis_storage_manager: bool, testing: bool, cache:str, target=50000):
+
+    storage_manager = get_storage_manager(storage_path, redis_storage_manager, testing=testing)
+
+    if cache:
+        if not cache.endswith(".json"):
+            cache = os.path.join(os.getcwd(), "cache.json")
+        else:
+            if not os.path.exists(os.path.abspath(os.path.join(cache, os.pardir))):
+                Path(os.path.abspath(os.path.join(cache, os.pardir))).mkdir(parents=True, exist_ok=True)
+    else:
+        cache = os.path.join(os.getcwd(), "cache.json")
+
+    last_part_processed = 0
+    lock = FileLock(cache + ".lock")
+    cache_dict = dict()
+    write_new = False
+
+    if os.path.exists(cache):
+        with lock:
+            with open(cache, "r", encoding="utf-8") as c:
+                try:
+                    cache_dict = json.load(c)
+                except:
+                    write_new = True
+    else:
+        write_new = True
+
+    if write_new:
+        with lock:
+            with open(cache, "w", encoding="utf-8") as c:
+                json.dump(cache_dict, c)
+
+    # skip if in cache
+    if tar in cache_dict:
+        if filename in cache_dict[tar]:
+            if cache_dict[tar][filename] == "completed":
+                return
+            else:
+                last_part_processed = cache_dict[tar][filename]
+        else:
+            filename_alt = ''
+            if '/' in filename:
+                filename_alt = filename.replace('/', '\\')
+            elif '\\' in filename:
+                filename_alt = filename.replace('\\', '/')
+            if filename_alt:
+                if filename_alt in cache_dict[tar]:
+                    if cache_dict[tar][filename_alt] == "completed":
+                        return
+                    else:
+                        last_part_processed = cache_dict[tar][filename]
+
+    openaire_csv = OpenaireProcessing(orcid_index=orcid_index, doi_csv=doi_csv, publishers_filepath_openaire=publishers_filepath_openaire, storage_manager=storage_manager, testing=testing)
+
+    index_citations_to_csv = []
+    data = []
+
+    target = target
+
+    skip_rows = target * last_part_processed
+
+    f = gzip.open(filename, 'rb')
+    source_data = f.readlines()
+    pbar = tqdm(total=len(source_data))
+    f.close()
+    filename = filename.name if isinstance(filename, TarInfo) else filename
+    filename_without_ext = filename.replace('.json', '').replace('.tar', '').replace('.gz', '')
+    filepath_ne = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}')
+    filepath_citations_ne = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}')
+
+    filepath = os.path.join(csv_dir, f'{os.path.basename(filename_without_ext)}.csv')
+    filepath_citations = os.path.join(preprocessed_citations_dir, f'{os.path.basename(filename_without_ext)}.csv')
+    pathoo(filepath)
+
+    def get_all_redis_ids_and_save_updates(sli_da):
+        all_br = []
+        all_ra = []
+        for entity in sli_da:
+
+            # start check: if line is processable
+            if entity:
+                d = json.loads(entity.decode('utf-8'))
+                if d.get("relationship"):
+                    if d.get("relationship").get("name") == "Cites":
+                        # end check: if line is processable
+
+                        ent_all_br, ent_all_ra = openaire_csv.extract_all_ids(json.loads(entity))
+                        all_br.extend(ent_all_br)
+                        all_ra.extend(ent_all_ra)
+
+        redis_validity_values_br = openaire_csv.get_reids_validity_list(all_br, "br")
+        redis_validity_values_ra = openaire_csv.get_reids_validity_list(all_ra, "ra")
+        openaire_csv.update_redis_values(redis_validity_values_br, redis_validity_values_ra)
+
+    def save_files(ent_list, citation_list, nf, is_last_sf=False):
+        if ent_list:
+            filename_str = filepath_ne+"_"+str(nf) + ".csv"
+            with open(filename_str, 'w', newline='', encoding='utf-8') as output_file:
+                dict_writer = csv.DictWriter(output_file, ent_list[0].keys(), delimiter=',', quotechar='"',
+                                             quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
+                dict_writer.writeheader()
+                dict_writer.writerows(ent_list)
+            ent_list = []
+
+        if citation_list:
+            filename_cit_str = filepath_citations_ne+"_"+str(nf) + ".csv"
+            with open(filename_cit_str, 'w', newline='', encoding='utf-8') as output_file_citations:
+                dict_writer = csv.DictWriter(output_file_citations, citation_list[0].keys(), delimiter=',',
+                                             quotechar='"', quoting=csv.QUOTE_NONNUMERIC, escapechar='\\')
+                dict_writer.writeheader()
+                dict_writer.writerows(citation_list)
+            citation_list = []
+
+        openaire_csv.memory_to_storage()
+
+        task_done(nf, is_last=is_last_sf)
+
+        return ent_list, citation_list
+
+    def task_done(file_part_number, is_last=False) -> None:
+        try:
+            if tar not in cache_dict:
+                cache_dict[tar] = dict()
+
+            if not is_last:
+                cache_dict[tar][filename] = file_part_number
+            else:
+                cache_dict[tar][filename] = "completed"
+
+            with lock:
+                with open(cache, 'r', encoding='utf-8') as aux_file:
+                    cur_cache_dict = json.load(aux_file)
+
+                    for k,v in cur_cache_dict.items():
+                        if not cache_dict.get(k) and cur_cache_dict.get(k):
+                            cache_dict[k] = v
+                        elif cache_dict[k] != v:
+                            tar_files_processed_values_dict = cache_dict[k]
+                            cur_tar_files_processed_values_dict = cur_cache_dict[k]
+
+                            for c, w in cur_tar_files_processed_values_dict.items():
+                                if tar_files_processed_values_dict.get(c) == "completed" or cur_tar_files_processed_values_dict.get(c) == "completed":
+                                    cur_tar_files_processed_values_dict[c] = "completed"
+                                elif isinstance(tar_files_processed_values_dict.get(c), int) and isinstance(cur_tar_files_processed_values_dict.get(c), int):
+                                    cur_tar_files_processed_values_dict[c] = max([tar_files_processed_values_dict.get(c), cur_tar_files_processed_values_dict.get(c)])
+                                elif isinstance(tar_files_processed_values_dict.get(c), int) or isinstance(cur_tar_files_processed_values_dict.get(c), int):
+                                    cur_tar_files_processed_values_dict[c] = tar_files_processed_values_dict.get(c) if isinstance(tar_files_processed_values_dict.get(c), int) else cur_tar_files_processed_values_dict.get(c)
+
+                            tar_files_processed_values_dict.update(cur_tar_files_processed_values_dict)
+                            cache_dict[k] = tar_files_processed_values_dict
+
+                    for k,v in cache_dict.items():
+                        if k not in cur_cache_dict:
+                            cur_cache_dict[k] = v
+
+                    for k,v in cur_cache_dict.items():
+                        if k not in cache_dict:
+                            cache_dict[k] = v
+
+                with open(cache, 'w', encoding='utf-8') as aux_file:
+                    json.dump(cache_dict, aux_file)
+
+        except Exception as e:
+            print(e)
+
+
+    start = skip_rows
+    cnt = skip_rows
+    end = start + target
+
+    if len(source_data[start:]) > target:
+        source_data_slice = source_data[start: end]
+    else:
+        source_data_slice = source_data[start:]
+
+    get_all_redis_ids_and_save_updates(source_data_slice)
+
+    for entity in source_data:
+
+        # in case the current entity is the <target>nth entity
+        if cnt == end:
+            start = cnt
+            end = start + target
+            if len(source_data[start:]) > target:
+                source_data_slice = source_data[start: end]
+            else:
+                source_data_slice = source_data[start:]
+
+            # update redis validated id list + save citation and meta file
+            get_all_redis_ids_and_save_updates(source_data_slice)
+            last_part_processed += 1
+            data, index_citations_to_csv = save_files(data, index_citations_to_csv, last_part_processed)
+
+        # real entity process
+        if entity:
+            d = json.loads(entity.decode('utf-8'))
+            if d.get("relationship"):
+                if d.get("relationship").get("name") == "Cites":
+
+                    norm_source_ids = []
+                    norm_target_ids = []
+
+                    any_source_id = ""
+                    any_target_id = ""
+
+                    source_entity = d.get("source")
+                    if source_entity:
+                        norm_source_ids = openaire_csv.get_norm_ids(source_entity['identifier'])
+                        if norm_source_ids:
+                            for e, nsi in enumerate(norm_source_ids):
+                                stored_validity = openaire_csv.validated_as(nsi)
+                                norm_source_ids[e]["valid"] = stored_validity
+
+
+                    target_entity = d.get("target")
+                    if target_entity:
+                        norm_target_ids = openaire_csv.get_norm_ids(target_entity['identifier'])
+                        if norm_target_ids:
+                            for i, nti in enumerate(norm_target_ids):
+                                stored_validity_t = openaire_csv.validated_as(nti)
+                                norm_target_ids[i]["valid"] = stored_validity_t
+
+                    # check that there is a citation we can handle (i.e.: expressed with ids we actually manage)
+                    if norm_source_ids and norm_target_ids:
+
+                        source_entity_upd_ids = {k:v for k,v in source_entity.items() if k != "identifier"}
+                        source_valid_ids = [x for x in norm_source_ids if x["valid"] is True]
+                        source_invalid_ids = [x for x in norm_source_ids if x["valid"] is False]
+                        source_to_be_val_ids = [x for x in norm_source_ids if x["valid"] is None]
+                        source_identifier = {}
+                        source_identifier["valid"] = source_valid_ids
+                        source_identifier["not_valid"] = source_invalid_ids
+                        source_identifier["to_be_val"] = source_to_be_val_ids
+                        source_entity_upd_ids["identifier"] = source_identifier
+                        #source_entity_upd_ids["redis_validity_lists"] = [redis_validity_values_br, redis_validity_values_ra]
+
+                        target_entity_upd_ids = {k:v for k,v in target_entity.items() if k != "identifier"}
+                        target_valid_ids = [x for x in norm_target_ids if x["valid"] is True]
+                        target_invalid_ids = [x for x in norm_target_ids if x["valid"] is False]
+                        target_to_be_val_ids = [x for x in norm_target_ids if x["valid"] is None]
+                        target_identifier = {}
+                        target_identifier["valid"] = target_valid_ids
+                        target_identifier["not_valid"] = target_invalid_ids
+                        target_identifier["to_be_val"] = target_to_be_val_ids
+                        target_entity_upd_ids["identifier"] = target_identifier
+                        #target_entity_upd_ids["redis_validity_lists"] = [redis_validity_values_br, redis_validity_values_ra]
+
+                        # creation of a new row in meta table because there are new ids to be validated.
+                        # "any_source_id" will be chosen among the valid source entity ids, if any
+                        if source_identifier["to_be_val"]:
+                            source_tab_data = openaire_csv.csv_creator(source_entity_upd_ids) #valid_citation_ids_s --> evitare rivalidazione ?
+                            if source_tab_data:
+                                processed_source_ids = source_tab_data["id"].split(" ")
+                                all_citing_valid = processed_source_ids
+                                if all_citing_valid: # It meanst that there is at least one valid id for the citing entity
+                                    any_source_id = all_citing_valid[0]
+                                    data.append(source_tab_data) # Otherwise the row should not be included in meta tables
+
+
+                        # skip creation of a new row in meta table because there is no new id to be validated
+                        # "any_source_id" will be chosen among the valid source entity ids, if any
+                        elif source_identifier["valid"]:
+                            all_citing_valid = source_identifier["valid"]
+                            any_source_id = all_citing_valid[0]["identifier"]
+
+                        # creation of a new row in meta table because there are new ids to be validated.
+                        # "any_target_id" will be chosen among the valid target entity ids, if any
+                        if target_identifier["to_be_val"]:
+                            target_tab_data = openaire_csv.csv_creator(target_entity_upd_ids)
+                            if target_tab_data:
+                                processed_target_ids = target_tab_data["id"].split(" ")
+                                all_cited_valid = processed_target_ids
+                                if all_cited_valid:
+                                    any_target_id = all_cited_valid[0]
+                                    data.append(target_tab_data) # otherwise the row should not be included in meta tables
+
+                        # skip creation of a new row in meta table because there is no new id to be validated
+                        # "any_target_id" will be chosen among the valid source entity ids, if any
+                        elif target_identifier["valid"]:
+                            all_cited_valid = target_identifier["valid"]
+                            any_target_id = all_cited_valid[0]["identifier"]
+
+
+                    if any_source_id and any_target_id:
+                        citation = dict()
+                        citation["citing"] = any_source_id
+                        citation["referenced"] = any_target_id
+                        index_citations_to_csv.append(citation)
+        pbar.update()
+        cnt += 1
+    last_part_processed += 1
+    data, index_citations_to_csv = save_files(data, index_citations_to_csv, last_part_processed, is_last_sf=True)
+    pbar.close()
+
+def get_storage_manager(storage_path: str, redis_storage_manager: bool, testing: bool):
+    if not redis_storage_manager:
+        if storage_path:
+            if not os.path.exists(storage_path):
+            # if parent dir does not exist, it is created
+                if not os.path.exists(os.path.abspath(os.path.join(storage_path, os.pardir))):
+                    Path(os.path.abspath(os.path.join(storage_path, os.pardir))).mkdir(parents=True, exist_ok=True)
+            if storage_path.endswith(".db"):
+                storage_manager = SqliteStorageManager(storage_path)
+            elif storage_path.endswith(".json"):
+                storage_manager = InMemoryStorageManager(storage_path)
+
+        if not storage_path and not redis_storage_manager:
+            new_path_dir = os.path.join(os.getcwd(), "storage")
+            if not os.path.exists(new_path_dir):
+                os.makedirs(new_path_dir)
+            storage_manager = SqliteStorageManager(os.path.join(new_path_dir, "id_valid_dict.db"))
+    elif redis_storage_manager:
+        if testing:
+            storage_manager = RedisStorageManager(testing=True)
+        else:
+            storage_manager = RedisStorageManager(testing=False)
+    return storage_manager
+
+
+def pathoo(path:str) -> None:
+    if not os.path.exists(os.path.dirname(path)):
+        os.makedirs(os.path.dirname(path))
+
+if __name__ == '__main__':
+    arg_parser = ArgumentParser('openaire_process.py', description='This script creates CSV files from Openaire JSON files, enriching them through of a DOI-ORCID index')
+    arg_parser.add_argument('-c', '--config', dest='config', required=False,
+                            help='Configuration file path')
+    required = not any(arg in sys.argv for arg in {'--config', '-c'})
+    arg_parser.add_argument('-cf', '--openaire', dest='openaire_json_dir', required=required,
+                            help='Openaire json files directory')
+    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
+                            help='Directory where CSV will be stored')
+    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
+                            help='CSV file path containing information about publishers (id, name, prefix)')
+    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
+                            help='DOI-ORCID index filepath, to enrich data')
+    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
+                            help='A CSV filepath containing what DOI to process, not mandatory')
+    arg_parser.add_argument('-ca', '--cache', dest='cache', required=False,
+                        help='The cache file path. This file will be deleted at the end of the process')
+    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
+                            help='Show a loading bar, elapsed time and estimated time')
+    arg_parser.add_argument('-sp', '--storage_path', dest='storage_path', required=False,
+                            help='path of the file where to store data concerning validated pids information.'
+                                 'Pay attention to specify a ".db" file in case you chose the SqliteStorageManager'
+                                 'and a ".json" file if you chose InMemoryStorageManager')
+    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
+                            help='parameter to define if the script is to be run in testing mode. Pay attention:'
+                                 'by default the script is run in test modality and thus the data managed by redis, '
+                                 'stored in a specific redis db, are not retrieved nor permanently saved, since an '
+                                 'instance of a FakeRedis class is created and deleted by the end of the process.')
+    arg_parser.add_argument('-r', '--redis_storage_manager', dest='redis_storage_manager', action='store_true', required=False,
+                            help='parameter to define whether or not to use redis as storage manager. Note that by default the parameter '
+                                 'value is set to false, which means that -unless it is differently stated- the storage manager used is'
+                                 'derived by the storage filepath type (i.e.: .db or .json). The redis db used by the storage manager is the n.2')
+    arg_parser.add_argument('-m', '--max_workers', dest='max_workers', required=False, default=1, type=int, help='Workers number')
+    args = arg_parser.parse_args()
+    config = args.config
+    settings = None
+    if config:
+        with open(config, encoding='utf-8') as f:
+            settings = yaml.full_load(f)
+    openaire_json_dir = settings['openaire_json_dir'] if settings else args.openaire_json_dir
+    openaire_json_dir = normalize_path(openaire_json_dir)
+    csv_dir = settings['output'] if settings else args.csv_dir
+    csv_dir = normalize_path(csv_dir)
+    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
+    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
+    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
+    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
+    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
+    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
+    cache = settings['cache_filepath'] if settings else args.cache
+    cache = normalize_path(cache) if cache else None
+    verbose = settings['verbose'] if settings else args.verbose
+    storage_path = settings['storage_path'] if settings else args.storage_path
+    storage_path = normalize_path(storage_path) if storage_path else None
+    testing = settings['testing'] if settings else args.testing
+    redis_storage_manager = settings['redis_storage_manager'] if settings else args.redis_storage_manager
+    max_workers = settings['max_workers'] if settings else args.max_workers
+
+    preprocess(openaire_json_dir=openaire_json_dir, publishers_filepath=publishers_filepath,
+               orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir, wanted_doi_filepath=wanted_doi_filepath, 
+               cache=cache, verbose=verbose, storage_path=storage_path, testing=testing, 
+               redis_storage_manager=redis_storage_manager, max_workers=max_workers)
```

### Comparing `oc_ds_converter-1.0.0/oc_ds_converter/run/pubmed_process.py` & `oc_ds_converter-1.0.1/oc_ds_converter/run/pubmed_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,187 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-# Copyright (c) 2023 Arianna Moretti <arianna.moretti4@unibo.it>
-#
-# Permission to use, copy, modify, and/or distribute this software for any purpose
-# with or without fee is hereby granted, provided that the above copyright notice
-# and this permission notice appear in all copies.
-#
-# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
-# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
-# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
-# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
-# SOFTWARE.
-
-import csv
-import os.path
-import sys
-from argparse import ArgumentParser
-from datetime import datetime
-from os.path import exists
-
-import pandas as pd
-import yaml
-from oc_ds_converter.lib.file_manager import normalize_path
-from oc_ds_converter.lib.jsonmanager import get_all_files_by_type
-from tqdm import tqdm
-
-from oc_ds_converter.pubmed.pubmed_processing import *
-
-
-def to_meta_file(cur_n, lines, interval, csv_dir):
-
-    if int(cur_n) != 0 and int(cur_n) % int(interval) == 0:
-        filename = "CSVFile_" + str(cur_n // interval)
-        filepath = os.path.join(csv_dir, f'{os.path.basename(filename)}.csv')
-        if exists(os.path.join(filepath)):
-            cur_datetime = datetime.now()
-            dt_string = cur_datetime.strftime("%d%m%Y_%H%M%S")
-            filepath = filepath[:-len(".csv")] + "_" + dt_string + ".csv"
-
-        with open(filepath, "w", encoding="utf8", newline="") as f_out:
-            dict_writer = csv.DictWriter(f_out, lines[0].keys(), delimiter=',', quotechar='"',
-                                         quoting=csv.QUOTE_ALL, escapechar='\\')
-            dict_writer.writeheader()
-            dict_writer.writerows(lines)
-
-        lines = []
-        return lines
-    else:
-        return lines
-
-
-def preprocess(pubmed_csv_dir:str, publishers_filepath:str, orcid_doi_filepath:str, csv_dir:str, journals_filepath:str, wanted_doi_filepath:str=None, verbose:bool=False, interval = 1000, testing=True, cache: str = None) -> None:
-    if not interval:
-        interval = 1000
-    else:
-        try:
-            interval = int(interval)
-        except:
-            interval = 1000
-
-    if not os.path.exists(csv_dir):
-        os.makedirs(csv_dir)
-    
-    filter = ["pmid", "doi", "title", "authors", "year", "journal", "references"]
-    if verbose:
-        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
-            what = list()
-            if publishers_filepath:
-                what.append('publishers mapping')
-            if orcid_doi_filepath:
-                what.append('DOI-ORCID index')
-            if wanted_doi_filepath:
-                what.append('wanted DOIs CSV')
-            log = '[INFO: pubmed_process] Processing: ' + '; '.join(what)
-            print(log)
-
-    pubmed_csv = PubmedProcessing(orcid_index=orcid_doi_filepath, doi_csv=wanted_doi_filepath, publishers_filepath_pubmed=publishers_filepath, journals_filepath=journals_filepath, testing=testing)
-    if verbose:
-        print(f'[INFO: pubmed_process] Getting all files from {pubmed_csv_dir}')
-
-
-    all_files, targz_fd = get_all_files_by_type(pubmed_csv_dir, ".csv")
-    lines = []
-    count = 0
-    skiprows = range(1, count) if count > 0 else None
-    rows_done = 0
-    if cache:
-        if not os.path.exists(cache):
-            with open(cache, 'w', encoding='utf8') as f:
-                f.write('0')
-        with open(cache, 'r', encoding='utf8') as f:
-            count = f.read().splitlines()[0]
-    dtype={'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': str, 'journal': str, 'references': str}
-    for file in all_files:
-        chunksize = 100000
-        with open(file, 'r', encoding='utf8') as f:
-            number_of_rows = sum(1 for _ in f) - 1
-        pbar = tqdm(total=number_of_rows)
-        pbar.update(count)
-        with pd.read_csv(file, usecols=filter, chunksize=chunksize, skiprows=skiprows, dtype=dtype) as reader:
-            for chunk in reader:
-                chunk.fillna("", inplace=True)
-                df_dict_list = chunk.to_dict("records")
-                filt_values = [d for d in df_dict_list if (d.get("cited_by") or d.get("references"))]
-
-                for item in filt_values:
-                    tabular_data = pubmed_csv.csv_creator(item)
-                    if tabular_data:
-                        lines.append(tabular_data)
-                        count += 1
-                        if int(count) != 0 and int(count) % int(interval) == 0:
-                            lines = to_meta_file(count, lines, interval, csv_dir)
-                            pubmed_csv.save_updated_pref_publishers_map()
-                            if cache:
-                                with open(cache, 'w', encoding='utf8') as f:
-                                    f.write(str(count + rows_done))
-                rows_done += len(chunk)
-                pbar.update(len(chunk))
-        pbar.close()
-    if len(lines) > 0:
-        count = count + (interval - (int(count) % int(interval)))
-        to_meta_file(count, lines, interval, csv_dir)
-        pubmed_csv.save_updated_pref_publishers_map()
-
-
-def pathoo(path:str) -> None:
-    if not os.path.exists(os.path.dirname(path)):
-        os.makedirs(os.path.dirname(path))
-
-if __name__ == '__main__':
-    arg_parser = ArgumentParser('pubmed_process.py', description='This script creates meta CSV files from pubmed preprocessed dump, enriching data through of a DOI-ORCID index')
-    arg_parser.add_argument('-c', '--config', dest='config', required=False,
-                            help='Configuration file path')
-    required = not any(arg in sys.argv for arg in {'--config', '-c'})
-    arg_parser.add_argument('-pm', '--pubmed', dest='pubmed_csv_dir', required=required,
-                            help='pubmed preprocessed csv files directory')
-    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
-                            help='Directory where CSV will be stored')
-    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
-                            help='CSV file path containing information about publishers (id, name, prefix, from)')
-    arg_parser.add_argument('-j', '--journals', dest='journals_filepath', required=False,
-                            help='JSON filepath containing information about the ISSN - journal names mapping')
-    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
-                            help='DOI-ORCID index filepath, to enrich data')
-    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
-                            help='A CSV filepath containing what DOI to process, not mandatory')
-    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
-                            help='Show a loading bar, elapsed time and estimated time')
-    arg_parser.add_argument('-int', '--interval', dest='interval',type=int, required=False, default=1000,
-                            help='int number of lines for each output csv. If nothing is declared, the default is 1000')
-    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
-                            help='testing flag to define what to use for data validation (fakeredis instance or real redis DB)')
-    arg_parser.add_argument('-c', '--cache', dest='cache', required=False,
-                            help='cache txt filepath')
-    args = arg_parser.parse_args()
-    config = args.config
-    settings = None
-    if config:
-        with open(config, encoding='utf-8') as f:
-            settings = yaml.full_load(f)
-    pubmed_csv_dir = settings['pubmed_csv_dir'] if settings else args.pubmed_csv_dir
-    interval = settings['interval'] if settings else args.interval
-    pubmed_csv_dir = normalize_path(pubmed_csv_dir)
-    csv_dir = settings['output'] if settings else args.csv_dir
-    csv_dir = normalize_path(csv_dir)
-    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
-    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
-    journals_filepath = settings['journals_filepath'] if settings else args.journals_filepath
-    journals_filepath = normalize_path(journals_filepath) if journals_filepath else None
-    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
-    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
-    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
-    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
-    verbose = settings['verbose'] if settings else args.verbose
-    testing = settings['testing'] if settings else args.testing
-    print("Data Preprocessing Phase: started")
-    preprocess(pubmed_csv_dir=pubmed_csv_dir, publishers_filepath=publishers_filepath, journals_filepath=journals_filepath, orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir, wanted_doi_filepath=wanted_doi_filepath, verbose=verbose, interval=interval, testing=testing, cache=args.cache)
+#!/usr/bin/python
+# -*- coding: utf-8 -*-
+# Copyright (c) 2023 Arianna Moretti <arianna.moretti4@unibo.it>
+#
+# Permission to use, copy, modify, and/or distribute this software for any purpose
+# with or without fee is hereby granted, provided that the above copyright notice
+# and this permission notice appear in all copies.
+#
+# THE SOFTWARE IS PROVIDED 'AS IS' AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+# REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
+# OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE,
+# DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
+# ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
+# SOFTWARE.
+
+import csv
+import os.path
+import sys
+from argparse import ArgumentParser
+from datetime import datetime
+from os.path import exists
+
+import pandas as pd
+import yaml
+from oc_ds_converter.lib.file_manager import normalize_path
+from oc_ds_converter.lib.jsonmanager import get_all_files_by_type
+from tqdm import tqdm
+
+from oc_ds_converter.pubmed.pubmed_processing import *
+
+
+def to_meta_file(cur_n, lines, interval, csv_dir):
+    if int(cur_n) != 0 and int(cur_n) % int(interval) == 0:
+        filename = "CSVFile_" + str(cur_n // interval)
+        filepath = os.path.join(csv_dir, f'{os.path.basename(filename)}.csv')
+        if exists(os.path.join(filepath)):
+            cur_datetime = datetime.now()
+            dt_string = cur_datetime.strftime("%d%m%Y_%H%M%S")
+            filepath = filepath[:-len(".csv")] + "_" + dt_string + ".csv"
+
+        with open(filepath, "w", encoding="utf8", newline="") as f_out:
+            dict_writer = csv.DictWriter(f_out, lines[0].keys(), delimiter=',', quotechar='"',
+                                         quoting=csv.QUOTE_ALL, escapechar='\\')
+            dict_writer.writeheader()
+            dict_writer.writerows(lines)
+
+        lines = []
+        return lines
+    else:
+        return lines
+
+
+def preprocess(pubmed_csv_dir: str, publishers_filepath: str, orcid_doi_filepath: str, csv_dir: str,
+               journals_filepath: str, wanted_doi_filepath: str = None, verbose: bool = False, interval=1000,
+               testing=True, cache: str = None) -> None:
+    if not interval:
+        interval = 1000
+    else:
+        try:
+            interval = int(interval)
+        except:
+            interval = 1000
+
+    if not os.path.exists(csv_dir):
+        os.makedirs(csv_dir)
+
+    filter = ["pmid", "doi", "title", "authors", "year", "journal", "references"]
+    if verbose:
+        if publishers_filepath or orcid_doi_filepath or wanted_doi_filepath:
+            what = list()
+            if publishers_filepath:
+                what.append('publishers mapping')
+            if orcid_doi_filepath:
+                what.append('DOI-ORCID index')
+            if wanted_doi_filepath:
+                what.append('wanted DOIs CSV')
+            log = '[INFO: pubmed_process] Processing: ' + '; '.join(what)
+            print(log)
+
+    pubmed_csv = PubmedProcessing(orcid_index=orcid_doi_filepath, doi_csv=wanted_doi_filepath,
+                                  publishers_filepath_pubmed=publishers_filepath, journals_filepath=journals_filepath,
+                                  testing=testing)
+    if verbose:
+        print(f'[INFO: pubmed_process] Getting all files from {pubmed_csv_dir}')
+
+    all_files, targz_fd = get_all_files_by_type(pubmed_csv_dir, ".csv")
+    lines = []
+    count = 0
+    skiprows = range(1, count) if count > 0 else None
+    rows_done = 0
+    if cache:
+        if not os.path.exists(cache):
+            with open(cache, 'w', encoding='utf8') as f:
+                f.write('0')
+        with open(cache, 'r', encoding='utf8') as f:
+            count = f.read().splitlines()[0]
+    dtype = {'pmid': str, 'doi': str, 'title': str, 'authors': str, 'year': str, 'journal': str, 'references': str}
+    for file in all_files:
+        chunksize = 100000
+        with open(file, 'r', encoding='utf8') as f:
+            number_of_rows = sum(1 for _ in f) - 1
+        pbar = tqdm(total=number_of_rows)
+        pbar.update(count)
+        with pd.read_csv(file, usecols=filter, chunksize=chunksize, skiprows=skiprows, dtype=dtype) as reader:
+            for chunk in reader:
+                chunk.fillna("", inplace=True)
+                df_dict_list = chunk.to_dict("records")
+                filt_values = [d for d in df_dict_list if (d.get("cited_by") or d.get("references"))]
+
+                for item in filt_values:
+                    tabular_data = pubmed_csv.csv_creator(item)
+                    if tabular_data:
+                        lines.append(tabular_data)
+                        count += 1
+                        if int(count) != 0 and int(count) % int(interval) == 0:
+                            lines = to_meta_file(count, lines, interval, csv_dir)
+                            pubmed_csv.save_updated_pref_publishers_map()
+                            if cache:
+                                with open(cache, 'w', encoding='utf8') as f:
+                                    f.write(str(count + rows_done))
+                rows_done += len(chunk)
+                pbar.update(len(chunk))
+        pbar.close()
+    if len(lines) > 0:
+        count = count + (interval - (int(count) % int(interval)))
+        to_meta_file(count, lines, interval, csv_dir)
+        pubmed_csv.save_updated_pref_publishers_map()
+
+
+def pathoo(path: str) -> None:
+    if not os.path.exists(os.path.dirname(path)):
+        os.makedirs(os.path.dirname(path))
+
+
+if __name__ == '__main__':
+    arg_parser = ArgumentParser('pubmed_process.py',
+                                description='This script creates meta CSV files from pubmed preprocessed dump, enriching data through of a DOI-ORCID index')
+    arg_parser.add_argument('-c', '--config', dest='config', required=False,
+                            help='Configuration file path')
+    required = not any(arg in sys.argv for arg in {'--config', '-c'})
+    arg_parser.add_argument('-pm', '--pubmed', dest='pubmed_csv_dir', required=required,
+                            help='pubmed preprocessed csv files directory')
+    arg_parser.add_argument('-out', '--output', dest='csv_dir', required=required,
+                            help='Directory where CSV will be stored')
+    arg_parser.add_argument('-p', '--publishers', dest='publishers_filepath', required=False,
+                            help='CSV file path containing information about publishers (id, name, prefix, from)')
+    arg_parser.add_argument('-j', '--journals', dest='journals_filepath', required=False,
+                            help='JSON filepath containing information about the ISSN - journal names mapping')
+    arg_parser.add_argument('-o', '--orcid', dest='orcid_doi_filepath', required=False,
+                            help='DOI-ORCID index filepath, to enrich data')
+    arg_parser.add_argument('-w', '--wanted', dest='wanted_doi_filepath', required=False,
+                            help='A CSV filepath containing what DOI to process, not mandatory')
+    arg_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', required=False,
+                            help='Show a loading bar, elapsed time and estimated time')
+    arg_parser.add_argument('-int', '--interval', dest='interval', type=int, required=False, default=1000,
+                            help='int number of lines for each output csv. If nothing is declared, the default is 1000')
+    arg_parser.add_argument('-t', '--testing', dest='testing', action='store_true', required=False,
+                            help='testing flag to define what to use for data validation (fakeredis instance or real redis DB)')
+    arg_parser.add_argument('-c', '--cache', dest='cache', required=False,
+                            help='cache txt filepath')
+    args = arg_parser.parse_args()
+    config = args.config
+    settings = None
+    if config:
+        with open(config, encoding='utf-8') as f:
+            settings = yaml.full_load(f)
+    pubmed_csv_dir = settings['pubmed_csv_dir'] if settings else args.pubmed_csv_dir
+    interval = settings['interval'] if settings else args.interval
+    pubmed_csv_dir = normalize_path(pubmed_csv_dir)
+    csv_dir = settings['output'] if settings else args.csv_dir
+    csv_dir = normalize_path(csv_dir)
+    publishers_filepath = settings['publishers_filepath'] if settings else args.publishers_filepath
+    publishers_filepath = normalize_path(publishers_filepath) if publishers_filepath else None
+    journals_filepath = settings['journals_filepath'] if settings else args.journals_filepath
+    journals_filepath = normalize_path(journals_filepath) if journals_filepath else None
+    orcid_doi_filepath = settings['orcid_doi_filepath'] if settings else args.orcid_doi_filepath
+    orcid_doi_filepath = normalize_path(orcid_doi_filepath) if orcid_doi_filepath else None
+    wanted_doi_filepath = settings['wanted_doi_filepath'] if settings else args.wanted_doi_filepath
+    wanted_doi_filepath = normalize_path(wanted_doi_filepath) if wanted_doi_filepath else None
+    verbose = settings['verbose'] if settings else args.verbose
+    testing = settings['testing'] if settings else args.testing
+    print("Data Preprocessing Phase: started")
+    preprocess(pubmed_csv_dir=pubmed_csv_dir, publishers_filepath=publishers_filepath,
+               journals_filepath=journals_filepath, orcid_doi_filepath=orcid_doi_filepath, csv_dir=csv_dir,
+               wanted_doi_filepath=wanted_doi_filepath, verbose=verbose, interval=interval, testing=testing,
+               cache=args.cache)
```

### Comparing `oc_ds_converter-1.0.0/PKG-INFO` & `oc_ds_converter-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,269 +1,232 @@
-Metadata-Version: 2.1
-Name: oc-ds-converter
-Version: 1.0.0
-Summary: A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta.
-License: ISC
-Author: arcangelo7
-Author-email: arcangelomas@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
-Requires-Dist: fakeredis (>=2.14.0,<3.0.0)
-Requires-Dist: filelock (>=3.12.2,<4.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: ndjson (>=0.3.1,<0.4.0)
-Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: pebble (>=5.0.3,<6.0.0)
-Requires-Dist: poetry (>=1.5.1,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: redis (>=4.5.5,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: self (>=2020.12.3,<2021.0.0)
-Requires-Dist: six (>=1.16.0,<2.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: update (>=0.0.1,<0.0.2)
-Requires-Dist: validators (>=0.20.0,<0.21.0)
-Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
-Requires-Dist: zstandard (>=0.21.0,<0.22.0)
-Description-Content-Type: text/markdown
-
-[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
-[![Run tests](https://github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/run_tests.yml)
-![Coverage](https://raw.githubusercontent.com/opencitations/ra_processor/main/test/coverage/coverage.svg)
-<!-- ![PyPI](https://img.shields.io/pypi/pyversions/oc_meta) -->
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/ra_processor)
-
-# OpenCitations Data Sources Converter
-
-This repository contains scripts for converting scholarly bibliographic metadata from various data sources into the format accepted by OpenCitations Meta. The data sources currently supported are:
-- [Crossref](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/crossref/crossref_processing.py)
-- [DataCite](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/datacite/datacite_processing.py)
-- [PubMed](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/pubmed/pubmed_processing.py)
-- [OpenAIRE](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/openaire/openaire_processing.py)
-- [JaLC](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/jalc/jalc_processing.py)
-- [mEDRA](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/medra/medra_processing.py)
-
-
-<!-- TABLE OF CONTENTS -->
-  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
-  <ol>
-    <li><a href="#about-the-project">About The Project</a></li>
-    <li><a href="#components">Software Components</a></li>
-    <li><a href="#validation">ID Validation Process</a></li>
-    <li><a href="#run">How to Run the Software</a></li>
-    <li><a href="#extend">How to Extend the Software</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contacts">Contacts</a></li>
-    <li><a href="#acknowledgements">Acknowledgements</a></li>
-    <li><a href="#references">References</a></li>
-  </ol>
-
-
-<!-- ABOUT THE PROJECT -->
-<h2 id="about-the-project"> About The Project </h2>
-
-The main function of this software is to perform a metadata crosswalk between the data sources providing bibliographic and citation data and the [OpenCitations Data Model (OCDM)](https://opencitations.net/model). At the same time, the software also handles the normalization and validation of the identifiers provided by the data source in all cases where it is not also the registration agency for those identifiers. The software generates **two main output datasets**, based on the data provided by a specific source:
-
-- **Bibliographic entities CSV tables**;
-  which are meant to be used as input for the [META software](https://github.com/opencitations/oc_meta.git), an OpenCitations tool and database for managing bibliographic entities' metadata. Example:
-
-| id                             | title                                                | author                                               | pub_date  | venue                                       | volume | issue | page   | type           | publisher                                      | editor |
-|--------------------------------|------------------------------------------------------|------------------------------------------------------|-----------|---------------------------------------------|--------|-------|--------|----------------|------------------------------------------------|--------|
-| doi:10.9799/ksfan.2012.25.1.069 | Nonthermal Sterilization and Shelf-life Extension of Seafood Products by Intense Pulsed Light Treatment | Cheigh, Chan-Ick [orcid:0000-0002-6227-4053]; Mun, Ji-Hye [orcid:0000-0002-6227-4053]; Chung, Myong-Soo | 2012-3-31 | The Korean Journal of Food And Nutrition [issn:1225-4339] | 25     | 1     | 69-76  | journal article | The Korean Society of Food and Nutrition [crossref:4768] |        |
-
-- **AnyID-to-Any-ID citations CSV tables**;
-  which will be used as input for the [INDEX software](https://github.com/opencitations/index), an OpenCitations tool and database for producing and managing citations between bibliographic entities identified by OMIDs (internal and unique identifiers assigned by OpenCitations). Example:
-
-| citing                          | cited                        |
-|---------------------------------|------------------------------|
-| doi:10.11426/nagare1970.2.4_1   | doi:10.1295/kobunshi.16.921  |
-
-
-In practice, the outputs generated by `oc_ds_converter` are used in subsequent steps of the data ingestion process within the OpenCitations infrastructure. Specifically, the metadata tables are used as input for META. The software assigns an OMID identifier to new entities and propagates an existing OMID to the entities already present in the OpenCitations databases, thereby deduplicating identical entities ingested from different data sources.
-
-Subsequently, the INDEX software, responsible for producing citation data compliant with the OpenCitations data model, takes as input the anyID-to-anyID citation tables produced by the `oc_ds_converter` software. It queries the META database to retrieve the OMID associated with each entity's identifier and produces OMID-to-OMID citations in various formats (RDF, SCHOLIX, CSV) as output.
-
-Here, a diagram of the OpenCitations ingestion workflow:
-![OpenCitations Ingestion Workflow](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/ingestion_workflow_overview.jpg)
-
-<!-- SOFTWARE COMPONENTS -->
-<h2 id="components"> Software Components </h2>
-
-The software is built upon three fundamental components, each addressing specific needs: 
-1. <a href="#mdc"> Metadata Crosswalk</a> ([oc_ds_converter](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter)) 
-2. <a href="#idv">Identifier Validation</a> ([oc_ds_converter/oc_idmanager](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter/oc_idmanager)) 
-3. <a href="#dsm">Data Storage Management</a> ([oc_ds_converter/oc_idmanager/oc_data_storage](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter/oc_idmanager/oc_data_storage))
-
-<h3 id="mdc">Metadata Crosswalk</h3>
-Within this layer, there is a specific plugin for each data source, which, in turn, contains a Python file (usually named after the data source + "_ processing.py," e.g., oc_ds_converter/datacite/datacite_processing.py). In this file, a class is defined to convert metadata provided by the specific source into metadata compliant with OCDM. For example, in the file datacite_processing.py, the class DataciteProcessing(RaProcessor) is defined, which contains the method `csv_creator(self, item: dict) -> dict`. This method is responsible for producing a dictionary of metadata representing a bibliographic entity extracted from the dump provided by DataCite. 
-<h3 id="idv"> Identifier Validation</h3>
-This software validates all identifiers not provided by the identifier registration agency itself. Currently, the identifiers handled by OpenCitations are: <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/doi.py">DOI</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/pmid.py">PMID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/pmcid.py">PMC</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/viaf.py">VIAF</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/wikidata.py">WIKIDATA</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/wikipedia.py">WIKIPEDIA</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/ror.py">ROR</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/orcid.py">ORCID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/arxiv.py">ARXIV</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/jid.py">JID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/issn.py">ISSN</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/isbn.py">ISBN</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/url.py">URL</a>. 
-
-Each identifier schema has its own class (e.g.: `PMIDManager(IdentifierManager)`, defined in `oc_ds_converter/oc_idmanager/pmid.py`), instantiated according to the model provided by the abstract class `IdentifierManager(metaclass=ABCMeta)`, defined in oc_ds_converter/oc_idmanager/base.py. 
-Each class provides methods for:
-<ol>
-  <li>normalising the id string</li>
-  <li>checking the correctness of the id syntax</li>
-  <li>verifying its existence using specific API services (if available)</li>
-</ol>
-
-<h3 id="dsm"> Data Storage Management </h3> 
-OpenCitations ds_converter currently offers three storage systems, which can be alternatively used: 
-
-* In Memory (class `InMemoryStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py)`
-* Redis (class `RedisStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`)
-* Sqlite (class `SqliteStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py`). 
-
-Each of these classes is defined as an instance of the abstract class `StorageManager(metaclass=ABCMeta)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`. 
-
-The type of storage manager used for a specific data source process can be chosen by the user (however, we suggest using the Redis storage manager). 
-An instance of the chosen storage manager will be used by all the ID Managers instantiated in the process to store validation data at the end of each data chunk management. 
-The temporary storage manager used while processing a data chunk is instead always an instance of the In-Memory storage manager (which is based on the use of a python dictionary). The reason for this choice lies in the fact that, in case of a run stop, the execution would restart processing from the beginning of the chunk that was being managed at the time of the interruption, and thus the data already memorized by a redis or sqlite storage manager would be duplicated, while the data memorized in an instance of an in-memory storage manager are just lost and reprocessed. 
-
-<!-- ID VALIDATION PROCESS -->
-<h2 id="validation">ID Validation Process</h2>
-In order to avoid redundant API checks, we rely on an ad-hoc data storage system. More in detail, in case the data source is also the id registration agency of at least a part of the identifiers provided in a data dump, we perform a full preliminary iteration of the data to store these identifiers as valid, without any further check. 
-
-![Perliminary data dump iteration](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/id_validation_pre_process_dump_iteration_diagram.png) 
-
-Subsequently, we perform another full iteration, validating all identifiers not registered by the data source itself. 
-
-![Data dump iteration for data validation](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/id_validation_process_dump_iteration_diagram.png) 
-
-Note that, to manage the large amount of data provided by each data source, the input dataset is generally divided into data chunks. As mentioned above, in order to avoid data duplication in case of a process interruption and restart, data concerning each chunk are temporarily stored in an instance of the in-memory storage manager (see InMemoryStorageManager(StorageManager) in oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py). The data stored in the temporary storage manager is transferred to the main storage manager (containing the ID validation data of the full input dataset) at the end of the chunk's process, when both the CSV tables concerning bibliographic metadata and citations are produced.
-For each encountered identifier to be validated, an ordered list of checks should be performed, stopping as soon as the validity value can be assessed:
-
-1. Search for the identifier in the in-memory storage manager, containing data concerning the current data chunk;
-2. Search for the identifier in the main storage manager, containing data concerning the whole dataset; 
-3. Search for the identifier in the OpenCitations databases, containing data of all the datasets ever ingested in OpenCitations.
-4. Use ID-schema specific API services to retrieve the validity information of the ID. 
-
-<!-- HOW TO RUN THE SOFTWARE -->
-<h2 id="run"> How to Run the Software </h2>
-
-To produce the citations and metadata CSV output from a data source, it is possible to execute its specific process by selecting the correct source from `oc_ds_converter/run/` directory. For example, the oc_ds_converter process for **JaLC** data source can be launched as follows:
-
-```
-python oc_ds_converter/run/jalc_process.py -ja /Volumes/my_disk/JALC_INPUT -out /Volumes/my_disk/JALC_OUTPUT -ca /Volumes/my_disk/JOCI_CACHE.json -r -m 3
-```
-
-This command launches a process of data conversion from the input data dump (located at `/Volumes/my_disk/JALC_INPUT`) into metadata CSV tables (stored at `/Volumes/my_disk/JALC_OUTPUT`) and citation CSV tables (stored in a directory automatically generated at `/Volumes/my_disk/JALC_OUTPUT_citations`), using up to 3 workers for the process parallelization (`-m 3`) and Redis as storage system (`-r`) . While the process is being executed, a cache file at `/Volumes/my_disk/JOCI_CACHE.json` is created and updated. 
-
-More in detail, each data source run script has a set of arguments that can be adapted to meet the peculiarities of the dataset. However, all the sources should accept a similar list of arguments: 
-
-- **'--config'**: The path to a configuration file, where the other arguments can be declared;
-- **'--input_location'**: The path to the input data;
-- **'--output_location'**: The path to the output directory where the metadata CSV files will be stored. From the name of this directory, the name of the directory where to store the citation CSV files will be derived automatically.
-- **'--publishers'**: The path to an optional support CSV file containing additional information about publishers, their crossref members and the DOI prefix they are associated with (id, name, prefix), used to enrich the metadata.
-- **'--orcid'**: The path to an optional support table mapping DOIs to ORCIDs of the publications' authors, used to enrich the metadata.
-- **'--wanted'**: The path to an optional CSV filepath containing a list of DOIs to process.
-- **'--cache'**: The cache file path, that will be automatically deleted at the end of the process.
-- **'--verbose'**: Argument which allows to declare whether a verbose description of the process execution is required. 
-- **'--storage_path'**: An argument to optionally choose the path of the file where to store data concerning validated IDs information, in case the process is executed using either an In-Memory or a Sqlite storage manager. Pay attention to specify a ".db" file in case a SqliteStorageManager is chosen and a ".json" file otherwise.
-- **'--testing'**: The parameter to define whether or not the script is to be run in testing mode.
-- **'--redis_storage_manager'**: A parameter to define whether or not to use redis as storage manager. In case Redis is not used, the storage manager type is derived by the storage path type (i.e. : In Memory storage in case the file is a JSON file, Sqlite in case of a .db file)
-- **'--max_workers'**: The integer number of workers used to run the process in parallel executions. 
-
-
-<!-- HOW TO EXTEND THE SOFTWARE -->
-<h2 id="extend"> How to Extend the Software </h2>
-
-### Manage a new Data Source
-In order to manage a new data source, two main software components need to be developed: 
-1. a script for reading the data source, extract the bibliographic entities' metadata, and produce the output tables;
-2. a script for reshaping the metadata of each bibliographic entity according to the OpenCitation data model.
-
-In addition to that, if the data source uses persistent identifiers not managed by OpenCitations yet, a new identifier manager should be developed too. 
-
-#### Data Source Reader Script 
-
-For each new data source, a python file should be added to the directory `oc_ds_converter/run/`. The file should be named after the data source, and perform the following tasks: 
-
-1. decopress and read the source dataset;
-2. manage the identifiers' validation process;
-3. extract from the source data a data structure representing each bibliographic resource;
-4. call a source-specific metadata crosswalk method to convert this data structure into an OCDM-compliant dictionary representing the bibliographic resource, to be stored as a CSV row;
-5. produce the output tables (citations and metadata)
-
-#### Metadata Crosswalk Script
-
-All source represents bibliographic records according to a specific data model, which has to be mapped into OCDM. To do so, we implement a source-specific child class of the class `RaProcessor` (defined in `oc_ds_converter/ra_processor.py`) for each new data source. The main method of all `RaProcessor` children classes is `csv_creator`, which is aimed at producing a row for an OpenCitations metadata table from a data structure representing a bibliographic entry according the source data model. As an example, see `OpenaireProcessing(RaProcessor)` class (in `oc_ds_converter/openaire/openaire_processing.py`). 
-
-
-### Add a new ID Manager
-
-For adding a new ID Manager:
-1. create a python file at `oc_ds_converter/oc_idmanager`, named after the id schema, e.g. `oc_ds_converter/oc_idmanager/viaf.py`.
-2. create a new class as an instance of the abstract class `IdentifierManager` (defined in `oc_ds_converter/oc_idmanager/base.py`), e.g.: `ViafManager(IdentifierManager)`, thus following the provided template. In particular:
-3. define all the id-schema specific required methods, i.e.: `syntax_ok`, to check whether the ID is compliant to its own schema syntax, `exists`, to check the ID's existence using the ID-specific API, `normalise`, to normalise the identifier string (for example by removing unexpected character and turing the uppercase into lowercase characters), and `is_valid`, for assessing the overall validity of the identifier.
-4. if possible, add additional ID-schema specific methods. For example, some ID schemas (such as ORCID and ISSN) are formed by following a specific check-digit mechanism, which provides a further control system to verify the ID validity: in these cases, it is possible to add also a `check_digit` method. 
-
-### Add a new Storage Manager
-
-For adding a new type of Storage Manager, i.e. relying on another storage system:
-1. create a python file at `oc_ds_converter/oc_idmanager/oc_data_storage` named after the storage system, e.g.: `oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`.
-2. create a new class as an instance of the abstract class `StorageManager` (defined in `oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`), e.g.: `RedisStorageManager(StorageManager)`, thus following the provided template. In particular:
-3. define all the storage-type-specific required methods, i.e.: `set_value`, to add a single key-value pair to the storage, `set_multi_value`, to store a list of key-value tuple pairs all at once,  `get_value`, to retrieve the value associated to a specific key, `del_value`, to delete a key-value pair, `delete_storage`, to delete all the data previously saved in the storage system, and `get_all_keys`, to retrieve the list of all the keys in the storage.
-
-### Test
-The repository is managed with [poetry](https://python-poetry.org/docs/). To activate the virtual environment:
-```
-poetry shell
-```
-To add a package as a dependency to the project:
-```
-poetry add <package>
-```
-To run all tests with poetry: 
-```
-poetry run test
-```
-To run specific tests:
-```
-python -m unittest discover -s test -p "*.py" 
-```
-
-
-<!-- LICENSE -->
-<h2 id="license">License</h2>
-
-Distributed under the ISC License. See `LICENSE` for more information.
-
-<!-- CONTACTS -->
-<h2 id="contacts">Contacts</h2>
-
-#### Authors and Current maintainers of the repository
-
-- Arianna Moretti - [@ariannamorettj](https://github.com/ariannamorettj) - arianna.moretti4@unibo.it
-- Arcangelo Massari - [@arcangelo7](https://github.com/arcangelo7) - arcangelo.massari@unibo.it
-- Elia Rizzetto - [@eliarizzetto](https://github.com/eliarizzetto) - elia.rizzetto@studio.unibo.it
-- Marta Soricetti - [@martasoricetti](https://github.com/martasoricetti) - marta.soricetti@studio.unibo.it
-
-Project Link: [https://github.com/opencitations/oc_ds_converter](https://github.com/opencitations/oc_ds_converter)
-
-
-<!-- ACKNOWLEDGEMENTS -->
-<h2 id="acknowledgements">Acknowledgements</h2>
-
-This project has been developed under the supervision of Prof. Silvio Peroni.
-
-- Silvio Peroni - [@essepuntato](https://github.com/essepuntato) - silvio.peroni@unibo.it
-
-<!-- REFERENCES -->
-<h2 id="references">References</h2>
-
-- [The OpenCitations Data Model](https://link.springer.com/chapter/10.1007/978-3-030-62466-8_28)
-- [OpenCitations Meta](https://doi.org/10.48550/arXiv.2306.16191)
-- [Metadata crosswalk for citation data production in OpenCitations](https://marketplace.sshopencloud.eu/workflow/MHwO4l)
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-
-
+[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
+[![Run tests](https://github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/run_tests.yml)
+![Coverage](https://raw.githubusercontent.com/opencitations/ra_processor/main/test/coverage/coverage.svg)
+<!-- ![PyPI](https://img.shields.io/pypi/pyversions/oc_meta) -->
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/ra_processor)
+
+# OpenCitations Data Sources Converter
+
+This repository contains scripts for converting scholarly bibliographic metadata from various data sources into the format accepted by OpenCitations Meta. The data sources currently supported are:
+- [Crossref](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/crossref/crossref_processing.py)
+- [DataCite](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/datacite/datacite_processing.py)
+- [PubMed](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/pubmed/pubmed_processing.py)
+- [OpenAIRE](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/openaire/openaire_processing.py)
+- [JaLC](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/jalc/jalc_processing.py)
+- [mEDRA](https://github.com/opencitations/oc_ds_converter/blob/658342c1921126515bc4330b8e6cfce0ead2ba48/oc_ds_converter/medra/medra_processing.py)
+
+
+<!-- TABLE OF CONTENTS -->
+  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
+  <ol>
+    <li><a href="#about-the-project">About The Project</a></li>
+    <li><a href="#components">Software Components</a></li>
+    <li><a href="#validation">ID Validation Process</a></li>
+    <li><a href="#run">How to Run the Software</a></li>
+    <li><a href="#extend">How to Extend the Software</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contacts">Contacts</a></li>
+    <li><a href="#acknowledgements">Acknowledgements</a></li>
+    <li><a href="#references">References</a></li>
+  </ol>
+
+
+<!-- ABOUT THE PROJECT -->
+<h2 id="about-the-project"> About The Project </h2>
+
+The main function of this software is to perform a metadata crosswalk between the data sources providing bibliographic and citation data and the [OpenCitations Data Model (OCDM)](https://opencitations.net/model). At the same time, the software also handles the normalization and validation of the identifiers provided by the data source in all cases where it is not also the registration agency for those identifiers. The software generates **two main output datasets**, based on the data provided by a specific source:
+
+- **Bibliographic entities CSV tables**;
+  which are meant to be used as input for the [META software](https://github.com/opencitations/oc_meta.git), an OpenCitations tool and database for managing bibliographic entities' metadata. Example:
+
+| id                             | title                                                | author                                               | pub_date  | venue                                       | volume | issue | page   | type           | publisher                                      | editor |
+|--------------------------------|------------------------------------------------------|------------------------------------------------------|-----------|---------------------------------------------|--------|-------|--------|----------------|------------------------------------------------|--------|
+| doi:10.9799/ksfan.2012.25.1.069 | Nonthermal Sterilization and Shelf-life Extension of Seafood Products by Intense Pulsed Light Treatment | Cheigh, Chan-Ick [orcid:0000-0002-6227-4053]; Mun, Ji-Hye [orcid:0000-0002-6227-4053]; Chung, Myong-Soo | 2012-3-31 | The Korean Journal of Food And Nutrition [issn:1225-4339] | 25     | 1     | 69-76  | journal article | The Korean Society of Food and Nutrition [crossref:4768] |        |
+
+- **AnyID-to-Any-ID citations CSV tables**;
+  which will be used as input for the [INDEX software](https://github.com/opencitations/index), an OpenCitations tool and database for producing and managing citations between bibliographic entities identified by OMIDs (internal and unique identifiers assigned by OpenCitations). Example:
+
+| citing                          | cited                        |
+|---------------------------------|------------------------------|
+| doi:10.11426/nagare1970.2.4_1   | doi:10.1295/kobunshi.16.921  |
+
+
+In practice, the outputs generated by `oc_ds_converter` are used in subsequent steps of the data ingestion process within the OpenCitations infrastructure. Specifically, the metadata tables are used as input for META. The software assigns an OMID identifier to new entities and propagates an existing OMID to the entities already present in the OpenCitations databases, thereby deduplicating identical entities ingested from different data sources.
+
+Subsequently, the INDEX software, responsible for producing citation data compliant with the OpenCitations data model, takes as input the anyID-to-anyID citation tables produced by the `oc_ds_converter` software. It queries the META database to retrieve the OMID associated with each entity's identifier and produces OMID-to-OMID citations in various formats (RDF, SCHOLIX, CSV) as output.
+
+Here, a diagram of the OpenCitations ingestion workflow:
+![OpenCitations Ingestion Workflow](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/ingestion_workflow_overview.jpg)
+
+<!-- SOFTWARE COMPONENTS -->
+<h2 id="components"> Software Components </h2>
+
+The software is built upon three fundamental components, each addressing specific needs: 
+1. <a href="#mdc"> Metadata Crosswalk</a> ([oc_ds_converter](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter)) 
+2. <a href="#idv">Identifier Validation</a> ([oc_ds_converter/oc_idmanager](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter/oc_idmanager)) 
+3. <a href="#dsm">Data Storage Management</a> ([oc_ds_converter/oc_idmanager/oc_data_storage](https://github.com/opencitations/oc_ds_converter/tree/297c71577232459a69ca1662011419d452971095/oc_ds_converter/oc_idmanager/oc_data_storage))
+
+<h3 id="mdc">Metadata Crosswalk</h3>
+Within this layer, there is a specific plugin for each data source, which, in turn, contains a Python file (usually named after the data source + "_ processing.py," e.g., oc_ds_converter/datacite/datacite_processing.py). In this file, a class is defined to convert metadata provided by the specific source into metadata compliant with OCDM. For example, in the file datacite_processing.py, the class DataciteProcessing(RaProcessor) is defined, which contains the method `csv_creator(self, item: dict) -> dict`. This method is responsible for producing a dictionary of metadata representing a bibliographic entity extracted from the dump provided by DataCite. 
+<h3 id="idv"> Identifier Validation</h3>
+This software validates all identifiers not provided by the identifier registration agency itself. Currently, the identifiers handled by OpenCitations are: <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/doi.py">DOI</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/pmid.py">PMID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/pmcid.py">PMC</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/viaf.py">VIAF</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/wikidata.py">WIKIDATA</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/wikipedia.py">WIKIPEDIA</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/ror.py">ROR</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/orcid.py">ORCID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/arxiv.py">ARXIV</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/jid.py">JID</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/issn.py">ISSN</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/isbn.py">ISBN</a>; <a href="https://github.com/opencitations/oc_ds_converter/blob/3bf5b93edf88c3f6cb1fe1860490533b5b9d1186/oc_ds_converter/oc_idmanager/url.py">URL</a>. 
+
+Each identifier schema has its own class (e.g.: `PMIDManager(IdentifierManager)`, defined in `oc_ds_converter/oc_idmanager/pmid.py`), instantiated according to the model provided by the abstract class `IdentifierManager(metaclass=ABCMeta)`, defined in oc_ds_converter/oc_idmanager/base.py. 
+Each class provides methods for:
+<ol>
+  <li>normalising the id string</li>
+  <li>checking the correctness of the id syntax</li>
+  <li>verifying its existence using specific API services (if available)</li>
+</ol>
+
+<h3 id="dsm"> Data Storage Management </h3> 
+OpenCitations ds_converter currently offers three storage systems, which can be alternatively used: 
+
+* In Memory (class `InMemoryStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py)`
+* Redis (class `RedisStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`)
+* Sqlite (class `SqliteStorageManager(StorageManager)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py`). 
+
+Each of these classes is defined as an instance of the abstract class `StorageManager(metaclass=ABCMeta)`, defined in `oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`. 
+
+The type of storage manager used for a specific data source process can be chosen by the user (however, we suggest using the Redis storage manager). 
+An instance of the chosen storage manager will be used by all the ID Managers instantiated in the process to store validation data at the end of each data chunk management. 
+The temporary storage manager used while processing a data chunk is instead always an instance of the In-Memory storage manager (which is based on the use of a python dictionary). The reason for this choice lies in the fact that, in case of a run stop, the execution would restart processing from the beginning of the chunk that was being managed at the time of the interruption, and thus the data already memorized by a redis or sqlite storage manager would be duplicated, while the data memorized in an instance of an in-memory storage manager are just lost and reprocessed. 
+
+<!-- ID VALIDATION PROCESS -->
+<h2 id="validation">ID Validation Process</h2>
+In order to avoid redundant API checks, we rely on an ad-hoc data storage system. More in detail, in case the data source is also the id registration agency of at least a part of the identifiers provided in a data dump, we perform a full preliminary iteration of the data to store these identifiers as valid, without any further check. 
+
+![Perliminary data dump iteration](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/id_validation_pre_process_dump_iteration_diagram.png) 
+
+Subsequently, we perform another full iteration, validating all identifiers not registered by the data source itself. 
+
+![Data dump iteration for data validation](https://github.com/ariannamorettj/OC_documents/blob/5115cf039b4baa2319c6c22cc270647861ae2f5a/id_validation_process_dump_iteration_diagram.png) 
+
+Note that, to manage the large amount of data provided by each data source, the input dataset is generally divided into data chunks. As mentioned above, in order to avoid data duplication in case of a process interruption and restart, data concerning each chunk are temporarily stored in an instance of the in-memory storage manager (see InMemoryStorageManager(StorageManager) in oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py). The data stored in the temporary storage manager is transferred to the main storage manager (containing the ID validation data of the full input dataset) at the end of the chunk's process, when both the CSV tables concerning bibliographic metadata and citations are produced.
+For each encountered identifier to be validated, an ordered list of checks should be performed, stopping as soon as the validity value can be assessed:
+
+1. Search for the identifier in the in-memory storage manager, containing data concerning the current data chunk;
+2. Search for the identifier in the main storage manager, containing data concerning the whole dataset; 
+3. Search for the identifier in the OpenCitations databases, containing data of all the datasets ever ingested in OpenCitations.
+4. Use ID-schema specific API services to retrieve the validity information of the ID. 
+
+<!-- HOW TO RUN THE SOFTWARE -->
+<h2 id="run"> How to Run the Software </h2>
+
+To produce the citations and metadata CSV output from a data source, it is possible to execute its specific process by selecting the correct source from `oc_ds_converter/run/` directory. For example, the oc_ds_converter process for **JaLC** data source can be launched as follows:
+
+```
+python oc_ds_converter/run/jalc_process.py -ja /Volumes/my_disk/JALC_INPUT -out /Volumes/my_disk/JALC_OUTPUT -ca /Volumes/my_disk/JOCI_CACHE.json -r -m 3
+```
+
+This command launches a process of data conversion from the input data dump (located at `/Volumes/my_disk/JALC_INPUT`) into metadata CSV tables (stored at `/Volumes/my_disk/JALC_OUTPUT`) and citation CSV tables (stored in a directory automatically generated at `/Volumes/my_disk/JALC_OUTPUT_citations`), using up to 3 workers for the process parallelization (`-m 3`) and Redis as storage system (`-r`) . While the process is being executed, a cache file at `/Volumes/my_disk/JOCI_CACHE.json` is created and updated. 
+
+More in detail, each data source run script has a set of arguments that can be adapted to meet the peculiarities of the dataset. However, all the sources should accept a similar list of arguments: 
+
+- **'--config'**: The path to a configuration file, where the other arguments can be declared;
+- **'--input_location'**: The path to the input data;
+- **'--output_location'**: The path to the output directory where the metadata CSV files will be stored. From the name of this directory, the name of the directory where to store the citation CSV files will be derived automatically.
+- **'--publishers'**: The path to an optional support CSV file containing additional information about publishers, their crossref members and the DOI prefix they are associated with (id, name, prefix), used to enrich the metadata.
+- **'--orcid'**: The path to an optional support table mapping DOIs to ORCIDs of the publications' authors, used to enrich the metadata.
+- **'--wanted'**: The path to an optional CSV filepath containing a list of DOIs to process.
+- **'--cache'**: The cache file path, that will be automatically deleted at the end of the process.
+- **'--verbose'**: Argument which allows to declare whether a verbose description of the process execution is required. 
+- **'--storage_path'**: An argument to optionally choose the path of the file where to store data concerning validated IDs information, in case the process is executed using either an In-Memory or a Sqlite storage manager. Pay attention to specify a ".db" file in case a SqliteStorageManager is chosen and a ".json" file otherwise.
+- **'--testing'**: The parameter to define whether or not the script is to be run in testing mode.
+- **'--redis_storage_manager'**: A parameter to define whether or not to use redis as storage manager. In case Redis is not used, the storage manager type is derived by the storage path type (i.e. : In Memory storage in case the file is a JSON file, Sqlite in case of a .db file)
+- **'--max_workers'**: The integer number of workers used to run the process in parallel executions. 
+
+
+<!-- HOW TO EXTEND THE SOFTWARE -->
+<h2 id="extend"> How to Extend the Software </h2>
+
+### Manage a new Data Source
+In order to manage a new data source, two main software components need to be developed: 
+1. a script for reading the data source, extract the bibliographic entities' metadata, and produce the output tables;
+2. a script for reshaping the metadata of each bibliographic entity according to the OpenCitation data model.
+
+In addition to that, if the data source uses persistent identifiers not managed by OpenCitations yet, a new identifier manager should be developed too. 
+
+#### Data Source Reader Script 
+
+For each new data source, a python file should be added to the directory `oc_ds_converter/run/`. The file should be named after the data source, and perform the following tasks: 
+
+1. decopress and read the source dataset;
+2. manage the identifiers' validation process;
+3. extract from the source data a data structure representing each bibliographic resource;
+4. call a source-specific metadata crosswalk method to convert this data structure into an OCDM-compliant dictionary representing the bibliographic resource, to be stored as a CSV row;
+5. produce the output tables (citations and metadata)
+
+#### Metadata Crosswalk Script
+
+All source represents bibliographic records according to a specific data model, which has to be mapped into OCDM. To do so, we implement a source-specific child class of the class `RaProcessor` (defined in `oc_ds_converter/ra_processor.py`) for each new data source. The main method of all `RaProcessor` children classes is `csv_creator`, which is aimed at producing a row for an OpenCitations metadata table from a data structure representing a bibliographic entry according the source data model. As an example, see `OpenaireProcessing(RaProcessor)` class (in `oc_ds_converter/openaire/openaire_processing.py`). 
+
+
+### Add a new ID Manager
+
+For adding a new ID Manager:
+1. create a python file at `oc_ds_converter/oc_idmanager`, named after the id schema, e.g. `oc_ds_converter/oc_idmanager/viaf.py`.
+2. create a new class as an instance of the abstract class `IdentifierManager` (defined in `oc_ds_converter/oc_idmanager/base.py`), e.g.: `ViafManager(IdentifierManager)`, thus following the provided template. In particular:
+3. define all the id-schema specific required methods, i.e.: `syntax_ok`, to check whether the ID is compliant to its own schema syntax, `exists`, to check the ID's existence using the ID-specific API, `normalise`, to normalise the identifier string (for example by removing unexpected character and turing the uppercase into lowercase characters), and `is_valid`, for assessing the overall validity of the identifier.
+4. if possible, add additional ID-schema specific methods. For example, some ID schemas (such as ORCID and ISSN) are formed by following a specific check-digit mechanism, which provides a further control system to verify the ID validity: in these cases, it is possible to add also a `check_digit` method. 
+
+### Add a new Storage Manager
+
+For adding a new type of Storage Manager, i.e. relying on another storage system:
+1. create a python file at `oc_ds_converter/oc_idmanager/oc_data_storage` named after the storage system, e.g.: `oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`.
+2. create a new class as an instance of the abstract class `StorageManager` (defined in `oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`), e.g.: `RedisStorageManager(StorageManager)`, thus following the provided template. In particular:
+3. define all the storage-type-specific required methods, i.e.: `set_value`, to add a single key-value pair to the storage, `set_multi_value`, to store a list of key-value tuple pairs all at once,  `get_value`, to retrieve the value associated to a specific key, `del_value`, to delete a key-value pair, `delete_storage`, to delete all the data previously saved in the storage system, and `get_all_keys`, to retrieve the list of all the keys in the storage.
+
+### Test
+The repository is managed with [poetry](https://python-poetry.org/docs/). To activate the virtual environment:
+```
+poetry shell
+```
+To add a package as a dependency to the project:
+```
+poetry add <package>
+```
+To run all tests with poetry: 
+```
+poetry run test
+```
+To run specific tests:
+```
+python -m unittest discover -s test -p "*.py" 
+```
+
+
+<!-- LICENSE -->
+<h2 id="license">License</h2>
+
+Distributed under the ISC License. See `LICENSE` for more information.
+
+<!-- CONTACTS -->
+<h2 id="contacts">Contacts</h2>
+
+#### Authors and Current maintainers of the repository
+
+- Arianna Moretti - [@ariannamorettj](https://github.com/ariannamorettj) - arianna.moretti4@unibo.it
+- Arcangelo Massari - [@arcangelo7](https://github.com/arcangelo7) - arcangelo.massari@unibo.it
+- Elia Rizzetto - [@eliarizzetto](https://github.com/eliarizzetto) - elia.rizzetto@studio.unibo.it
+- Marta Soricetti - [@martasoricetti](https://github.com/martasoricetti) - marta.soricetti@studio.unibo.it
+
+Project Link: [https://github.com/opencitations/oc_ds_converter](https://github.com/opencitations/oc_ds_converter)
+
+
+<!-- ACKNOWLEDGEMENTS -->
+<h2 id="acknowledgements">Acknowledgements</h2>
+
+This project has been developed under the supervision of Prof. Silvio Peroni.
+
+- Silvio Peroni - [@essepuntato](https://github.com/essepuntato) - silvio.peroni@unibo.it
+
+<!-- REFERENCES -->
+<h2 id="references">References</h2>
+
+- [The OpenCitations Data Model](https://link.springer.com/chapter/10.1007/978-3-030-62466-8_28)
+- [OpenCitations Meta](https://doi.org/10.48550/arXiv.2306.16191)
+- [Metadata crosswalk for citation data production in OpenCitations](https://marketplace.sshopencloud.eu/workflow/MHwO4l)
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+
```

#### html2text {}

```diff
@@ -1,27 +1,8 @@
-Metadata-Version: 2.1 Name: oc-ds-converter Version: 1.0.0 Summary: A library
-for converting metadata provided by various data sources, e.g. Crossref,
-DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta. License:
-ISC Author: arcangelo7 Author-email: arcangelomas@gmail.com Requires-Python:
->=3.8,<4.0 Classifier: License :: OSI Approved Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
-Requires-Dist: fakeredis (>=2.14.0,<3.0.0) Requires-Dist: filelock
-(>=3.12.2,<4.0.0) Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: ndjson
-(>=0.3.1,<0.4.0) Requires-Dist: packaging (>=23.1,<24.0) Requires-Dist: pandas
-(>=2.0.1,<3.0.0) Requires-Dist: pebble (>=5.0.3,<6.0.0) Requires-Dist: poetry
-(>=1.5.1,<2.0.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist:
-redis (>=4.5.5,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
-self (>=2020.12.3,<2021.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-
-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: update (>=0.0.1,<0.0.2) Requires-
-Dist: validators (>=0.20.0,<0.21.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
-Requires-Dist: zstandard (>=0.21.0,<0.22.0) Description-Content-Type: text/
-markdown [[https://img.shields.io/badge/powered%20by-OpenCitations-
+[[https://img.shields.io/badge/powered%20by-OpenCitations-
 %239931FC?labelColor=2D22DE]](http://opencitations.net) [![Run tests](https://
 github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/
 badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/
 run_tests.yml) ![Coverage](https://raw.githubusercontent.com/opencitations/
 ra_processor/main/test/coverage/coverage.svg) ![GitHub code size in bytes]
 (https://img.shields.io/github/languages/code-size/opencitations/ra_processor)
 # OpenCitations Data Sources Converter This repository contains scripts for
```

