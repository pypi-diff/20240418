# Comparing `tmp/quackosm-0.5.3.tar.gz` & `tmp/quackosm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.5.3.tar", last modified: Fri Apr  5 17:36:04 2024, max compression
+gzip compressed data, was "quackosm-0.6.0.tar", last modified: Wed Apr 17 12:12:18 2024, max compression
```

## Comparing `quackosm-0.5.3.tar` & `quackosm-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0    11339 2024-04-05 17:35:36.291367 quackosm-0.5.3/LICENSE
--rw-r--r--   0        0        0    25727 2024-04-05 17:35:36.291367 quackosm-0.5.3/README.md
--rw-r--r--   0        0        0     4326 2024-04-05 17:36:04.067172 quackosm-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      560 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_constants.py
--rw-r--r--   0        0        0      135 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_exceptions.py
--rw-r--r--   0        0        0     4406 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0     6013 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/_typing.py
--rw-r--r--   0        0        0    23859 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/cli.py
--rw-r--r--   0        0        0     1875 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/conftest.py
--rw-r--r--   0        0        0    51009 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/functions.py
--rw-r--r--   0        0        0    19065 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     3141 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1687 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4098 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   107058 2024-04-05 17:35:36.303367 quackosm-0.5.3/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/conftest.py
--rw-r--r--   0        0        0    24088 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    40294 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      919 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0     1472 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-05 17:35:36.303367 quackosm-0.5.3/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0     5405 2024-04-05 17:35:36.307367 quackosm-0.5.3/tests/test_files/osmconf.ini
--rw-r--r--   0        0        0    27504 1970-01-01 00:00:00.000000 quackosm-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-04-17 12:11:55.611431 quackosm-0.6.0/LICENSE
+-rw-r--r--   0        0        0    25727 2024-04-17 12:11:55.611431 quackosm-0.6.0/README.md
+-rw-r--r--   0        0        0     4333 2024-04-17 12:12:18.743414 quackosm-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_constants.py
+-rw-r--r--   0        0        0      135 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     6497 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0     6013 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/_typing.py
+-rw-r--r--   0        0        0    23859 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/cli.py
+-rw-r--r--   0        0        0     1875 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/conftest.py
+-rw-r--r--   0        0        0    51009 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/functions.py
+-rw-r--r--   0        0        0    19065 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     3141 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1687 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4098 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-04-17 12:11:55.619431 quackosm-0.6.0/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   113903 2024-04-17 12:11:55.623432 quackosm-0.6.0/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/conftest.py
+-rw-r--r--   0        0        0    24088 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    29285 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/test_osm_tags_filtering.py
+-rw-r--r--   0        0        0    36680 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      919 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0     1472 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0     5405 2024-04-17 12:11:55.623432 quackosm-0.6.0/tests/test_files/osmconf.ini
+-rw-r--r--   0        0        0    27511 1970-01-01 00:00:00.000000 quackosm-0.6.0/PKG-INFO
```

### Comparing `quackosm-0.5.3/LICENSE` & `quackosm-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/README.md` & `quackosm-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/pyproject.toml` & `quackosm-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.5.3"
+version = "0.6.0"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas",
     "shapely>=2",
@@ -44,15 +44,15 @@
 Homepage = "https://kraina-ai.github.io/quackosm"
 Repository = "https://github.com/kraina-ai/quackosm"
 Documentation = "https://kraina-ai.github.io/quackosm"
 Changelog = "https://github.com/kraina-ai/quackosm/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 cli = [
-    "typer[all]",
+    "typer[all]>=0.9.0",
     "osmnx",
     "h3>=4.0.0b1",
     "h3ronpy>=0.18.0",
     "s2",
     "python-geohash",
 ]
 
@@ -184,15 +184,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.5.3"
+current_version = "0.6.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.5.3/quackosm/__init__.py` & `quackosm-0.6.0/quackosm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.5.3/quackosm/_osm_tags_filters.py` & `quackosm-0.6.0/quackosm/_osm_tags_filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,44 @@
 
     raise AttributeError(
         "Provided tags don't match required type definitions"
         " (OsmTagsFilter or GroupedOsmTagsFilter)."
     )
 
 
