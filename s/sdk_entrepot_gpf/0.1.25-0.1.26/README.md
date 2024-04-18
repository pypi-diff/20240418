# Comparing `tmp/sdk_entrepot_gpf-0.1.25.tar.gz` & `tmp/sdk_entrepot_gpf-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk_entrepot_gpf-0.1.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sdk_entrepot_gpf-0.1.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sdk_entrepot_gpf-0.1.25.tar` & `sdk_entrepot_gpf-0.1.26.tar`

### file list

```diff
@@ -1,267 +1,267 @@
--rw-r--r--   0        0        0      350 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/bug.md
--rw-r--r--   0        0        0      361 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      429 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/enhancement.md
--rw-r--r--   0        0        0      307 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/other.md
--rw-r--r--   0        0        0      370 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/quality.md
--rw-r--r--   0        0        0      383 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/tooling.md
--rw-r--r--   0        0        0      176 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/labeler.yml
--rw-r--r--   0        0        0      506 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/release.yml
--rw-r--r--   0        0        0     1412 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/ci-dev.yml
--rw-r--r--   0        0        0     1406 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/ci-prod.yml
--rw-r--r--   0        0        0      856 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0     1961 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.gitignore
--rw-r--r--   0        0        0    23461 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.pylintrc
--rw-r--r--   0        0        0      200 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.pypirc
--rw-r--r--   0        0        0     2299 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.vscode/settings.json
--rw-r--r--   0        0        0     6231 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/LICENSE
--rw-r--r--   0        0        0      134 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/MANIFEST.in
--rw-r--r--   0        0        0      533 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/README.md
--rwxr-xr-x   0        0        0      691 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/check.sh
--rw-r--r--   0        0        0        5 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/.gitignore
--rw-r--r--   0        0        0     1968 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/Dockerfile
--rw-r--r--   0        0        0      808 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/README.md
--rw-r--r--   0        0        0      248 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/config/apache/website.conf
--rw-r--r--   0        0        0      291 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/docker-compose.yml
--rw-r--r--   0        0        0       46 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/.gitignore
--rw-r--r--   0        0        0      394 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/custom.css
--rw-r--r--   0        0        0      748 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/extra.css
--rw-r--r--   0        0        0    39005 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/neoteroi.css
--rw-r--r--   0        0        0     1150 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0    12622 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.excalidraw
--rw-r--r--   0        0        0   193450 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.png
--rw-r--r--   0        0        0    15848 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/logo.png
--rw-r--r--   0        0        0     4429 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/comme-executable.md
--rw-r--r--   0        0        0     4960 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/comme-module.md
--rw-r--r--   0        0        0     6776 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/configuration.md
--rw-r--r--   0        0        0    29083 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/configuration_details.md
--rw-r--r--   0        0        0     6052 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/development.md
--rw-r--r--   0        0        0     1327 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/index.md
--rw-r--r--   0        0        0      131 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/auth.md
--rw-r--r--   0        0        0      336 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/io.md
--rw-r--r--   0        0        0      338 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/store.md
--rw-r--r--   0        0        0       68 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow.md
--rw-r--r--   0        0        0      314 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow/action.md
--rw-r--r--   0        0        0      368 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow/resolver.md
--rw-r--r--   0        0        0    11758 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/resolveurs.md
--rw-r--r--   0        0        0     5557 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_1_archive.md
--rw-r--r--   0        0        0     6731 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_2_flux_vecteur.md
--rw-r--r--   0        0        0     5137 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_3_flux_raster.md
--rw-r--r--   0        0        0     4161 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/upload_descriptor.md
--rw-r--r--   0        0        0    22205 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/workflow.md
--rw-r--r--   0        0        0     2201 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/mkdocs.yml
--rw-r--r--   0        0        0      114 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/mypy.ini
--rw-r--r--   0        0        0     1371 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/pyproject.toml
--rw-r--r--   0        0        0      689 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/Errors.py
--rw-r--r--   0        0        0       93 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__init__.py
--rw-r--r--   0        0        0    48450 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__main__.py
--rw-r--r--   0        0        0    11475 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/default.ini
--rw-r--r--   0        0        0     1202 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
--rw-r--r--   0        0        0      870 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
--rw-r--r--   0        0        0     1226 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
--rw-r--r--   0        0        0     2183 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
--rw-r--r--   0        0        0     6924 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
--rw-r--r--   0        0        0      255 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
--rwxr-xr-x   0        0        0        5 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2297 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
--rwxr-xr-x   0        0        0      655 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
--rw-r--r--   0        0        0   430828 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
--rw-r--r--   0        0        0      588 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
--rw-r--r--   0        0        0     4003 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
--rw-r--r--   0        0        0      529 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
--rw-r--r--   0        0        0       52 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
--rw-r--r--   0        0        0   991843 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
--rw-r--r--   0        0        0      525 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
--rw-r--r--   0        0        0     4391 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
--rw-r--r--   0        0        0      411 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
--rw-r--r--   0        0        0   368640 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
--rw-r--r--   0        0        0   676357 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
--rw-r--r--   0        0        0       84 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
--rw-r--r--   0        0        0     1731 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
--rw-r--r--   0        0        0     5019 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
--rw-r--r--   0        0        0    15492 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
--rw-r--r--   0        0        0     9884 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
--rw-r--r--   0        0        0    11561 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
--rw-r--r--   0        0        0     9209 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
--rw-r--r--   0        0        0    15240 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
--rw-r--r--   0        0        0     8059 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Authentifier.py
--rw-r--r--   0        0        0      274 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Errors.py
--rw-r--r--   0        0        0     1493 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Token.py
--rw-r--r--   0        0        0       46 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/__init__.py
--rw-r--r--   0        0        0     2589 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/FileHelper.py
--rw-r--r--   0        0        0     6939 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/JsonHelper.py
--rw-r--r--   0        0        0      916 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/PrintLogHelper.py
--rw-r--r--   0        0        0       59 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/__init__.py
--rw-r--r--   0        0        0    15811 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/ApiRequester.py
--rw-r--r--   0        0        0      607 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Color.py
--rw-r--r--   0        0        0     5695 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Config.py
--rw-r--r--   0        0        0     5318 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Dataset.py
--rw-r--r--   0        0        0     4143 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/DescriptorFileReader.py
--rw-r--r--   0        0        0     6878 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Errors.py
--rw-r--r--   0        0        0     2909 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/JsonConverter.py
--rw-r--r--   0        0        0     4416 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/OutputManager.py
--rw-r--r--   0        0        0     4075 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
--rw-r--r--   0        0        0       47 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/__init__.py
--rw-r--r--   0        0        0      793 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/SingleInstance.py
--rw-r--r--   0        0        0      637 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/Singleton.py
--rw-r--r--   0        0        0       33 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/__init__.py
--rw-r--r--   0        0        0        1 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/py.typed
--rw-r--r--   0        0        0     1209 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/AbstractCommonFile.py
--rw-r--r--   0        0        0     2486 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Annexe.py
--rw-r--r--   0        0        0      222 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Check.py
--rw-r--r--   0        0        0      584 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/CheckExecution.py
--rw-r--r--   0        0        0     4269 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Configuration.py
--rw-r--r--   0        0        0     3400 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Datastore.py
--rw-r--r--   0        0        0     3363 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Endpoint.py
--rw-r--r--   0        0        0      183 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Errors.py
--rw-r--r--   0        0        0     2586 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Metadata.py
--rw-r--r--   0        0        0     2140 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Offering.py
--rw-r--r--   0        0        0      332 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Permission.py
--rw-r--r--   0        0        0      231 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Processing.py
--rw-r--r--   0        0        0     2026 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/ProcessingExecution.py
--rw-r--r--   0        0        0     1005 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Static.py
--rw-r--r--   0        0        0    14998 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoreEntity.py
--rw-r--r--   0        0        0     1933 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoredData.py
--rw-r--r--   0        0        0      235 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Tms.py
--rw-r--r--   0        0        0     7270 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Upload.py
--rw-r--r--   0        0        0     1010 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/User.py
--rw-r--r--   0        0        0     1432 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/__init__.py
--rw-r--r--   0        0        0     2521 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CommentInterface.py
--rw-r--r--   0        0        0     2025 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
--rw-r--r--   0        0        0     1051 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CsfInterface.py
--rw-r--r--   0        0        0     1102 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/DownloadInterface.py
--rw-r--r--   0        0        0      805 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/EventInterface.py
--rw-r--r--   0        0        0     1262 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/FullEditInterface.py
--rw-r--r--   0        0        0      869 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/LogsInterface.py
--rw-r--r--   0        0        0     1116 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
--rw-r--r--   0        0        0      998 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
--rw-r--r--   0        0        0     2107 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/SharingInterface.py
--rw-r--r--   0        0        0     2329 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/TagInterface.py
--rw-r--r--   0        0        0       88 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/__init__.py
--rw-r--r--   0        0        0      512 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Errors.py
--rw-r--r--   0        0        0    20884 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Workflow.py
--rw-r--r--   0        0        0       40 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/__init__.py
--rw-r--r--   0        0        0     5726 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
--rw-r--r--   0        0        0     7077 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
--rw-r--r--   0        0        0     1776 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
--rw-r--r--   0        0        0     5149 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/DeleteAction.py
--rw-r--r--   0        0        0     3172 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditAction.py
--rw-r--r--   0        0        0     2551 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py
--rw-r--r--   0        0        0     6827 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/OfferingAction.py
--rw-r--r--   0        0        0     2153 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/PermissionAction.py
--rw-r--r--   0        0        0    19885 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
--rw-r--r--   0        0        0     7452 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
--rw-r--r--   0        0        0    20644 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/UploadAction.py
--rw-r--r--   0        0        0       72 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/__init__.py
--rw-r--r--   0        0        0     2267 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
--rw-r--r--   0        0        0     3389 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
--rw-r--r--   0        0        0     1933 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
--rw-r--r--   0        0        0      708 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
--rw-r--r--   0        0        0     4533 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/Errors.py
--rw-r--r--   0        0        0     6076 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
--rw-r--r--   0        0        0     3838 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
--rw-r--r--   0        0        0     5760 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
--rw-r--r--   0        0        0     1908 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
--rw-r--r--   0        0        0      110 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/__init__.py
--rw-r--r--   0        0        0      960 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/ErrorsTestCase.py
--rw-r--r--   0        0        0     1739 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/GpfTestCase.py
--rw-r--r--   0        0        0     3419 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/MainTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/__init__.py
--rw-r--r--   0        0        0      369 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_authentifier.ini
--rw-r--r--   0        0        0      308 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_overload.ini
--rw-r--r--   0        0        0      594 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_requester.ini
--rw-r--r--   0        0        0       40 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_upload.ini
--rw-r--r--   0        0        0       69 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_value_type.ini
--rw-r--r--   0        0        0      460 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
--rw-r--r--   0        0        0      305 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
--rw-r--r--   0        0        0        5 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
--rw-r--r--   0        0        0       11 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
--rw-r--r--   0        0        0        5 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
--rw-r--r--   0        0        0     2659 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/workflows/bad-workflow.jsonc
--rw-r--r--   0        0        0       53 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/FileHelper/md5.txt
--rw-r--r--   0        0        0       78 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_not_parsable.json
--rw-r--r--   0        0        0       52 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_not_valid.json
--rw-r--r--   0        0        0      108 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_parsable.json
--rw-r--r--   0        0        0      563 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema.json
--rw-r--r--   0        0        0      485 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema_invalid.json
--rw-r--r--   0        0        0       23 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/dict.json
--rw-r--r--   0        0        0       21 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/list.json
--rw-r--r--   0        0        0        2 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/not-valid.json
--rw-r--r--   0        0        0       31 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/text.txt
--rw-r--r--   0        0        0     7428 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/AuthentifierTestCase.py
--rw-r--r--   0        0        0     1187 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/TokenTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/__init__.py
--rw-r--r--   0        0        0     1060 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/FileHelperTestCase.py
--rw-r--r--   0        0        0     9967 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/JsonHelperTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/__init__.py
--rw-r--r--   0        0        0    23354 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ApiRequesterTestCase.py
--rw-r--r--   0        0        0     3599 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ConfigTestCase.py
--rw-r--r--   0        0        0     2225 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/DatasetTestCase.py
--rw-r--r--   0        0        0     3197 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ErrorsTestCase.py
--rw-r--r--   0        0        0     1202 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/JsonConverterTestCase.py
--rw-r--r--   0        0        0     1774 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/io/UploadDescriptorFileReaderTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/io/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/AbstractCommonFileTestCase.py
--rw-r--r--   0        0        0     2587 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/AnnexeTestCase.py
--rw-r--r--   0        0        0     2025 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/CheckExecutionTestCase.py
--rw-r--r--   0        0        0     7221 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ConfigurationTestCase.py
--rw-r--r--   0        0        0     4849 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/DatastoreTestCase.py
--rw-r--r--   0        0        0     5595 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/EndpointTestCase.py
--rw-r--r--   0        0        0     1152 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ErrorsTestCase.py
--rw-r--r--   0        0        0     2297 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/MetadataTestCase.py
--rw-r--r--   0        0        0     2687 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/OfferingTestCase.py
--rw-r--r--   0        0        0     4691 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ProcessingExecutionTestCase.py
--rw-r--r--   0        0        0    26065 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/StoreEntityTestCase.py
--rw-r--r--   0        0        0     3137 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/StoredDataTestCase.py
--rw-r--r--   0        0        0    11003 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/UploadTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/__init__.py
--rw-r--r--   0        0        0     5134 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CommentInterfaceTestCase.py
--rw-r--r--   0        0        0     2790 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     2536 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CsfInterfaceTestCase.py
--rw-r--r--   0        0        0     1767 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/DownloadInterfaceTestCase.py
--rw-r--r--   0        0        0     1663 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/EventInterfaceTestCase.py
--rw-r--r--   0        0        0     2326 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/FullEditInterfaceTestCase.py
--rw-r--r--   0        0        0     2243 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/PartialEditInterfaceTestCase.py
--rw-r--r--   0        0        0     1569 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/ReUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     4039 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/SharingInterfaceTestCase.py
--rw-r--r--   0        0        0     3899 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/TagInterfaceTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/__init__.py
--rw-r--r--   0        0        0    28836 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/WorkflowTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/__init__.py
--rw-r--r--   0        0        0     3595 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ActionAbstractTestCase.py
--rw-r--r--   0        0        0    10471 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ConfigurationActionTestCase.py
--rw-r--r--   0        0        0     2502 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/CopyConfigurationActionTestCase.py
--rw-r--r--   0        0        0    12123 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/DeleteActionTestCase.py
--rw-r--r--   0        0        0     5262 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditActionTestCase.py
--rw-r--r--   0        0        0     2392 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py
--rw-r--r--   0        0        0    16051 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/OfferingActionTestCase.py
--rw-r--r--   0        0        0     1547 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/PermissionActionTestCase.py
--rw-r--r--   0        0        0    24541 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ProcessingExecutionActionTestCase.py
--rw-r--r--   0        0        0    10675 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/SynchronizeOfferingActionTestCase.py
--rw-r--r--   0        0        0    26204 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/UploadActionTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/__init__.py
--rw-r--r--   0        0        0     2133 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/AbstractResolverTestCase.py
--rw-r--r--   0        0        0     2401 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DateResolverTestCase.py
--rw-r--r--   0        0        0     1124 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DictResolverTestCase.py
--rw-r--r--   0        0        0     5479 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/FileResolverTestCase.py
--rw-r--r--   0        0        0     7361 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/GlobalResolverTestCase.py
--rw-r--r--   0        0        0    15246 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/StoreEntityResolverTestCase.py
--rw-r--r--   0        0        0     2237 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/UserResolverTestCase.py
--rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/__init__.py
--rw-r--r--   0        0        0   116760 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/classes.png
--rw-r--r--   0        0        0     9175 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/classes.uxf
--rw-r--r--   0        0        0    43510 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/interfaces.png
--rw-r--r--   0        0        0     7059 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/interfaces.uxf
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0      350 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      361 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      429 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/enhancement.md
+-rw-r--r--   0        0        0      307 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/other.md
+-rw-r--r--   0        0        0      370 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/quality.md
+-rw-r--r--   0        0        0      383 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/tooling.md
+-rw-r--r--   0        0        0      176 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/labeler.yml
+-rw-r--r--   0        0        0      506 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/release.yml
+-rw-r--r--   0        0        0     1412 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/ci-dev.yml
+-rw-r--r--   0        0        0     1406 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/ci-prod.yml
+-rw-r--r--   0        0        0      856 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0     1961 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.gitignore
+-rw-r--r--   0        0        0    23461 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.pylintrc
+-rw-r--r--   0        0        0      200 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.pypirc
+-rw-r--r--   0        0        0     2299 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.vscode/settings.json
+-rw-r--r--   0        0        0     6826 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/LICENSE
+-rw-r--r--   0        0        0      134 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/MANIFEST.in
+-rw-r--r--   0        0        0      533 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/README.md
+-rwxr-xr-x   0        0        0      691 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/check.sh
+-rw-r--r--   0        0        0        5 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/.gitignore
+-rw-r--r--   0        0        0     1968 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/Dockerfile
+-rw-r--r--   0        0        0      808 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/README.md
+-rw-r--r--   0        0        0      248 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/config/apache/website.conf
+-rw-r--r--   0        0        0      291 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/docker-compose.yml
+-rw-r--r--   0        0        0       46 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/.gitignore
+-rw-r--r--   0        0        0      394 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/custom.css
+-rw-r--r--   0        0        0      748 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/extra.css
+-rw-r--r--   0        0        0    39005 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/neoteroi.css
+-rw-r--r--   0        0        0     1150 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0    12622 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.excalidraw
+-rw-r--r--   0        0        0   193450 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.png
+-rw-r--r--   0        0        0    15848 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/assets/images/logo.png
+-rw-r--r--   0        0        0     4429 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/comme-executable.md
+-rw-r--r--   0        0        0     4960 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/comme-module.md
+-rw-r--r--   0        0        0     6776 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/configuration.md
+-rw-r--r--   0        0        0    29083 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/configuration_details.md
+-rw-r--r--   0        0        0     6052 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/development.md
+-rw-r--r--   0        0        0     1327 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/index.md
+-rw-r--r--   0        0        0      131 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/auth.md
+-rw-r--r--   0        0        0      336 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/io.md
+-rw-r--r--   0        0        0      338 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/store.md
+-rw-r--r--   0        0        0       68 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow.md
+-rw-r--r--   0        0        0      314 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow/action.md
+-rw-r--r--   0        0        0      368 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow/resolver.md
+-rw-r--r--   0        0        0    11758 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/resolveurs.md
+-rw-r--r--   0        0        0     5557 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_1_archive.md
+-rw-r--r--   0        0        0     6731 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_2_flux_vecteur.md
+-rw-r--r--   0        0        0     5137 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_3_flux_raster.md
+-rw-r--r--   0        0        0     4161 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/upload_descriptor.md
+-rw-r--r--   0        0        0    22205 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/workflow.md
+-rw-r--r--   0        0        0     2201 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/mkdocs.yml
+-rw-r--r--   0        0        0      114 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/mypy.ini
+-rw-r--r--   0        0        0     1371 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0      689 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/Errors.py
+-rw-r--r--   0        0        0       93 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__init__.py
+-rw-r--r--   0        0        0    48883 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__main__.py
+-rw-r--r--   0        0        0    11504 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/default.ini
+-rw-r--r--   0        0        0     1202 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
+-rw-r--r--   0        0        0      870 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
+-rw-r--r--   0        0        0     1226 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
+-rw-r--r--   0        0        0     1968 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
+-rw-r--r--   0        0        0     6924 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
+-rw-r--r--   0        0        0      255 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
+-rwxr-xr-x   0        0        0        5 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2297 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
+-rwxr-xr-x   0        0        0      655 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
+-rw-r--r--   0        0        0   430828 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      588 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
+-rw-r--r--   0        0        0     4003 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
+-rw-r--r--   0        0        0      529 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
+-rw-r--r--   0        0        0       52 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
+-rw-r--r--   0        0        0   991843 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
+-rw-r--r--   0        0        0      525 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
+-rw-r--r--   0        0        0     4391 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
+-rw-r--r--   0        0        0      411 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
+-rw-r--r--   0        0        0   368640 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
+-rw-r--r--   0        0        0   676357 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
+-rw-r--r--   0        0        0       84 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
+-rw-r--r--   0        0        0     1731 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
+-rw-r--r--   0        0        0     5019 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
+-rw-r--r--   0        0        0    15492 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
+-rw-r--r--   0        0        0     9884 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
+-rw-r--r--   0        0        0    11561 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
+-rw-r--r--   0        0        0     9209 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
+-rw-r--r--   0        0        0    15240 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
+-rw-r--r--   0        0        0     8333 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Authentifier.py
+-rw-r--r--   0        0        0      274 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Errors.py
+-rw-r--r--   0        0        0     1493 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Token.py
+-rw-r--r--   0        0        0       46 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/__init__.py
+-rw-r--r--   0        0        0     2589 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/FileHelper.py
+-rw-r--r--   0        0        0     6939 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/JsonHelper.py
+-rw-r--r--   0        0        0      916 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/PrintLogHelper.py
+-rw-r--r--   0        0        0       59 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/__init__.py
+-rw-r--r--   0        0        0    16028 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/ApiRequester.py
+-rw-r--r--   0        0        0      607 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Color.py
+-rw-r--r--   0        0        0     5695 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Config.py
+-rw-r--r--   0        0        0     5318 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Dataset.py
+-rw-r--r--   0        0        0     4143 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/DescriptorFileReader.py
+-rw-r--r--   0        0        0     6878 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Errors.py
+-rw-r--r--   0        0        0     2909 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/JsonConverter.py
+-rw-r--r--   0        0        0     4416 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/OutputManager.py
+-rw-r--r--   0        0        0     4075 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
+-rw-r--r--   0        0        0       47 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/__init__.py
+-rw-r--r--   0        0        0      793 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/SingleInstance.py
+-rw-r--r--   0        0        0      637 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/Singleton.py
+-rw-r--r--   0        0        0       33 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/py.typed
+-rw-r--r--   0        0        0     1209 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/AbstractCommonFile.py
+-rw-r--r--   0        0        0     2486 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Annexe.py
+-rw-r--r--   0        0        0      222 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Check.py
+-rw-r--r--   0        0        0      584 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/CheckExecution.py
+-rw-r--r--   0        0        0     4269 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Configuration.py
+-rw-r--r--   0        0        0     3400 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Datastore.py
+-rw-r--r--   0        0        0     3363 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Endpoint.py
+-rw-r--r--   0        0        0      183 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Errors.py
+-rw-r--r--   0        0        0     2586 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Metadata.py
+-rw-r--r--   0        0        0     2140 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Offering.py
+-rw-r--r--   0        0        0      332 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Permission.py
+-rw-r--r--   0        0        0      231 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Processing.py
+-rw-r--r--   0        0        0     2026 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/ProcessingExecution.py
+-rw-r--r--   0        0        0     1005 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Static.py
+-rw-r--r--   0        0        0    14998 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoreEntity.py
+-rw-r--r--   0        0        0     1933 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoredData.py
+-rw-r--r--   0        0        0      235 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Tms.py
+-rw-r--r--   0        0        0     7270 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Upload.py
+-rw-r--r--   0        0        0     1010 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/User.py
+-rw-r--r--   0        0        0     1432 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/__init__.py
+-rw-r--r--   0        0        0     2521 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CommentInterface.py
+-rw-r--r--   0        0        0     2025 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
+-rw-r--r--   0        0        0     1051 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CsfInterface.py
+-rw-r--r--   0        0        0     1102 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/DownloadInterface.py
+-rw-r--r--   0        0        0      805 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/EventInterface.py
+-rw-r--r--   0        0        0     1262 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/FullEditInterface.py
+-rw-r--r--   0        0        0      869 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/LogsInterface.py
+-rw-r--r--   0        0        0     1116 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
+-rw-r--r--   0        0        0      998 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
+-rw-r--r--   0        0        0     2107 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/SharingInterface.py
+-rw-r--r--   0        0        0     2329 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/TagInterface.py
+-rw-r--r--   0        0        0       88 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/__init__.py
+-rw-r--r--   0        0        0      512 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Errors.py
+-rw-r--r--   0        0        0    20884 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Workflow.py
+-rw-r--r--   0        0        0       40 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/__init__.py
+-rw-r--r--   0        0        0     5726 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
+-rw-r--r--   0        0        0     7077 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
+-rw-r--r--   0        0        0     1776 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
+-rw-r--r--   0        0        0     5149 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/DeleteAction.py
+-rw-r--r--   0        0        0     3172 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditAction.py
+-rw-r--r--   0        0        0     2551 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py
+-rw-r--r--   0        0        0     6827 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/OfferingAction.py
+-rw-r--r--   0        0        0     2153 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/PermissionAction.py
+-rw-r--r--   0        0        0    19885 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
+-rw-r--r--   0        0        0     7452 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
+-rw-r--r--   0        0        0    22943 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/UploadAction.py
+-rw-r--r--   0        0        0       72 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2267 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
+-rw-r--r--   0        0        0     3389 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
+-rw-r--r--   0        0        0     1933 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
+-rw-r--r--   0        0        0      708 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
+-rw-r--r--   0        0        0     4533 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/Errors.py
+-rw-r--r--   0        0        0     6076 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
+-rw-r--r--   0        0        0     3838 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
+-rw-r--r--   0        0        0     5760 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
+-rw-r--r--   0        0        0     1908 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
+-rw-r--r--   0        0        0      110 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1739 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/GpfTestCase.py
+-rw-r--r--   0        0        0     3419 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/MainTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_authentifier.ini
+-rw-r--r--   0        0        0      308 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_overload.ini
+-rw-r--r--   0        0        0      594 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_requester.ini
+-rw-r--r--   0        0        0       40 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_upload.ini
+-rw-r--r--   0        0        0       69 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_value_type.ini
+-rw-r--r--   0        0        0      460 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
+-rw-r--r--   0        0        0      305 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
+-rw-r--r--   0        0        0        5 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
+-rw-r--r--   0        0        0       11 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
+-rw-r--r--   0        0        0        5 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
+-rw-r--r--   0        0        0     2659 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/workflows/bad-workflow.jsonc
+-rw-r--r--   0        0        0       53 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/FileHelper/md5.txt
+-rw-r--r--   0        0        0       78 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_not_parsable.json
+-rw-r--r--   0        0        0       52 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_not_valid.json
+-rw-r--r--   0        0        0      108 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_parsable.json
+-rw-r--r--   0        0        0      563 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema.json
+-rw-r--r--   0        0        0      485 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema_invalid.json
+-rw-r--r--   0        0        0       23 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/dict.json
+-rw-r--r--   0        0        0       21 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/list.json
+-rw-r--r--   0        0        0        2 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/not-valid.json
+-rw-r--r--   0        0        0       31 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/text.txt
+-rw-r--r--   0        0        0     7428 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/AuthentifierTestCase.py
+-rw-r--r--   0        0        0     1187 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/TokenTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/__init__.py
+-rw-r--r--   0        0        0     1060 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/FileHelperTestCase.py
+-rw-r--r--   0        0        0     9967 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/JsonHelperTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/__init__.py
+-rw-r--r--   0        0        0    23350 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ApiRequesterTestCase.py
+-rw-r--r--   0        0        0     3599 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ConfigTestCase.py
+-rw-r--r--   0        0        0     2225 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/DatasetTestCase.py
+-rw-r--r--   0        0        0     3197 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1202 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/JsonConverterTestCase.py
+-rw-r--r--   0        0        0     1774 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/UploadDescriptorFileReaderTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/AbstractCommonFileTestCase.py
+-rw-r--r--   0        0        0     2587 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/AnnexeTestCase.py
+-rw-r--r--   0        0        0     2025 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/CheckExecutionTestCase.py
+-rw-r--r--   0        0        0     7221 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ConfigurationTestCase.py
+-rw-r--r--   0        0        0     4849 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/DatastoreTestCase.py
+-rw-r--r--   0        0        0     5595 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/EndpointTestCase.py
+-rw-r--r--   0        0        0     1152 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ErrorsTestCase.py
+-rw-r--r--   0        0        0     2297 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/MetadataTestCase.py
+-rw-r--r--   0        0        0     2687 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/OfferingTestCase.py
+-rw-r--r--   0        0        0     4691 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ProcessingExecutionTestCase.py
+-rw-r--r--   0        0        0    26065 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/StoreEntityTestCase.py
+-rw-r--r--   0        0        0     3137 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/StoredDataTestCase.py
+-rw-r--r--   0        0        0    11003 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/UploadTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/__init__.py
+-rw-r--r--   0        0        0     5134 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CommentInterfaceTestCase.py
+-rw-r--r--   0        0        0     2790 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     2536 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CsfInterfaceTestCase.py
+-rw-r--r--   0        0        0     1767 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/DownloadInterfaceTestCase.py
+-rw-r--r--   0        0        0     1663 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/EventInterfaceTestCase.py
+-rw-r--r--   0        0        0     2326 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/FullEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     2243 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/PartialEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     1569 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/ReUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     4039 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/SharingInterfaceTestCase.py
+-rw-r--r--   0        0        0     3899 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/TagInterfaceTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/__init__.py
+-rw-r--r--   0        0        0    28836 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/workflow/WorkflowTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/workflow/__init__.py
+-rw-r--r--   0        0        0     3595 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ActionAbstractTestCase.py
+-rw-r--r--   0        0        0    10471 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ConfigurationActionTestCase.py
+-rw-r--r--   0        0        0     2502 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/CopyConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    12123 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/DeleteActionTestCase.py
+-rw-r--r--   0        0        0     5262 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditActionTestCase.py
+-rw-r--r--   0        0        0     2392 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    16051 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/OfferingActionTestCase.py
+-rw-r--r--   0        0        0     1547 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/PermissionActionTestCase.py
+-rw-r--r--   0        0        0    24541 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ProcessingExecutionActionTestCase.py
+-rw-r--r--   0        0        0    10675 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/SynchronizeOfferingActionTestCase.py
+-rw-r--r--   0        0        0    45012 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/UploadActionTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2133 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/AbstractResolverTestCase.py
+-rw-r--r--   0        0        0     2401 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DateResolverTestCase.py
+-rw-r--r--   0        0        0     1124 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DictResolverTestCase.py
+-rw-r--r--   0        0        0     5479 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/FileResolverTestCase.py
+-rw-r--r--   0        0        0     7361 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/GlobalResolverTestCase.py
+-rw-r--r--   0        0        0    15246 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/StoreEntityResolverTestCase.py
+-rw-r--r--   0        0        0     2237 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/UserResolverTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0   116760 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/classes.png
+-rw-r--r--   0        0        0     9175 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/classes.uxf
+-rw-r--r--   0        0        0    43510 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/interfaces.png
+-rw-r--r--   0        0        0     7059 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/interfaces.uxf
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.26/PKG-INFO
```

