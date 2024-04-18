# Comparing `tmp/vetiver-0.2.4.tar.gz` & `tmp/vetiver-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vetiver-0.2.4.tar", last modified: Mon Jan  8 14:58:15 2024, max compression
+gzip compressed data, was "vetiver-0.2.5.tar", last modified: Thu Apr 18 21:14:49 2024, max compression
```

## Comparing `vetiver-0.2.4.tar` & `vetiver-0.2.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.066121 vetiver-0.2.4/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.011412 vetiver-0.2.4/.github/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.017990 vetiver-0.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      834 2023-10-27 16:16:21.000000 vetiver-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      595 2023-10-27 16:16:21.000000 vetiver-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      255 2023-10-27 16:16:21.000000 vetiver-0.2.4/.github/ISSUE_TEMPLATE/release-checklist.md
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.019082 vetiver-0.2.4/.github/workflows/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3773 2024-01-08 14:55:07.000000 vetiver-0.2.4/.github/workflows/docs.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      322 2023-10-27 16:16:21.000000 vetiver-0.2.4/.github/workflows/precommit.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4284 2024-01-08 14:55:07.000000 vetiver-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4901 2023-10-27 16:16:21.000000 vetiver-0.2.4/.github/workflows/weekly.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1978 2023-10-27 16:16:21.000000 vetiver-0.2.4/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      592 2023-10-27 16:16:21.000000 vetiver-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5243 2023-10-27 16:16:21.000000 vetiver-0.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1082 2023-10-27 16:16:21.000000 vetiver-0.2.4/LICENSE
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      419 2023-10-27 16:16:21.000000 vetiver-0.2.4/MAINTAINERS.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2023-10-27 16:16:21.000000 vetiver-0.2.4/MANIFEST.in
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2333 2023-10-27 16:16:21.000000 vetiver-0.2.4/Makefile
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5419 2024-01-08 14:58:15.065891 vetiver-0.2.4/PKG-INFO
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3444 2023-10-27 16:16:21.000000 vetiver-0.2.4/README.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      494 2023-10-27 16:16:21.000000 vetiver-0.2.4/docker-compose.yml
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.020895 vetiver-0.2.4/docs/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       87 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      213 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/Makefile
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.011668 vetiver-0.2.4/docs/_extensions/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.011735 vetiver-0.2.4/docs/_extensions/machow/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.023370 vetiver-0.2.4/docs/_extensions/machow/interlinks/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       22 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      654 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/README.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      126 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      997 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/example.qmd
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4742 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7534 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/interlinks.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      447 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/objects_siuba.json
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      970 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/objects_vetiver.inv
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    11583 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/_extensions/machow/interlinks/objects_vetiver.json
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2475 2024-01-08 14:55:07.000000 vetiver-0.2.4/docs/_quarto.yml
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     8294 2024-01-08 14:55:10.000000 vetiver-0.2.4/docs/changelog.md
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7586 2024-01-08 14:55:07.000000 vetiver-0.2.4/docs/custom_code.qmd
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.024618 vetiver-0.2.4/docs/figures/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)   173095 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/figures/logo.png
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    19004 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/figures/logo.svg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    39341 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/figures/square-logo.svg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3400 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/index.qmd
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      135 2023-10-27 16:16:21.000000 vetiver-0.2.4/docs/version_config.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.024884 vetiver-0.2.4/examples/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.025500 vetiver-0.2.4/examples/coffeeratings/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      352 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings/Dockerfile
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      287 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings/app.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.012160 vetiver-0.2.4/examples/coffeeratings/v/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.025968 vetiver-0.2.4/examples/coffeeratings/v/20220415T174503Z-06d9b/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      455 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings/v/20220415T174503Z-06d9b/data.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1035 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1566 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings/vetiver_requirements.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1649 2023-10-27 16:16:21.000000 vetiver-0.2.4/examples/coffeeratings.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2751 2024-01-08 14:55:07.000000 vetiver-0.2.4/pyproject.toml
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.012419 vetiver-0.2.4/script/
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.026400 vetiver-0.2.4/script/setup-docker/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       53 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-docker/.gitignore
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      343 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-docker/docker.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.027214 vetiver-0.2.4/script/setup-rsconnect/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      122 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-rsconnect/add-users.sh
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      505 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-rsconnect/dump_api_keys.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      466 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-rsconnect/rstudio-connect.gcfg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       48 2023-10-27 16:16:21.000000 vetiver-0.2.4/script/setup-rsconnect/users.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1158 2024-01-08 14:58:15.066527 vetiver-0.2.4/setup.cfg
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       39 2023-10-27 16:16:21.000000 vetiver-0.2.4/setup.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)       93 2023-10-27 16:16:21.000000 vetiver-0.2.4/tox.ini
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.030560 vetiver-0.2.4/vetiver/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1506 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1972 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/attach_pkgs.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.032494 vetiver-0.2.4/vetiver/data/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      521 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/data/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)   181099 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/data/chicago.csv
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1281 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/data/mtcars.csv
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5103 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/data/sacramento.csv
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.033882 vetiver-0.2.4/vetiver/handlers/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        0 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/__init__.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4076 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/base.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1109 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/sklearn.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2611 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/spacy.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1296 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/statsmodels.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1344 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/torch.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1406 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/handlers/xgboost.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1186 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/helpers.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1351 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/meta.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      680 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/mock.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     7858 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/monitor.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3384 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/pin_read_write.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5712 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/prototype.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3239 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/rsconnect.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)    12478 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/server.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.035762 vetiver-0.2.4/vetiver/templates/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3829 2023-11-07 00:36:26.000000 vetiver-0.2.4/vetiver/templates/model_card.qmd
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3155 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/templates/monitoring_dashboard.qmd
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      964 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/templates.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.058826 vetiver-0.2.4/vetiver/tests/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      136 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/rsconnect_api_keys.json
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.063586 vetiver-0.2.4/vetiver/tests/snapshots/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3155 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/tests/snapshots/monitoring_dashboard.qmd
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      616 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/snapshots/test_monitor.json
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1929 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_add_endpoint.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      605 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_build_api.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5552 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_build_vetiver_model.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1990 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_custom_handler.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      311 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_mock_data.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4086 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_monitor.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      416 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_no_handler.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      874 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_pin_write.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1679 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_prepare_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3285 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_pytorch.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2711 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_rsconnect.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3404 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/tests/test_server.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2585 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_sklearn.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5161 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_spacy.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1949 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_statsmodels.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      450 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/tests/test_templates.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1207 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/tests/test_write_app.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1842 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/tests/test_write_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2379 2023-10-27 16:18:43.000000 vetiver-0.2.4/vetiver/tests/test_xgboost.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      232 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/types.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     1378 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/utils.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4331 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/vetiver_model.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     4274 2023-10-27 16:16:21.000000 vetiver-0.2.4/vetiver/write_docker.py
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     2993 2024-01-08 14:55:07.000000 vetiver-0.2.4/vetiver/write_fastapi.py
-drwxr-xr-x   0 isabelzimmerman   (501) staff       (20)        0 2024-01-08 14:58:15.064319 vetiver-0.2.4/vetiver.egg-info/
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     5419 2024-01-08 14:58:14.000000 vetiver-0.2.4/vetiver.egg-info/PKG-INFO
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)     3127 2024-01-08 14:58:15.000000 vetiver-0.2.4/vetiver.egg-info/SOURCES.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        1 2024-01-08 14:58:14.000000 vetiver-0.2.4/vetiver.egg-info/dependency_links.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)      493 2024-01-08 14:58:14.000000 vetiver-0.2.4/vetiver.egg-info/requires.txt
--rw-r--r--   0 isabelzimmerman   (501) staff       (20)        8 2024-01-08 14:58:14.000000 vetiver-0.2.4/vetiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.542636 vetiver-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.518636 vetiver-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.522636 vetiver-0.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/ISSUE_TEMPLATE/release-checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.526636 vetiver-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-18 21:14:45.000000 vetiver-0.2.5/.github/workflows/weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-18 21:14:45.000000 vetiver-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-18 21:14:45.000000 vetiver-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-18 21:14:45.000000 vetiver-0.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 21:14:45.000000 vetiver-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 21:14:45.000000 vetiver-0.2.5/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:45.000000 vetiver-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-18 21:14:45.000000 vetiver-0.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-18 21:14:49.542636 vetiver-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-18 21:14:45.000000 vetiver-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 21:14:45.000000 vetiver-0.2.5/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.526636 vetiver-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.518636 vetiver-0.2.5/docs/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.518636 vetiver-0.2.5/docs/_extensions/machow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.526636 vetiver-0.2.5/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/example.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/objects_siuba.json
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/objects_vetiver.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_extensions/machow/interlinks/objects_vetiver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/custom_code.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.526636 vetiver-0.2.5/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   173095 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/figures/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/figures/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/figures/square-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 21:14:45.000000 vetiver-0.2.5/docs/version_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.530636 vetiver-0.2.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.530636 vetiver-0.2.5/examples/coffeeratings/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.518636 vetiver-0.2.5/examples/coffeeratings/v/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.530636 vetiver-0.2.5/examples/coffeeratings/v/20220415T174503Z-06d9b/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings/v/20220415T174503Z-06d9b/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings/vetiver_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-18 21:14:45.000000 vetiver-0.2.5/examples/coffeeratings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-18 21:14:45.000000 vetiver-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.518636 vetiver-0.2.5/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.530636 vetiver-0.2.5/script/setup-docker/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-docker/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-docker/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.530636 vetiver-0.2.5/script/setup-rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-rsconnect/add-users.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-rsconnect/dump_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-rsconnect/rstudio-connect.gcfg
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 21:14:45.000000 vetiver-0.2.5/script/setup-rsconnect/users.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-18 21:14:49.542636 vetiver-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 21:14:45.000000 vetiver-0.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 21:14:45.000000 vetiver-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.534636 vetiver-0.2.5/vetiver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/attach_pkgs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.534636 vetiver-0.2.5/vetiver/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   181099 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/data/chicago.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/data/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/data/sacramento.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.534636 vetiver-0.2.5/vetiver/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/handlers/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/pin_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/rsconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.538636 vetiver-0.2.5/vetiver/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/templates/model_card.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/templates/monitoring_dashboard.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.542636 vetiver-0.2.5/vetiver/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/rsconnect_api_keys.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.542636 vetiver-0.2.5/vetiver/tests/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/snapshots/monitoring_dashboard.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/snapshots/test_monitor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_add_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_build_vetiver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_custom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_pin_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_prepare_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_rsconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_spacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_write_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_write_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/tests/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/vetiver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/write_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-18 21:14:45.000000 vetiver-0.2.5/vetiver/write_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:14:49.542636 vetiver-0.2.5/vetiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-18 21:14:49.000000 vetiver-0.2.5/vetiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-18 21:14:49.000000 vetiver-0.2.5/vetiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:14:49.000000 vetiver-0.2.5/vetiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-18 21:14:49.000000 vetiver-0.2.5/vetiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 21:14:49.000000 vetiver-0.2.5/vetiver.egg-info/top_level.txt
```

### Comparing `vetiver-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `vetiver-0.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `vetiver-0.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/.github/workflows/docs.yml` & `vetiver-0.2.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/.github/workflows/tests.yml` & `vetiver-0.2.5/.github/workflows/tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -148,7 +148,28 @@
         shell: bash
         run: |
           pip install ".[dev,all_models]"
 
       - name: Run Tests
         shell: bash
         run: make typecheck
