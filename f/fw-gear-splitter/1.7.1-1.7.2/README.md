# Comparing `tmp/fw_gear_splitter-1.7.1-py3-none-any.whl.zip` & `tmp/fw_gear_splitter-1.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 22668 bytes, number of entries: 13
--rw-r--r--  2.0 unx      135 b- defN 80-Jan-01 00:00 fw_gear_splitter/__init__.py
--rw-r--r--  2.0 unx    11169 b- defN 80-Jan-01 00:00 fw_gear_splitter/geometry.py
--rw-r--r--  2.0 unx    18267 b- defN 80-Jan-01 00:00 fw_gear_splitter/main.py
--rw-r--r--  2.0 unx     9467 b- defN 80-Jan-01 00:00 fw_gear_splitter/metadata.py
--rw-r--r--  2.0 unx     1383 b- defN 80-Jan-01 00:00 fw_gear_splitter/parser.py
+-rw-r--r--  2.0 unx      136 b- defN 80-Jan-01 00:00 fw_gear_splitter/__init__.py
+-rw-r--r--  2.0 unx    11153 b- defN 80-Jan-01 00:00 fw_gear_splitter/geometry.py
+-rw-r--r--  2.0 unx    18250 b- defN 80-Jan-01 00:00 fw_gear_splitter/main.py
+-rw-r--r--  2.0 unx     9468 b- defN 80-Jan-01 00:00 fw_gear_splitter/metadata.py
+-rw-r--r--  2.0 unx     1384 b- defN 80-Jan-01 00:00 fw_gear_splitter/parser.py
 -rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitter/__init__.py
--rw-r--r--  2.0 unx     6372 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitter/base.py
--rw-r--r--  2.0 unx    15170 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitters.py
--rw-r--r--  2.0 unx     2243 b- defN 80-Jan-01 00:00 fw_gear_splitter/utils.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3323 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1101 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.7.1.dist-info/RECORD
-13 files, 69848 bytes uncompressed, 20826 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx     6373 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitter/base.py
+-rw-r--r--  2.0 unx    15179 b- defN 80-Jan-01 00:00 fw_gear_splitter/splitters.py
+-rw-r--r--  2.0 unx     2244 b- defN 80-Jan-01 00:00 fw_gear_splitter/utils.py
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3323 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_splitter-1.7.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1101 b- defN 16-Jan-01 00:00 fw_gear_splitter-1.7.2.dist-info/RECORD
+13 files, 69829 bytes uncompressed, 20826 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: fw_gear_splitter/splitters.py
 Comment: 
 
 Filename: fw_gear_splitter/utils.py
 Comment: 
 
-Filename: fw_gear_splitter-1.7.1.dist-info/LICENSE
+Filename: fw_gear_splitter-1.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_splitter-1.7.1.dist-info/METADATA
+Filename: fw_gear_splitter-1.7.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_splitter-1.7.1.dist-info/WHEEL
+Filename: fw_gear_splitter-1.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_splitter-1.7.1.dist-info/RECORD
+Filename: fw_gear_splitter-1.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gear_splitter/__init__.py

```diff
@@ -1,5 +1,6 @@
 """The fw_gear_splitter package."""
+
 from importlib import metadata
 
 pkg_name = __package__
 __version__ = metadata.version(__package__)
```

## fw_gear_splitter/geometry.py

```diff
@@ -205,15 +205,14 @@
     n = len(orientations)
     if n == 0:
         return 1, []
 
     # Start by incrementing phase at each change in orientation
     normal_list = []
     phases_by_index = []
-    major_dim_list = []
     phase_index = 0
     last_normal = None
     for index in range(n):
         v = orientations[index]
         normal = compute_normal(v).round(decimals=4)
         normal_list.append(normal)
         if last_normal is not None:
@@ -247,15 +246,15 @@
     """
     n = len(locations)
     if n < 2:
         return 1, numpy.zeros(shape=n)
 
     # Ensure that locations is an ndarray
     if not isinstance(locations, ndarray):
-        location = numpy.asarray(locations)
+        location = numpy.asarray(locations)  # noqa
     # Round all slice locations to nearest 0.01 mm
     locations = np.round(locations, decimals=2)
 
     # Lines from Anchor A-B below are computing the number of sign changes in the direction of locations
     # Example: Computations below upon a locations vector with 2 direction changes and thus 3 phases
     # locations =   [1,3,5,7,9, 5,7,9,11,13,15,  1, 3, 5, 7, 9,11]
     # indexes =     [  1,2,3,4, 5,6,7, 8, 9,10, 11,12,13,14,15,15]
```