### Comparing `sdk_entrepot_gpf-0.1.25/.github/workflows/ci-dev.yml` & `sdk_entrepot_gpf-0.1.26/.github/workflows/ci-dev.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/.github/workflows/ci-prod.yml` & `sdk_entrepot_gpf-0.1.26/.github/workflows/ci-prod.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/.github/workflows/code-quality.yml` & `sdk_entrepot_gpf-0.1.26/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/.gitignore` & `sdk_entrepot_gpf-0.1.26/.gitignore`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/.pylintrc` & `sdk_entrepot_gpf-0.1.26/.pylintrc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/.vscode/settings.json` & `sdk_entrepot_gpf-0.1.26/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/CHANGELOG.md` & `sdk_entrepot_gpf-0.1.26/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # CHANGE LOG
 
+## v0.1.26
+
+### [Added]
+
+* UploadAction: possibilité vérification totale des fichiers livrés avant de fermer la livraison #124
+
+### [Changed]
+
+* Plus de limitation sur le type de l'upload dans le fichier upload_descriptor, permet la livraison des nouveaux types sans mise à jour du SDK. #117
+* Authentification : affichage du code TOTP en mode debug et affichage de la pile d'exécution que si l'authentification échoue complètement.
+
+### [Fixed]
+
+* Timeout mauvaise gestion valeur par défaut pour les upload de fichiers #125
+* ajout upload_partial_edit et stored_data_partial_edit #129
+
 ## v0.1.25
 
 ### [Added]
 
 * workflow : ajout de EditUsedDataConfigurationAction #105
 * DeleteAction: meilleur gestion cas sans élément à supprimé #115
 * UploadAction: les conflits de livraisons et timeout lors de la livraison ne bloquent pas la suite du traitement #119, #121