+def merge_key_value_pairs_to_osm_tags_filter(
+    key_value_pairs: list[tuple[str, Union[list[str], str, bool]]],
+) -> OsmTagsFilter:
+    merged_osm_tag_filter = _merge_multiple_osm_tags_filters(
+        {osm_tag_filter_key: osm_tag_filter_value}
+        for osm_tag_filter_key, osm_tag_filter_value in key_value_pairs
+    )
+    return merged_osm_tag_filter
+
+
+def check_if_any_osm_tags_filter_value_is_positive(
+    osm_tags_filter: Union[GroupedOsmTagsFilter, OsmTagsFilter],
+) -> bool:
+    if is_expected_type(osm_tags_filter, OsmTagsFilter):
+        return any(
+            osm_tag_filter_value != False  # noqa: E712
+            for osm_tag_filter_value in cast(OsmTagsFilter, osm_tags_filter).values()
+        )
+    elif is_expected_type(osm_tags_filter, GroupedOsmTagsFilter):
+        return any(
+            check_if_any_osm_tags_filter_value_is_positive(osm_tags_filter_group)
+            for osm_tags_filter_group in cast(GroupedOsmTagsFilter, osm_tags_filter).values()
+        )
+
+    raise AttributeError(
+        "Provided tags don't match required type definitions"
+        " (OsmTagsFilter or GroupedOsmTagsFilter)."
+    )
+
+
 def _merge_grouped_osm_tags_filter(grouped_filter: GroupedOsmTagsFilter) -> OsmTagsFilter:
     """
     Merge grouped osm tags filter into a base one.
 
     Function merges all filter categories into a single one for an OSM loader to use.
 
     Args:
@@ -106,23 +136,41 @@
 
     result: OsmTagsFilter = {}
     for osm_tags_filter in osm_tags_filters:
         for osm_tag_key, osm_tag_value in osm_tags_filter.items():
             if osm_tag_key not in result:
                 result[osm_tag_key] = []
 
+            is_current_value_positive = (
+                isinstance(result[osm_tag_key], (list, bool)) and result[osm_tag_key]
+            )
+            is_current_value_negative = result[osm_tag_key] == False  # noqa: E712
+
+            # If current value is negative and filter already have positive value
+            # If current value is positive and filter already have negative value
+            if (is_current_value_positive and osm_tag_value == False) or (  # noqa: E712
+                is_current_value_negative and osm_tag_value != False  # noqa: E712
+            ):
+                raise ValueError(
+                    "Provided OSM tags filter values cannot be merged."
+                    f" There is a conflict between the following values with '{osm_tag_key}' key:"
+                    f" {result[osm_tag_key]} and {osm_tag_value}."
+                )
+
             # If filter is already a positive boolean, skip
             if isinstance(result[osm_tag_key], bool) and result[osm_tag_key]:
                 continue
 
             current_values_list = cast(list[str], result[osm_tag_key])
 
             # Check bool
-            if isinstance(osm_tag_value, bool) and osm_tag_value:
+            if osm_tag_value == True:  # noqa: E712
                 result[osm_tag_key] = True
+            elif osm_tag_value == False:  # noqa: E712
+                result[osm_tag_key] = False
             # Check string
             elif isinstance(osm_tag_value, str) and osm_tag_value not in current_values_list:
                 current_values_list.append(osm_tag_value)
             # Check list
             elif isinstance(osm_tag_value, list):
                 new_values = [value for value in osm_tag_value if value not in current_values_list]
                 current_values_list.extend(new_values)
```

### Comparing `quackosm-0.5.3/quackosm/_osm_way_polygon_features.py` & `quackosm-0.6.0/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/_rich_progress.py` & `quackosm-0.6.0/quackosm/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/_typing.py` & `quackosm-0.6.0/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/cli.py` & `quackosm-0.6.0/quackosm/cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/conftest.py` & `quackosm-0.6.0/quackosm/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/functions.py` & `quackosm-0.6.0/quackosm/functions.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_extracts/__init__.py` & `quackosm-0.6.0/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.6.0/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_extracts/bbbike.py` & `quackosm-0.6.0/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.6.0/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.6.0/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/osm_way_polygon_features.json` & `quackosm-0.6.0/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/quackosm/pbf_file_reader.py` & `quackosm-0.6.0/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,21 @@
 from geoarrow.pyarrow import io
 from pyarrow_ops import drop_duplicates
 from shapely.geometry import LinearRing, Polygon
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 from quackosm._constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
 from quackosm._exceptions import EmptyResultWarning
-from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter, merge_osm_tags_filter
+from quackosm._osm_tags_filters import (
+    GroupedOsmTagsFilter,
+    OsmTagsFilter,
+    check_if_any_osm_tags_filter_value_is_positive,
+    merge_key_value_pairs_to_osm_tags_filter,
+    merge_osm_tags_filter,
+)
 from quackosm._osm_way_polygon_features import OsmWayPolygonConfig, parse_dict_to_config_object
 from quackosm._rich_progress import (  # type: ignore[attr-defined]
     TaskProgressBar,
     TaskProgressSpinner,
     log_message,
     show_total_elapsed_time,
 )
@@ -134,15 +140,21 @@
             osm_extract_source (OsmExtractSource): A source for automatic downloading of
                 OSM extracts. Can be Geofabrik, BBBike, OSMfr or any. Defaults to `any`.
             silent_mode (bool): Disable progress bars.
             allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't
                 covered by any OSM extract. Defaults to `False`.
         """
         self.tags_filter = tags_filter