+
+  release-pypi:
+    name: "Release to pypi"
+    runs-on: ubuntu-latest
+    if: github.event_name == 'release'
+    needs: [test-no-extras, tests, test-rsconnect]
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+      - name: "Build Package"
+        run: |
+          python -m pip install build wheel
+          python -m build --sdist --wheel
+
+      - name: "Deploy to Test PyPI"
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `vetiver-0.2.4/.github/workflows/weekly.yml` & `vetiver-0.2.5/.github/workflows/weekly.yml`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/.gitignore` & `vetiver-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/.pre-commit-config.yaml` & `vetiver-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/CODE_OF_CONDUCT.md` & `vetiver-0.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/LICENSE` & `vetiver-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/Makefile` & `vetiver-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/PKG-INFO` & `vetiver-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vetiver
-Version: 0.2.4
+Version: 0.2.5
 Summary: Version, share, deploy, and monitor models.
 Home-page: https://github.com/rstudio/vetiver-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Keywords: data,mlops
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vetiver Version: 0.2.4 Summary: Version, share,
+Metadata-Version: 2.1 Name: vetiver Version: 0.2.5 Summary: Version, share,
 deploy, and monitor models. Home-page: https://github.com/rstudio/vetiver-
 python Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co
 License: MIT Keywords: data,mlops Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: pandas
 Requires-Dist: fastapi Requires-Dist: pydantic Requires-Dist: joblib Requires-