```

### Comparing `sdk_entrepot_gpf-0.1.25/LICENSE` & `sdk_entrepot_gpf-0.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/README.md` & `sdk_entrepot_gpf-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/check.sh` & `sdk_entrepot_gpf-0.1.26/check.sh`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docker/Dockerfile` & `sdk_entrepot_gpf-0.1.26/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docker/README.md` & `sdk_entrepot_gpf-0.1.26/docker/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/css/extra.css` & `sdk_entrepot_gpf-0.1.26/docs/assets/css/extra.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/css/neoteroi.css` & `sdk_entrepot_gpf-0.1.26/docs/assets/css/neoteroi.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/images/favicon.ico` & `sdk_entrepot_gpf-0.1.26/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.excalidraw` & `sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.excalidraw`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.png` & `sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/assets/images/logo.png` & `sdk_entrepot_gpf-0.1.26/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/comme-executable.md` & `sdk_entrepot_gpf-0.1.26/docs/comme-executable.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/comme-module.md` & `sdk_entrepot_gpf-0.1.26/docs/comme-module.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/configuration.md` & `sdk_entrepot_gpf-0.1.26/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/configuration_details.md` & `sdk_entrepot_gpf-0.1.26/docs/configuration_details.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/development.md` & `sdk_entrepot_gpf-0.1.26/docs/development.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/index.md` & `sdk_entrepot_gpf-0.1.26/docs/index.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/resolveurs.md` & `sdk_entrepot_gpf-0.1.26/docs/resolveurs.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/tutoriel_1_archive.md` & `sdk_entrepot_gpf-0.1.26/docs/tutoriel_1_archive.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/tutoriel_2_flux_vecteur.md` & `sdk_entrepot_gpf-0.1.26/docs/tutoriel_2_flux_vecteur.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/tutoriel_3_flux_raster.md` & `sdk_entrepot_gpf-0.1.26/docs/tutoriel_3_flux_raster.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/upload_descriptor.md` & `sdk_entrepot_gpf-0.1.26/docs/upload_descriptor.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/docs/workflow.md` & `sdk_entrepot_gpf-0.1.26/docs/workflow.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/mkdocs.yml` & `sdk_entrepot_gpf-0.1.26/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/pyproject.toml` & `sdk_entrepot_gpf-0.1.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/Errors.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__main__.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,20 +110,21 @@
         o_sub_parser = o_sub_parsers.add_parser("config", help="Configuration")
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin du fichier où sauvegarder la configuration (si null, la configuration est affichée)")
         o_sub_parser.add_argument("--section", "-s", type=str, default=None, help="Se limiter à une section")
         o_sub_parser.add_argument("--option", "-o", type=str, default=None, help="Se limiter à une option (la section doit être renseignée)")
 
         # Parser pour upload
         s_epilog_upload = """Trois types de lancement :
-        * création / mise à jour de livraison : `--file FILE [--behavior BEHAVIOR]`
+        * création / mise à jour de livraison : `--file FILE [--behavior BEHAVIOR] [--check-before-close]`
         * détail d'une livraison, optionnel ouverture ou fermeture : `--id ID [--open | --close]`
         * liste des livraisons, optionnel filtre sur l'info et tags : `[--infos INFOS] [--tags TAGS]`
         """
         o_sub_parser = o_sub_parsers.add_parser("upload", help="Livraisons", epilog=s_epilog_upload, formatter_class=argparse.RawTextHelpFormatter)
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier descriptor dont on veut effectuer la livraison)")
+        o_sub_parser.add_argument("--check-before-close", action="store_true", default=False, help="Si on vérifie l'ensemble de la livraison avant de fermer la livraison (uniquement avec --file|-f)")
         o_sub_parser.add_argument("--behavior", "-b", choices=UploadAction.BEHAVIORS, default=None, help="Action à effectuer si la livraison existe déjà (uniquement avec -f)")
         o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche la livraison demandée")
         o_exclusive = o_sub_parser.add_mutually_exclusive_group()
         o_exclusive.add_argument("--open", action="store_true", default=False, help="Rouvrir une livraison fermée (uniquement avec --id)")
         o_exclusive.add_argument("--close", action="store_true", default=False, help="Fermer une livraison ouverte (uniquement avec --id)")
         o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les livraisons selon les infos")
         o_sub_parser.add_argument("--tags", "-t", type=str, default=None, help="Filtrer les livraisons selon les tags")