-        self.merged_tags_filter = merge_osm_tags_filter(tags_filter) if tags_filter else None
+        self.is_tags_filter_positive = (
+            check_if_any_osm_tags_filter_value_is_positive(self.tags_filter)
+            if self.tags_filter is not None
+            else False
+        )
+        self.expanded_tags_filter: Optional[Union[GroupedOsmTagsFilter, OsmTagsFilter]] = None
+        self.merged_tags_filter: Optional[Union[GroupedOsmTagsFilter, OsmTagsFilter]] = None
         self.geometry_filter = geometry_filter
         self.allow_uncovered_geometry = allow_uncovered_geometry
         self.osm_extract_source = osm_extract_source
         self.working_directory = Path(working_directory)
         self.working_directory.mkdir(parents=True, exist_ok=True)
         self.connection: duckdb.DuckDBPyConnection = None
         self.encountered_query_exception = False
@@ -211,15 +223,17 @@
         Returns:
             Path: Path to the generated GeoParquet file.
         """
         if filter_osm_ids is None:
             filter_osm_ids = []
 
         if explode_tags is None:
-            explode_tags = self.tags_filter is not None and not keep_all_tags
+            explode_tags = (
+                self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
+            )
 
         with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as self.tmp_dir_name:
             self.tmp_dir_path = Path(self.tmp_dir_name)
             try:
                 self.encountered_query_exception = False
                 self.connection = _set_up_duckdb_connection(tmp_dir_path=self.tmp_dir_path)
                 result_file_path = result_file_path or self._generate_result_file_path(
@@ -290,15 +304,17 @@
                 " geometry_filter first: PbfFileReader(geometry_filter=..., **kwargs)."
             )
 
         if filter_osm_ids is None:
             filter_osm_ids = []
 
         if explode_tags is None:
-            explode_tags = self.tags_filter is not None and not keep_all_tags
+            explode_tags = (
+                self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
+            )
 
         result_file_path = Path(
             result_file_path
             or self._generate_result_file_path_from_geometry(
                 filter_osm_ids=filter_osm_ids,
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
@@ -415,15 +431,17 @@
         if isinstance(file_paths, (str, Path)):
             file_paths = [file_paths]
 
         if filter_osm_ids is None:
             filter_osm_ids = []
 
         if explode_tags is None:
-            explode_tags = self.tags_filter is not None and not keep_all_tags
+            explode_tags = (
+                self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
+            )
 
         parsed_geoparquet_files = []
         for file_path in file_paths:
             parsed_geoparquet_file = self.convert_pbf_to_gpq(
                 file_path,
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
@@ -608,14 +626,24 @@
         ignore_cache: bool = False,
         save_as_wkt: bool = False,
     ) -> Path:
         if not result_file_path.exists() or ignore_cache:
             start_time = time.time()
 
             elements = self.connection.sql(f"SELECT * FROM ST_READOSM('{Path(pbf_path)}');")
+
+            if self.tags_filter is None:
+                self.expanded_tags_filter = None
+                self.merged_tags_filter = None
+            else:
+                self.expanded_tags_filter = self._expand_osm_tags_filter(elements)
+                self.merged_tags_filter = merge_osm_tags_filter(
+                    cast(Union[GroupedOsmTagsFilter, OsmTagsFilter], self.expanded_tags_filter)
+                )
+
             converted_osm_parquet_files = self._prefilter_elements_ids(elements, filter_osm_ids)
 
             self._delete_directories(
                 [
                     "nodes_filtered_non_distinct_ids",
                     "nodes_prepared_ids",
                     "ways_valid_ids",
@@ -830,14 +858,80 @@
             ]
             return geometry.__class__(
                 sorted(oriented_geoms, key=lambda geom: (geom.centroid.x, geom.centroid.y))
             )
 
         return geometry
 
+    def _expand_osm_tags_filter(
+        self, elements: "duckdb.DuckDBPyRelation"
+    ) -> Union[GroupedOsmTagsFilter, OsmTagsFilter]:
+        is_any_key_expandable = False
+        if is_expected_type(self.tags_filter, GroupedOsmTagsFilter):
+            grouped_osm_tags_filter = cast(GroupedOsmTagsFilter, self.tags_filter)
+            is_any_key_expandable = any(
+                any("*" in key for key in osm_tags_filter.keys())
+                for osm_tags_filter in grouped_osm_tags_filter.values()
+            )
+        else:
+            osm_tags_filter = cast(OsmTagsFilter, self.tags_filter)
+            is_any_key_expandable = any("*" in key for key in osm_tags_filter.keys())
+
+        if not is_any_key_expandable:
+            return cast(Union[GroupedOsmTagsFilter, OsmTagsFilter], self.tags_filter)
+
+        with TaskProgressSpinner("Preparing OSM tags filter", "0", self.silent_mode):
+            if is_expected_type(self.tags_filter, GroupedOsmTagsFilter):
+                grouped_osm_tags_filter = cast(GroupedOsmTagsFilter, self.tags_filter)
+                return {
+                    group: self._expand_single_osm_tags_filter(elements, osm_tags_filter)
+                    for group, osm_tags_filter in grouped_osm_tags_filter.items()
+                }
+            else:
+                osm_tags_filter = cast(OsmTagsFilter, self.tags_filter)
+                return self._expand_single_osm_tags_filter(elements, osm_tags_filter)
+
+    def _expand_single_osm_tags_filter(
+        self, elements: "duckdb.DuckDBPyRelation", osm_tags_filter: OsmTagsFilter
+    ) -> OsmTagsFilter:
+        osm_tags_filter_key_value_pairs = []
+        for osm_tag_filter_key, osm_tag_filter_value in osm_tags_filter.items():
+            new_tags_to_add = [osm_tag_filter_key]
+
+            if "*" in osm_tag_filter_key:
+                sql_like_value = self._replace_star_value_in_string(osm_tag_filter_key)
+
+                new_tags_to_add = list(
+                    self.connection.sql(
+                        f"""
+                        WITH distinct_tags AS (
+                            SELECT DISTINCT unnest(map_keys(tags)) tag
+                            FROM ({elements.sql_query()})
+                            WHERE tags IS NOT NULL
+                        )
+                        SELECT tag FROM distinct_tags
+                        WHERE tag LIKE '{sql_like_value}'
+                        """
+                    ).fetchnumpy()["tag"]
+                )
+
+            for new_tag_to_add in sorted(new_tags_to_add, key=str.casefold):
+                osm_tags_filter_key_value_pairs.append((new_tag_to_add, osm_tag_filter_value))
+
+        return merge_key_value_pairs_to_osm_tags_filter(osm_tags_filter_key_value_pairs)
+
+    def _replace_star_value_in_string(self, value: str) -> str:
+        value_with_star = value
+
+        while "**" in value_with_star:
+            value_with_star = value_with_star.replace("**", "*")
+
+        value_with_percent = value_with_star.replace("*", "%")
+        return self._sql_escape(value_with_percent)
+
     def _prefilter_elements_ids(
         self, elements: "duckdb.DuckDBPyRelation", filter_osm_ids: list[str]
     ) -> ConvertedOSMParquetFiles:
         sql_filter = self._generate_osm_tags_sql_filter()
         filtered_tags_clause = self._generate_filtered_tags_clause()
 
         is_intersecting = self.geometry_filter is not None
@@ -1153,36 +1247,59 @@
                         raise ex
                     sleep(0.5)
                 finally:
                     tries -= 1
 
     def _generate_osm_tags_sql_filter(self) -> str:
         """Prepare features filter clauses based on tags filter."""
-        filter_clauses = ["(1=1)"]
+        positive_filter_clauses: list[str] = []
+        negative_filter_clauses: list[str] = []
 
         if self.merged_tags_filter:
-            filter_clauses.clear()
+            positive_filter_clauses.clear()
 
             for filter_tag_key, filter_tag_value in self.merged_tags_filter.items():
-                if isinstance(filter_tag_value, bool) and filter_tag_value:
-                    filter_clauses.append(f"(list_contains(map_keys(tags), '{filter_tag_key}'))")
-                elif isinstance(filter_tag_value, str):
-                    escaped_value = self._sql_escape(filter_tag_value)
-                    filter_clauses.append(
-                        f"list_extract(map_extract(tags, '{filter_tag_key}'), 1) ="
-                        f" '{escaped_value}'"
-                    )
-                elif isinstance(filter_tag_value, list) and filter_tag_value:
-                    values_list = [f"'{self._sql_escape(value)}'" for value in filter_tag_value]
-                    filter_clauses.append(
-                        f"list_extract(map_extract(tags, '{filter_tag_key}'), 1) IN"
-                        f" ({', '.join(values_list)})"
-                    )
+                if filter_tag_value == True:  # noqa: E712
+                    positive_filter_clauses.append(
+                        f"(list_contains(map_keys(tags), '{filter_tag_key}'))"
+                    )
+                elif filter_tag_value == False:  # noqa: E712
+                    negative_filter_clauses.append(
+                        f"(not list_contains(map_keys(tags), '{filter_tag_key}'))"
+                    )
+                elif isinstance(filter_tag_value, (str, list)):
+                    filter_tag_values = filter_tag_value
+                    if isinstance(filter_tag_value, str):
+                        filter_tag_values = [filter_tag_value]
+                    for single_filter_tag_value in filter_tag_values:
+                        if "*" in single_filter_tag_value:
+                            sql_like_value = self._replace_star_value_in_string(
+                                single_filter_tag_value
+                            )
+                            positive_filter_clauses.append(
+                                f"(list_extract(map_extract(tags, '{filter_tag_key}'), 1) LIKE"
+                                f" '{sql_like_value}')"
+                            )
+                        else:
+                            escaped_value = self._sql_escape(single_filter_tag_value)
+                            positive_filter_clauses.append(
+                                f"(list_extract(map_extract(tags, '{filter_tag_key}'), 1) ="
+                                f" '{escaped_value}')"
+                            )
+
+        if not positive_filter_clauses:
+            positive_filter_clauses.append("(1=1)")
+
+        joined_filter_clauses = " OR ".join(positive_filter_clauses)
+        if negative_filter_clauses:
+            joined_filter_clauses = (
+                f"({joined_filter_clauses}) AND ({' AND '.join(negative_filter_clauses)})"
+            )
 
-        return " OR ".join(filter_clauses)
+        return joined_filter_clauses
 
     def _generate_filtered_tags_clause(self) -> str:
         """Prepare filtered tags clause by removing tags commonly ignored by OGR."""
         tags_to_ignore = [
             "area",
             "created_by",
             "converted_by",
@@ -2186,15 +2303,15 @@
 
     def _generate_osm_tags_sql_select(
         self, parsed_geometries: "duckdb.DuckDBPyRelation", keep_all_tags: bool, explode_tags: bool
     ) -> list[str]:
         """Prepare features filter clauses based on tags filter."""
         osm_tag_keys_select_clauses = []
 
-        no_tags_filter = not self.merged_tags_filter
+        no_tags_filter = not self.merged_tags_filter or not self.is_tags_filter_positive
         tags_filter_and_keep_all_tags = self.merged_tags_filter and keep_all_tags
         keep_tags_compact = not explode_tags
 
         if (no_tags_filter and keep_tags_compact) or (
             tags_filter_and_keep_all_tags and keep_tags_compact
         ):
             osm_tag_keys_select_clauses = ["tags"]
@@ -2213,65 +2330,76 @@
             osm_tag_keys_select_clauses = [
                 f"list_extract(map_extract(tags, '{osm_tag_key}'), 1) as \"{osm_tag_key}\""
                 for osm_tag_key in sorted(list(osm_tag_keys))
             ]
         elif self.merged_tags_filter and keep_tags_compact:
             filter_tag_clauses = []
             for filter_tag_key, filter_tag_value in self.merged_tags_filter.items():
-                if isinstance(filter_tag_value, bool) and filter_tag_value:
+                if filter_tag_value == True:  # noqa: E712
                     filter_tag_clauses.append(f"tag_entry.key = '{filter_tag_key}'")
-                elif isinstance(filter_tag_value, str):
-                    escaped_value = self._sql_escape(filter_tag_value)
-                    filter_tag_clauses.append(
-                        f"(tag_entry.key = '{filter_tag_key}' AND tag_entry.value ="
-                        f" '{escaped_value}')"
-                    )
-                elif isinstance(filter_tag_value, list) and filter_tag_value:
-                    values_list = [f"'{self._sql_escape(value)}'" for value in filter_tag_value]
-                    filter_tag_clauses.append(
-                        f"(tag_entry.key = '{filter_tag_key}' AND tag_entry.value IN"
-                        f" ({', '.join(values_list)}))"
-                    )
+                elif isinstance(filter_tag_value, (str, list)):
+                    filter_tag_values = filter_tag_value
+                    if isinstance(filter_tag_value, str):
+                        filter_tag_values = [filter_tag_value]
+                    for single_filter_tag_value in filter_tag_values:
+                        if "*" in single_filter_tag_value:
+                            sql_like_value = self._replace_star_value_in_string(
+                                single_filter_tag_value
+                            )
+                            filter_tag_clauses.append(
+                                f"(tag_entry.key = '{filter_tag_key}' AND tag_entry.value LIKE"
+                                f" '{sql_like_value}')"
+                            )
+                        else:
+                            escaped_value = self._sql_escape(single_filter_tag_value)
+                            filter_tag_clauses.append(
+                                f"(tag_entry.key = '{filter_tag_key}' AND tag_entry.value ="
+                                f" '{escaped_value}')"
+                            )
             osm_tag_keys_select_clauses = [
                 f"""
                 map_from_entries(
                     [
                         tag_entry
                         for tag_entry in map_entries(tags)
                         if {" OR ".join(filter_tag_clauses)}
                     ]
                 ) as tags
                 """
             ]
         elif self.merged_tags_filter and explode_tags:
             for filter_tag_key, filter_tag_value in self.merged_tags_filter.items():
-                if isinstance(filter_tag_value, bool) and filter_tag_value:
+                if filter_tag_value == True:  # noqa: E712
                     osm_tag_keys_select_clauses.append(
                         f"list_extract(map_extract(tags, '{filter_tag_key}'), 1) as"
                         f' "{filter_tag_key}"'
                     )
-                elif isinstance(filter_tag_value, str):
-                    escaped_value = self._sql_escape(filter_tag_value)
-                    osm_tag_keys_select_clauses.append(
-                        f"""
-                        CASE WHEN list_extract(
-                            map_extract(tags, '{filter_tag_key}'), 1
-                        ) = '{escaped_value}'
-                        THEN '{escaped_value}'
-                        ELSE NULL
-                        END as "{filter_tag_key}"
-                        """
-                    )
-                elif isinstance(filter_tag_value, list) and filter_tag_value:
-                    values_list = [f"'{self._sql_escape(value)}'" for value in filter_tag_value]
+                elif isinstance(filter_tag_value, (str, list)):
+                    filter_tag_clauses = []
+                    filter_tag_values = filter_tag_value
+                    if isinstance(filter_tag_value, str):
+                        filter_tag_values = [filter_tag_value]
+                    for single_filter_tag_value in filter_tag_values:
+                        if "*" in single_filter_tag_value:
+                            sql_like_value = self._replace_star_value_in_string(
+                                single_filter_tag_value
+                            )
+                            filter_tag_clauses.append(
+                                f"list_extract(map_extract(tags, '{filter_tag_key}'), 1) LIKE"
+                                f" '{sql_like_value}'"
+                            )
+                        else:
+                            escaped_value = self._sql_escape(single_filter_tag_value)
+                            filter_tag_clauses.append(
+                                f"list_extract(map_extract(tags, '{filter_tag_key}'), 1) ="
+                                f" '{escaped_value}'"
+                            )
                     osm_tag_keys_select_clauses.append(
                         f"""
