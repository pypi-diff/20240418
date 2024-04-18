# Comparing `tmp/copernicusmarine-1.1.0.tar.gz` & `tmp/copernicusmarine-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.1.0.tar", max compression
+gzip compressed data, was "copernicusmarine-1.1.1.tar", max compression
```

## Comparing `copernicusmarine-1.1.0.tar` & `copernicusmarine-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0    13827 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0    27828 2024-04-05 08:12:37.399094 copernicusmarine-1.1.0/README.md
--rw-r--r--   0        0        0      972 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    32697 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11545 2024-04-02 16:01:38.670061 copernicusmarine-1.1.0/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     3784 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9618 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3037 2024-04-04 15:12:27.177965 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12732 2024-04-02 16:01:38.670061 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    12954 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     4455 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2806 2024-04-02 12:36:55.419847 copernicusmarine-1.1.0/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2385 2024-04-02 12:36:55.419847 copernicusmarine-1.1.0/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2132 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0      603 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     7622 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    18522 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     1710 2024-03-28 08:53:43.597785 copernicusmarine-1.1.0/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0     9735 2024-04-04 15:26:44.853507 copernicusmarine-1.1.0/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     5528 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2646 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2484 2024-04-02 16:01:38.670061 copernicusmarine-1.1.0/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     8009 2024-04-02 16:01:38.670061 copernicusmarine-1.1.0/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0     1706 2024-03-28 15:56:59.209743 copernicusmarine-1.1.0/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0    15349 2024-04-04 15:26:44.857507 copernicusmarine-1.1.0/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    18095 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5567 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     1961 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5817 2024-04-02 12:36:55.419847 copernicusmarine-1.1.0/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     3545 2024-04-04 15:26:44.857507 copernicusmarine-1.1.0/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0      731 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6469 2024-04-04 15:26:44.857507 copernicusmarine-1.1.0/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6150 2024-04-04 15:26:44.857507 copernicusmarine-1.1.0/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6620 2024-04-02 16:01:38.670061 copernicusmarine-1.1.0/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-03-28 08:16:08.728348 copernicusmarine-1.1.0/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      901 2024-04-05 09:26:56.440706 copernicusmarine-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    29633 1970-01-01 00:00:00.000000 copernicusmarine-1.1.0/setup.py
--rw-r--r--   0        0        0    28850 1970-01-01 00:00:00.000000 copernicusmarine-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0    29145 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/README.md
+-rw-r--r--   0        0        0      972 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    28918 2024-04-17 11:09:20.414412 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11545 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     3784 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9616 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3033 2024-04-17 11:09:20.414412 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12730 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13437 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     4455 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2806 2024-04-02 15:26:12.686202 copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2385 2024-04-02 15:26:12.686202 copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2132 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0     1233 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/environment_variables.py
+-rw-r--r--   0        0        0      603 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     7622 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    19332 2024-04-18 13:58:11.735885 copernicusmarine-1.1.1/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     2132 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0     9735 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     5614 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2683 2024-04-17 11:09:20.418412 copernicusmarine-1.1.1/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2484 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     8009 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0     1706 2024-03-28 15:56:56.847755 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0    15349 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    18583 2024-04-18 13:58:11.735885 copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5567 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     1961 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5817 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     3545 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0      731 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6469 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6150 2024-04-04 15:26:42.410893 copernicusmarine-1.1.1/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6620 2024-04-03 07:33:56.619712 copernicusmarine-1.1.1/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-03-28 08:53:31.384112 copernicusmarine-1.1.1/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      901 2024-04-18 14:17:59.870855 copernicusmarine-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    30966 1970-01-01 00:00:00.000000 copernicusmarine-1.1.1/setup.py
+-rw-r--r--   0        0        0    30167 1970-01-01 00:00:00.000000 copernicusmarine-1.1.1/PKG-INFO
```

### Comparing `copernicusmarine-1.1.0/LICENSE.txt` & `copernicusmarine-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/README.md` & `copernicusmarine-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,34 @@
 ### General configuration
 
 #### Cache Usage
 Cachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:
 - on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
 - on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
 
+### Network configuration
+
 #### Disable SSL
+
 A global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:
+
 - on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
 - on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
 
+#### Trust Env for python libraries
+
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries: requests and aiohttp. By default, those libraries will have `trust_env` values set to `True`. If you want to deactivate this, you can set `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for example if you don't want those libraries to read your `.netrc` file as it has been reported that having a `.netrc` with a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox.
+
+#### Proxy
+
+To use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:
+
+- set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.
+- use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.
+
 ## Command Line Interface (CLI)
 
 ### The `--help` option
 To discover commands and their available options, consider appending `--help` on any command line.
 
 Example:
 ```bash
```

#### html2text {}

```diff
@@ -33,33 +33,51 @@
 existing users of legacy services such as MOTU, OPeNDAP or FTP. ### General
 configuration #### Cache Usage Cachier library is used for caching part of the
 requests (as result of `describe` or `login`). By default, the cache will be
 located in the home folder. If you need to change the location of the cache,
 you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to
 point to the desired directory: - on **UNIX** platforms: `export
 COPERNICUSMARINE_CACHE_DIRECTORY=` - on **Windows** platforms: `set
-COPERNICUSMARINE_CACHE_DIRECTORY=` #### Disable SSL A global SSL context is
-used when making HTTP calls using the `copernicusmarine` Toolbox. For some
-reason, it can lead to unexpected behavior depending on your network
-configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
+COPERNICUSMARINE_CACHE_DIRECTORY=` ### Network configuration #### Disable SSL A
+global SSL context is used when making HTTP calls using the `copernicusmarine`
+Toolbox. For some reason, it can lead to unexpected behavior depending on your
+network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
 environment variable to any value to globally disable the usage of SSL in the
 toolbox: - on **UNIX** platforms: `export
 COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` - on **Windows** platforms: `set
-COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` ## Command Line Interface (CLI) ###
-The `--help` option To discover commands and their available options, consider
-appending `--help` on any command line. Example: ```bash copernicusmarine --
-help ``` Returns: ```bash Usage: copernicusmarine [OPTIONS] COMMAND [ARGS]...
-Options: -V, --version Show the version and exit. -h, --help Show this message
-and exit. Commands: describe Print Copernicus Marine catalog as JSON. get
-Download originally produced data files. login Create a configuration file with
-your Copernicus Marine credentials. subset Download subsets of datasets as
-NetCDF files or Zarr stores. ``` ### Command `describe` Retrieve metadata
-information about all products/datasets and display as JSON output: ```bash
-copernicusmarine describe --include-datasets ``` The JSON output can also be
-saved as follows: ```bash copernicusmarine describe --include-datasets >
+COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` #### Trust Env for python libraries
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries:
+requests and aiohttp. By default, those libraries will have `trust_env` values
+set to `True`. If you want to deactivate this, you can set
+`COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for
+example if you don't want those libraries to read your `.netrc` file as it has
+been reported that having a `.netrc` with a line: "default login anonymous
+password user@site" is incompatible with S3 connection required by the toolbox.
+#### Proxy To use proxies, as describe in the [aiohttp documentation](https://
+docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two
+options: - set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:
+pass@some.proxy.com"`. It should work even with
+`COPERNICUSMARINE_TRUST_ENV=False`. - use a `.netrc` file but be aware that
+having a line: "default login anonymous password user@site" is incompatible
+with S3 connection required by the toolbox. Also note that if you have
+`COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC`
+environment variable is set with a specified location, the `.netrc` file will
+be read from the specified location there rather than from `~/.netrc`. ##
+Command Line Interface (CLI) ### The `--help` option To discover commands and
+their available options, consider appending `--help` on any command line.
+Example: ```bash copernicusmarine --help ``` Returns: ```bash Usage:
+copernicusmarine [OPTIONS] COMMAND [ARGS]... Options: -V, --version Show the
+version and exit. -h, --help Show this message and exit. Commands: describe
+Print Copernicus Marine catalog as JSON. get Download originally produced data
+files. login Create a configuration file with your Copernicus Marine
+credentials. subset Download subsets of datasets as NetCDF files or Zarr
+stores. ``` ### Command `describe` Retrieve metadata information about all
+products/datasets and display as JSON output: ```bash copernicusmarine describe
+--include-datasets ``` The JSON output can also be saved as follows: ```bash
+copernicusmarine describe --include-datasets >
 all_datasets_copernicusmarine.json ``` ### Command `login` Create a single
 configuration file `.copernicusmarine-credentials` allowing to access all
 Copernicus Marine Data Store data services. By default, the file is saved in
 user's home directory. Example: ```bash > copernicusmarine login username :
 johndoe password : INFO - Configuration files stored in /Users/
 foo/.copernicusmarine ``` If `.copernicusmarine-credentials` already exists,
 the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/__init__.py` & `copernicusmarine-1.1.1/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.1.1/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.1.1/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import asyncio
 import logging
-import os
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import Enum
 from importlib.metadata import version as package_version
 from itertools import groupby
-from typing import Any, Dict, Iterator, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import nest_asyncio
 import pystac
-from aiohttp import ContentTypeError
+from aiohttp import ContentTypeError, ServerDisconnectedError
 from cachier.core import cachier
 from tqdm import tqdm
 
 from copernicusmarine.aioretry import RetryInfo, RetryPolicyStrategy, retry
 from copernicusmarine.command_line_interface.exception_handler import (
     log_exception_debug,
 )
+from copernicusmarine.core_functions.environment_variables import (
+    COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS,
+)
 from copernicusmarine.core_functions.sessions import (
     get_configured_aiohttp_session,
+    get_https_proxy,
 )
 from copernicusmarine.core_functions.utils import (
     CACHE_BASE_DIRECTORY,
     construct_query_params_for_marine_data_store_monitoring,
     datetime_parser,
     map_reject_none,
     next_or_raise_exception,
     rolling_batch_gather,
 )
 
 logger = logging.getLogger("copernicus_marine_root_logger")
 
-_S = TypeVar("_S")
-_T = TypeVar("_T")
-
 
 class _ServiceName(str, Enum):
     GEOSERIES = "arco-geo-series"
     TIMESERIES = "arco-time-series"
     FILES = "original-files"
     WMTS = "wmts"
     OMI_ARCO = "omi-arco"
@@ -63,17 +63,15 @@
 MARINE_DATA_STORE_STAC_BASE_URL_STAGING = (
     "https://stac-dta.marine.copernicus.eu/metadata"
 )
 MARINE_DATA_STORE_STAC_ROOT_CATALOG_URL_STAGING = (
     MARINE_DATA_STORE_STAC_BASE_URL_STAGING + "/catalog.stac.json"
 )
 
-MAX_CONCURRENT_REQUESTS = int(
-    os.getenv("COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS", "15")
-)
+MAX_CONCURRENT_REQUESTS = int(COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS)
 
 
 @dataclass(frozen=True)
 class _Service:
     service_name: _ServiceName
     short_name: _ServiceShortName
 
@@ -361,36 +359,39 @@
         return filter_catalogue_with_strings(self, tokens)
 
 
 class CatalogParserConnection:
     def __init__(self, proxy: Optional[str] = None) -> None:
         self.proxy = proxy
         self.session = get_configured_aiohttp_session()
+        self.proxy = get_https_proxy()
         self.__max_retries = 5
         self.__sleep_time = 1
 
     @retry("_retry_policy")
     async def get_json_file(self, url: str) -> dict[str, Any]:
         logger.debug(f"Fetching json file at this url: {url}")
         async with self.session.get(
             url,
             params=construct_query_params_for_marine_data_store_monitoring(),
+            proxy=self.proxy,
         ) as response:
             return await response.json()
 
     async def close(self) -> None:
         await self.session.close()
 
     def _retry_policy(self, info: RetryInfo) -> RetryPolicyStrategy:
         if not isinstance(
             info.exception,
             (
                 TimeoutError,
                 ConnectionResetError,
                 ContentTypeError,
+                ServerDisconnectedError,
             ),
         ):
             logger.error(
                 f"Unexpected error while downloading: {info.exception}"
             )
             return True, 0
         logger.debug(
@@ -815,141 +816,24 @@
 
     progress_bar.update()
     asyncio.run(connection.close())
 
     return full_catalog
 
 
-def variable_title_to_standard_name(variable_title: str) -> str:
-    return variable_title.lower().replace(" ", "_")
-
-
-def variable_to_pick(layer: dict[str, Any]) -> bool:
-    return (
-        layer["variableId"] != "__DEFAULT__"
-        and layer["subsetVariableIds"]
-        and len(layer["subsetVariableIds"]) == 1
-    )
-
-
-def _to_service(
-    service_name: str,
-    stac_asset: dict,
-    layer_elements,
-) -> Optional[CopernicusMarineService]:
-    service_format_asset = stac_asset.get("type")
-    service_url = stac_asset.get("href")
-    try:
-        service_type = _service_type_from_web_api_string(service_name)
-        service_format = None
-        if service_format_asset and "zarr" in service_format_asset:
-            service_format = CopernicusMarineServiceFormat.ZARR
-        elif service_format_asset and "sqlite3" in service_format_asset:
-            service_format = CopernicusMarineServiceFormat.SQLITE
-        if service_url and not service_url.endswith("thredds/dodsC/"):
-            return CopernicusMarineService(
-                service_type=service_type,
-                uri=service_url,
-                service_format=service_format,
-                variables=[
-                    to_variable(layer, stac_asset)
-                    for layer in layer_elements
-                    if variable_to_pick(layer)
-                ],
-            )
-        else:
-            return None
-    except ServiceNotHandled as service_not_handled:
-        log_exception_debug(service_not_handled)
-        return None
-
-
-def to_coordinates(
-    subset_attributes: Tuple[str, dict[str, Any]],
-    layer: dict[str, Any],
-    asset: dict,
-) -> CopernicusMarineCoordinates:
-    coordinate_name = subset_attributes[0]
-    values: Optional[str]
-    if coordinate_name == "depth":
-        values = layer.get("zValues")
-    elif coordinate_name == "time":
-        values = layer.get("tValues")
-    else:
-        values = None
-    view_dim = asset.get("viewDims", {}).get(coordinate_name, {})
-    chunking_length = view_dim.get("chunkLen")
-    if isinstance(chunking_length, dict):
-        chunking_length = chunking_length.get(layer["variableId"])
-    return CopernicusMarineCoordinates(
-        coordinates_id=subset_attributes[0],
-        units=view_dim.get("units", ""),
-        minimum_value=view_dim.get("min") or view_dim.get(values, [None])[0],
-        maximum_value=view_dim.get("max") or view_dim.get(values, [None])[0],
-        step=view_dim.get("step"),
-        values=values,
-        chunking_length=chunking_length,
-        chunk_type=view_dim.get("chunkType"),
-        chunk_reference_coordinate=view_dim.get("chunkRefCoord"),
-        chunk_geometric_factor=view_dim.get("chunkGeometricFactor", {})
-        .get("chunkGeometricFactor", {})
-        .get(layer["variableId"]),
-    )
-
-
-def to_variable(
-    layer: dict[str, Any], asset: dict
-) -> CopernicusMarineVariable:
-    return CopernicusMarineVariable(
-        short_name=layer["variableId"],
-        standard_name=variable_title_to_standard_name(layer["variableTitle"]),
-        units=layer["units"],
-        bbox=layer["bbox"],
-        coordinates=[
-            to_coordinates(subset_attr, layer, asset)
-            for subset_attr in layer["subsetAttrs"].items()
-        ],
-    )
-
-
 @dataclass
 class DistinctDatasetVersionPart:
     dataset_id: str
     dataset_version: str
     dataset_part: str
     layer_elements: List
     raw_services: Dict
     stac_items_values: Optional[Dict]
 
 
-def mds_stac_to_services(
-    distinct_dataset_version: DistinctDatasetVersionPart,
-) -> List[CopernicusMarineService]:
-    copernicus_marine_services = []
-
-    stac_assets = (
-        distinct_dataset_version.stac_items_values
-        and distinct_dataset_version.stac_items_values.get("assets", None)
-    )
-    if stac_assets:
-        for (
-            service_name,
-            service_url,
-        ) in stac_assets.items():
-            service = _to_service(
-                service_name,
-                service_url,
-                distinct_dataset_version.layer_elements,
-            )
-            if service:
-                copernicus_marine_services.append(service)
-
-    return copernicus_marine_services
-
-
 REGEX_PATTERN_DATE_YYYYMM = r"[12]\d{3}(0[1-9]|1[0-2])"
 PART_SEPARATOR = "--ext--"
 
 
 def get_version_and_part_from_full_dataset_id(
     full_dataset_id: str,
 ) -> Tuple[str, str, str]:
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.1.1/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,23 +70,23 @@
 @force_dataset_version_option
 @force_dataset_part_option
 @click.option(
     "--username",
     type=str,
     default=None,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + " COPERNICUSMARINE_SERVICE_USERNAME"
     + ", or else look for configuration files, or else ask for user input.",
 )
 @click.option(
     "--password",
     type=str,
     default=None,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + " COPERNICUSMARINE_SERVICE_PASSWORD"
     + ", or else look for configuration files, or else ask for user input.",
 )
 @click.option(
     "--no-directories",
     "-nd",
     cls=MutuallyExclusiveOption,
     is_flag=True,
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,37 +26,37 @@
 
     Create a configuration file under the $HOME/.copernicusmarine directory (overwritable with option --credentials-file).
     """,  # noqa
     epilog="""
     Examples:
 
     \b
-    COPERNICUS_MARINE_SERVICE_USERNAME=<USERNAME> COPERNICUS_MARINE_SERVICE_PASSWORD=<PASSWORD> copernicusmarine login
+    COPERNICUSMARINE_SERVICE_USERNAME=<USERNAME> COPERNICUSMARINE_SERVICE_PASSWORD=<PASSWORD> copernicusmarine login
 
     \b
     copernicusmarine login --username <USERNAME> --password <PASSWORD>
 
     \b
     copernicusmarine login
     > Username: [USER-INPUT]
     > Password: [USER-INPUT]
     """,  # noqa
 )
 @click.option(
     "--username",
     hide_input=False,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + " COPERNICUSMARINE_SERVICE_USERNAME"
     + ", or else ask for user input.",
 )
 @click.option(
     "--password",
     hide_input=True,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + " COPERNICUSMARINE_SERVICE_PASSWORD"
     + ", or else ask for user input.",
 )
 @click.option(
     "--configuration-file-directory",
     type=click.Path(path_type=pathlib.Path),
     default=DEFAULT_CLIENT_BASE_DIRECTORY,
     help="Path to the directory where the configuration file is stored.",
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/group_subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,23 +89,23 @@
 @force_dataset_version_option
 @force_dataset_part_option
 @click.option(
     "--username",
     type=str,
     default=None,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_USERNAME"
+    + " COPERNICUSMARINE_SERVICE_USERNAME"
     + ", or else look for configuration files, or else ask for user input.",
 )
 @click.option(
     "--password",
     type=str,
     default=None,
     help="If not set, search for environment variable"
-    + " COPERNICUS_MARINE_SERVICE_PASSWORD"
+    + " COPERNICUSMARINE_SERVICE_PASSWORD"
     + ", or else look for configuration files, or else ask for user input.",
 )
 @click.option(
     "--variable",
     "-v",
     "variables",
     type=str,
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.1.1/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/credentials_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import base64
 import configparser
 import logging
-import os
 import pathlib
 from datetime import timedelta
 from netrc import netrc
 from platform import system
 from typing import Literal, Optional, Tuple
 
 import click
 import lxml.html
 import requests
 from cachier.core import cachier
 
+from copernicusmarine.core_functions.environment_variables import (
+    COPERNICUSMARINE_SERVICE_PASSWORD,
+    COPERNICUSMARINE_SERVICE_USERNAME,
+)
 from copernicusmarine.core_functions.sessions import (
     get_configured_request_session,
 )
 from copernicusmarine.core_functions.utils import (
     CACHE_BASE_DIRECTORY,
     DEFAULT_CLIENT_BASE_DIRECTORY,
 )
@@ -88,19 +91,18 @@
 
 
 def _retrieve_credential_from_environment_variable(
     credential_type: Literal["username", "password"]
 ) -> Optional[str]:
     if credential_type == "username":
         logger.debug("username loaded from environment variable")
-        return os.getenv("COPERNICUS_MARINE_SERVICE_USERNAME")
+        return COPERNICUSMARINE_SERVICE_USERNAME
     if credential_type == "password":
         logger.debug("password loaded from environment variable")
-        return os.getenv("COPERNICUS_MARINE_SERVICE_PASSWORD")
-    return None
+        return COPERNICUSMARINE_SERVICE_PASSWORD
 
 
 def _retrieve_credential_from_custom_configuration_files(
     credential_type: Literal["username", "password"],
     credentials_file: pathlib.Path,
     host: str = "default_host",
 ) -> Optional[str]:
@@ -227,27 +229,31 @@
 def _check_credentials_with_cas(username: str, password: str) -> bool:
     logger.debug("Checking user credentials...")
     service = "copernicus-marine-client"
     cmems_cas_login_url = (
         f"https://cmems-cas.cls.fr/cas/login?service={service}"
     )
     conn_session = get_configured_request_session()
-    login_session = conn_session.get(cmems_cas_login_url)
+    login_session = conn_session.get(
+        cmems_cas_login_url, proxies=conn_session.proxies
+    )
     login_from_html = lxml.html.fromstring(login_session.text)
     hidden_elements_from_html = login_from_html.xpath(
         '//form//input[@type="hidden"]'
     )
     playload = {
         he.attrib["name"]: he.attrib["value"]
         for he in hidden_elements_from_html
     }
     playload["username"] = username
     playload["password"] = password
     logger.debug(f"POSTing credentials to {cmems_cas_login_url}...")
-    login_response = conn_session.post(cmems_cas_login_url, data=playload)
+    login_response = conn_session.post(
+        cmems_cas_login_url, data=playload, proxies=conn_session.proxies
+    )
     login_success = 'class="success"' in login_response.text
     logger.debug("User credentials checked")
     return login_success
 
 
 @cachier(stale_after=timedelta(hours=48), cache_dir=CACHE_BASE_DIRECTORY)
 def _are_copernicus_marine_credentials_valid(
@@ -277,22 +283,28 @@
         credential = _retrieve_credential_from_environment_variable(
             credential_type
         )
         if not credential:
             credential = _retrieve_credential_from_configuration_files(
                 credential_type=credential_type,
                 credentials_file=credentials_file,
-                host="my.cmems-du.eu",
+                host="nrt.cmems-du.eu",
             )
             if not credential:
-                credential = _retrieve_credential_from_prompt(
-                    credential_type, hide_input=hide_input
+                credential = _retrieve_credential_from_configuration_files(
+                    credential_type=credential_type,
+                    credentials_file=credentials_file,
+                    host="my.cmems-du.eu",
                 )
                 if not credential:
-                    raise ValueError(f"{credential} cannot be None")
+                    credential = _retrieve_credential_from_prompt(
+                        credential_type, hide_input=hide_input
+                    )
+                    if not credential:
+                        raise ValueError(f"{credential} cannot be None")
     else:
         logger.debug("Credentials loaded from function arguments")
     return credential
 
 
 def get_and_check_username_password(
     username: Optional[str],
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/exceptions.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/exceptions.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/services_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -464,14 +464,19 @@
         force_part=force_dataset_part_label
     )
     if not force_dataset_part_label:
         logger.info(
             "Dataset part was not specified, the first "
             f'one was selected: "{dataset_part.name}"'
         )
+    if dataset_part.retired_date:
+        warning_dataset_will_be_deprecated(
+            dataset_id, dataset_version, dataset_part
+        )
+
     if force_service_type:
         logger.info(
             f"You forced selection of service: "
             f"{force_service_type.service_name.value}"
         )
         service = _select_forced_service(
             dataset_version_part=dataset_part,
@@ -515,14 +520,31 @@
     return None
 
 
 class ServiceNotAvailable(Exception):
     ...
 
 
+def warning_dataset_will_be_deprecated(
+    dataset_id: str,
+    dataset_version: CopernicusMarineDatasetVersion,
+    dataset_part: CopernicusMarineVersionPart,
+):
+    logger.warn(
+        f"""The dataset {dataset_id}"""
+        f"""{f", version '{dataset_version.label}'"
+             if dataset_version.label != 'default' else ''}"""
+        f"""{(f"and part '{dataset_part.name}'"
+              if dataset_part.name != 'default' else '')}"""
+        f"""{"," if dataset_version.label != 'default' else ""}"""
+        f""" will be retired on the {dataset_part.retired_date}."""
+        """ After this date, it will no longer be available on the toolbox."""
+    )
+
+
 def _service_not_available_error(
     dataset_version_part: CopernicusMarineVersionPart,
     command_type: CommandType,
 ) -> ServiceNotAvailable:
     dataset_available_service_types = [
         service.service_type.short_name.value
         for service in dataset_version_part.services
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/sessions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,57 @@
-import os
 import ssl
 from typing import Optional
 
 import aiohttp
 import certifi
 import nest_asyncio
 import requests
 import xarray
 
 from copernicusmarine.core_functions.custom_zarr_store import CustomS3Store
+from copernicusmarine.core_functions.environment_variables import (
+    COPERNICUSMARINE_DISABLE_SSL_CONTEXT,
+    COPERNICUSMARINE_TRUST_ENV,
+    PROXY_HTTP,
+    PROXY_HTTPS,
+)
 from copernicusmarine.core_functions.utils import (
     construct_query_params_for_marine_data_store_monitoring,
     parse_access_dataset_url,
 )
 
-TRUST_ENV = True
+TRUST_ENV = COPERNICUSMARINE_TRUST_ENV == "True"
+PROXIES = {}
+if PROXY_HTTP:
+    PROXIES["http"] = PROXY_HTTP
+if PROXY_HTTPS:
+    PROXIES["https"] = PROXY_HTTPS
 
 
 def _get_ssl_context() -> Optional[ssl.SSLContext]:
-    if os.getenv("COPERNICUSMARINE_DISABLE_SSL_CONTEXT") is not None:
+    if COPERNICUSMARINE_DISABLE_SSL_CONTEXT is not None:
         return None
     return ssl.create_default_context(cafile=certifi.where())
 
 
 def get_configured_aiohttp_session() -> aiohttp.ClientSession:
     nest_asyncio.apply()
     connector = aiohttp.TCPConnector(ssl=_get_ssl_context())
     return aiohttp.ClientSession(connector=connector, trust_env=TRUST_ENV)
 
 
+def get_https_proxy() -> Optional[str]:
+    return PROXIES.get("https")
+
+
 def get_configured_request_session() -> requests.Session:
     session = requests.Session()
     session.trust_env = TRUST_ENV
     session.verify = certifi.where()
+    session.proxies = PROXIES
     return session
 
 
 def open_zarr(
     dataset_url: str,
     copernicus_marine_username: Optional[str] = None,
     **kwargs,
@@ -51,13 +66,13 @@
     )
     kwargs.update(
         {
             "storage_options": {
                 "params": construct_query_params_for_marine_data_store_monitoring(
                     username=copernicus_marine_username
                 ),
-                "client_kwargs": {"trust_env": TRUST_ENV},
+                "client_kwargs": {"trust_env": TRUST_ENV, "proxies": PROXIES},
                 "ssl": _get_ssl_context(),
             }
         }
     )
     return xarray.open_zarr(store, **kwargs)
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,30 @@
     TypeVar,
     Union,
 )
 
 import xarray
 from requests import PreparedRequest
 
+from copernicusmarine.core_functions.environment_variables import (
+    COPERNICUSMARINE_CACHE_DIRECTORY,
+)
+
 logger = logging.getLogger("copernicus_marine_root_logger")
 
 OVERWRITE_SHORT_OPTION = "--overwrite"
 OVERWRITE_LONG_OPTION = "--overwrite-output-data"
 OVERWRITE_OPTION_HELP_TEXT = (
     "If specified and if the file already exists on destination, then it will be "
     "overwritten instead of creating new one with unique index."
 )
 
 FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE = "Do you want to proceed with download?"
 
-USER_DEFINED_CACHE_DIRECTORY = os.getenv(
-    "COPERNICUSMARINE_CACHE_DIRECTORY", ""
-)
+USER_DEFINED_CACHE_DIRECTORY = COPERNICUSMARINE_CACHE_DIRECTORY
 DEFAULT_CLIENT_BASE_DIRECTORY = (
     pathlib.Path(USER_DEFINED_CACHE_DIRECTORY)
     if USER_DEFINED_CACHE_DIRECTORY
     else pathlib.Path.home()
 ) / ".copernicusmarine"
 
 CACHE_BASE_DIRECTORY = DEFAULT_CLIENT_BASE_DIRECTORY / "cache"
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.1.1/copernicusmarine/core_functions/versions_verifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,9 +66,10 @@
             else "https://stac.marine.copernicus.eu/mdsVersions.json"
         )
         logger.debug(f"Getting required versions from {url_mds_versions}")
         session = get_configured_request_session()
         mds_versions: dict[str, str] = session.get(
             url_mds_versions,
             params=construct_query_params_for_marine_data_store_monitoring(),
+            proxies=session.proxies,
         ).json()["clientVersions"]
         return mds_versions
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/common_download.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_arco_series.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/download_original_files.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/subset_xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,20 +219,33 @@
     depth_parameters: DepthParameters,
 ) -> xarray.Dataset:
     def convert_elevation_to_depth(dataset: xarray.Dataset):
         if "elevation" in dataset.dims:
             attrs = dataset["elevation"].attrs
             dataset = dataset.reindex(elevation=dataset.elevation[::-1])
             dataset["elevation"] = dataset.elevation * (-1)
+            attrs["positive"] = "down"
             dataset = dataset.rename({"elevation": "depth"})
             dataset.depth.attrs = attrs
         return dataset
 
+    def update_elevation_attributes(dataset: xarray.Dataset):
+        if "elevation" in dataset.dims:
+            attrs = dataset["elevation"].attrs
+            attrs["positive"] = "up"
+            attrs["standard_name"] = "elevation"
+            attrs["long_name"] = "Elevation"
+            attrs["units"] = "m"
+            dataset["elevation"].attrs = attrs
+        return dataset
+
     if depth_parameters.vertical_dimension_as_originally_produced:
         dataset = convert_elevation_to_depth(dataset)
+    else:
+        dataset = update_elevation_attributes(dataset)
     minimum_depth = depth_parameters.minimum_depth
     maximum_depth = depth_parameters.maximum_depth
     if minimum_depth is not None or maximum_depth is not None:
         coords = (
             dataset.coords if isinstance(dataset, xarray.Dataset) else dataset
         )
         if "elevation" in coords:
```

