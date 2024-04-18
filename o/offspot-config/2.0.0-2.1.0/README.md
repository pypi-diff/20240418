# Comparing `tmp/offspot_config-2.0.0.tar.gz` & `tmp/offspot_config-2.1.0.tar.gz`

## Comparing `offspot_config-2.0.0.tar` & `offspot_config-2.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 offspot_config-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    30298 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/builder.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/constants.py
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/file.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/packages.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/zim.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/__init__.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/base.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/checksum.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/file.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/mainconfig.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/oci.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/output.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/str.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/ways.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/dashboard.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/containers.py
--rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/firmware.py
--rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_catalog.py
--rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_checks.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_humanid.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_inputs.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_link.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_reader.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_zim.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.0.0/LICENSE
--rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.0.0/README.md
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 offspot_config-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    29716 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/file.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/zim.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/base.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/checksum.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/file.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/mainconfig.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/oci.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/output.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/str.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/inputs/ways.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/dashboard.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/containers.py
+-rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/firmware.py
+-rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.1.0/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_catalog.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_checks.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_humanid.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_inputs.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_link.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_reader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.1.0/tests/test_zim.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.1.0/LICENSE
+-rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.1.0/README.md
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.1.0/PKG-INFO
```

### Comparing `offspot_config-2.0.0/.pre-commit-config.yaml` & `offspot_config-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/CHANGELOG.md` & `offspot_config-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.1.0] - 2024-04-18
+
+### Added
+
+- [inputs.checksum] `Checksum` gets a `to_dict()` method
+- [dashboard] `Reader` gets an optional `checksum`
+
+### Changed
+
+- [builder] Removed useless download.kiwix.org special behavior for reader checksum. Checksum now on Reader
+- [builder] Using captive-portal 1.4.1
+- [inputs.base] Version-only base image def now targets uncompressed URL
+- [inputs.base] BaseConfig gets an optional `checksum` and populates base_file accordingly
+- [inputs.base] Version-only base image def now also retrieves Checksum via expected .md5 endpoint
+
 ## [2.0.0] - 2024-04-16
 
 ### Added
 
 - [inputs.file] File now includes a `checksum` property (optional)
 - [inputs.checksum] Checksum now includes an `as_aria` property (`algo=digest` formatted string)
```

### Comparing `offspot_config-2.0.0/tasks.py` & `offspot_config-2.1.0/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/builder.py` & `offspot_config-2.1.0/src/offspot_config/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from __future__ import annotations
 
 import re
 from pathlib import PurePath as Path
 from typing import Any
-from urllib.parse import urlsplit
 
 from offspot_config.catalog import app_catalog, get_app_path
 from offspot_config.constants import CONTENT_TARGET_PATH
 from offspot_config.inputs.base import BaseConfig
 from offspot_config.inputs.checksum import Checksum
 from offspot_config.inputs.file import FileConfig
 from offspot_config.inputs.str import BlockStr
 from offspot_config.oci_images import OCIImage
 from offspot_config.packages import AppPackage, FilesPackage, ZimPackage
 from offspot_config.utils.dashboard import Link, Reader
-from offspot_config.utils.download import read_checksum_from
 from offspot_config.utils.sizes import (
     get_margin_for,
     get_min_image_size_for,
     get_raw_content_size_for,
 )
 from offspot_config.utils.yaml import yaml_dump
 