-                        CASE WHEN list_extract(
-                            map_extract(tags, '{filter_tag_key}'), 1
-                        ) IN ({', '.join(values_list)})
+                        CASE WHEN {' OR '.join(filter_tag_clauses)}
                         THEN list_extract(map_extract(tags, '{filter_tag_key}'), 1)
                         ELSE NULL
                         END as "{filter_tag_key}"
                         """
                     )
 
         if len(osm_tag_keys_select_clauses) > 100:
@@ -2308,46 +2436,56 @@
                 in the `tags_filter`. When `True`, will override the optional grouping defined
                 in the `tags_filter`. Defaults to `False`.
 
         Returns:
             duckdb.DuckDBPyRelation: Parsed features_relation.
         """
         if (
-            not self.tags_filter
-            or not is_expected_type(self.tags_filter, GroupedOsmTagsFilter)
+            not self.expanded_tags_filter
+            or not self.is_tags_filter_positive
+            or not is_expected_type(self.expanded_tags_filter, GroupedOsmTagsFilter)
             or keep_all_tags
         ):
             return features_relation
 
         grouped_features_relation: "duckdb.DuckDBPyRelation"
-        grouped_tags_filter = cast(GroupedOsmTagsFilter, self.tags_filter)
+        grouped_tags_filter = cast(GroupedOsmTagsFilter, self.expanded_tags_filter)
 
         if explode_tags:
             case_clauses = []
             for group_name in sorted(grouped_tags_filter.keys()):
                 osm_filter = grouped_tags_filter[group_name]
                 case_when_clauses = []
                 for osm_tag_key, osm_tag_value in osm_filter.items():