@@ -338,21 +339,22 @@
         if b_res:
             Config().om.info(message_ok.format(upload=upload), green_colored=True)
         else:
             Config().om.error(message_ko.format(upload=upload))
         return b_res
 
     @staticmethod
-    def upload_from_descriptor_file(file: Union[Path, str], behavior: Optional[str] = None, datastore: Optional[str] = None) -> Dict[str, Any]:
+    def upload_from_descriptor_file(file: Union[Path, str], behavior: Optional[str] = None, datastore: Optional[str] = None, check_before_close: bool = False) -> Dict[str, Any]:
         """réalisation des livraison décrite par le fichier
 
         Args:
             file (Union[Path, str]): chemin du fichier descripteur de livraison
             behavior (Optional[str]): comportement dans le cas où une livraison de même nom existe, comportment par défaut su None
             datastore (Optional[str]): datastore à utilisé, datastore par défaut si None
+            check_before_close (bool): Vérification de l'arborescence de la livraison avant fermeture.
 
         Returns:
             Dict[str, Any]: dictionnaire avec le résultat des livraisons :
                 "ok" : liste des livraisons sans problèmes,
                 "upload_fail": dictionnaire nom livraison : erreur remonté lors de la livraison
                 "check_fail": liste des livraisons dont les vérification ont échouée
         """