## fw_gear_splitter/main.py

```diff
@@ -1,8 +1,9 @@
 """Module to run gear."""
+
 import logging
 import typing as t
 import zipfile
 from pathlib import Path
 
 import pandas as pd
 from fw_file.dicom import DICOMCollection
@@ -46,17 +47,15 @@
         return
     frames_found = split[split["decision"] > 0]
     log.debug(
         "%s found %d localizer frames",
         splitter.__class__.__name__,
         frames_found.shape[0],
     )
-    dataframe.loc[dataframe["path"] == split["path"], "score"] += split[
-        "decision"
-    ]  # type: ignore
+    dataframe.loc[dataframe["path"] == split["path"], "score"] += split["decision"]  # type: ignore
 
 
 def gen_split_score(dcm: DICOMCollection) -> pd.DataFrame:
     """Generate 'voting' score for each frame in DICOM.
 
     Voting score comes from multiple splitting algorithms and tries to
     find a concensus among these different methods.
@@ -417,15 +416,15 @@
         # Don't try to split if there is only one slice.
         if len(dcm) == 1:
             log.info("Only one slice present in archive.")
             return tuple(), True
 
         collections = split_dicom(dcm, group_by, split_localizer, max_geom_splits)
         # If collections = None, splitter encountered an error (see log)
-        if collections == None:
+        if not collections:
             log.info("Archive was not split due to an error.")
             return tuple(), False
         # If nothing was split out
         elif len(collections.items()) in (0, 1):
             log.info("Archive was not split; nothing to split was found.")
             # Return an empty tuple
             return tuple(), True
```

## fw_gear_splitter/metadata.py

```diff
@@ -1,8 +1,9 @@
 """Metadata handling."""
+
 import datetime
 import logging
 import re
 import typing as t
 from collections import Counter
 from pathlib import Path
```

## fw_gear_splitter/parser.py

```diff
@@ -1,8 +1,9 @@
 """Parser module to parse gear config.json."""
+
 import typing as t
 from pathlib import Path
 
 from flywheel_gear_toolkit import GearToolkitContext
 
 
 def parse_config(
```

## fw_gear_splitter/splitter/base.py

```diff
@@ -1,8 +1,9 @@
 """Base splitter classes."""
+
 # pylint: disable=invalid-name
 import abc
 import typing as t
 
 import numpy as np
 import pandas as pd
 from fw_file.base import File
```

## fw_gear_splitter/splitters.py

```diff
@@ -1,8 +1,9 @@
 """Splitter implementations."""
+
 # pylint: disable=invalid-name,invalid-unary-operand-type,arguments-differ
 import typing as t
 import warnings
 
 import numpy as np
 import pandas as pd
 from fw_file.base import File
@@ -279,15 +280,15 @@
                     localizer
         """
         if not drop_cols:
             drop_cols = ["value", "p"]
         unique = dataframe.groupby(self.tags).size().reset_index()
         primary_val = unique.iloc[unique.iloc[:, -1].idxmax(), :]
         # pylint: disable=unused-variable
-        values = [getattr(primary_val, tag) for tag in self.tags]
+        values = [getattr(primary_val, tag) for tag in self.tags]  # noqa
         # pylint: enable=unused-variable
         query = []
         # for tag, val in zip(self.tags, values):
         #    query.append(f"{tag} == {quote_val(val)}")
         for i, tag in enumerate(self.tags):
             query.append(f"dataframe.{tag} == values[{i}]")
         query_str = " and ".join(query)
```

## fw_gear_splitter/utils.py

```diff
@@ -1,8 +1,9 @@
 """Splitter utilities."""
+
 import typing as t
 
 import pandas as pd
 from flywheel_gear_toolkit import GearToolkitContext
 from fw_file.dicom import DICOMCollection
```

## Comparing `fw_gear_splitter-1.7.1.dist-info/LICENSE` & `fw_gear_splitter-1.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_splitter-1.7.1.dist-info/METADATA` & `fw_gear_splitter-1.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fw-gear-splitter
-Version: 1.7.1
+Version: 1.7.2
 Summary: DICOM splitter based on unique tags, or localizers
 License: MIT
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flywheel-gear-toolkit (>=0.6.18,<0.7.0)
 Requires-Dist: flywheel-sdk (>=16.0.0,<17.0.0)
 Requires-Dist: fw-file (>=3,<4)