-                    if isinstance(osm_tag_value, bool) and osm_tag_value:
+                    if osm_tag_value == True:  # noqa: E712
                         case_when_clauses.append(
                             f"WHEN \"{osm_tag_key}\" IS NOT NULL THEN '{osm_tag_key}=' ||"
                             f' "{osm_tag_key}"'
                         )
-                    elif isinstance(osm_tag_value, str):
-                        escaped_value = self._sql_escape(osm_tag_value)
+                    elif isinstance(osm_tag_value, (str, list)):
+                        filter_tag_clauses = []
+                        osm_tag_values = osm_tag_value
+                        if isinstance(osm_tag_value, str):
+                            osm_tag_values = [osm_tag_value]
+                        for single_osm_tag_value in osm_tag_values:
+                            if "*" in single_osm_tag_value:
+                                sql_like_value = self._replace_star_value_in_string(
+                                    single_osm_tag_value
+                                )
+                                filter_tag_clauses.append(
+                                    f"\"{osm_tag_key}\" LIKE '{sql_like_value}'"
+                                )
+                            else:
+                                escaped_value = self._sql_escape(single_osm_tag_value)
+                                filter_tag_clauses.append(f"\"{osm_tag_key}\" = '{escaped_value}'")
                         case_when_clauses.append(
-                            f"WHEN \"{osm_tag_key}\" = '{escaped_value}' THEN '{osm_tag_key}=' ||"
+                            f"WHEN {' OR '.join(filter_tag_clauses)} THEN '{osm_tag_key}=' ||"
                             f' "{osm_tag_key}"'
                         )