@@ -37,17 +35,17 @@
 METRICS_VAR_LOG_PATH_HOST = Path("/var/log/metrics")
 METRICS_VAR_LOG_PATH_CONT = Path("/var/log/host/metrics")
 KIWIX_ZIM_LOAD_BALANCER_URL = "https://download.kiwix.org/zim/"
 
 # data source for “internal images” (out of catalog)
 INTERNAL_IMAGES = {
     "captive-portal": {
-        "source": "ghcr.io/offspot/captive-portal:1.4",
-        "filesize": 184627200,
-        "fullsize": 184559684,
+        "source": "ghcr.io/offspot/captive-portal:1.4.1",
+        "filesize": 189911040,
+        "fullsize": 189841976,
     },
     "dashboard": {
         "source": "ghcr.io/offspot/dashboard:1.3.1",
         "filesize": 124354560,
         "fullsize": 124261524,
     },
     "file-browser": {
@@ -205,31 +203,20 @@
         if self.with_dashboard:
             return
 
         self.with_dashboard = True
 
         # Add files for requested readers
         for reader in self.dashboard_readers:
-            checksum = None
-            # download.kiwix.org is known to provide digests via mirrorbrain
-            if urlsplit(reader.download_url).netloc == "download.kiwix.org":
-                try:
-                    checksum = Checksum(
-                        algo="md5",
-                        value=read_checksum_from(f"{reader.download_url}.md5"),
-                    )
-                # we cant assume this this work forever
-                except Exception:
-                    ...
             self.add_file(
                 url_or_content=reader.download_url,
                 to=str(KIWIXSERVE_DATA_PATH / reader.filename),
                 via="direct",
                 size=reader.size,
-                checksum=checksum,
+                checksum=reader.checksum,
                 is_url=True,
             )
 
         image = get_internal_image("dashboard")
         self.config["oci_images"].add(image)
 
         # add to compose
```

### Comparing `offspot_config-2.0.0/src/offspot_config/catalog.json` & `offspot_config-2.1.0/src/offspot_config/catalog.json`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/catalog.py` & `offspot_config-2.1.0/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/constants.py` & `offspot_config-2.1.0/src/offspot_config/constants.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/file.py` & `offspot_config-2.1.0/src/offspot_config/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,40 +29,40 @@
     kind: str = "file"  # Item interface
 
     unpack_formats: list[str]
 
     def __init__(self, payload: dict[str, str | int | dict[str, str]]):
         self.unpack_formats = ["direct", *SUPPORTED_UNPACKING_FORMATS]
         self.url: urllib.parse.ParseResult | None = None
+        self.to: pathlib.Path = pathlib.Path(str(payload["to"])).resolve()
+        self.via: str = str(payload.get("via", "direct"))
         self.content: str = str(payload.get("content", "") or "").strip()
+        self.checksum: Checksum | None = None
+        self._size = -1
+        self._fullsize: int | None = None
 
         if not self.content:
             try:
                 self.url = urllib.parse.urlparse(str(payload["url"]))
             except Exception as exc:
                 raise ValueError(f"URL “{payload.get('url')}” is incorrect") from exc
 
-        self.to: pathlib.Path = pathlib.Path(str(payload["to"])).resolve()
         if not self.to.is_relative_to(DATA_PART_PATH):
             raise ValueError(f"{self.to} not a descendent of {DATA_PART_PATH}")
 
-        self.via: str = str(payload.get("via", "direct"))
         if self.via not in self.unpack_formats:
             raise NotImplementedError(f"Unsupported handler `{self.via}`")
 
         # optional checksum
-        self.checksum = None
         if "checksum" in payload and isinstance(payload["checksum"], dict):
             self.checksum = Checksum(**payload["checksum"])
 
-        # initialized has unknown
-        self._size = -1
+        # initialized as unknown
         if "size" in payload and isinstance(payload["size"], (int, str)):
             self._size: int = int(payload["size"])
-        self._fullsize: int | None = None
         if "fullsize" in payload and isinstance(payload["fullsize"], (int, str)):
             self._fullsize = int(payload["fullsize"])
 
     @property
     def source(self) -> str:  # Item interface
         return self.geturl()
 
@@ -120,12 +120,14 @@
 
     def __repr__(self) -> str:
         msg = f"File(to={self.to}, via={self.via}"
         if self.url:
             msg += f", url={self.geturl()}"
         if self.content:
             msg += f", content={self.content.splitlines()[0][:10]}"
-        msg += f", size={self.size})"
+        msg += f", size={self.size}"
+        msg += f", checksum={self.checksum.as_aria if self.checksum else None}"
+        msg += ")"
         return msg
 
     def __str__(self) -> str:
         return repr(self)
```

### Comparing `offspot_config-2.0.0/src/offspot_config/oci_images.py` & `offspot_config-2.1.0/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/packages.py` & `offspot_config-2.1.0/src/offspot_config/packages.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/zim.py` & `offspot_config-2.1.0/src/offspot_config/zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/inputs/checksum.py` & `offspot_config-2.1.0/src/offspot_config/inputs/checksum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from attrs import define
+from attrs import asdict, define
 from typeguard import typechecked
 
 from offspot_config.constants import SUPPORTED_CHECKSUM_ALGORITHMS
 from offspot_config.utils.download import read_checksum_from
 
 
 @typechecked
@@ -43,7 +43,10 @@
             self.kind = "digest"
         return self.value
 
     @property
     def as_aria(self) -> str:
         """aria2-compatible checksum format: {algo}={digest}"""
         return f"{self.algo}={self.digest}"
+
+    def to_dict(self) -> dict[str, str]:
+        return asdict(self)
```

### Comparing `offspot_config-2.0.0/src/offspot_config/inputs/file.py` & `offspot_config-2.1.0/src/offspot_config/inputs/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/inputs/mainconfig.py` & `offspot_config-2.1.0/src/offspot_config/inputs/mainconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     all_images: list[OCIImage] = field(factory=list)
 
     def __attrs_post_init__(self):
         if isinstance(self.base, dict):
             self.base = BaseConfig(**self.base)
 
         if isinstance(self.base.source, str):
-            self.base_file = get_base_from(self.base.source)
+            self.base_file = get_base_from(self.base)
 
         if isinstance(self.output, dict):
             self.output = OutputConfig(**self.output)
 
         all_tos = [fileconf.to for fileconf in self.files]
         dup_tos = [to for to in all_tos if all_tos.count(to) > 1]
         if len(dup_tos):
```

### Comparing `offspot_config-2.0.0/src/offspot_config/inputs/output.py` & `offspot_config-2.1.0/src/offspot_config/inputs/output.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/utils/download.py` & `offspot_config-2.1.0/src/offspot_config/utils/download.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/utils/misc.py` & `offspot_config-2.1.0/src/offspot_config/utils/misc.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/utils/sizes.py` & `offspot_config-2.1.0/src/offspot_config/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_config/utils/yaml.py` & `offspot_config-2.1.0/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/ap.py` & `offspot_config-2.1.0/src/offspot_runtime/ap.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/checks.py` & `offspot_config-2.1.0/src/offspot_runtime/checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/configlib.py` & `offspot_config-2.1.0/src/offspot_runtime/configlib.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/containers.py` & `offspot_config-2.1.0/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-2.1.0/src/offspot_runtime/dnsmasqspoof.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/ethernet.py` & `offspot_config-2.1.0/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/firmware.py` & `offspot_config-2.1.0/src/offspot_runtime/firmware.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/fromfile.py` & `offspot_config-2.1.0/src/offspot_runtime/fromfile.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/hostname.py` & `offspot_config-2.1.0/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/src/offspot_runtime/timezone.py` & `offspot_config-2.1.0/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/tests/conftest.py` & `offspot_config-2.1.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest  # pyright: ignore [reportMissingImports]
 
 
-@pytest.fixture
+@pytest.fixture(scope="session")
 def mini_config_yaml():
     yield """
 ---
 base:
   source: https://drive.offspot.it/base/offspot-base-arm64-1.2.0.img
   rootfs_size: 2638217216
 output:
```

### Comparing `offspot_config-2.0.0/tests/test_checks.py` & `offspot_config-2.1.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/tests/test_humanid.py` & `offspot_config-2.1.0/tests/test_humanid.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/tests/test_link.py` & `offspot_config-2.1.0/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/tests/test_reader.py` & `offspot_config-2.1.0/tests/test_reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import pytest  # pyright: ignore [reportMissingImports]
 
+from offspot_config.inputs.checksum import Checksum
 from offspot_config.utils.dashboard import Reader
 
 REALISTIC_VALUES = [
     (
         "linux",
         "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_x86_64_2.3.1-4.appimage",
         "kiwix-desktop_x86_64_2.3.1-4.appimage",
         146629824,
+        "899279fb76e357afe33bbdd968750376",
     ),
     (
         "android",
         "https://download.kiwix.org/release/kiwix-android/kiwix-3.9.1.apk",
         "kiwix-3.9.1.apk",
         79629012,
+        "d2ede8e23b4095718c508f44a341f687",
     ),
     (
         "windows",
         "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_windows_x64_2.3.1-2.zip",
         "kiwix-desktop_windows_x64_2.3.1-2.zip",
         126628211,
+        "adf9b64b5c6906427d7a1c8bdfc31546",
     ),
     (
         "macos",
         "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
         "kiwix-desktop-macos_3.1.0.dmg",
         16051402,
+        "747fd0841b56d2d5158e0e65646b1be1",
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "url, expected_filename",
     [
@@ -52,114 +57,170 @@
         ("https://www.freecodecamp.org/news/css-unit-guide/", "css-unit-guide"),
     ],
 )
 def test_filename_from_url(url: str, expected_filename: str):
     assert Reader.filename_from_url(url) == expected_filename
 
 
+def get_checksum_from(md5sum: str) -> Checksum:
+    return Checksum(algo="md5", value=md5sum)
+
+
 def test_reader_is_tuple():
     platform = "windows"
     url = "http://some.tld/file"
     filename = "one"
     size = 4
-    assert Reader(platform, url, filename, size) == (platform, url, filename, size)
+    checksum = None
+    assert Reader(platform, url, filename, size, checksum) == (
+        platform,
+        url,
+        filename,
+        size,
+        checksum,
+    )
     assert Reader(
-        download_url=url, size=size, platform=platform, filename=filename
-    ) == (platform, url, filename, size)
-    assert isinstance(Reader(platform, url, filename, size), Reader)
-    assert isinstance(Reader(platform, url, filename, size), tuple)
-    tuple_ = (platform, url, filename, size)
+        download_url=url,
+        size=size,
+        platform=platform,
+        filename=filename,
+        checksum=checksum,
+    ) == (platform, url, filename, size, checksum)
+    assert isinstance(Reader(platform, url, filename, size, checksum), Reader)
+    assert isinstance(Reader(platform, url, filename, size, checksum), tuple)
+    tuple_ = (platform, url, filename, size, checksum)
     casted = Reader._make(tuple_)
     assert isinstance(casted, Reader)
 
 
-@pytest.mark.parametrize("platform, download_url, filename, size", REALISTIC_VALUES)
-def test_reader_using(platform: str, download_url: str, filename: str, size: int):
-    assert Reader.using(platform, download_url) == Reader(
-        platform, download_url, filename, size
+@pytest.mark.parametrize(
+    "platform, download_url, filename, size, md5sum", REALISTIC_VALUES
+)
+def test_reader_using(
+    platform: str, download_url: str, filename: str, size: int, md5sum: str
+):
+    assert Reader.using(
+        platform, download_url, checksum=get_checksum_from(md5sum)
+    ) == Reader(
+        platform,
+        download_url,
+        filename,
+        size,
+        get_checksum_from(md5sum),
+    )
+    assert Reader.using(platform=platform, download_url=download_url) == Reader(
+        platform,
+        download_url,
+        filename,
+        size,
+        None,
     )
     assert Reader.using(platform=platform, download_url=download_url) == Reader(
-        platform, download_url, filename, size
+        platform,
+        download_url,
+        filename,
+        size,
     )
 
 
-@pytest.mark.parametrize("platform, download_url, filename, size", REALISTIC_VALUES)
-def test_invalid_data(platform: str, download_url: str, filename: str, size: int):
+@pytest.mark.parametrize(
+    "platform, download_url, filename, size, md5sum", REALISTIC_VALUES
+)
+def test_invalid_data(
+    platform: str, download_url: str, filename: str, size: int, md5sum: str
+):
     with pytest.raises(TypeError):
         Reader(platform, download_url, filename)  # pyright: ignore [reportCallIssue]
     with pytest.raises(TypeError):
         Reader(
             platform,
             download_url,
             filename,
             size,
+            get_checksum_from(md5sum),
             32,  # pyright: ignore [reportCallIssue]
         )
     with pytest.raises(TypeError):
         Reader(platform=platform)  # pyright: ignore [reportCallIssue]
     with pytest.raises(TypeError):
         Reader(download_url=download_url)  # pyright: ignore [reportCallIssue]
     with pytest.raises(TypeError):
         Reader.using(
             platform, download_url, filename, size  # pyright: ignore [reportCallIssue]
         )
 
 
 def test_sort_order():
-    readers = [Reader(*values) for values in REALISTIC_VALUES]
+    readers = [
+        Reader(*values[:-1], checksum=get_checksum_from(md5sum=values[-1]))
+        for values in REALISTIC_VALUES
+    ]
     sorted_readers = sorted(readers, key=Reader.sort)
     assert readers != sorted_readers
     assert [r.platform for r in sorted_readers] == [
         "windows",
         "android",
         "macos",
         "linux",
     ]
 
 
 @pytest.mark.parametrize(
-    "platform, download_url, filename, size, expected_dict",
+    "platform, download_url, filename, size, md5sum, expected_dict",
     [
         (
             "android",
             "https://download.kiwix.org/release/kiwix-android/kiwix-3.9.1.apk",
             "kiwix-3.9.1.apk",
             79629012,
+            None,
             {
                 "platform": "android",
                 "download_url": "https://download.kiwix.org/release/kiwix-android/kiwix-3.9.1.apk",
                 "filename": "kiwix-3.9.1.apk",
                 "size": 79629012,
+                "checksum": None,
             },
         ),
         (
             "windows",
             "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_windows_x64_2.3.1-2.zip",
             "kiwix-desktop_windows_x64_2.3.1-2.zip",
             126628211,
+            "adf9b64b5c6906427d7a1c8bdfc31546",
             {
                 "platform": "windows",
                 "download_url": "https://download.kiwix.org/release/kiwix-desktop/kiwix-desktop_windows_x64_2.3.1-2.zip",
                 "filename": "kiwix-desktop_windows_x64_2.3.1-2.zip",
                 "size": 126628211,
+                "checksum": {
+                    "algo": "md5",
+                    "value": "adf9b64b5c6906427d7a1c8bdfc31546",
+                    "kind": "digest",
+                },
             },
         ),
         (
             "macos",
             "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
             None,
             None,
+            None,
             {
                 "platform": "macos",
                 "download_url": "https://download.kiwix.org/release/kiwix-desktop-macos/kiwix-desktop-macos_3.1.0.dmg",
                 "filename": "kiwix-desktop-macos_3.1.0.dmg",
                 "size": 16051402,
+                "checksum": None,
             },
         ),
     ],
 )
-def test_to_dict(platform, download_url, filename, size, expected_dict):
+def test_to_dict(platform, download_url, filename, size, md5sum, expected_dict):
+    checksum = get_checksum_from(md5sum) if md5sum else None
     if filename and size:
-        reader = Reader(platform, download_url, filename, size)
+        reader = Reader(platform, download_url, filename, size, checksum)
     else:
-        reader = Reader.using(platform=platform, download_url=download_url)
+        reader = Reader.using(
+            platform=platform, download_url=download_url, checksum=checksum
+        )
     assert reader.to_dict() == expected_dict
```

### Comparing `offspot_config-2.0.0/tests/test_zim.py` & `offspot_config-2.1.0/tests/test_zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/.gitignore` & `offspot_config-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/LICENSE` & `offspot_config-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/README.md` & `offspot_config-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/pyproject.toml` & `offspot_config-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.0.0/PKG-INFO` & `offspot_config-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: offspot-config
-Version: 2.0.0
+Version: 2.1.0
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
```