```

### Comparing `vetiver-0.2.4/README.md` & `vetiver-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/README.md` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/README.md`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/example.qmd` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/example.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/interlinks.lua` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/interlinks.py` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/interlinks.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/objects_vetiver.inv` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/objects_vetiver.inv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_extensions/machow/interlinks/objects_vetiver.json` & `vetiver-0.2.5/docs/_extensions/machow/interlinks/objects_vetiver.json`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/_quarto.yml` & `vetiver-0.2.5/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/changelog.md` & `vetiver-0.2.5/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # Release notes
 
 
 For full details, view the [commit logs](https://github.com/rstudio/vetiver-python/commits/).
 
+## v0.2.5
+## What's Changed
+
+[**Full Changelog**](https://github.com/rstudio/vetiver-python/compare/v0.2.4...v0.2.5)
+
+* MAINT: refactor tests in [GH209](https://github.com/rstudio/vetiver-python/pull/209)
+* DOCS: Update link to custom handlers documentation in [GH208](https://github.com/rstudio/vetiver-python/pull/208)
+* ENH: add `Field` examples to model prototypes in [GH210](https://github.com/rstudio/vetiver-python/pull/210)
+
 
 ## v0.2.4
 ## What's Changed
 
 [**Full Changelog**](https://github.com/rstudio/vetiver-python/compare/v0.2.3...v0.2.4)
 
 * MAINT: drop Python 3.7 support in [GH199](https://github.com/rstudio/vetiver-python/pull/199)
```