-Requires-Dist: importlib-metadata (>=3.7.0,<4.0.0)
 Requires-Dist: pandas (>=1.2.1,<2.0.0)
 Requires-Dist: pylibjpeg (>=1.1.1,<2.0.0)
 Requires-Dist: pylibjpeg-libjpeg (>=1.1.0,<2.0.0)
 Requires-Dist: pylibjpeg-openjpeg (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
```

## Comparing `fw_gear_splitter-1.7.1.dist-info/RECORD` & `fw_gear_splitter-1.7.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-fw_gear_splitter/__init__.py,sha256=ga8HPszNy5k9r2PR-_xTwZq5q20wru1BHO6M4mqLbi8,135
-fw_gear_splitter/geometry.py,sha256=3xWjbWsj7aUmuFckSrGeBg7jQMMFjfGUvNd-CFilCoU,11169
-fw_gear_splitter/main.py,sha256=jNY8Noktm6iCACr3Bk0kRWnMzcP-2FMH37loV30lvOs,18267
-fw_gear_splitter/metadata.py,sha256=s4KEO4Pwqn084zL7W17R2ofDH7rZqrgikjCPIdpdspQ,9467
-fw_gear_splitter/parser.py,sha256=lYc_ihkU-0SQv8Q2Cz5sk7jhcE34opV2GzrM5j_IpnA,1383
+fw_gear_splitter/__init__.py,sha256=QGD2uK2ieAOlHM65bd20Ah1Uczw1YoTxhcBgvctH4gc,136
+fw_gear_splitter/geometry.py,sha256=j0c7rmnaP040e7tCOw7kVGdR2EFhL-K74hNWd4Sk0xI,11153
+fw_gear_splitter/main.py,sha256=v79Jfe65KntjF2DXhl3gmhLR2bu-wurp6Y1S7ZPKdyU,18250
+fw_gear_splitter/metadata.py,sha256=b0kqckJ4IQg7XMtkrhEHnenWYRnLvPnfxPey7g_4bhA,9468
+fw_gear_splitter/parser.py,sha256=s2vQbtyFMO_SnI-fqi8pmtm-IhlGHGVIux2iBHmd0G4,1384
 fw_gear_splitter/splitter/__init__.py,sha256=PeCzMJ2dMdzODEJ4CP7foHb3a-hk-L5OgPzeDFkv97s,38
-fw_gear_splitter/splitter/base.py,sha256=cnM0d8l46dZqwbDjw_mEsBsH8QJLrfGin5np6VbHD6U,6372
-fw_gear_splitter/splitters.py,sha256=OrZhdD2XLAWbw4PRi58fYp-SwsyCZyJmiaNUdmNnEhY,15170
-fw_gear_splitter/utils.py,sha256=MmXOTS5Ktj53Eo2TTuvHnwLvRj8qtS3fBRkHFqnCOd4,2243
-fw_gear_splitter-1.7.1.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
-fw_gear_splitter-1.7.1.dist-info/METADATA,sha256=fM2chq7nlv7z9ZfjERgpkzZyKb5ilrjYb5EbIlGyPL8,3323
-fw_gear_splitter-1.7.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-fw_gear_splitter-1.7.1.dist-info/RECORD,,
+fw_gear_splitter/splitter/base.py,sha256=Sz_VwGBWd3vLqXJ6WAomqUGuzshcNvOlL_3JymgP7do,6373
+fw_gear_splitter/splitters.py,sha256=DpfCRvgNLbpThvXGL4XWRcTqTLBALgTzykB3qBjJ0-o,15179
+fw_gear_splitter/utils.py,sha256=8uVlSW-q9I557-f5fS1rjPOF8_5EaguLDhij8PqxvdA,2244
+fw_gear_splitter-1.7.2.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
+fw_gear_splitter-1.7.2.dist-info/METADATA,sha256=EJByHAe_ZEP3Ac-dq1MCKYtxIM1_z4csew_K9NtIFe8,3323
+fw_gear_splitter-1.7.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+fw_gear_splitter-1.7.2.dist-info/RECORD,,
```