@@ -366,15 +368,15 @@
         # on fait toutes les livraisons
         Config().om.info(f"LIVRAISONS : ({len(o_dfu.datasets)})", green_colored=True)
         for o_dataset in o_dfu.datasets:
             s_nom = o_dataset.upload_infos["name"]
             Config().om.info(f"{Color.BLUE} * {s_nom}{Color.END}")
             try:
                 o_ua = UploadAction(o_dataset, behavior=s_behavior)
-                o_upload = o_ua.run(datastore)
+                o_upload = o_ua.run(datastore, check_before_close=check_before_close)
                 l_uploads.append(o_upload)
             except Exception as e:
                 s_nom = o_dataset.upload_infos["name"]
                 d_upload_fail[s_nom] = e
                 Config().om.error(f"livraison {s_nom} : {e}")
 
         # vérification des livraisons
@@ -450,15 +452,15 @@
         """Création/Gestion des Livraison (Upload).
         Si un fichier descriptor est précisé, on effectue la livraison.
         Si un id est précisé, on affiche la livraison.
         Sinon on liste les Livraisons avec éventuellement des filtres.
         """
         if self.o_args.file is not None:
             # on livre les données selon le fichier descripteur donné
-            d_res = self.upload_from_descriptor_file(self.o_args.file, self.o_args.behavior, self.o_args.datastore)
+            d_res = self.upload_from_descriptor_file(self.o_args.file, self.o_args.behavior, self.o_args.datastore, self.o_args.check_before_close)
             # Affichage du bilan
             Config().om.info("-" * 100)
             if d_res["upload_fail"] or d_res["check_fail"]:
                 Config().om.info("RÉCAPITULATIF DES PROBLÈMES :", green_colored=True)
                 if d_res["upload_fail"]:
                     Config().om.error(f"{len(d_res['upload_fail'])} livraisons échoués :\n" + "\n".join([f" * {s_nom} : {e_error}" for s_nom, e_error in d_res["upload_fail"].items()]))
                 if d_res["check_fail"]:
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/default.ini` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/default.ini`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,18 @@
 datastore_get=${store_api:root_datastore}
 
 # Me
 me_get=${store_api:root_url}/users/me
 
 # Upload
 upload_list=${store_api:root_datastore}/uploads