### Comparing `vetiver-0.2.4/docs/custom_code.qmd` & `vetiver-0.2.5/docs/custom_code.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/figures/logo.png` & `vetiver-0.2.5/docs/figures/logo.png`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/figures/logo.svg` & `vetiver-0.2.5/docs/figures/logo.svg`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/figures/square-logo.svg` & `vetiver-0.2.5/docs/figures/square-logo.svg`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/docs/index.qmd` & `vetiver-0.2.5/docs/index.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 You can use vetiver with:
 
 -   [scikit-learn](https://scikit-learn.org/)
 -   [torch](https://pytorch.org/)
 -   [statsmodels](https://www.statsmodels.org/stable/index.html)
 -   [xgboost](https://xgboost.readthedocs.io/en/stable/)
 -   [spacy](https://spacy.io/)
--   or utilize [custom handlers](https://rstudio.github.io/vetiver-python/stable/advancedusage/custom_handler.html) to support your own models!
+-   or utilize [custom handlers](https://rstudio.github.io/vetiver-python/stable/custom_code.html) to support your own models!
 
 ## Installation
 
 You can install the released version of vetiver from [PyPI](https://pypi.org/project/vetiver/):
 
 ```python
 python -m pip install vetiver
```

#### html2text {}

```diff
@@ -12,33 +12,33 @@
 vetiver, see: - the documentation at
 vetiver.rstudio.com/> - the R package at
 rstudio.github.io/vetiver-r/> You can use vetiver with: - [scikit-learn](https:
 //scikit-learn.org/) - [torch](https://pytorch.org/) - [statsmodels](https://
 www.statsmodels.org/stable/index.html) - [xgboost](https://
 xgboost.readthedocs.io/en/stable/) - [spacy](https://spacy.io/) - or utilize
 [custom handlers](https://rstudio.github.io/vetiver-python/stable/
-advancedusage/custom_handler.html) to support your own models! ## Installation
-You can install the released version of vetiver from [PyPI](https://pypi.org/
-project/vetiver/): ```python python -m pip install vetiver ``` And the
-development version from [GitHub](https://github.com/rstudio/vetiver-python)
-with: ```python python -m pip install git+https://github.com/rstudio/vetiver-
-python ``` ## Example A `VetiverModel()` object collects the information needed
-to store, version, and deploy a trained model. ```python from vetiver import
-mock, VetiverModel X, y = mock.get_mock_data() model = mock.get_mock_model
-().fit(X, y) v = VetiverModel(model, model_name='mock_model', prototype_data=X)
-``` You can **version** and **share** your `VetiverModel()` by choosing a
-[pins](https://rstudio.github.io/pins-python/) "board" for it, including a
-local folder, RStudio Connect, Amazon S3, and more. ```python from pins import
-board_temp from vetiver import vetiver_pin_write model_board = board_temp
-(versioned = True, allow_pickle_read = True) vetiver_pin_write(model_board, v)
-``` You can **deploy** your pinned `VetiverModel()` using `VetiverAPI()`, an
-extension of [FastAPI](https://fastapi.tiangolo.com/). ```python from vetiver
-import VetiverAPI app = VetiverAPI(v, check_prototype = True) ``` To start a
-server using this object, use `app.run(port = 8080)` or your port of choice. ##
-Contributing This project is released with a [Contributor Code of Conduct]
-(https://www.contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html). By
-contributing to this project, you agree to abide by its terms. - For questions
-and discussions about deploying models, statistical modeling, and machine
-learning, please [post on RStudio Community](https://community.rstudio.com/new-
+custom_code.html) to support your own models! ## Installation You can install
+the released version of vetiver from [PyPI](https://pypi.org/project/vetiver/):
+```python python -m pip install vetiver ``` And the development version from
+[GitHub](https://github.com/rstudio/vetiver-python) with: ```python python -
+m pip install git+https://github.com/rstudio/vetiver-python ``` ## Example A
+`VetiverModel()` object collects the information needed to store, version, and
+deploy a trained model. ```python from vetiver import mock, VetiverModel X, y =
+mock.get_mock_data() model = mock.get_mock_model().fit(X, y) v = VetiverModel
+(model, model_name='mock_model', prototype_data=X) ``` You can **version** and
+**share** your `VetiverModel()` by choosing a [pins](https://rstudio.github.io/
+pins-python/) "board" for it, including a local folder, RStudio Connect, Amazon
+S3, and more. ```python from pins import board_temp from vetiver import
+vetiver_pin_write model_board = board_temp(versioned = True, allow_pickle_read
+= True) vetiver_pin_write(model_board, v) ``` You can **deploy** your pinned
+`VetiverModel()` using `VetiverAPI()`, an extension of [FastAPI](https://
+fastapi.tiangolo.com/). ```python from vetiver import VetiverAPI app =
+VetiverAPI(v, check_prototype = True) ``` To start a server using this object,
+use `app.run(port = 8080)` or your port of choice. ## Contributing This project
+is released with a [Contributor Code of Conduct](https://www.contributor-
+covenant.org/version/2/1/CODE_OF_CONDUCT.html). By contributing to this
+project, you agree to abide by its terms. - For questions and discussions about
+deploying models, statistical modeling, and machine learning, please [post on
+RStudio Community](https://community.rstudio.com/new-
 topic?category_id=15&tags=vetiver,question). - If you think you have
 encountered a bug, please [submit an issue](https://github.com/rstudio/vetiver-
 python/issues).
```

### Comparing `vetiver-0.2.4/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib` & `vetiver-0.2.5/examples/coffeeratings/v/20220415T174503Z-06d9b/v.joblib`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/examples/coffeeratings/vetiver_requirements.txt` & `vetiver-0.2.5/examples/coffeeratings/vetiver_requirements.txt`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/examples/coffeeratings.py` & `vetiver-0.2.5/examples/coffeeratings.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/pyproject.toml` & `vetiver-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # warnings) should be suppressed even if they are an included file or
 # within the transitive closure of an included file. Paths may contain
 # wildcard characters ** (a directory or multiple levels of
 # directories), * (a sequence of zero or more characters), or ? (a
 # single character).
 ignore = [
     #"vetiver/__init__.py",
-    #"vetiver/attach_pkgs.py",
+    "vetiver/attach_pkgs.py",
     "vetiver/helpers.py",
     "vetiver/meta.py",
     "vetiver/mock.py",
     "vetiver/model_card.py",
     "vetiver/monitor.py",
     "vetiver/pin_read_write.py",
     "vetiver/prototype.py",
```

### Comparing `vetiver-0.2.4/setup.cfg` & `vetiver-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/__init__.py` & `vetiver-0.2.5/vetiver/__init__.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/attach_pkgs.py` & `vetiver-0.2.5/vetiver/attach_pkgs.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/data/chicago.csv` & `vetiver-0.2.5/vetiver/data/chicago.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/data/mtcars.csv` & `vetiver-0.2.5/vetiver/data/mtcars.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/data/sacramento.csv` & `vetiver-0.2.5/vetiver/data/sacramento.csv`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/base.py` & `vetiver-0.2.5/vetiver/handlers/base.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/sklearn.py` & `vetiver-0.2.5/vetiver/handlers/sklearn.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/spacy.py` & `vetiver-0.2.5/vetiver/handlers/spacy.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/statsmodels.py` & `vetiver-0.2.5/vetiver/handlers/statsmodels.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/torch.py` & `vetiver-0.2.5/vetiver/handlers/torch.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/handlers/xgboost.py` & `vetiver-0.2.5/vetiver/handlers/xgboost.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/helpers.py` & `vetiver-0.2.5/vetiver/helpers.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/meta.py` & `vetiver-0.2.5/vetiver/meta.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/mock.py` & `vetiver-0.2.5/vetiver/mock.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/monitor.py` & `vetiver-0.2.5/vetiver/monitor.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/pin_read_write.py` & `vetiver-0.2.5/vetiver/pin_read_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .vetiver_model import VetiverModel
 from .meta import VetiverMeta
-from .utils import inform
+from .utils import inform, serialize_prototype
 import warnings
 import logging
 
 _log = logging.getLogger(__name__)
 
 
 class ModelCard(UserWarning):
@@ -68,18 +68,24 @@
         name=model.model_name,
         type="joblib",
         description=model.description,
         metadata={
             "user": model.metadata.user,
             "vetiver_meta": {
                 "required_pkgs": model.metadata.required_pkgs,
-                "prototype": None if not model.prototype else model.prototype().json(),
-                "python_version": None
-                if not model.metadata.python_version
-                else list(model.metadata.python_version),
+                "prototype": (
+                    None
+                    if not model.prototype
+                    else serialize_prototype(model.prototype)
+                ),
+                "python_version": (
+                    None
+                    if not model.metadata.python_version
+                    else list(model.metadata.python_version)
+                ),
             },
         },
         versioned=versioned,
     )
 
 
 def vetiver_pin_read(board, name: str, version: str = None) -> VetiverModel:
```

### Comparing `vetiver-0.2.4/vetiver/prototype.py` & `vetiver-0.2.5/vetiver/prototype.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 except ImportError:
     # python < 3.10
     NoneType = type(None)
 
 import pandas as pd
 import numpy as np
 import pydantic
+from pydantic import Field
 from warnings import warn
 from .types import create_prototype
 
 
 class InvalidPTypeError(Exception):
     """
     Throw an error if prototype cannot be recognised
@@ -155,15 +156,16 @@
             return value
 
     dict_data = dict(enumerate(data[0], 0))
     # pydantic requires strings as indicies
     # if its a numpy type, we have to take the Python type due to Pydantic
 
     dict_data = {
-        f"{key}": (type(value.item()), _item(value)) for key, value in dict_data.items()
+        f"{key}": (type(value.item()), Field(..., example=_item(value)))
+        for key, value in dict_data.items()
     }
     prototype = create_prototype(**dict_data)
     return prototype
 
 
 @vetiver_create_prototype.register
 def _(data: dict):
@@ -178,15 +180,22 @@
 
     # if it comes from vetiver's /prototype endpoint
     dict_data = {}
     if data.keys() >= {"properties", "title", "type"}:
         # automatically create for simple prototypes
         try:
             for key, value in data["properties"].items():
-                dict_data.update({key: (type(value["default"]), value["default"])})
+                dict_data.update(
+                    {
+                        key: (
+                            type(value["example"]),
+                            Field(..., example=value["example"]),
+                        )
+                    }
+                )
         # error for complex objects
         except KeyError:
             raise InvalidPTypeError(
                 "Failed to create dict prototype for this data. "
                 "Please use pandas DataFrame or pydantic BaseModel."
             )
         return create_prototype(**dict_data)
@@ -219,9 +228,9 @@
     """
     return None
 
 
 def _to_field(data):
     basemodel_input = dict()
     for key, value in data.items():
-        basemodel_input[key] = (type(value), value)
+        basemodel_input[key] = (type(value), Field(..., example=value))
     return basemodel_input
```

### Comparing `vetiver-0.2.4/vetiver/rsconnect.py` & `vetiver-0.2.5/vetiver/rsconnect.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/server.py` & `vetiver-0.2.5/vetiver/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+import json
+import logging
 import re
+import webbrowser
+from textwrap import dedent
+from typing import Callable, List, Union
+from urllib.parse import urljoin
+from warnings import warn
+
 import httpx
-import json
+import pandas as pd
 import requests
 import uvicorn
-import logging
-import pandas as pd
-from fastapi import FastAPI, Request, testclient
+from fastapi import FastAPI, Request
 from fastapi.exceptions import RequestValidationError
 from fastapi.openapi.utils import get_openapi
-from fastapi.responses import HTMLResponse, RedirectResponse, PlainTextResponse
-from textwrap import dedent
-from warnings import warn
-from urllib.parse import urljoin
-from typing import Callable, List, Union
+from fastapi.responses import HTMLResponse, PlainTextResponse, RedirectResponse
 
+from .helpers import api_data_to_frame, response_to_frame
+from .meta import VetiverMeta
 from .utils import _jupyter_nb, get_workbench_path
 from .vetiver_model import VetiverModel
-from .meta import VetiverMeta
-from .helpers import api_data_to_frame, response_to_frame
 
 
 class VetiverAPI:
     """Create model aware API
 
     Parameters
     ----------
@@ -247,37 +249,45 @@
                 predictions = endpoint_fx(served_data, **kw)
 
                 if isinstance(predictions, List):
                     return {endpoint_name: predictions}
                 else:
                     return predictions
 
-    def run(self, port: int = 8000, host: str = "127.0.0.1", **kw):
+    def run(self, port: int = 8000, host: str = "127.0.0.1", quiet_open=False, **kw):
         """
         Start API
 
         Parameters
         ----------
         port : int
             An integer that indicates the server port that should be listened on.
         host : str
             A valid IPv4 or IPv6 address, which the application will listen on.
+        quiet_open : bool
+            If host is a localhost address, try to automatically open API in browser
 
         Examples
         -------
         >>> import vetiver as vt
         >>> X, y = vt.get_mock_data()
         >>> model = vt.get_mock_model().fit(X, y)
         >>> v = vt.VetiverModel(model = model, model_name = "model", prototype_data = X)
         >>> v_api = vt.VetiverAPI(model = v, check_prototype = True)
         >>> v_api.run()     # doctest: +SKIP
         """
         _jupyter_nb()
         self.workbench_path = get_workbench_path(port)
-
+        if port and host:
+            try:
+                if host == "127.0.0.1" and not quiet_open:
+                    # quality of life for developing APIs locally
+                    webbrowser.open(f"http://{host}:{port}")
+            except Exception:
+                pass
         if self.workbench_path:
             uvicorn.run(
                 self.app, port=port, host=host, root_path=self.workbench_path, **kw
             )
         else:
             uvicorn.run(self.app, port=port, host=host, **kw)
 
@@ -317,17 +327,16 @@
     Examples
     -------
     >>> import vetiver
     >>> X, y = vetiver.get_mock_data()
     >>> endpoint = vetiver.vetiver_endpoint(url='http://127.0.0.1:8000/predict')
     >>> vetiver.predict(endpoint, X)     # doctest: +SKIP
     """
-    if isinstance(endpoint, testclient.TestClient):
-        requester = endpoint
-        endpoint = requester.app.root_path
+    if "test_client" in kw:
+        requester = kw.pop("test_client")
     else:
         requester = requests
 
     # TO DO: arrow format
     # TO DO: dispatch
 
     if isinstance(data, pd.DataFrame):
```

### Comparing `vetiver-0.2.4/vetiver/templates/model_card.qmd` & `vetiver-0.2.5/vetiver/templates/model_card.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/templates/monitoring_dashboard.qmd` & `vetiver-0.2.5/vetiver/templates/monitoring_dashboard.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/templates.py` & `vetiver-0.2.5/vetiver/templates.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/snapshots/monitoring_dashboard.qmd` & `vetiver-0.2.5/vetiver/tests/snapshots/monitoring_dashboard.qmd`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/snapshots/test_monitor.json` & `vetiver-0.2.5/vetiver/tests/snapshots/test_monitor.json`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_add_endpoint.py` & `vetiver-0.2.5/vetiver/tests/test_statsmodels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 import pytest
 
-import numpy as np
-import pandas as pd
-from fastapi.testclient import TestClient
-
-from vetiver import mock, VetiverModel, VetiverAPI
-from vetiver.helpers import api_data_to_frame
-import vetiver
+sm = pytest.importorskip("statsmodels.api", reason="statsmodels library not installed")
 
+statsmodels = pytest.importorskip(
+    "statsmodels", reason="statsmodels library not installed"
+)
 
-@pytest.fixture
-def vetiver_model():
-    np.random.seed(500)
-    X, y = mock.get_mock_data()
-    model = mock.get_mock_model().fit(X, y)
-    v = VetiverModel(
-        model=model,
-        prototype_data=X,
-        model_name="my_model",
-        versioned=None,
-        description="A regression model for testing purposes",
-    )
-
-    return v
-
-
-def sum_values(x):
-    return x.sum().to_list()
+import numpy as np  # noqa
+import pandas as pd  # noqa
+from fastapi.testclient import TestClient  # noqa
 
-
-def sum_values_no_prototype(x):
-    return api_data_to_frame(x).sum().to_list()
+import vetiver  # noqa
 
 
 @pytest.fixture
-def vetiver_client(vetiver_model):  # With check_prototype=True
+def model():
 
-    app = VetiverAPI(vetiver_model, check_prototype=True)
-    app.vetiver_post(sum_values, "sum")
+    X, y = vetiver.get_mock_data()
+    glm = sm.GLM(y, X).fit()
 
-    app.app.root_path = "/sum"
-    client = TestClient(app.app)
+    v = vetiver.VetiverModel(glm, "glm", X)
+    return v
 
-    return client
 
+def test_vetiver_build(client):
+    data = [{"B": 0, "C": 0, "D": 0}]
 
-@pytest.fixture
-def vetiver_client_check_ptype_false(vetiver_model):  # With check_prototype=False
+    response = vetiver.predict(endpoint="/predict/", data=data, test_client=client)
 
-    app = VetiverAPI(vetiver_model, check_prototype=False)
-    app.vetiver_post(sum_values_no_prototype, "sum")
+    assert response.iloc[0, 0] == 0.0
+    assert len(response) == 1
 
-    app.app.root_path = "/sum"
-    client = TestClient(app.app)
 
-    return client
+def test_batch(client):
+    data = pd.DataFrame(np.random.randint(0, 100, size=(100, 4)), columns=list("ABCD"))
 
+    response = vetiver.predict(endpoint="/predict/", data=data, test_client=client)
 
-def test_endpoint_adds_ptype(vetiver_client):
+    assert len(response) == 100
 
-    data = pd.DataFrame({"B": [1, 1, 1], "C": [2, 2, 2], "D": [3, 3, 3]})
-    response = vetiver.predict(endpoint=vetiver_client, data=data)
 
-    assert isinstance(response, pd.DataFrame)
-    assert response.to_json() == '{"sum":{"0":3,"1":6,"2":9}}', response.to_json()
+def test_no_ptype(client_no_prototype):
+    data = [0, 0, 0]
 
+    response = vetiver.predict(
+        endpoint="/predict/", data=data, test_client=client_no_prototype
+    )
+
+    assert response.iloc[0, 0] == 0.0
+    assert len(response) == 1
 
-def test_endpoint_adds_no_ptype(vetiver_client_check_ptype_false):
 
-    data = pd.DataFrame({"B": [1, 1, 1], "C": [2, 2, 2], "D": [3, 3, 3]})
-    response = vetiver.predict(endpoint=vetiver_client_check_ptype_false, data=data)
+def test_serialize(model):
+    import pins
 
-    assert isinstance(response, pd.DataFrame)
-    assert response.to_json() == '{"sum":{"0":3,"1":6,"2":9}}', response.to_json()
+    board = pins.board_temp(allow_pickle_read=True)
+    vetiver.vetiver_pin_write(board=board, model=model)
+    assert isinstance(
+        board.pin_read("glm"),
+        statsmodels.genmod.generalized_linear_model.GLMResultsWrapper,
+    )
+    board.pin_delete("glm")
```

### Comparing `vetiver-0.2.4/vetiver/tests/test_custom_handler.py` & `vetiver-0.2.5/vetiver/tests/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_monitor.py` & `vetiver-0.2.5/vetiver/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_pin_write.py` & `vetiver-0.2.5/vetiver/tests/test_pin_write.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import pytest
 
-from vetiver.mock import get_mock_data, get_mock_model
-from vetiver.pin_read_write import vetiver_pin_write
-from vetiver.vetiver_model import VetiverModel
+from vetiver import mock, vetiver_pin_write, VetiverModel
 import sklearn
 import pins
 
 # Load data, model
-X_df, y = get_mock_data()
-model = get_mock_model().fit(X_df, y)
+X_df, y = mock.get_mock_data()
+model = mock.get_mock_model().fit(X_df, y)
 
 
 def test_board_pin_write_error():
     v = VetiverModel(
         model=model, prototype_data=X_df, model_name="model", versioned=None
     )
     board = pins.board_temp()
```

### Comparing `vetiver-0.2.4/vetiver/tests/test_prepare_docker.py` & `vetiver-0.2.5/vetiver/tests/test_prepare_docker.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_rsconnect.py` & `vetiver-0.2.5/vetiver/tests/test_rsconnect.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_server.py` & `vetiver-0.2.5/vetiver/tests/test_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 from vetiver import (
     mock,
     VetiverModel,
     VetiverAPI,
     vetiver_create_prototype,
     InvalidPTypeError,
     vetiver_endpoint,
+    predict,
 )
 from pydantic import BaseModel, conint
 from fastapi.testclient import TestClient
 import numpy as np
 import pytest
 import sys
 
 
 @pytest.fixture
-def vetiver_model():
+def model():
     np.random.seed(500)
     X, y = mock.get_mock_data()
     model = mock.get_mock_model().fit(X, y)
     v = VetiverModel(
         model=model,
         prototype_data=X,
         model_name="my_model",
         versioned=None,
         description="A regression model for testing purposes",
     )
     return v
 
 
 @pytest.fixture
-def client(vetiver_model):
-    app = VetiverAPI(vetiver_model)
-
-    return TestClient(app.app)
-
-
-@pytest.fixture
-def complex_prototype_model():
+def complex_prototype_client():
     np.random.seed(500)
 
     class CustomPrototype(BaseModel):
         B: conint(gt=42)
         C: conint(gt=42)
         D: conint(gt=42)
 
@@ -79,35 +73,36 @@
         "version": None,
         "url": None,
         "required_pkgs": ["scikit-learn"],
         "python_version": list(sys.version_info),  # JSON will return a list
     }
 
 
-def test_get_prototype(client, vetiver_model):
+def test_get_prototype(client, model):
     response = client.get("/prototype")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "properties": {
-            "B": {"default": 55, "type": "integer"},
-            "C": {"default": 65, "type": "integer"},
-            "D": {"default": 17, "type": "integer"},
+            "B": {"example": 55, "type": "integer"},
+            "C": {"example": 65, "type": "integer"},
+            "D": {"example": 17, "type": "integer"},
         },
+        "required": ["B", "C", "D"],
         "title": "prototype",
         "type": "object",
     }
 
     assert (
-        vetiver_model.prototype.construct().dict()
+        model.prototype.construct().dict()
         == vetiver_create_prototype(response.json()).construct().dict()
     )
 
 
-def test_complex_prototype(complex_prototype_model):
-    response = complex_prototype_model.get("/prototype")
+def test_complex_prototype(complex_prototype_client):
+    response = complex_prototype_client.get("/prototype")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "properties": {
             "B": {"exclusiveMinimum": 42, "type": "integer"},
             "C": {"exclusiveMinimum": 42, "type": "integer"},
             "D": {"exclusiveMinimum": 42, "type": "integer"},
         },
@@ -116,12 +111,17 @@
         "type": "object",
     }
 
     with pytest.raises(InvalidPTypeError):
         vetiver_create_prototype(response.json())
 
 
+def test_predict_wrong_input(client):
+    with pytest.raises(TypeError):
+        predict(endpoint="/predict/", data=[{"B": 43, "C": 43}], test_client=client)
+
+
 def test_vetiver_endpoint():
     url_raw = "http://127.0.0.1:8000/predict/"
     url = vetiver_endpoint(url_raw)
 
     assert url == "http://127.0.0.1:8000/predict"
```

### Comparing `vetiver-0.2.4/vetiver/tests/test_sklearn.py` & `vetiver-0.2.5/vetiver/tests/test_sklearn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,69 @@
 import pytest
-
 import numpy as np
 import pandas as pd
 from requests.exceptions import HTTPError
-from fastapi.testclient import TestClient
-
-from vetiver import mock, VetiverModel, VetiverAPI
+from vetiver import mock, VetiverModel
 from vetiver.server import predict
 
 np.random.seed(500)
 X, y = mock.get_mock_data()
 
 
 @pytest.fixture
-def vetiver_model():
+def model() -> VetiverModel:
     np.random.seed(500)
     model = mock.get_mock_model().fit(X, y)
     v = VetiverModel(
         model=model,
         prototype_data=X,
         model_name="my_model",
         versioned=None,
         description="A regression model for testing purposes",
     )
 
     return v
 
 
-@pytest.fixture
-def vetiver_client(vetiver_model):  # With check_ptype=True
-    app = VetiverAPI(vetiver_model, check_prototype=True)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
-
-
-@pytest.fixture
-def vetiver_client_check_ptype_false(vetiver_model):  # With check_ptype=False
-    app = VetiverAPI(vetiver_model, check_prototype=False)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
-
-
 @pytest.mark.parametrize(
-    "data,length",
-    [({"B": 0, "C": 0, "D": 0}, 1), (pd.Series(data=[0, 0, 0]), 1), (X, 100)],
+    "data,expected_length",
+    [
+        ([{"B": 0, "C": 0, "D": 0}], 1),
+        (pd.Series(data=[0, 0, 0], index=["B", "C", "D"]), 1),
+        (X, 100),
+    ],
 )
-def test_predict_sklearn_ptype(data, length, vetiver_client):
-
-    response = predict(endpoint=vetiver_client, data=data)
-
+def test_predict_sklearn_ptype(data, expected_length, client):
+    response = predict(endpoint="/predict/", data=data, test_client=client)
     assert isinstance(response, pd.DataFrame), response
     assert response.iloc[0, 0] == 44.47
-    assert len(response) == length
+    assert len(response) == expected_length
 
 
 @pytest.mark.parametrize(
     "data,length",
     [({"B": 0, "C": 0, "D": 0}, 1), (pd.Series(data=[0, 0, 0]), 1), (X, 100)],
 )
-def test_predict_sklearn_no_ptype(data, length, vetiver_client_check_ptype_false):
-    X, y = mock.get_mock_data()
-    response = predict(endpoint=vetiver_client_check_ptype_false, data=data)
+def test_predict_sklearn_no_ptype(data, length, client_no_prototype):
+    response = predict(endpoint="/predict/", data=data, test_client=client_no_prototype)
 
     assert isinstance(response, pd.DataFrame), response
     assert response.iloc[0, 0] == 44.47
     assert len(response) == length
 
 
 @pytest.mark.parametrize("data", [(0), 0, 0.0, "0"])
-def test_predict_sklearn_type_error(data, vetiver_client):
+def test_predict_sklearn_type_error(data, client):
 
     msg = str(
         "[{'type': 'list_type', 'loc': ('body',), 'msg': 'Input should be a valid list', \
         'input': '0', 'url': 'https://errors.pydantic.dev/2.0.3/v/list_type'}]"
     )
 
     with pytest.raises(TypeError, match=msg):
-        predict(endpoint=vetiver_client, data=data)
+        predict(endpoint="/predict/", data=data, test_client=client)
 
 
-def test_predict_server_error(vetiver_model):
-    X, y = mock.get_mock_data()
-    app = VetiverAPI(vetiver_model, check_prototype=True)
-    app.app.root_path = "/i_do_not_exists"
-    client = TestClient(app.app)
+def test_predict_server_error(client):
 
     with pytest.raises(HTTPError):
-        predict(endpoint=client, data=X)
+        predict(endpoint="/i_do_not_exists/", data=X, test_client=client)
```

### Comparing `vetiver-0.2.4/vetiver/tests/test_spacy.py` & `vetiver-0.2.5/vetiver/tests/test_spacy.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,43 +28,18 @@
 
 
 @pytest.fixture
 def spacy_model():
     return nlp
 
 
-@pytest.fixture()
-def vetiver_client_with_prototype(spacy_model):  # With check_prototype=True
-    df = pd.DataFrame({"new_column": ["one", "two", "three"]})
-    v = vetiver.VetiverModel(spacy_model, "animals", prototype_data=df)
-    app = vetiver.VetiverAPI(v, check_prototype=True)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
-
-
-@pytest.fixture(scope="function")
-def vetiver_client_with_prototype_series(spacy_model):  # With check_prototype=True
-    df = pd.Series({"new_column": ["one", "two", "three"]})
-    v = vetiver.VetiverModel(spacy_model, "animals", prototype_data=df)
-    app = vetiver.VetiverAPI(v, check_prototype=True)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-    return client
-
-
 @pytest.fixture
-def vetiver_client_no_prototype(spacy_model):  # With check_prototype=False
-    v = vetiver.VetiverModel(spacy_model, "animals")
-    app = vetiver.VetiverAPI(v, check_prototype=False)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
+def model(spacy_model) -> TestClient:
+    df = pd.DataFrame({"new_column": ["one", "two", "three"]})
+    return vetiver.VetiverModel(spacy_model, "animals", prototype_data=df)
 
 
 @pytest.mark.parametrize("data", ["a", 1, [1, 2, 3]])
 def test_bad_prototype_data(data, spacy_model):
     with pytest.raises(TypeError):
         vetiver.VetiverModel(spacy_model, "animals", prototype_data=data)
 
@@ -81,21 +56,36 @@
         vetiver.VetiverModel(spacy_model, "animals", prototype_data=data)
 
 
 @pytest.mark.parametrize("data", [{"col": "1"}, pd.DataFrame({"col": ["1"]})])
 def test_good_prototype_shape(data, spacy_model):
     v = vetiver.VetiverModel(spacy_model, "animals", prototype_data=data)
 
-    assert v.prototype.construct().dict() == {"col": "1"}
+    try:
+        model_schema = v.prototype.model_json_schema()
+        expected = {
+            "properties": {
+                "col": {"example": "1", "title": "Col", "type": "string"},
+            },
+            "required": ["col"],
+            "title": "prototype",
+            "type": "object",
+        }
+    except AttributeError:  # pydantic v1
+        model_schema = v.prototype.schema_json()
+        expected = '{"title": "prototype", "type": "object", "properties": \
+{"col": {"title": "Col", "example": "1", "type": "string"}}, "required": ["col"]}'
+
+    assert model_schema == expected
 
 
-def test_vetiver_predict_with_prototype(vetiver_client_with_prototype):
+def test_vetiver_predict_with_prototype(client: TestClient):
     df = pd.DataFrame({"new_column": ["turtles", "i have a dog"]})
 
-    response = vetiver.predict(endpoint=vetiver_client_with_prototype, data=df)
+    response = vetiver.predict(endpoint="/predict/", data=df, test_client=client)
 
     assert isinstance(response, pd.DataFrame), response
     assert response.to_dict() == {
         "0": {
             "text": "turtles",
             "ents": [],
             "sents": [{"start": 0, "end": 7}],
@@ -111,18 +101,20 @@
                 {"id": 2, "start": 7, "end": 8},
                 {"id": 3, "start": 9, "end": 12},
             ],
         },
     }
 
 
-def test_vetiver_predict_no_prototype(vetiver_client_no_prototype):
+def test_vetiver_predict_no_prototype(client_no_prototype: TestClient):
     df = pd.DataFrame({"uhhh": ["turtles", "i have a dog"]})
 
-    response = vetiver.predict(endpoint=vetiver_client_no_prototype, data=df)
+    response = vetiver.predict(
+        endpoint="/predict/", data=df, test_client=client_no_prototype
+    )
 
     assert isinstance(response, pd.DataFrame), response
     assert response.to_dict() == {
         "0": {
             "text": "turtles",
             "ents": [],
             "sents": [{"start": 0, "end": 7}],
```

### Comparing `vetiver-0.2.4/vetiver/tests/test_write_app.py` & `vetiver-0.2.5/vetiver/tests/test_write_app.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_write_docker.py` & `vetiver-0.2.5/vetiver/tests/test_write_docker.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/tests/test_xgboost.py` & `vetiver-0.2.5/vetiver/tests/test_xgboost.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import vetiver  # noqa
 
 PREDICT_VALUE = 19.963224411010742
 
 
 @pytest.fixture
-def xgb_model():
+def model():
     # read in data
     dtrain = xgb.DMatrix(mtcars.drop(columns="mpg"), label=mtcars["mpg"])
     # specify parameters via map
     param = {
         "max_depth": 2,
         "eta": 1,
         "objective": "reg:squarederror",
@@ -26,69 +26,50 @@
     }
     num_round = 2
     fit = xgb.train(param, dtrain, num_round)
 
     return vetiver.VetiverModel(fit, "xgb", mtcars.drop(columns="mpg"))
 
 
-@pytest.fixture
-def vetiver_client(xgb_model):  # With check_prototype=True
-    app = vetiver.VetiverAPI(xgb_model, check_prototype=True)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
-
-
-@pytest.fixture
-def vetiver_client_check_ptype_false(xgb_model):  # With check_prototype=True
-    app = vetiver.VetiverAPI(xgb_model, check_prototype=False)
-    app.app.root_path = "/predict"
-    client = TestClient(app.app)
-
-    return client
+def test_required_pkgs(model):
+    assert model.metadata.required_pkgs == ["xgboost"]
+    assert not model.metadata.user
 
 
-def test_model(xgb_model):
-    v = xgb_model
-
-    assert v.metadata.required_pkgs == ["xgboost"]
-    assert not v.metadata.user
-
-
-def test_vetiver_build(vetiver_client):
+def test_vetiver_build(client):
     data = mtcars.head(1).drop(columns="mpg")
 
-    response = vetiver.predict(endpoint=vetiver_client, data=data)
+    response = vetiver.predict(endpoint="/predict/", data=data, test_client=client)
 
     assert response.iloc[0, 0] == PREDICT_VALUE
     assert len(response) == 1
 
 
-def test_batch(vetiver_client):
+def test_batch(client):
     data = mtcars.head(3).drop(columns="mpg")
 
-    response = vetiver.predict(endpoint=vetiver_client, data=data)
+    response = vetiver.predict(endpoint="/predict/", data=data, test_client=client)
 
     assert response.iloc[0, 0] == PREDICT_VALUE
     assert len(response) == 3
 
 
-def test_no_ptype(vetiver_client_check_ptype_false):
+def test_no_ptype(client_no_prototype):
     data = mtcars.head(1).drop(columns="mpg")
 
-    response = vetiver.predict(endpoint=vetiver_client_check_ptype_false, data=data)
-
+    response = vetiver.predict(
+        endpoint="/predict/", data=data, test_client=client_no_prototype
+    )
     assert response.iloc[0, 0] == PREDICT_VALUE
     assert len(response) == 1
 
 
-def test_serialize(xgb_model):
+def test_serialize(model):
     import pins
 
     board = pins.board_temp(allow_pickle_read=True)
-    vetiver.vetiver_pin_write(board=board, model=xgb_model)
+    vetiver.vetiver_pin_write(board=board, model=model)
     assert isinstance(
         board.pin_read("xgb"),
         xgb.Booster,
     )
     board.pin_delete("xgb")
```

### Comparing `vetiver-0.2.4/vetiver/vetiver_model.py` & `vetiver-0.2.5/vetiver/vetiver_model.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/write_docker.py` & `vetiver-0.2.5/vetiver/write_docker.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver/write_fastapi.py` & `vetiver-0.2.5/vetiver/write_fastapi.py`

 * *Files identical despite different names*

### Comparing `vetiver-0.2.4/vetiver.egg-info/PKG-INFO` & `vetiver-0.2.5/vetiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vetiver
-Version: 0.2.4
+Version: 0.2.5
 Summary: Version, share, deploy, and monitor models.
 Home-page: https://github.com/rstudio/vetiver-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Keywords: data,mlops
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vetiver Version: 0.2.4 Summary: Version, share,
+Metadata-Version: 2.1 Name: vetiver Version: 0.2.5 Summary: Version, share,
 deploy, and monitor models. Home-page: https://github.com/rstudio/vetiver-
 python Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co
 License: MIT Keywords: data,mlops Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: pandas
 Requires-Dist: fastapi Requires-Dist: pydantic Requires-Dist: joblib Requires-
```

### Comparing `vetiver-0.2.4/vetiver.egg-info/SOURCES.txt` & `vetiver-0.2.5/vetiver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -79,22 +79,22 @@
 vetiver/handlers/sklearn.py
 vetiver/handlers/spacy.py
 vetiver/handlers/statsmodels.py
 vetiver/handlers/torch.py
 vetiver/handlers/xgboost.py
 vetiver/templates/model_card.qmd
 vetiver/templates/monitoring_dashboard.qmd
+vetiver/tests/__init__.py
+vetiver/tests/conftest.py
 vetiver/tests/rsconnect_api_keys.json
 vetiver/tests/test_add_endpoint.py
-vetiver/tests/test_build_api.py
 vetiver/tests/test_build_vetiver_model.py
 vetiver/tests/test_custom_handler.py
 vetiver/tests/test_mock_data.py
 vetiver/tests/test_monitor.py
-vetiver/tests/test_no_handler.py
 vetiver/tests/test_pin_write.py
 vetiver/tests/test_prepare_docker.py
 vetiver/tests/test_pytorch.py
 vetiver/tests/test_rsconnect.py
 vetiver/tests/test_server.py
 vetiver/tests/test_sklearn.py
 vetiver/tests/test_spacy.py
```