-                    elif isinstance(osm_tag_value, list) and osm_tag_value:
-                        values_list = [f"'{self._sql_escape(value)}'" for value in osm_tag_value]
-                        case_when_clauses.append(
-                            f"WHEN \"{osm_tag_key}\" IN ({', '.join(values_list)}) THEN"
-                            f" '{osm_tag_key}=' || \"{osm_tag_key}\""
-                        )
+
                 case_clause = f'CASE {" ".join(case_when_clauses)} END AS "{group_name}"'
                 case_clauses.append(case_clause)
 
             joined_case_clauses = ", ".join(case_clauses)
             grouped_features_relation = self.connection.sql(
                 f"""
                 SELECT feature_id, {joined_case_clauses}, geometry
@@ -2358,31 +2496,40 @@
             case_clauses = []
             group_names = sorted(grouped_tags_filter.keys())
             for group_name in group_names:
                 osm_filter = grouped_tags_filter[group_name]
                 case_when_clauses = []
                 for osm_tag_key, osm_tag_value in osm_filter.items():
                     element_clause = f"element_at(tags, '{osm_tag_key}')[1]"
-                    if isinstance(osm_tag_value, bool) and osm_tag_value:
+                    if osm_tag_value == True:  # noqa: E712
                         case_when_clauses.append(
                             f"WHEN {element_clause} IS NOT NULL THEN '{osm_tag_key}=' ||"
                             f" {element_clause}"
                         )
-                    elif isinstance(osm_tag_value, str):
-                        escaped_value = self._sql_escape(osm_tag_value)
+                    elif isinstance(osm_tag_value, (str, list)):
+                        filter_tag_clauses = []
+                        osm_tag_values = osm_tag_value
+                        if isinstance(osm_tag_value, str):
+                            osm_tag_values = [osm_tag_value]
+                        for single_osm_tag_value in osm_tag_values:
+                            if "*" in single_osm_tag_value:
+                                sql_like_value = self._replace_star_value_in_string(
+                                    single_osm_tag_value
+                                )
+                                filter_tag_clauses.append(
+                                    f"{element_clause} LIKE '{sql_like_value}'"
+                                )
+                            else:
+                                escaped_value = self._sql_escape(single_osm_tag_value)
+                                filter_tag_clauses.append(f"{element_clause} = '{escaped_value}'")
                         case_when_clauses.append(
-                            f"WHEN {element_clause} = '{escaped_value}' THEN '{osm_tag_key}=' ||"
+                            f"WHEN {' OR '.join(filter_tag_clauses)} THEN '{osm_tag_key}=' ||"
                             f" {element_clause}"
                         )
-                    elif isinstance(osm_tag_value, list) and osm_tag_value:
-                        values_list = [f"'{self._sql_escape(value)}'" for value in osm_tag_value]
-                        case_when_clauses.append(
-                            f"WHEN {element_clause} IN ({', '.join(values_list)}) THEN"
-                            f" '{osm_tag_key}=' || {element_clause}"
-                        )
+
                 case_clause = f'CASE {" ".join(case_when_clauses)} END'
                 case_clauses.append(case_clause)
 
             group_names_as_sql_strings = [f"'{group_name}'" for group_name in group_names]
             groups_map = (
                 f"map([{', '.join(group_names_as_sql_strings)}], [{', '.join(case_clauses)}])"
             )
```

### Comparing `quackosm-0.5.3/tests/base/conftest.py` & `quackosm-0.6.0/tests/base/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/base/test_cli.py` & `quackosm-0.6.0/tests/base/test_cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/base/test_osm_extracts.py` & `quackosm-0.6.0/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/base/test_pbf_file_reader.py` & `quackosm-0.6.0/tests/base/test_pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,77 +37,14 @@
 from quackosm.pbf_file_reader import PbfFileReader
 from tests.base.conftest import geometry_box
 
 ut = TestCase()
 LFS_DIRECTORY_URL = "https://github.com/kraina-ai/srai-test-files/raw/main/files/"
 
 
-@pytest.mark.parametrize(  # type: ignore
-    "test_file_name,query,expected_result_length,expected_features_columns_length",
-    [
-        (
-            "d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf",
-            None,
-            678,
-            271,
-        ),
-        (
-            "eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf",
-            None,
-            1,
-            22,
-        ),
-        ("529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf", None, 0, 0),
-        (
-            "d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf",
-            HEX2VEC_FILTER,
-            97,
-            10,
-        ),
-        (
-            "eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf",
-            HEX2VEC_FILTER,
-            0,
-            0,
-        ),
-        (
-            "d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf",
-            GEOFABRIK_LAYERS,
-            433,
-            22,
-        ),
-        (
-            "eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf",
-            GEOFABRIK_LAYERS,
-            0,
-            0,
-        ),
-    ],
-)
-def test_pbf_reader(
-    test_file_name: str,
-    query: OsmTagsFilter,
-    expected_result_length: int,
-    expected_features_columns_length: int,
-):
-    """Test proper files loading in `PbfFileReader`."""
-    features_gdf = PbfFileReader(tags_filter=query).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / test_file_name],
-        explode_tags=True,
-        ignore_cache=True,
-    )
-    assert (
-        len(features_gdf) == expected_result_length
-    ), f"Mismatched result length ({len(features_gdf)}, {expected_result_length})"
-    assert len(features_gdf.columns) == expected_features_columns_length + 1, (
-        f"Mismatched columns length ({len(features_gdf.columns)},"
-        f" {expected_features_columns_length + 1})"
-    )
-
-
 @pytest.mark.parametrize("tags_filter", [None, HEX2VEC_FILTER, GEOFABRIK_LAYERS])  # type: ignore
 @pytest.mark.parametrize("explode_tags", [None, True, False])  # type: ignore
 @pytest.mark.parametrize("keep_all_tags", [True, False])  # type: ignore
 @pytest.mark.parametrize("save_as_wkt", [True, False])  # type: ignore
 def test_pbf_to_geoparquet_parsing(
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]],
     explode_tags: Optional[bool],
@@ -255,65 +192,14 @@
         features_gdf = PbfFileReader(
             geometry_filter=geometry, allow_uncovered_geometry=allow_uncovered_geometry
         ).get_features_gdf_from_geometry(ignore_cache=True)
         assert len(features_gdf) == 0
 
 
 @pytest.mark.parametrize(  # type: ignore
-    "filter_osm_id,osm_tags_filter,keep_all_tags,expected_tags_keys",
-    [
-        ("way/389888402", {"building": "apartments"}, False, ["building"]),
-        (
-            "way/389888402",
-            {"building": "apartments"},
-            True,
-            [
-                "addr:city",
-                "addr:country",
-                "addr:housenumber",
-                "addr:postcode",
-                "addr:street",
-                "building",
-                "building:levels",
-            ],
-        ),
-        ("way/627022271", {"leisure": "garden"}, False, ["leisure"]),
-        (
-            "way/627022271",
-            {"leisure": "garden"},
-            True,
-            [
-                "addr:country",
-                "leisure",
-                "name",
-            ],
-        ),
-    ],
-)
-def test_pbf_reader_proper_tags_reading(
-    filter_osm_id: str,
-    osm_tags_filter: Union[OsmTagsFilter, GroupedOsmTagsFilter],
-    keep_all_tags: bool,
-    expected_tags_keys: list[str],
-):
-    """Test proper tags reading with filtering in `PbfFileReader`."""
-    file_name = "monaco.osm.pbf"
-    features_gdf = PbfFileReader(tags_filter=osm_tags_filter).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
-        ignore_cache=True,
-        filter_osm_ids=[filter_osm_id],
-        explode_tags=False,
-        keep_all_tags=keep_all_tags,
-    )
-    assert len(features_gdf) == 1
-    returned_tags_keys = list(features_gdf.iloc[0].tags.keys())
-    ut.assertListEqual(returned_tags_keys, expected_tags_keys)
-
-
-@pytest.mark.parametrize(  # type: ignore
     "geometry",
     [
         box(
             minx=7.416486207767861,
             miny=43.7310867041912,
             maxx=7.421931388477276,
             maxy=43.73370705597216,
```

### Comparing `quackosm-0.5.3/tests/benchmark/test_big_file.py` & `quackosm-0.6.0/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.6.0/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.6.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.6.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.6.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/monaco.osm.pbf` & `quackosm-0.6.0/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/monaco_boundary.geojson` & `quackosm-0.6.0/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/tests/test_files/osmconf.ini` & `quackosm-0.6.0/tests/test_files/osmconf.ini`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.3/PKG-INFO` & `quackosm-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.5.3
+Version: 0.6.0
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -30,15 +30,15 @@
 Requires-Dist: typeguard
 Requires-Dist: psutil
 Requires-Dist: pooch
 Requires-Dist: tqdm
 Requires-Dist: beautifulsoup4
 Requires-Dist: pyarrow-ops
 Requires-Dist: requests
-Requires-Dist: typer[all]; extra == "cli"
+Requires-Dist: typer[all]>=0.9.0; extra == "cli"
 Requires-Dist: osmnx; extra == "cli"
 Requires-Dist: h3>=4.0.0b1; extra == "cli"
 Requires-Dist: h3ronpy>=0.18.0; extra == "cli"
 Requires-Dist: s2; extra == "cli"
 Requires-Dist: python-geohash; extra == "cli"
 Provides-Extra: cli
 Description-Content-Type: text/markdown
```

