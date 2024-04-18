# Comparing `tmp/OctoBot-Tentacles-Manager-2.9.8.tar.gz` & `tmp/OctoBot-Tentacles-Manager-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.8.tar", last modified: Wed Jan 10 13:21:15 2024, max compression
+gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.9.tar", last modified: Thu Jan 18 15:55:42 2024, max compression
```

## Comparing `OctoBot-Tentacles-Manager-2.9.8.tar` & `OctoBot-Tentacles-Manager-2.9.9.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.688673 OctoBot-Tentacles-Manager-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.672673 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-10 13:21:15.000000 OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-10 13:21:15.688673 OctoBot-Tentacles-Manager-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.672673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/util/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/util/tentacles_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22513 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/compiled_package_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Mode_config.template
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Social_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Strategies_config.template
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/TA_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Util_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/description_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/artifact_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.676673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/loaders/tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.680673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/profiles_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.680673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.680673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/artifact_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/metadata_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/profile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_requirements_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.680673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/s3_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.680673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_fetching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/install_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/repair_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/single_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/tentacles_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/update_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-10 13:21:15.688673 OctoBot-Tentacles-Manager-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.672673 OctoBot-Tentacles-Manager-2.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/api/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/configuration/test_tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/configuration/test_tentacles_setup_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/exporters/test_tentacle_bundle_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/loaders/test_tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/managers/test_tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/util/test_tentacle_fetching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.684673 OctoBot-Tentacles-Manager-2.9.8/tests/workers/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_update_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 13:21:15.688673 OctoBot-Tentacles-Manager-2.9.8/upload_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/upload_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/upload_tests/_test_nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-10 13:20:41.000000 OctoBot-Tentacles-Manager-2.9.8/upload_tests/test_s3_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.865266 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-18 15:55:42.000000 OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.869267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.869267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.869267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/util/tentacles_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.869267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22513 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.869267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/compiled_package_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.873267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Mode_config.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Social_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Strategies_config.template
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/TA_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Util_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/description_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.873267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/artifact_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.873267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/loaders/tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.873267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/profiles_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.873267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.877267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/artifact_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/metadata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/profile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_requirements_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.877267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/s3_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.877267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.877267 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/repair_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/single_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/tentacles_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/update_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-18 15:55:42.885267 OctoBot-Tentacles-Manager-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.865266 OctoBot-Tentacles-Manager-2.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/api/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/configuration/test_tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/configuration/test_tentacles_setup_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/exporters/test_tentacle_bundle_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/loaders/test_tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/managers/test_tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/util/test_tentacle_fetching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/tests/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_update_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 15:55:42.881267 OctoBot-Tentacles-Manager-2.9.9/upload_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/upload_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/upload_tests/_test_nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-18 15:55:10.000000 OctoBot-Tentacles-Manager-2.9.9/upload_tests/test_s3_uploader.py
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/CHANGELOG.md` & `OctoBot-Tentacles-Manager-2.9.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.9.9] - 2023-01-18
+### Updated
+- tentacles: log url on fetching error
+
 ## [2.9.8] - 2023-01-10
 ### Updated
 - tentacles: log artifact modification date and hash
 
 ## [2.9.7] - 2023-01-09
 ### Updated
 - dependencies
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/LICENSE` & `OctoBot-Tentacles-Manager-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.8
+Version: 2.9.9
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Tentacles-Manager [2.9.8](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.9](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt` & `OctoBot-Tentacles-Manager-2.9.9/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.8
+Version: 2.9.9
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Tentacles-Manager [2.9.8](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.9](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/README.md` & `OctoBot-Tentacles-Manager-2.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Tentacles-Manager [2.9.8](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.9](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-VERSION = "2.9.8"
+VERSION = "2.9.9"
 PROJECT_NAME = "OctoBot-Tentacles-Manager"
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/configurator.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/creator.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/inspector.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/installer.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/loader.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/loader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/updater.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/api/util/tentacles_management.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/api/util/tentacles_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/cli.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/config_file.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/config_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/constants.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/compiled_package_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/compiled_package_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Mode_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Mode_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/templates/Social_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/templates/Social_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/creators/tentacle_creator.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/creators/tentacle_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/enums.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/artifact_exporter.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/artifact_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/exporters/tentacle_package_exporter.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/exporters/tentacle_package_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/loaders/tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/loaders/tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/profiles_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/profiles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/python_modules_requirements_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/python_modules_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacle_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacle_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacles_init_files_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacles_init_files_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/managers/tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/managers/tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/artifact.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/artifact.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/artifact_metadata.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/artifact_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/metadata_factory.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/metadata_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/profile_metadata.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/profile_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/tentacle_metadata.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/tentacle_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/profile.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_factory.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_package.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_requirements_tree.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_requirements_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/models/tentacle_type.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/models/tentacle_type.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/uploaders/uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/uploaders/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/file_util.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/file_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/hashing.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/hashing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/os_util.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_cleaner.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_cleaner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_explorer.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_explorer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_fetching.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  License along with this library.
 import aiofiles
 import zipfile
 import os
 import os.path as path
 import shutil
 
+import octobot_commons.logging as commons_logging
 import octobot_commons.aiohttp_util as aiohttp_util
 import octobot_tentacles_manager.constants as constants
 import octobot_tentacles_manager.util as util
 
 DOWNLOADED_DATA_CHUNK_SIZE = 60000
 
 
@@ -33,14 +34,19 @@
         if should_download:
             if aiohttp_session is None:
                 raise RuntimeError("Missing aiohttp_session argument")
             compressed_file = f"downloaded_{tentacles_temp_dir}"
             last_modified = await _download_tentacles(compressed_file, tentacles_path_or_url, aiohttp_session)
             await util.log_tentacles_file_details(compressed_file, last_modified)
         await _extract_tentacles(compressed_file, tentacles_temp_dir, merge_dirs)
+    except Exception as err:
+        commons_logging.get_logger("TentaclesFetching").warning(
+            f"Error when fetching tentacles from {tentacles_path_or_url}: {err} ({err.__class__.__name__})"
+        )
+        raise
     finally:
         if should_download and path.isfile(compressed_file):
             os.remove(compressed_file)
 
 
 def cleanup_temp_dirs(target_path):
     if path.exists(target_path):
```

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/util/tentacle_filter.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/util/tentacle_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/install_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/repair_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/repair_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/single_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/single_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/tentacles_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/tentacles_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/octobot_tentacles_manager/workers/update_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/octobot_tentacles_manager/workers/update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/setup.py` & `OctoBot-Tentacles-Manager-2.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/test_configurator.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/test_configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/test_creator.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/test_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/test_installer.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/test_installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/test_uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/test_uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/api/test_updater.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/api/test_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/configuration/test_tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/configuration/test_tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/configuration/test_tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/configuration/test_tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/exporters/test_tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/exporters/test_tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/loaders/test_tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/loaders/test_tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/managers/test_tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/managers/test_tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/util/test_tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/util/test_tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/tests/workers/test_update_worker.py` & `OctoBot-Tentacles-Manager-2.9.9/tests/workers/test_update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/upload_tests/__init__.py` & `OctoBot-Tentacles-Manager-2.9.9/upload_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/upload_tests/_test_nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/upload_tests/_test_nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.8/upload_tests/test_s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.9/upload_tests/test_s3_uploader.py`

 * *Files identical despite different names*