-upload_create=${routing:upload_list}
-upload_get=${routing:upload_list}/{upload}
-upload_delete=${routing:upload_list}/{upload}
+upload_create=${upload_list}
+upload_get=${upload_list}/{upload}
+upload_delete=${upload_get}
+upload_partial_edit=${upload_get}
 upload_add_tags=${upload_get}/tags
 upload_delete_tags=${upload_get}/tags
 upload_push_data=${upload_get}/data
 upload_delete_data=${upload_get}/data
 upload_push_md5=${upload_get}/md5
 upload_delete_md5=${upload_push_md5}
 upload_close=${upload_get}/close
@@ -71,15 +72,16 @@
 upload_add_sharing=${upload_list_sharings}
 upload_remove_sharing=${upload_list_sharings}
 upload_list_events=${upload_get}/events
 
 # StoredData
 stored_data_list=${store_api:root_datastore}/stored_data
 stored_data_get=${stored_data_list}/{stored_data}
-stored_data_delete=${stored_data_list}/{stored_data}
+stored_data_delete=${stored_data_get}
+stored_data_partial_edit=${stored_data_get}
 stored_data_add_tags=${stored_data_get}/tags
 stored_data_delete_tags=${stored_data_get}/tags
 stored_data_list_comment=${stored_data_get}/comments
 stored_data_add_comment=${stored_data_list_comment}
 stored_data_edit_comment=${stored_data_list_comment}/{comment}
 stored_data_remove_comment=${stored_data_list_comment}/{comment}
 stored_data_list_sharings=${stored_data_get}/sharings
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999984929591049%*

 * *Differences: {"'properties'": "{'datasets': {'items': {'properties': {'upload_infos': {'properties': {'type': "*

 * *                 "{delete: ['enum']}}}}}}}"}*