### Comparing `copernicusmarine-1.1.0/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.1.1/copernicusmarine/download_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/logging_conf.json` & `copernicusmarine-1.1.1/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/login.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.1.1/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.1.0/pyproject.toml` & `copernicusmarine-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
```

### Comparing `copernicusmarine-1.1.0/setup.py` & `copernicusmarine-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicusmarine = '
                      'copernicusmarine.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicusmarine',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': '',
-    'long_description': '\n<h1 align="center">Copernicus Marine Service Toolbox (CLI & Python)</h1>\n<div align="center">\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>\n  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>\n</div>\n\n![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:\n- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.\n- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.\n- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.\n\n## Installation\nFor installation, multiple options are available depending on your setup:\n\n### Mamba | Conda\nA `conda` package is available on [Anaconda](https://anaconda.org/conda-forge/copernicusmarine).\n\nYou can install it using `mamba` (or conda) through the `conda-forge` channel with the following command:\n```bash\nmamba install conda-forge::copernicusmarine --yes\n```\n\nTo upgrade the Toolbox with mamba (or conda):\n```bash\nmamba update --name copernicusmarine copernicusmarine --yes\n```\n\n### Docker\nA docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nFirst step is to pull the container image:\n```bash\ndocker pull copernicusmarine/copernicusmarine:latest\n```\n\nThen run it:\n```bash\ndocker run -it --rm copernicusmarine/copernicusmarine --version\n```\n\n### Pip\nOtherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the package** to the newest available version, run:\n```bash\npython -m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.\n\n### General configuration\n\n#### Cache Usage\nCachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:\n- on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n- on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n\n#### Disable SSL\nA global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:\n- on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n## Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands and their available options, consider appending `--help` on any command line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\n\nReturns:\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version  Show the version and exit.\n  -h, --help     Show this message and exit.\n\nCommands:\n  describe  Print Copernicus Marine catalog as JSON.\n  get       Download originally produced data files.\n  login     Create a configuration file with your Copernicus Marine credentials.\n  subset    Download subsets of datasets as NetCDF files or Zarr stores.\n```\n\n### Command `describe`\nRetrieve metadata information about all products/datasets and display as JSON output:\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output can also be saved as follows:\n```bash\ncopernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command `login`\nCreate a single configuration file `.copernicusmarine-credentials` allowing to access all Copernicus Marine Data Store data services. By default, the file is saved in user\'s home directory.\n\nExample:\n```bash\n> copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.\n\n#### Access points migration and evolution\nIf you still have a configuration for legacy services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.\nIf the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the files.\n\n### Command `subset`\nRemotely subset a dataset, based on variable names, geographical and temporal parameters.\n\nExample:\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1D-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO - 2024-04-03T10:18:18Z - <xarray.Dataset> Size: 3kB\nDimensions:    (depth: 50, latitude: 2, longitude: 1, time: 3)\nCoordinates:\n  * depth      (depth) float32 200B 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03\n  * latitude   (latitude) float32 8B 28.0 28.08\n  * longitude  (longitude) float32 4B 0.08333\n  * time       (time) datetime64[ns] 24B 2021-01-01 2021-01-02 2021-01-03\nData variables:\n    thetao     (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\n    so         (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\nAttributes: (12/20)\n    Conventions:               CF-1.0\n    bulletin_date:             2020-12-01\n    ...                        ...\n    references:                http://marine.copernicus.eu\n    copernicusmarine_version:  1.1.0\nINFO - 2024-04-03T10:18:18Z - Estimated size of the dataset file is 0.002 MB.\n\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this confirmation, use the option `--force-download`.\n\n#### Note about `--subset-method` option\nBy default, the `subset` feature uses the `nearest` method of xarray. By specifying `--subset-method strict`, you can only request dimension strictly inside the dataset, useful for **operational use-case**.\n\n#### Note about longitude range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.\n- If the requested longitude range:\n  - **does not cross** the antemeridian, then return the dataset between range -180 and 180.\n  - **does cross** the antemeridian, then return the dataset between range 0 and 360.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530, 560], the result dataset will be in [170, 200].\n\n\n#### Note about `--netcdf-compression-enabled` and `--netcdf-compression-level` options\nWhen subsetting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option `--netcdf-compression-enabled`. The downloaded file will be lighter but it will take more time to write it (because of the compression task). If you don\'t provide it, the task will be faster, but the file heavier.\nOtherwise, if you decide to write your data in Zarr format (`.zarr` extension), the original compression used in the Copernicus Marine Data Store will be applied, which means that the download task will be fast **and** the file compressed. In that case, you cannot use the `--netcdf-compression-enabled`.\n\nHere are the default parameters added to xarray in the background when using the option: `{\'zlib\': True, \'complevel\': 1, \'contiguous\': False, \'shuffle\': True}`\n\nIn addition to this option, you can also provide the `--netcdf-compression-level` option and customize the NetCDF compression level between 0 (no compression) and 9 (maximal compression).\n\n#### Note about `--netcdf3-compatible` option\nThe `--netcdf3-compatible` option has been added to allow the downloaded dataset to be compatible with the netCDF3 format. It uses the `format="NETCDF3_CLASSIC"` of the xarray [to_netcdf](https://docs.xarray.dev/en/latest/generated/xarray.Dataset.to_netcdf.html) method.\n\n### Command `get`\nDownload the dataset file(s) as originally produced, based on the datasetID or the path to files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:39:18Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:39:18Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:39:18Z - Downloading using service original-files...\nINFO - 2024-04-03T11:39:19Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB - 2023-11-12T23:47:13Z\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB - 2023-11-12T23:47:14Z\nPrinted 20 out of 29 files\n\nTotal size of the download: 252.94 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default:\n- After the header displays a summary of the request, a download confirmation is asked. To skip this user\'s action, add option `--force-download`.\n- Files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with `-o/--output-directory`.\n\nOption `--show-outputnames` displays the full paths of the output files, if required.\n\nOption `--create-file-list` only creates a file containing the names of the targeted files instead of downloading them. You have to input a file name, e.g. `--create-file-list my_files.txt`. The format needs to be `.txt` or `.csv`:\n\n- If the user inputs a filename that ends in `.txt`, then the file contains only the full s3 path to the targeted files and is compatible with the `--file-list` option.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.txt\n```\nThe content of `selected_files_for_2021.txt` would be:\n```\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc\n```\n\n- If the user inputs a filename that ends in `.csv` the file contains the following columns, separated by a comma: `filename`, `size` (in Bytes), `last_modified_datetime`, and `etag`. It is **not** compatible "as is" with the `--file-list` option and would need further post-processing from user\'s side.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.csv\n```\n The content of `selected_files_for_2021.csv` would be:\n```\nfilename,size,last_modified_datetime,etag\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc,12295906,2023-11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc,12436177,2023-11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953"\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc,12386940,2023-11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc,12398208,2023-11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1"\n```\nIf specified, no other action will be performed.\n\n\n#### Note about sync option\nOption `--sync` allows to download original files only if not exist and not up to date. The Toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.\nThe logic is largely inspired from [s5cmd package sync command](https://github.com/peak/s5cmd#sync).\nOption `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because, for example, the executed `get` command contains a filter that excludes this specific file.\n\nLimitations:\n- `--sync` is not compatible with `--no-directories`.\n- `--sync` only works with `--dataset-version`.\n- `--sync` functionality is not available for datasets with several parts (like INSITU or static datasets for example).\n\n#### Note about filtering options\nOption `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:51:15Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:51:15Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:51:15Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:51:15Z - Downloading using service original-files...\nINFO - 2024-04-03T11:51:17Z - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular expression for more advanced files selection:\n\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:52:43Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:52:43Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:52:43Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:52:43Z - Downloading using service original-files...\nINFO - 2024-04-03T11:52:44Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a list of files for more advanced files selection.\nThe file can contain complete absolute paths for each target file (default behavior) or only a partial path defined by the user, as shown below.\n\nExample of `file_list.txt` with absolute paths:\n```txt\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc\n```\n\nExample of `file_list.txt` with partial paths matching the absolute paths (equivalent to previous example):\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n> **_NOTE:_** This option is compatible with the file generated by the `--create-file-list` option if you generated a ".txt" file.\n\nThen the following command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO - 2024-04-03T12:57:44Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T12:57:44Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T12:57:44Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T12:57:44Z - Downloading using service original-files...\nINFO - 2024-04-03T12:57:45Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--index-parts` to retrieve the index files of INSITU datasets (as listed on the [Copernicus Marine File Browser](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)).\n> **_NOTE:_** In the future, it is planned to have the index files for those datasets directly available through the `--filter`, `--regex` and/or `--file-list` options. Meanwhile, check this [Help Center article for a working example](https://help.marine.copernicus.eu/en/articles/9133855-how-to-download-insitu-data-using-index-files).\n\n\nThen the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\nReturns:\n```\nINFO - 2024-04-03T12:58:40Z - Dataset version was not specified, the latest one was selected: "202311"\nINFO - 2024-04-03T12:58:40Z - Dataset part was not specified, the first one was selected: "history"\nINFO - 2024-04-03T12:58:40Z - You forced selection of service: original-files\nINFO - 2024-04-03T12:58:40Z - Downloading using service original-files...\nINFO - 2024-04-03T12:58:41Z - You requested the download of the following files:\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 333.13 kB - 2024-04-02T08:40:30Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 466.38 kB - 2024-04-03T12:51:52Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-03T08:33:37Z\n\nTotal size of the download: 2.52 MB\nDo you want to proceed with download? [Y/n]:\n```\n\n### Shared options\nBoth `subset` and `get` commands provide these options:\n\n#### Option `--overwrite-output-data`\nWhen specified, the existing files will be overwritten.\nOtherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).\n\n#### Option `--create-template`\nOption to create a file in your current directory containing request parameters. If specified, no other action will be performed.\nIt will create the following files depending on the feature:\n- `subset`\nExample:\n```bash\ncopernicusmarine subset --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: subset_template.json\n```\n- `get`\nExample:\n```bash\ncopernicusmarine get --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: get_template.json\n```\n\n#### Option `--request-file`\nThis option allows to specify request parameters but in a provided `.json` file, useful for batch processing.\nYou can try the following templates or use the `--create-template` option to create both `subset` or `get` template request files.\n\n- Template for `subset` data request:\n```json\n{\n    "dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n    "start_datetime": "2022-04-11",\n    "end_datetime": "2023-08-11",\n    "minimum_longitude": -182.79,\n    "maximum_longitude": -179.69,\n    "minimum_latitude": -40,\n    "maximum_latitude": -36,\n    "minimum_depth": 0,\n    "maximum_depth": 0,\n    "variables": ["thetao"],\n    "output_directory": "./data/",\n    "force_download": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine subset --request-file template_subset_data_request.json\n```\n\n- Template for `get` data request:\n```json\n{\n    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",\n    "filter": "*01yav_200[0-2]*",\n    "force_download": false,\n    "log_level": "INFO",\n    "no_directories": false,\n    "no_metadata_cache": false,\n    "output_directory": "./data/",\n    "overwrite_output_data": false,\n    "overwrite_metadata_cache": false,\n    "show_outputnames": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.\n\n#### Option `--dataset-version`\nYou can use the `--dataset-version` option to fetch a specific dataset version. Particularly useful to keep an operational chain working when an evolution impact the chosen dataset.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.\n\n#### Option `--log-level`\nSet the details printed to console by the command (based on standard logging library).\nAvailable values are: `[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`\n\n## Python package (API)\nThe `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).\n\n## Documentation\nA detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide).\n\n## Contribution\nWe welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-request).\n\n## Future improvements & Roadmap\nTo keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users\' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-roadmap).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register?redirect=%2Fproducts)\n- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)\n## Licence\nLicensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n',
+    'long_description': '\n<h1 align="center">Copernicus Marine Service Toolbox (CLI & Python)</h1>\n<div align="center">\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/v/copernicusmarine.svg?style=flat-square" alt="PyPI" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/pypi/pyversions/copernicusmarine.svg?style=flat-square" alt="PyPI Supported Versions" /></a>\n  <a href="https://pypi.org/project/copernicusmarine/"><img src="https://img.shields.io/badge/platform-windows | linux | macos-lightgrey?style=flat-square" alt="Supported Platforms" /></a>\n  <a href="https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12"><img src="https://img.shields.io/badge/licence-EUPL-lightblue?style=flat-square" alt="Licence" /></a>\n</div>\n\n![Copernicus Marine Service and Mercator Ocean international logos](https://www.mercator-ocean.eu/wp-content/uploads/2022/05/Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers capabilities through both **Command Line Interface (CLI)** and **Python API**:\n- **Metadata Information**: List and retrieve metadata information on all variables, datasets, products, and their associated documentation.\n- **Subset Datasets**: Subset datasets to extract only the parts of interest, in preferred format, such as Analysis-Ready Cloud-Optimized (ARCO) Zarr or NetCDF file format.\n- **Advanced Filters**: Apply simple or advanced filters to get multiple files, in original formats like NetCDF/GeoTIFF, via direct Marine Data Store connections.\n- **No Quotas**: Enjoy no quotas, neither on volume size nor bandwidth.\n\n## Installation\nFor installation, multiple options are available depending on your setup:\n\n### Mamba | Conda\nA `conda` package is available on [Anaconda](https://anaconda.org/conda-forge/copernicusmarine).\n\nYou can install it using `mamba` (or conda) through the `conda-forge` channel with the following command:\n```bash\nmamba install conda-forge::copernicusmarine --yes\n```\n\nTo upgrade the Toolbox with mamba (or conda):\n```bash\nmamba update --name copernicusmarine copernicusmarine --yes\n```\n\n### Docker\nA docker image is also available here: [https://hub.docker.com/r/copernicusmarine/copernicusmarine](https://hub.docker.com/r/copernicusmarine/copernicusmarine)\n\nFirst step is to pull the container image:\n```bash\ndocker pull copernicusmarine/copernicusmarine:latest\n```\n\nThen run it:\n```bash\ndocker run -it --rm copernicusmarine/copernicusmarine --version\n```\n\n### Pip\nOtherwise, if you already have an environment (safer to clone it), the package can be installed using the `pip` command:\n```bash\npython -m pip install copernicusmarine\n```\n\nAnd to **upgrade the package** to the newest available version, run:\n```bash\npython -m pip install copernicusmarine --upgrade\n```\n\n## User Guide\nFor more comprehensive details on how to use the `copernicusmarine` Toolbox, please refer to our [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide). It ensures a smooth migration for existing users of legacy services such as MOTU, OPeNDAP or FTP.\n\n### General configuration\n\n#### Cache Usage\nCachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:\n- on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n- on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`\n\n### Network configuration\n\n#### Disable SSL\n\nA global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:\n\n- on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n#### Trust Env for python libraries\n\nTo do HTTP calls, the Copernicus Marine Toolbox uses two python libraries: requests and aiohttp. By default, those libraries will have `trust_env` values set to `True`. If you want to deactivate this, you can set `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for example if you don\'t want those libraries to read your `.netrc` file as it has been reported that having a `.netrc` with a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox.\n\n#### Proxy\n\nTo use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:\n\n- set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.\n- use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.\n\n## Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands and their available options, consider appending `--help` on any command line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\n\nReturns:\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version  Show the version and exit.\n  -h, --help     Show this message and exit.\n\nCommands:\n  describe  Print Copernicus Marine catalog as JSON.\n  get       Download originally produced data files.\n  login     Create a configuration file with your Copernicus Marine credentials.\n  subset    Download subsets of datasets as NetCDF files or Zarr stores.\n```\n\n### Command `describe`\nRetrieve metadata information about all products/datasets and display as JSON output:\n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output can also be saved as follows:\n```bash\ncopernicusmarine describe --include-datasets > all_datasets_copernicusmarine.json\n```\n\n### Command `login`\nCreate a single configuration file `.copernicusmarine-credentials` allowing to access all Copernicus Marine Data Store data services. By default, the file is saved in user\'s home directory.\n\nExample:\n```bash\n> copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration files stored in /Users/foo/.copernicusmarine\n```\n\nIf `.copernicusmarine-credentials` already exists, the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-configuration-file`).\n\nYou can use the `--skip-if-user-logged-in` option to skip the configuration file overwrite if the user is already logged in.\n\n#### Access points migration and evolution\nIf you still have a configuration for legacy services (e.g. `~/motuclient/motuclient-python.ini`, `~/.netrc` or `~/_netrc`) in your home directory, it will automatically be taken into account with commands `get` and `subset` without the need for running the `login` command.\nIf the configuration files are already available in another directory, when running commands `subset` or `get`, you can use the `--credentials-file` option to point to the files.\n\n### Command `subset`\nRemotely subset a dataset, based on variable names, geographical and temporal parameters.\n\nExample:\n```bash\ncopernicusmarine subset --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1D-m --variable thetao --variable so --start-datetime 2021-01-01 --end-datetime 2021-01-03 --minimum-longitude 0.0 --maximum-longitude 0.1 --minimum-latitude 28.0 --maximum-latitude 28.1\n```\nReturns:\n```bash\nINFO - 2024-04-03T10:18:18Z - <xarray.Dataset> Size: 3kB\nDimensions:    (depth: 50, latitude: 2, longitude: 1, time: 3)\nCoordinates:\n  * depth      (depth) float32 200B 0.5058 1.556 2.668 ... 5.292e+03 5.698e+03\n  * latitude   (latitude) float32 8B 28.0 28.08\n  * longitude  (longitude) float32 4B 0.08333\n  * time       (time) datetime64[ns] 24B 2021-01-01 2021-01-02 2021-01-03\nData variables:\n    thetao     (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\n    so         (time, depth, latitude, longitude) float32 1kB dask.array<chunksize=(3, 1, 2, 1), meta=np.ndarray>\nAttributes: (12/20)\n    Conventions:               CF-1.0\n    bulletin_date:             2020-12-01\n    ...                        ...\n    references:                http://marine.copernicus.eu\n    copernicusmarine_version:  1.1.0\nINFO - 2024-04-03T10:18:18Z - Estimated size of the dataset file is 0.002 MB.\n\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default, after the display of the summary of the dataset subset, a download confirmation is asked. To skip this confirmation, use the option `--force-download`.\n\n#### Note about `--subset-method` option\nBy default, the `subset` feature uses the `nearest` method of xarray. By specifying `--subset-method strict`, you can only request dimension strictly inside the dataset, useful for **operational use-case**.\n\n#### Note about longitude range\nOptions `--minimum-longitude` and `--maximum-longitude` work as follows:\n- If the result of the substraction ( `--maximum-longitude` minus `--minimum-longitude` ) is superior or equal to 360, then return the full dataset.\n- If the requested longitude range:\n  - **does not cross** the antemeridian, then return the dataset between range -180 and 180.\n  - **does cross** the antemeridian, then return the dataset between range 0 and 360.\n\nNote that you can request any longitudes you want. A modulus is applied to bring the result between -180° and 360°. For example, if you request [530, 560], the result dataset will be in [170, 200].\n\n\n#### Note about `--netcdf-compression-enabled` and `--netcdf-compression-level` options\nWhen subsetting data, if you decide to write your data as a NetCDF file (which is the default behavior), then you can provide the extra option `--netcdf-compression-enabled`. The downloaded file will be lighter but it will take more time to write it (because of the compression task). If you don\'t provide it, the task will be faster, but the file heavier.\nOtherwise, if you decide to write your data in Zarr format (`.zarr` extension), the original compression used in the Copernicus Marine Data Store will be applied, which means that the download task will be fast **and** the file compressed. In that case, you cannot use the `--netcdf-compression-enabled`.\n\nHere are the default parameters added to xarray in the background when using the option: `{\'zlib\': True, \'complevel\': 1, \'contiguous\': False, \'shuffle\': True}`\n\nIn addition to this option, you can also provide the `--netcdf-compression-level` option and customize the NetCDF compression level between 0 (no compression) and 9 (maximal compression).\n\n#### Note about `--netcdf3-compatible` option\nThe `--netcdf3-compatible` option has been added to allow the downloaded dataset to be compatible with the netCDF3 format. It uses the `format="NETCDF3_CLASSIC"` of the xarray [to_netcdf](https://docs.xarray.dev/en/latest/generated/xarray.Dataset.to_netcdf.html) method.\n\n### Command `get`\nDownload the dataset file(s) as originally produced, based on the datasetID or the path to files.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --service original-files\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:39:18Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:39:18Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:39:18Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:39:18Z - Downloading using service original-files...\nINFO - 2024-04-03T11:39:19Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_19930101_19931231_R20221101_RE01.nc - 8.83 MB - 2023-11-12T23:47:13Z\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20120101_20121231_R20221101_RE01.nc - 8.62 MB - 2023-11-12T23:47:14Z\nPrinted 20 out of 29 files\n\nTotal size of the download: 252.94 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nBy default:\n- After the header displays a summary of the request, a download confirmation is asked. To skip this user\'s action, add option `--force-download`.\n- Files are downloaded to the current directory applying the original folder structure. To avoid this behavior, add `--no-directories` and specify a destination with `-o/--output-directory`.\n\nOption `--show-outputnames` displays the full paths of the output files, if required.\n\nOption `--create-file-list` only creates a file containing the names of the targeted files instead of downloading them. You have to input a file name, e.g. `--create-file-list my_files.txt`. The format needs to be `.txt` or `.csv`:\n\n- If the user inputs a filename that ends in `.txt`, then the file contains only the full s3 path to the targeted files and is compatible with the `--file-list` option.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.txt\n```\nThe content of `selected_files_for_2021.txt` would be:\n```\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc\n```\n\n- If the user inputs a filename that ends in `.csv` the file contains the following columns, separated by a comma: `filename`, `size` (in Bytes), `last_modified_datetime`, and `etag`. It is **not** compatible "as is" with the `--file-list` option and would need further post-processing from user\'s side.\n\nExample:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m --filter "*2021*" --create-file-list selected_files_for_2021.csv\n```\n The content of `selected_files_for_2021.csv` would be:\n```\nfilename,size,last_modified_datetime,etag\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc,12295906,2023-11-12 23:47:05.466000+00:00,"e8a7e564f676a08bf601bcdeaebdc563"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc,12436177,2023-11-12 23:47:05.540000+00:00,"d4a22dfb6c7ed85860c4a122c45eb953"\n[... truncated for brevity..]\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211101_20211130_R20230101_RE01.nc,12386940,2023-11-12 23:47:06.358000+00:00,"ea15d1f70fcc7f2ce404184d983530ff"\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20211201_20211231_R20230101_RE01.nc,12398208,2023-11-12 23:47:06.456000+00:00,"585f49867aaefa2ce9d6e68dd468b5e1"\n```\nIf specified, no other action will be performed.\n\n\n#### Note about sync option\nOption `--sync` allows to download original files only if not exist and not up to date. The Toolbox checks the destination folder against the source folder. It can be combined with filters. Note that if set with `--overwrite-output-data`, the latter will be ignored.\nThe logic is largely inspired from [s5cmd package sync command](https://github.com/peak/s5cmd#sync).\nOption `--sync-delete` will work as `--sync` with the added fonctionnality that it deletes any local file that has not been found on the remote server. Note that the files found on the server are also filtered. Hence, a file present locally might be deleted even if it is on the server because, for example, the executed `get` command contains a filter that excludes this specific file.\n\nLimitations:\n- `--sync` is not compatible with `--no-directories`.\n- `--sync` only works with `--dataset-version`.\n- `--sync` functionality is not available for datasets with several parts (like INSITU or static datasets for example).\n\n#### Note about filtering options\nOption `--filter` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files:\n```bash\ncopernicusmarine get --dataset-id cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --filter "*01yav_200[0-2]*"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:51:15Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:51:15Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:51:15Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:51:15Z - Downloading using service original-files...\nINFO - 2024-04-03T11:51:17Z - You requested the download of the following files:\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB\ns3://mdl-native/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--regex` allows to specify a regular expression for more advanced files selection:\n\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --regex ".*01yav_20(00|01|02).*.nc"\n```\nReturns:\n```bash\nINFO - 2024-04-03T11:52:43Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T11:52:43Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T11:52:43Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T11:52:43Z - Downloading using service original-files...\nINFO - 2024-04-03T11:52:44Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nOption `--file-list` allows to specify a list of files for more advanced files selection.\nThe file can contain complete absolute paths for each target file (default behavior) or only a partial path defined by the user, as shown below.\n\nExample of `file_list.txt` with absolute paths:\n```txt\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210101_20210131_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210201_20210228_R20230101_RE01.nc\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1M-m_202012/2021/CMEMS_v5r1_IBI_PHY_MY_PdE_01mav_20210301_20210331_R20230101_RE01.nc\n```\n\nExample of `file_list.txt` with partial paths matching the absolute paths (equivalent to previous example):\n```txt\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc\nCMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc\n```\n> **_NOTE:_** This option is compatible with the file generated by the `--create-file-list` option if you generated a ".txt" file.\n\nThen the following command:\n```bash\ncopernicusmarine get -i cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m --file-list file_list.txt\n```\nReturns:\n```bash\nINFO - 2024-04-03T12:57:44Z - Dataset version was not specified, the latest one was selected: "202211"\nINFO - 2024-04-03T12:57:44Z - Dataset part was not specified, the first one was selected: "default"\nINFO - 2024-04-03T12:57:44Z - Service was not specified, the default one was selected: "original-files"\nINFO - 2024-04-03T12:57:44Z - Downloading using service original-files...\nINFO - 2024-04-03T12:57:45Z - You requested the download of the following files:\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20000101_20001231_R20221101_RE01.nc - 8.93 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20010101_20011231_R20221101_RE01.nc - 8.91 MB - 2023-11-12T23:47:13Z\ns3://mdl-native-10/native/IBI_MULTIYEAR_PHY_005_002/cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m_202211/CMEMS_v5r1_IBI_PHY_MY_NL_01yav_20020101_20021231_R20221101_RE01.nc - 8.75 MB - 2023-11-12T23:47:13Z\n\nTotal size of the download: 26.59 MB\nDo you want to proceed with download? [Y/n]:\n```\n\nAlso, there is a specific command `--index-parts` to retrieve the index files of INSITU datasets (as listed on the [Copernicus Marine File Browser](https://data.marine.copernicus.eu/product/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/files?subdataset=cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311--ext--history&path=INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034%2Fcmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311%2F)).\n> **_NOTE:_** In the future, it is planned to have the index files for those datasets directly available through the `--filter`, `--regex` and/or `--file-list` options. Meanwhile, check this [Help Center article for a working example](https://help.marine.copernicus.eu/en/articles/9133855-how-to-download-insitu-data-using-index-files).\n\n\nThen the following command:\n```\ncopernicusmarine get --dataset-id cmems_obs-ins_blk_phybgcwav_mynrt_na_irr --index-parts\n```\nReturns:\n```\nINFO - 2024-04-03T12:58:40Z - Dataset version was not specified, the latest one was selected: "202311"\nINFO - 2024-04-03T12:58:40Z - Dataset part was not specified, the first one was selected: "history"\nINFO - 2024-04-03T12:58:40Z - You forced selection of service: original-files\nINFO - 2024-04-03T12:58:40Z - Downloading using service original-files...\nINFO - 2024-04-03T12:58:41Z - You requested the download of the following files:\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_history.txt - 333.13 kB - 2024-04-02T08:40:30Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_latest.txt - 466.38 kB - 2024-04-03T12:51:52Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_monthly.txt - 1.51 MB - 2024-03-05T18:09:43Z\ns3://mdl-native-08/native/INSITU_BLK_PHYBGCWAV_DISCRETE_MYNRT_013_034/cmems_obs-ins_blk_phybgcwav_mynrt_na_irr_202311/index_platform.txt - 209.27 kB - 2024-04-03T08:33:37Z\n\nTotal size of the download: 2.52 MB\nDo you want to proceed with download? [Y/n]:\n```\n\n### Shared options\nBoth `subset` and `get` commands provide these options:\n\n#### Option `--overwrite-output-data`\nWhen specified, the existing files will be overwritten.\nOtherwise, if the files already exist on destination, new ones with a unique index will be created once the download has been accepted (or once `--force-download` is provided).\n\n#### Option `--create-template`\nOption to create a file in your current directory containing request parameters. If specified, no other action will be performed.\nIt will create the following files depending on the feature:\n- `subset`\nExample:\n```bash\ncopernicusmarine subset --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: subset_template.json\n```\n- `get`\nExample:\n```bash\ncopernicusmarine get --create-template\n```\nReturns:\n```txt\nINFO - 2024-04-04T14:38:09Z - Template created at: get_template.json\n```\n\n#### Option `--request-file`\nThis option allows to specify request parameters but in a provided `.json` file, useful for batch processing.\nYou can try the following templates or use the `--create-template` option to create both `subset` or `get` template request files.\n\n- Template for `subset` data request:\n```json\n{\n    "dataset_id": "cmems_mod_glo_phy-thetao_anfc_0.083deg_P1D-m",\n    "start_datetime": "2022-04-11",\n    "end_datetime": "2023-08-11",\n    "minimum_longitude": -182.79,\n    "maximum_longitude": -179.69,\n    "minimum_latitude": -40,\n    "maximum_latitude": -36,\n    "minimum_depth": 0,\n    "maximum_depth": 0,\n    "variables": ["thetao"],\n    "output_directory": "./data/",\n    "force_download": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine subset --request-file template_subset_data_request.json\n```\n\n- Template for `get` data request:\n```json\n{\n    "dataset_id": "cmems_mod_ibi_phy_my_0.083deg-3D_P1Y-m",\n    "filter": "*01yav_200[0-2]*",\n    "force_download": false,\n    "log_level": "INFO",\n    "no_directories": false,\n    "no_metadata_cache": false,\n    "output_directory": "./data/",\n    "overwrite_output_data": false,\n    "overwrite_metadata_cache": false,\n    "show_outputnames": true\n}\n```\n\nExample:\n```bash\ncopernicusmarine get --request-file template_get_data_request.json\n```\n\n#### Option `--credentials-file`\nYou can use the `--credentials-file` option to point to a credentials file. The file can be either `.copernicusmarine-credentials`, `motuclient-python.ini`, `.netrc` or `_netrc`.\n\n#### Option `--dataset-version`\nYou can use the `--dataset-version` option to fetch a specific dataset version. Particularly useful to keep an operational chain working when an evolution impact the chosen dataset.\n\n#### Option `--dataset-part`\nYou can use the `--dataset-part` option to fecth a specific part for the chosen dataset version.\n\n#### Option `--log-level`\nSet the details printed to console by the command (based on standard logging library).\nAvailable values are: `[DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]`\n\n## Python package (API)\nThe `copernicusmarine` exposes a Python interface to allow you to [call commands as functions](https://marine.copernicus.eu/python-interface).\n\n## Documentation\nA detailed standalone API documentation is under construction and will come at a later stage. For the moment, see the [Help Center](https://help.marine.copernicus.eu/en/collections/9054839-copernicus-marine-toolbox-guide).\n\n## Contribution\nWe welcome contributions from the community to enhance this package. If you find any issues or have suggestions for improvements, please check out our [Report Template](https://help.marine.copernicus.eu/en/articles/8218546-reporting-an-issue-or-feature-request).\n\n## Future improvements & Roadmap\nTo keep up to date with the most recent and planned advancements, including revisions, corrections, and feature requests generated from users\' feedback, please refer to our [Roadmap](https://help.marine.copernicus.eu/en/articles/8218641-next-milestones-and-roadmap).\n\n## Join the community\nGet in touch!\n- Create your [Copernicus Marine Account](https://data.marine.copernicus.eu/register?redirect=%2Fproducts)\n- [Log in](https://data.marine.copernicus.eu/login?redirect=%2Fproducts) and chat with us (bottom right corner of [Copernicus Marine Service](https://marine.copernicus.eu/))\n- Join our [training workshops](https://marine.copernicus.eu/services/user-learning-services)\n- Network y/our [Copernicus Stories](https://twitter.com/cmems_eu)\n- Watch [our videos](https://www.youtube.com/channel/UC71ceOVy7WtVC7F04BKoEew)\n## Licence\nLicensed under the [EUPL](https://joinup.ec.europa.eu/collection/eupl/eupl-text-eupl-12)\n',
     'author': 'Copernicus Marine User Support',
     'author_email': 'servicedesk.cmems@mercator-ocean.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 install_requires = \ ['aiohttp>=3.8.5', 'boto3>=1.25', 'cachier>=2.2.1',
 'click>=8.0.4', 'dask>=2022', 'lxml>=4.9.0', 'nest-asyncio>=1.5.8',
 'netCDF4>=1.5.4', 'pystac>=1.8.3', 'requests>=2.27.1', 'semver>=3.0.2',
 'setuptools>=68.2.2', 'tqdm>=4.65.0', 'xarray>=2023.4.0', 'zarr>=2.13.3']
 entry_points = \ {'console_scripts': ['copernicusmarine = '
 'copernicusmarine.command_line_interface.copernicus_marine:
 command_line_interface']} setup_kwargs = { 'name': 'copernicusmarine',
-'version': '1.1.0', 'description': '', 'long_description': '\n
+'version': '1.1.1', 'description': '', 'long_description': '\n
         ************ CCooppeerrnniiccuuss MMaarriinnee SSeerrvviiccee TToooollbbooxx ((CCLLII && PPyytthhoonn)) ************
 \n
   \n _[_P_y_P_I_]\n _[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _V_e_r_s_i_o_n_s_]\n _[_S_u_p_p_o_r_t_e_d_ _P_l_a_t_f_o_r_m_s_]\n _[_L_i_c_e_n_c_e_]\n
 \n\n![Copernicus Marine Service and Mercator Ocean international logos](https:/
 /www.mercator-ocean.eu/wp-content/uploads/2022/05/
 Cartouche_CMEMS_poisson_MOi.png)\n\n## Features\nThe `copernicusmarine` offers
 capabilities through both **Command Line Interface (CLI)** and **Python API**:
@@ -48,32 +48,49 @@
 existing users of legacy services such as MOTU, OPeNDAP or FTP.\n\n### General
 configuration\n\n#### Cache Usage\nCachier library is used for caching part of
 the requests (as result of `describe` or `login`). By default, the cache will
 be located in the home folder. If you need to change the location of the cache,
 you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to
 point to the desired directory:\n- on **UNIX** platforms: `export
 COPERNICUSMARINE_CACHE_DIRECTORY=`\n- on **Windows** platforms: `set
-COPERNICUSMARINE_CACHE_DIRECTORY=`\n\n#### Disable SSL\nA global SSL context is
-used when making HTTP calls using the `copernicusmarine` Toolbox. For some
-reason, it can lead to unexpected behavior depending on your network
-configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
-environment variable to any value to globally disable the usage of SSL in the
-toolbox:\n- on **UNIX** platforms: `export
-COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms: `set
-COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n## Command Line Interface
-(CLI)\n\n### The `--help` option\nTo discover commands and their available
-options, consider appending `--help` on any command line.\n\nExample:
-\n```bash\ncopernicusmarine --help\n```\n\nReturns:\n```bash\nUsage:
-copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n -V, --version Show
-the version and exit.\n -h, --help Show this message and exit.\n\nCommands:\n
-describe Print Copernicus Marine catalog as JSON.\n get Download originally
-produced data files.\n login Create a configuration file with your Copernicus
-Marine credentials.\n subset Download subsets of datasets as NetCDF files or
-Zarr stores.\n```\n\n### Command `describe`\nRetrieve metadata information
-about all products/datasets and display as JSON output:
+COPERNICUSMARINE_CACHE_DIRECTORY=`\n\n### Network configuration\n\n#### Disable
+SSL\n\nA global SSL context is used when making HTTP calls using the
+`copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior
+depending on your network configuration. You can set the
+`COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to
+globally disable the usage of SSL in the toolbox:\n\n- on **UNIX** platforms:
+`export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n- on **Windows** platforms:
+`set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`\n\n#### Trust Env for python
+libraries\n\nTo do HTTP calls, the Copernicus Marine Toolbox uses two python
+libraries: requests and aiohttp. By default, those libraries will have
+`trust_env` values set to `True`. If you want to deactivate this, you can set
+`COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for
+example if you don\'t want those libraries to read your `.netrc` file as it has
+been reported that having a `.netrc` with a line: "default login anonymous
+password user@site" is incompatible with S3 connection required by the
+toolbox.\n\n#### Proxy\n\nTo use proxies, as describe in the [aiohttp
+documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-
+support) you can use two options:\n\n- set the `HTTPS_PROXY` variable. For eg:
+`HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with
+`COPERNICUSMARINE_TRUST_ENV=False`.\n- use a `.netrc` file but be aware that
+having a line: "default login anonymous password user@site" is incompatible
+with S3 connection required by the toolbox. Also note that if you have
+`COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC`
+environment variable is set with a specified location, the `.netrc` file will
+be read from the specified location there rather than from `~/.netrc`.\n\n##
+Command Line Interface (CLI)\n\n### The `--help` option\nTo discover commands
+and their available options, consider appending `--help` on any command
+line.\n\nExample:\n```bash\ncopernicusmarine --help\n```\n\nReturns:
+\n```bash\nUsage: copernicusmarine [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n -
+V, --version Show the version and exit.\n -h, --help Show this message and
+exit.\n\nCommands:\n describe Print Copernicus Marine catalog as JSON.\n get
+Download originally produced data files.\n login Create a configuration file
+with your Copernicus Marine credentials.\n subset Download subsets of datasets
+as NetCDF files or Zarr stores.\n```\n\n### Command `describe`\nRetrieve
+metadata information about all products/datasets and display as JSON output:
 \n```bash\ncopernicusmarine describe --include-datasets\n```\n\nThe JSON output
 can also be saved as follows:\n```bash\ncopernicusmarine describe --include-
 datasets > all_datasets_copernicusmarine.json\n```\n\n### Command
 `login`\nCreate a single configuration file `.copernicusmarine-credentials`
 allowing to access all Copernicus Marine Data Store data services. By default,
 the file is saved in user\'s home directory.\n\nExample:\n```bash\n>
 copernicusmarine login\nusername : johndoe\npassword :\nINFO - Configuration
```

### Comparing `copernicusmarine-1.1.0/PKG-INFO` & `copernicusmarine-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicusmarine
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 License: EUPL-1.2
 Author: Copernicus Marine User Support
 Author-email: servicedesk.cmems@mercator-ocean.eu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
@@ -92,19 +92,34 @@
 ### General configuration
 
 #### Cache Usage
 Cachier library is used for caching part of the requests (as result of `describe` or `login`). By default, the cache will be located in the home folder. If you need to change the location of the cache, you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to point to the desired directory:
 - on **UNIX** platforms: `export COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
 - on **Windows** platforms: `set COPERNICUSMARINE_CACHE_DIRECTORY=<PATH>`
 
+### Network configuration
+
 #### Disable SSL
+
 A global SSL context is used when making HTTP calls using the `copernicusmarine` Toolbox. For some reason, it can lead to unexpected behavior depending on your network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT` environment variable to any value to globally disable the usage of SSL in the toolbox:
+
 - on **UNIX** platforms: `export COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
 - on **Windows** platforms: `set COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True`
 
+#### Trust Env for python libraries
+
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries: requests and aiohttp. By default, those libraries will have `trust_env` values set to `True`. If you want to deactivate this, you can set `COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for example if you don't want those libraries to read your `.netrc` file as it has been reported that having a `.netrc` with a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox.
+
+#### Proxy
+
+To use proxies, as describe in the [aiohttp documentation](https://docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two options:
+
+- set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:pass@some.proxy.com"`. It should work even with `COPERNICUSMARINE_TRUST_ENV=False`.
+- use a `.netrc` file but be aware that having a line: "default login anonymous password user@site" is incompatible with S3 connection required by the toolbox. Also note that if you have `COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC` environment variable is set with a specified location, the `.netrc` file will be read from the specified location there rather than from `~/.netrc`.
+
 ## Command Line Interface (CLI)
 
 ### The `--help` option
 To discover commands and their available options, consider appending `--help` on any command line.
 
 Example:
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copernicusmarine Version: 1.1.0 Summary: License:
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.1.1 Summary: License:
 EUPL-1.2 Author: Copernicus Marine User Support Author-email:
 servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.5) Requires-Dist: boto3 (>=1.25) Requires-Dist: cachier (>=2.2.1)
@@ -47,33 +47,51 @@
 existing users of legacy services such as MOTU, OPeNDAP or FTP. ### General
 configuration #### Cache Usage Cachier library is used for caching part of the
 requests (as result of `describe` or `login`). By default, the cache will be
 located in the home folder. If you need to change the location of the cache,
 you can set the environment variable `COPERNICUSMARINE_CACHE_DIRECTORY` to
 point to the desired directory: - on **UNIX** platforms: `export
 COPERNICUSMARINE_CACHE_DIRECTORY=` - on **Windows** platforms: `set
-COPERNICUSMARINE_CACHE_DIRECTORY=` #### Disable SSL A global SSL context is
-used when making HTTP calls using the `copernicusmarine` Toolbox. For some
-reason, it can lead to unexpected behavior depending on your network
-configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
+COPERNICUSMARINE_CACHE_DIRECTORY=` ### Network configuration #### Disable SSL A
+global SSL context is used when making HTTP calls using the `copernicusmarine`
+Toolbox. For some reason, it can lead to unexpected behavior depending on your
+network configuration. You can set the `COPERNICUSMARINE_DISABLE_SSL_CONTEXT`
 environment variable to any value to globally disable the usage of SSL in the
 toolbox: - on **UNIX** platforms: `export
 COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` - on **Windows** platforms: `set
-COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` ## Command Line Interface (CLI) ###
-The `--help` option To discover commands and their available options, consider
-appending `--help` on any command line. Example: ```bash copernicusmarine --
-help ``` Returns: ```bash Usage: copernicusmarine [OPTIONS] COMMAND [ARGS]...
-Options: -V, --version Show the version and exit. -h, --help Show this message
-and exit. Commands: describe Print Copernicus Marine catalog as JSON. get
-Download originally produced data files. login Create a configuration file with
-your Copernicus Marine credentials. subset Download subsets of datasets as
-NetCDF files or Zarr stores. ``` ### Command `describe` Retrieve metadata
-information about all products/datasets and display as JSON output: ```bash
-copernicusmarine describe --include-datasets ``` The JSON output can also be
-saved as follows: ```bash copernicusmarine describe --include-datasets >
+COPERNICUSMARINE_DISABLE_SSL_CONTEXT=True` #### Trust Env for python libraries
+To do HTTP calls, the Copernicus Marine Toolbox uses two python libraries:
+requests and aiohttp. By default, those libraries will have `trust_env` values
+set to `True`. If you want to deactivate this, you can set
+`COPERNICUSMARINE_TRUST_ENV=False` (default `True`). This can be useful for
+example if you don't want those libraries to read your `.netrc` file as it has
+been reported that having a `.netrc` with a line: "default login anonymous
+password user@site" is incompatible with S3 connection required by the toolbox.
+#### Proxy To use proxies, as describe in the [aiohttp documentation](https://
+docs.aiohttp.org/en/stable/client_advanced.html#proxy-support) you can use two
+options: - set the `HTTPS_PROXY` variable. For eg: `HTTPS_PROXY="http://user:
+pass@some.proxy.com"`. It should work even with
+`COPERNICUSMARINE_TRUST_ENV=False`. - use a `.netrc` file but be aware that
+having a line: "default login anonymous password user@site" is incompatible
+with S3 connection required by the toolbox. Also note that if you have
+`COPERNICUSMARINE_TRUST_ENV=True` (the default value) then if `NETRC`
+environment variable is set with a specified location, the `.netrc` file will
+be read from the specified location there rather than from `~/.netrc`. ##
+Command Line Interface (CLI) ### The `--help` option To discover commands and
+their available options, consider appending `--help` on any command line.
+Example: ```bash copernicusmarine --help ``` Returns: ```bash Usage:
+copernicusmarine [OPTIONS] COMMAND [ARGS]... Options: -V, --version Show the
+version and exit. -h, --help Show this message and exit. Commands: describe
+Print Copernicus Marine catalog as JSON. get Download originally produced data
+files. login Create a configuration file with your Copernicus Marine
+credentials. subset Download subsets of datasets as NetCDF files or Zarr
+stores. ``` ### Command `describe` Retrieve metadata information about all
+products/datasets and display as JSON output: ```bash copernicusmarine describe
+--include-datasets ``` The JSON output can also be saved as follows: ```bash
+copernicusmarine describe --include-datasets >
 all_datasets_copernicusmarine.json ``` ### Command `login` Create a single
 configuration file `.copernicusmarine-credentials` allowing to access all
 Copernicus Marine Data Store data services. By default, the file is saved in
 user's home directory. Example: ```bash > copernicusmarine login username :
 johndoe password : INFO - Configuration files stored in /Users/
 foo/.copernicusmarine ``` If `.copernicusmarine-credentials` already exists,
 the user is asked for confirmation to overwrite (`--overwrite`/`--overwrite-
```