```diff
@@ -27,19 +27,14 @@
                             "name": {
                                 "type": "string"
                             },
                             "srs": {
                                 "type": "string"
                             },
                             "type": {
-                                "enum": [
-                                    "RASTER",
-                                    "VECTOR",
-                                    "ARCHIVE"
-                                ],
                                 "type": "string"
                             }
                         },
                         "required": [
                             "description",
                             "name",
                             "srs",
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/workflow.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Authentifier.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Authentifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import time
 import traceback
 from http import HTTPStatus
 from typing import Dict, Optional
 import requests
 import pyotp
 
@@ -83,14 +84,16 @@
         """
         o_response = None
         try:
             # Préparation données d'authentification
             d_data = self.__request_params.copy()
             if self.__totp:
                 d_data["totp"] = self.__totp.now()
+                # On affiche le TOTP Code en mode debug :
+                Config().om.debug(f"TOTP code : {d_data['totp']} ({datetime.datetime.now():%H:%M:%S})")
             # Requête KeyCloak de récupération du jeton
             o_response = requests.post(
                 self.__token_url,
                 data=d_data,
                 headers={
                     "content-type": "application/x-www-form-urlencoded",
                 },
@@ -99,30 +102,32 @@
             if o_response.status_code == HTTPStatus.OK:
                 self.__last_token = Token(o_response.json())
             else:
                 # On tente de récupérer le message
                 try:
                     s_message = o_response.json()["error_description"]
                 except Exception:
-                    s_message = "pas de raison indiqué"
+                    s_message = "pas de raison indiquée"
                 raise requests.exceptions.HTTPError(f"Code retour authentification KeyCloak = {o_response.status_code} ({s_message})", response=o_response, request=o_response.request)
         except Exception as e_error:
             if isinstance(e_error, requests.exceptions.HTTPError):
                 Config().om.warning(e_error.args[0])
             else:
                 Config().om.warning("La récupération du jeton d'authentification a échoué...")
-            # Affiche la pile d'exécution
-            Config().om.debug(traceback.format_exc())
             # Une erreur s'est produite : attend un peu et relance une nouvelle fois la fonction
             if nb_attempts > 0:
                 time.sleep(self.__sec_between_attempt)
                 self.__request_new_token(nb_attempts - 1)
             # Le nombre de tentatives est atteint : comme dirait Jim, this is the end...
             else:
+                # On affiche un message d'erreur
                 Config().om.error(f"La récupération du jeton d'authentification a échoué après {self.__nb_attempts} tentatives")
+                # Affiche la pile d'exécution
+                Config().om.debug(traceback.format_exc())
+                # On propage l'erreur
                 raise e_error
 
     def get_access_token_string(self) -> str:
         """Retourne le jeton d'authentification sous forme de chaîne de caractères.
 
         Returns:
             Un jeton valide
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Token.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Token.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/FileHelper.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/FileHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/JsonHelper.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/JsonHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/PrintLogHelper.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/PrintLogHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/ApiRequester.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/ApiRequester.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,18 @@
                 # timeout selon la taille du fichier
                 d_timeout_dict: Dict[str, Optional[int]] = dict(JsonHelper.loads(s_timeout, "du dictionnaire des timeout pour {route_name}"))
                 # on rajoute une valeur par défaut
                 d_timeout_dict["-1000"] = -1000
                 i_index_timeout = max(int(i) for i in d_timeout_dict if int(i) <= file_path.stat().st_size)
                 timeout = d_timeout_dict[str(i_index_timeout)]
 
+        if timeout and timeout < 0:
+            s_default_timeout = Config().get("store_api", "timeout")
+            timeout = None if not s_default_timeout or s_default_timeout == "null" else int(s_default_timeout)
+
         # Ouverture du fichier et remplissage du tuple de fichier
         with file_path.open("rb") as o_file_binary:
             o_tuple_file = (file_path.name, o_file_binary)
             o_dict_files = {file_key: o_tuple_file}
 
             # Requête
             return self.route_request(route_name, route_params=route_params, method=method, params=params, data=data, files=o_dict_files, timeout=timeout)
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Color.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Color.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Config.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Config.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Dataset.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Dataset.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/DescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/DescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Errors.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/JsonConverter.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/JsonConverter.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/OutputManager.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/OutputManager.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/SingleInstance.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/Singleton.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/Singleton.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/AbstractCommonFile.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/AbstractCommonFile.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Annexe.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Annexe.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/CheckExecution.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/CheckExecution.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Configuration.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Configuration.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Datastore.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Datastore.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Endpoint.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Endpoint.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Metadata.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Metadata.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Offering.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Offering.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/ProcessingExecution.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/ProcessingExecution.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Static.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Static.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoreEntity.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoreEntity.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoredData.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoredData.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Upload.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Upload.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/User.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/User.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/__init__.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/__init__.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CommentInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CommentInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CsfInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CsfInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/DownloadInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/DownloadInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/EventInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/EventInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/FullEditInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/FullEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/LogsInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/LogsInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/PartialEditInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/PartialEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/SharingInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/SharingInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/TagInterface.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/TagInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Errors.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Workflow.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ActionAbstract.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ActionAbstract.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/DeleteAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/DeleteAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/OfferingAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/OfferingAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/PermissionAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/PermissionAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/UploadAction.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/UploadAction.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,49 +30,58 @@
 
     def __init__(self, dataset: Dataset, behavior: Optional[str] = None) -> None:
         self.__dataset: Dataset = dataset
         self.__upload: Optional[Upload] = None
         # On suit le comportement donnée en paramètre ou à défaut celui de la config
         self.__behavior: str = behavior if behavior is not None else Config().get_str("upload", "behavior_if_exists")
 
-    def run(self, datastore: Optional[str]) -> Upload:
+    def run(self, datastore: Optional[str], check_before_close: bool = False) -> Upload:
         """Crée la livraison décrite dans le dataset et livre les données avant de
         retourner la livraison créée.
 
         Args:
             datastore (Optional[str]): id du datastore à utiliser. Si None, le datastore sera récupéré dans la configuration.
+            check_before_close (bool): Vérification de l'arborescence de la livraison avant fermeture.
 
         Raises:
             GpfSdkError: levée si création non effectuée
 
         Returns:
             livraison créée
         """
         Config().om.info("Création et complétion d'une livraison...")
         # Création de la livraison
         self.__create_upload(datastore)
 
+        if not self.upload:
+            raise GpfSdkError("Erreur à la création de la livraison.")
         # Cas livraison fermé = déjà traité : on sort
-        if self.upload and not self.upload.is_open():
+        if not self.upload.is_open():
             return self.upload
 
         # Ajout des tags
         self.__add_tags()
         # Ajout des commentaires
         self.__add_comments()
-        # Envoie des fichiers de données
-        self.__push_data_files()
-        # Envoie des fichiers md5
-        self.__push_md5_files()
+        # Envoie des fichiers de données (pas de vérification sur les problèmes de livraison si check_before_close)
+        self.__push_data_files(not check_before_close)
+        # Envoie des fichiers md5 (pas de vérification sur les problèmes de livraison si check_before_close)
+        self.__push_md5_files(not check_before_close)
+        if check_before_close:
+            Config().om.info(f"Livraison {self.upload}: vérification de l'arborescent avant livraison ...")
+            # vérification de la livraison des fichiers de données + ficher md5
+            l_error = self.__check_file_uploaded(list(self.__dataset.data_files.items()) + [(p_file, "") for p_file in self.__dataset.md5_files])
+            if l_error:
+                raise UploadFileError(f"Livraison {self.upload['name']} : Problème de livraison pour {len(l_error)} fichiers. Il faut relancer la livraison.", l_error)
         # Fermeture de la livraison
         self.__close()
         # Affiche et retourne la livraison
         if self.upload is not None:
             # Affichage
-            Config().om.info(f"Livraison créée et complétée : {self.__upload}")
+            Config().om.info(f"Livraison créée et complétée : {self.upload}")
             Config().om.info("Création et complétion d'une livraison : terminé")
             # Retour
             return self.upload
         # On ne devrait pas arriver ici...
         raise GpfSdkError("Erreur à la création de la livraison.")
 
     def __create_upload(self, datastore: Optional[str]) -> None:
@@ -109,70 +118,81 @@
         else:
             # Si la livraison est nulle, on en crée une nouvelle (on utilise les champs de "upload_infos" du dataset)
             self.__upload = Upload.api_create(self.__dataset.upload_infos, route_params={"datastore": datastore})
             Config().om.info(f"Livraison {self.__upload['name']} créée avec succès.")
 
     def __add_tags(self) -> None:
         """Ajoute les tags."""
-        if self.__upload is not None and self.__dataset.tags is not None:
+        if self.__upload is not None and self.__dataset.tags:
             Config().om.info(f"Livraison {self.__upload['name']} : ajout des {len(self.__dataset.tags)} tags...")
             self.__upload.api_add_tags(self.__dataset.tags)
             Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.tags)} tags ont été ajoutés avec succès.")
 
     def __add_comments(self) -> None:
         """Ajoute les commentaires."""
         if self.__upload is not None:
             Config().om.info(f"Livraison {self.__upload['name']} : ajout des {len(self.__dataset.comments)} commentaires...")
             l_actual_comments = [d_comment["text"] for d_comment in self.__upload.api_list_comments() if d_comment]
             for s_comment in self.__dataset.comments:
                 if s_comment not in l_actual_comments:
                     self.__upload.api_add_comment({"text": s_comment})
             Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.comments)} commentaires ont été ajoutés avec succès.")
 
-    def __push_data_files(self) -> None:
-        """Téléverse les fichiers de données (listés dans le dataset)."""
+    def __push_data_files(self, check_conflict: bool = True) -> None:
+        """Téléverse les fichiers de données (listés dans le dataset).
+
+        Args:
+            check_conflict (bool): Si une vérification de la bonne livraison des fichier en conflict ou en timeout est lancée.
+        """
         if self.__upload is not None:
             # Liste les fichiers déjà téléversés sur l'entrepôt et récupère leur taille
             Config().om.info(f"Livraison {self.__upload['name']} : récupération de l'arborescence des données déjà téléversées...")
             i_file_upload = self.__push_files(
                 list(self.__dataset.data_files.items()),
                 self.__upload.api_push_data_file,
                 self.__upload.api_delete_data_file,
+                check_conflict,
             )
 
-            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.data_files)} fichiers de données ont été ajoutés avec succès. ({i_file_upload} livrer lors de ce traitement)")
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.data_files)} fichiers de données ont été ajoutés avec succès. ({i_file_upload} livré(s) lors de ce traitement)")
 
-    def __push_md5_files(self) -> None:
-        """Téléverse les fichiers de clefs (listés dans le dataset)."""
+    def __push_md5_files(self, check_conflict: bool = True) -> None:
+        """Téléverse les fichiers de clefs (listés dans le dataset).
+
+        Args:
+            check_conflict (bool): Si une vérification de la bonne livraison des fichier en conflict ou en timeout est lancée..
+        """
         if self.__upload is not None:
             i_file_upload = self.__push_files(
                 [(p_file, "") for p_file in self.__dataset.md5_files],
                 self.__normalise_api_push_md5_file,
                 self.__upload.api_delete_md5_file,
+                check_conflict,
             )
-            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.md5_files)} fichiers md5 ont été ajoutés avec succès. ({i_file_upload} livrer lors de ce traitement)")
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.md5_files)} fichiers md5 ont été ajoutés avec succès. ({i_file_upload} livré(s) lors de ce traitement)")
 
     def __normalise_api_push_md5_file(self, path: Path, nom: str) -> None:
         """fonction cachant api_push_md5_file pour avoir une fonction ayant les même entrées que api_push_data_file, utilisé comme paramétre de __push_files
 
         Args:
             path (Path): chemin le la chef MD5
             nom (str): non du ficher md5
         """
         if self.__upload is None:
             raise GpfSdkError(f"Aucune livraison de définie - impossible de livrer {nom}")
         self.__upload.api_push_md5_file(path)
 
-    def __push_files(self, l_files: List[Tuple[Path, str]], f_api_push: Callable[[Path, str], None], f_api_delete: Callable[[str], None]) -> int:
+    def __push_files(self, l_files: List[Tuple[Path, str]], f_api_push: Callable[[Path, str], None], f_api_delete: Callable[[str], None], check_conflict: bool = True) -> int:
         """pousse un ficher de données ou un ficher md5 sur le store. Gére la reprise de Livraison et les conflicts lors de la livraison.
 
         Args:
             l_files (List[Tuple[Path, str]]): liste de tuple Path du ficher à livre, nom du ficher sous la gpf
             f_api_push (Callable[[Path, str], None]): fonction pour livrer les données
             f_api_delete (Callable[[str], None]): fonction pour supprimé les données si livrer partiellement.
+            check_conflict (bool): Si une vérification de la bonne livraison des fichier en conflict ou en timeout est lancée..
 
         Returns:
             int: nombre de ficher réellement téléverser durant l'action
         """
         if self.__upload is None:
             raise GpfSdkError("Aucune livraison de définie")
         # Liste les fichiers téléversés sur l'entrepôt et récupère leur taille
@@ -200,26 +220,41 @@
             try:
                 # livraison du fichier
                 f_api_push(p_file_path, s_api_path)
                 i_file_upload += 1
                 Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: terminé")
             except requests.Timeout:
                 Config().om.warning(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: timeout.")
-                l_conflict.append((p_file_path, s_data_api_path))
+                l_conflict.append((p_file_path, s_api_path))
             except ConflictError:
                 Config().om.warning(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: conflict.")
-                l_conflict.append((p_file_path, s_data_api_path))
-        if l_conflict:
+                l_conflict.append((p_file_path, s_api_path))
+        if not check_conflict and l_conflict:
+            # pas de vérification des conflicts
+            Config().om.info(f"Livraison {self.__upload}: {len(l_conflict)} fichiers en conflict : " + "\n * ".join([s_data_api_path for (p_file_path, s_data_api_path) in l_conflict]))
+        elif l_conflict:
+            # vérification des fichiers en conflict
             Config().om.info(f"Livraison {self.__upload}: {len(l_conflict)} fichiers en conflict, vérification de leur livraisons...")
-            l_error = self._check_file_uploaded(l_conflict)
+            l_error = self.__check_file_uploaded(l_conflict)
             if l_error:
                 raise UploadFileError(f"Livraison {self.__upload['name']} : Problème de livraison pour {len(l_error)} fichiers. Il faut relancer la livraison.", l_error)
         return i_file_upload
 
-    def _check_file_uploaded(self, l_files: List[Tuple[Path, str]]) -> List[Tuple[Path, str]]:
+    def __check_file_uploaded(self, l_files: List[Tuple[Path, str]]) -> List[Tuple[Path, str]]:
+        """vérifie si les fichiers donnée en entrée soit bien livrer
+
+        Args:
+            l_files (List[Tuple[Path, str]]): liste des ficher à vérifier (path du fichier, chemin du fichier sur la GPF)
+
+        Raises:
+            GpfSdkError: _description_
+
+        Returns:
+            List[Tuple[Path, str]]: liste des fichiers en erreur (path du fichier, chemin du fichier sur la GPF)
+        """
         if self.__upload is None:
             raise GpfSdkError("Aucune livraison de définie")
         # on recharge la l'arborescence
         l_arborescence = self.__upload.api_tree()
         d_destination_taille = UploadAction.parse_tree(l_arborescence)
         l_error: List[Tuple[Path, str]] = []
         # vérifications
```

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DateResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DateResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DictResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DictResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/Errors.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/FileResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/FileResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/UserResolver.py` & `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/UserResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/GpfTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/GpfTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/MainTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/MainTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_conf/test_requester.ini` & `sdk_entrepot_gpf-0.1.26/tests/_conf/test_requester.ini`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_data/workflows/bad-workflow.jsonc` & `sdk_entrepot_gpf-0.1.26/tests/_data/workflows/bad-workflow.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema.json` & `sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/auth/AuthentifierTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/auth/AuthentifierTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/auth/TokenTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/auth/TokenTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/helper/FileHelperTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/helper/FileHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/helper/JsonHelperTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/helper/JsonHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/ApiRequesterTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/ApiRequesterTestCase.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         o_mock_stat.st_size = 10
         # pas de timeout
         with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
             with patch.object(Path, "stat", return_value=o_mock_stat):
                 with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
                     ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
                     o_mock_open.assert_called_once_with("rb")
-                    o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=-1000)
+                    o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=600)
         o_mock_stat.reset_mock()
 
         # timeout None
         for s_route_name in ["test_upload_none_1", "test_upload_none_2", "test_upload_none_3"]:
             with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
                 with patch.object(Path, "stat", return_value=o_mock_stat):
                     with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
@@ -417,15 +417,15 @@
                     ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
                     o_mock_open.assert_called_once_with("rb")
                     o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=60)
         o_mock_stat.reset_mock()
 
         # timeout selon taille du fichier
         s_route_name = "test_upload_variable"
-        for i_taille_ficher, i_timeout in [(1, -1000), (15, 15), (16, 15), (35, 30), (65, None), (70, 70), (700000, 70)]:
+        for i_taille_ficher, i_timeout in [(1, 600), (15, 15), (16, 15), (35, 30), (65, None), (70, 70), (700000, 70)]:
             o_mock_stat.st_size = i_taille_ficher
             with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
                 with patch.object(Path, "stat", return_value=o_mock_stat):
                     with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
                         ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
                         o_mock_open.assert_called_once_with("rb")
                         o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=i_timeout)
```

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/ConfigTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/ConfigTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/DatasetTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/DatasetTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/JsonConverterTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/JsonConverterTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/io/UploadDescriptorFileReaderTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/io/UploadDescriptorFileReaderTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/AbstractCommonFileTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/AbstractCommonFileTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/AnnexeTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/AnnexeTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/CheckExecutionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/CheckExecutionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/ConfigurationTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/ConfigurationTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/DatastoreTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/DatastoreTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/EndpointTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/EndpointTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/MetadataTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/MetadataTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/OfferingTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/OfferingTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/ProcessingExecutionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/ProcessingExecutionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/StoreEntityTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/StoreEntityTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/StoredDataTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/StoredDataTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/UploadTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/UploadTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/CommentInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/CommentInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/CsfInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/CsfInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/DownloadInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/DownloadInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/EventInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/EventInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/FullEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/FullEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/PartialEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/PartialEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/ReUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/ReUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/SharingInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/SharingInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/store/interface/TagInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/store/interface/TagInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/WorkflowTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/WorkflowTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ActionAbstractTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ActionAbstractTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/CopyConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/CopyConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/DeleteActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/DeleteActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/OfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/OfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/PermissionActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/PermissionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ProcessingExecutionActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ProcessingExecutionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/action/SynchronizeOfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/action/SynchronizeOfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/AbstractResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/AbstractResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DateResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DateResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DictResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DictResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/FileResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/FileResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/GlobalResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/GlobalResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/StoreEntityResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/StoreEntityResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/UserResolverTestCase.py` & `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/UserResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/uml/classes.png` & `sdk_entrepot_gpf-0.1.26/uml/classes.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/uml/classes.uxf` & `sdk_entrepot_gpf-0.1.26/uml/classes.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/uml/interfaces.png` & `sdk_entrepot_gpf-0.1.26/uml/interfaces.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/uml/interfaces.uxf` & `sdk_entrepot_gpf-0.1.26/uml/interfaces.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.25/PKG-INFO` & `sdk_entrepot_gpf-0.1.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk_entrepot_gpf
-Version: 0.1.25
+Version: 0.1.26
 Summary: SDK Python pour simplifier l'utilisation de l'API Entrepôt de la Géoplateforme.
 Author-email: Valentin Sasyan <valentin.sasyan@ign.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

