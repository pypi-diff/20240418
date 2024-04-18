# Comparing `tmp/musify-0.9.0.tar.gz` & `tmp/musify-0.9.1.tar.gz`

## Comparing `musify-0.9.0.tar` & `musify-0.9.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 musify-0.9.0/musify/__init__.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 musify-0.9.0/musify/exception.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 musify-0.9.0/musify/field.py
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 musify-0.9.0/musify/report.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 musify-0.9.0/musify/types.py
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 musify-0.9.0/musify/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/__init__.py
--rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/authorise.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/exception.py
--rw-r--r--   0        0        0    10229 2020-02-02 00:00:00.000000 musify-0.9.0/musify/api/request.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/base.py
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/enum.py
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/printer.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 musify-0.9.0/musify/core/result.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/__init__.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/base.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/exception.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/image.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 musify-0.9.0/musify/file/path_mapper.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/__init__.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/collection.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/__init__.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/collection.py
--rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/core/object.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/__init__.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/base.py
--rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/collection.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/exception.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/__init__.py
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/library.py
--rw-r--r--   0        0        0    24639 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/library/musicbee.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/__init__.py
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/base.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/m3u.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/utils.py
--rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/playlist/xautopf.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/__init__.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/field.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/flac.py
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/m4a.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/mp3.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/track.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/utils.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/wma.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/base.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/reader.py
--rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/local/track/tags/writer.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/__init__.py
--rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/api.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/base.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/enum.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/exception.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/factory.py
--rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/library.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/object.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/response.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/types.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/__init__.py
--rw-r--r--   0        0        0    23087 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/check.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/search.py
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/core/processors/wrangle.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/base.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/exception.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/factory.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/library.py
--rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/object.py
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/processors.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/__init__.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/api.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/base.py
--rw-r--r--   0        0        0    29516 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/item.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/misc.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 musify-0.9.0/musify/libraries/remote/spotify/api/playlist.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/filter.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/handlers.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 musify-0.9.0/musify/log/logger.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/__init__.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/base.py
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/compare.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/download.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/exception.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/filter.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/filter_matcher.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/limit.py
--rw-r--r--   0        0        0    21695 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/match.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/sort.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 musify-0.9.0/musify/processors/time.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 musify-0.9.0/.gitignore
--rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.9.0/LICENSE
--rw-r--r--   0        0        0    15052 2020-02-02 00:00:00.000000 musify-0.9.0/README.md
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 musify-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 musify-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 musify-0.9.1/musify/__init__.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 musify-0.9.1/musify/exception.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 musify-0.9.1/musify/field.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 musify-0.9.1/musify/report.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 musify-0.9.1/musify/types.py
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 musify-0.9.1/musify/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/__init__.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/authorise.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/exception.py
+-rw-r--r--   0        0        0    10229 2020-02-02 00:00:00.000000 musify-0.9.1/musify/api/request.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/base.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/enum.py
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/printer.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 musify-0.9.1/musify/core/result.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/__init__.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/base.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/exception.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/image.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 musify-0.9.1/musify/file/path_mapper.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/__init__.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/collection.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/__init__.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/collection.py
+-rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/core/object.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/__init__.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/base.py
+-rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/collection.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/exception.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/__init__.py
+-rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/library.py
+-rw-r--r--   0        0        0    24639 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/library/musicbee.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/__init__.py
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/base.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/m3u.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/utils.py
+-rw-r--r--   0        0        0    28389 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/playlist/xautopf.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/__init__.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/field.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/flac.py
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/m4a.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/mp3.py
+-rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/track.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/utils.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/wma.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/base.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/reader.py
+-rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/local/track/tags/writer.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/__init__.py
+-rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/api.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/base.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/enum.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/exception.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/factory.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/library.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/object.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/response.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/types.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/__init__.py
+-rw-r--r--   0        0        0    23087 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/check.py
+-rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/search.py
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/core/processors/wrangle.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/base.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/exception.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/factory.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/library.py
+-rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/object.py
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/processors.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/__init__.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/api.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/base.py
+-rw-r--r--   0        0        0    29516 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/item.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/misc.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 musify-0.9.1/musify/libraries/remote/spotify/api/playlist.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/filter.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/handlers.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 musify-0.9.1/musify/log/logger.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/__init__.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/base.py
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/compare.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/download.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/exception.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/filter.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/filter_matcher.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/limit.py
+-rw-r--r--   0        0        0    22140 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/match.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/sort.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 musify-0.9.1/musify/processors/time.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 musify-0.9.1/.gitignore
+-rw-r--r--   0        0        0    35184 2020-02-02 00:00:00.000000 musify-0.9.1/LICENSE
+-rw-r--r--   0        0        0    15052 2020-02-02 00:00:00.000000 musify-0.9.1/README.md
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 musify-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 musify-0.9.1/PKG-INFO
```

### Comparing `musify-0.9.0/musify/exception.py` & `musify-0.9.1/musify/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/field.py` & `musify-0.9.1/musify/field.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/report.py` & `musify-0.9.1/musify/report.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/types.py` & `musify-0.9.1/musify/types.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/utils.py` & `musify-0.9.1/musify/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/api/authorise.py` & `musify-0.9.1/musify/api/authorise.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/api/exception.py` & `musify-0.9.1/musify/api/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/api/request.py` & `musify-0.9.1/musify/api/request.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/core/base.py` & `musify-0.9.1/musify/core/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/core/enum.py` & `musify-0.9.1/musify/core/enum.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/core/printer.py` & `musify-0.9.1/musify/core/printer.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/file/base.py` & `musify-0.9.1/musify/file/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/file/exception.py` & `musify-0.9.1/musify/file/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/file/image.py` & `musify-0.9.1/musify/file/image.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/file/path_mapper.py` & `musify-0.9.1/musify/file/path_mapper.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/collection.py` & `musify-0.9.1/musify/libraries/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/core/collection.py` & `musify-0.9.1/musify/libraries/core/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/core/object.py` & `musify-0.9.1/musify/libraries/core/object.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/collection.py` & `musify-0.9.1/musify/libraries/local/collection.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/exception.py` & `musify-0.9.1/musify/libraries/local/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/library/library.py` & `musify-0.9.1/musify/libraries/local/library/library.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/library/musicbee.py` & `musify-0.9.1/musify/libraries/local/library/musicbee.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/playlist/base.py` & `musify-0.9.1/musify/libraries/local/playlist/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/playlist/m3u.py` & `musify-0.9.1/musify/libraries/local/playlist/m3u.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/playlist/utils.py` & `musify-0.9.1/musify/libraries/local/playlist/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/playlist/xautopf.py` & `musify-0.9.1/musify/libraries/local/playlist/xautopf.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/field.py` & `musify-0.9.1/musify/libraries/local/track/field.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/flac.py` & `musify-0.9.1/musify/libraries/local/track/flac.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/m4a.py` & `musify-0.9.1/musify/libraries/local/track/m4a.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/mp3.py` & `musify-0.9.1/musify/libraries/local/track/mp3.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/track.py` & `musify-0.9.1/musify/libraries/local/track/track.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/utils.py` & `musify-0.9.1/musify/libraries/local/track/utils.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/wma.py` & `musify-0.9.1/musify/libraries/local/track/wma.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/tags/base.py` & `musify-0.9.1/musify/libraries/local/track/tags/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/tags/reader.py` & `musify-0.9.1/musify/libraries/local/track/tags/reader.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/local/track/tags/writer.py` & `musify-0.9.1/musify/libraries/local/track/tags/writer.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/api.py` & `musify-0.9.1/musify/libraries/remote/core/api.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/base.py` & `musify-0.9.1/musify/libraries/remote/core/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/enum.py` & `musify-0.9.1/musify/libraries/remote/core/enum.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/exception.py` & `musify-0.9.1/musify/libraries/remote/core/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/factory.py` & `musify-0.9.1/musify/libraries/remote/core/factory.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/library.py` & `musify-0.9.1/musify/libraries/remote/core/library.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/object.py` & `musify-0.9.1/musify/libraries/remote/core/object.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/response.py` & `musify-0.9.1/musify/libraries/remote/core/response.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/processors/check.py` & `musify-0.9.1/musify/libraries/remote/core/processors/check.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/processors/search.py` & `musify-0.9.1/musify/libraries/remote/core/processors/search.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/core/processors/wrangle.py` & `musify-0.9.1/musify/libraries/remote/core/processors/wrangle.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/base.py` & `musify-0.9.1/musify/libraries/remote/spotify/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/exception.py` & `musify-0.9.1/musify/libraries/remote/spotify/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/factory.py` & `musify-0.9.1/musify/libraries/remote/spotify/factory.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/library.py` & `musify-0.9.1/musify/libraries/remote/spotify/library.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/object.py` & `musify-0.9.1/musify/libraries/remote/spotify/object.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/processors.py` & `musify-0.9.1/musify/libraries/remote/spotify/processors.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/api/api.py` & `musify-0.9.1/musify/libraries/remote/spotify/api/api.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/api/base.py` & `musify-0.9.1/musify/libraries/remote/spotify/api/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/api/item.py` & `musify-0.9.1/musify/libraries/remote/spotify/api/item.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/api/misc.py` & `musify-0.9.1/musify/libraries/remote/spotify/api/misc.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/libraries/remote/spotify/api/playlist.py` & `musify-0.9.1/musify/libraries/remote/spotify/api/playlist.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/log/filter.py` & `musify-0.9.1/musify/log/filter.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/log/handlers.py` & `musify-0.9.1/musify/log/handlers.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/log/logger.py` & `musify-0.9.1/musify/log/logger.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/base.py` & `musify-0.9.1/musify/processors/base.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/compare.py` & `musify-0.9.1/musify/processors/compare.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/download.py` & `musify-0.9.1/musify/processors/download.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/exception.py` & `musify-0.9.1/musify/processors/exception.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/filter.py` & `musify-0.9.1/musify/processors/filter.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/filter_matcher.py` & `musify-0.9.1/musify/processors/filter_matcher.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/limit.py` & `musify-0.9.1/musify/processors/limit.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/match.py` & `musify-0.9.1/musify/processors/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,54 +300,41 @@
         match_on_filtered = set()
         for match_field in to_collection(match_on, set):
             if match_field == Tag.ALL:
                 match_on_filtered.update(match_field.all())
             else:
                 match_on_filtered.add(match_field)
 
+        min_score = limit_value(min_score, floor=0.01, ceil=1.0)
         max_score = limit_value(max_score, floor=0.01, ceil=1.0)
         self._log_algorithm(source=source, extra=[f"max_score={max_score}"])
 
         with ThreadPoolExecutor(thread_name_prefix="matcher") as executor:
             scores = self._score(
                 source=source,
                 results=results,
                 executor=executor,
                 match_on=match_on_filtered,
                 allow_karaoke=allow_karaoke
             )
 
-        result = None
-        best_score = 0
-
-        def sum_nested_scores(futures: list[list[Future[float]]]) -> float:
-            """Sum the scores from a given list of nested Futures"""
-            scores_summed = [sum(score.result() for score in nested) / len(nested) for nested in futures]
-            return sum(scores_summed) / len(scores_summed)
-
-        for result, result_scores in scores:
-            result_scores = [
-                sum_nested_scores(score) if isinstance(score, list) else score.result()
-                for score in result_scores.values()
-            ]
-            best_score = sum(result_scores) / len(result_scores)
-            if best_score > max_score:
-                break
+        result, score = self._get_match_from_scores(scores, max_score=max_score)
 
-        min_score = limit_value(min_score, floor=0.01, ceil=1.0)
-        if best_score > min_score:
+        if result is not None and score > min_score:
             extra = [
-                f"best score: {'%.2f' % round(best_score, 2)} > {'%.2f' % round(min_score, 2)}"
-                if best_score < max_score else
-                f"max score reached: {'%.2f' % round(best_score, 2)} > {'%.2f' % round(max_score, 2)}"
+                f"best score: {score:.2f} > {min_score:.2f}"
+                if score < max_score else
+                f"max score reached: {score:.2f} > {max_score:.2f}"
             ]
             self._log_match(source=source, result=result, extra=extra)
             return result
         else:
-            self._log_test(source=source, result=result, test=best_score, extra=[f"NO MATCH: {best_score}<{min_score}"])
+            self._log_test(
+                source=source, result=result, test=score, extra=[f"NO MATCH: {score:.2f}<{min_score:.2f}"]
+            )
 
     def _score[T: MusifyObject](
             self,
             source: T,
             results: Iterable[T],
             executor: Executor,
             match_on: set[TagField] = ALL_TAG_FIELDS,
@@ -428,14 +415,42 @@
                     source=item, results=result.items, match_on=match_on, allow_karaoke=allow_karaoke, executor=executor
                 )
                 for _, item_score in item_scores:
                     scores[Tag.ALL].append([score for score in item_score.values() if not isinstance(score, list)])
 
         return scores
 
+    def _get_match_from_scores[T: MusifyObject](
+            self,
+            scores: Iterable[tuple[T, dict[TagField, Future[float] | list[list[Future[float]]]]]],
+            max_score: float,
+    ) -> tuple[T | None, float]:
+        best_result = None
+        best_score = 0
+
+        def sum_nested_scores(futures: list[list[Future[float]]]) -> float:
+            """Sum the scores from a given list of nested Futures"""
+            scores_summed = [sum(score.result() for score in nested) / len(nested) for nested in futures]
+            return sum(scores_summed) / len(scores_summed)
+
+        for result, result_scores in scores:
+            result_scores = [
+                sum_nested_scores(score) if isinstance(score, list) else score.result()
+                for score in result_scores.values()
+            ]
+            score = sum(result_scores) / len(result_scores)
+            if score > best_score:
+                best_score = score
+                best_result = result
+
+            if best_score > max_score:
+                break
+
+        return best_result, best_score
+
     def as_dict(self) -> dict[str, Any]:
         return {
             "clean_tags": {
                 "remove_all": self.clean_tags_remove_all,
                 "split_all": self.clean_tags_split_all,
                 "config": self.clean_tags_config,
             },
```

### Comparing `musify-0.9.0/musify/processors/sort.py` & `musify-0.9.1/musify/processors/sort.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/musify/processors/time.py` & `musify-0.9.1/musify/processors/time.py`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/.gitignore` & `musify-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/LICENSE` & `musify-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/README.md` & `musify-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `musify-0.9.0/pyproject.toml` & `musify-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 [tool.hatch.version]
 source = "versioningit"
 
 [tool.versioningit.format]
 # WORKAROUND: commits for actual production releases keep getting identified as dirty and/or with distance
 #  Delete this config when fixed. It should be the commented lines below each (i.e. the default formats)
+#distance = "{next_version}.dev{distance}+{vcs}{rev}"
 dirty = "{base_version}"
 #dirty = "{base_version}+d{build_date:%Y%m%d}"
 distance-dirty = "{base_version}"
 #distance-dirty = "{next_version}.dev{distance}+{vcs}{rev}.d{build_date:%Y%m%d}"
 
 [tool.hatch.build.targets.sdist]
 include = ["musify"]
```

### Comparing `musify-0.9.0/PKG-INFO` & `musify-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: musify
-Version: 0.9.0
+Version: 0.9.1
 Summary: Synchronise your music library to local or remote libraries
 Project-URL: Documentation, https://geo-martino.github.io/musify/
 Project-URL: Release Notes, https://geo-martino.github.io/musify/release-history.html
 Project-URL: Contribute, https://geo-martino.github.io/musify/contributing.html
 Project-URL: Source code, https://github.com/geo-martino/musify
 Project-URL: Issues, https://github.com/geo-martino/musify/issues
 Author-email: George Martin Marino <gm.engineer+musify@pm.me>
@@ -27,25 +27,39 @@
 Requires-Dist: requests~=2.31
 Requires-Dist: tqdm~=4.66
 Requires-Dist: xmltodict~=0.13
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
 Requires-Dist: versioningit; extra == 'build'
 Provides-Extra: dev
+Requires-Dist: autodocsumm~=0.2; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: graphviz~=0.20; extra == 'dev'
 Requires-Dist: grip~=4.6; extra == 'dev'
-Requires-Dist: musify[build,docs,test]; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: pycountry~=23.12; extra == 'dev'
+Requires-Dist: pytest-mock~=3.12; extra == 'dev'
+Requires-Dist: pytest-xdist~=3.5; extra == 'dev'
+Requires-Dist: pytest~=8.0; extra == 'dev'
+Requires-Dist: pyyaml~=6.0; extra == 'dev'
+Requires-Dist: renku-sphinx-theme; extra == 'dev'
+Requires-Dist: requests-mock~=1.11; extra == 'dev'
+Requires-Dist: sphinx-autodoc-typehints<3.0,>=1.25; extra == 'dev'
+Requires-Dist: sphinxext-opengraph~=0.9; extra == 'dev'
+Requires-Dist: sphinx~=7.2; extra == 'dev'
+Requires-Dist: versioningit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm~=0.2; extra == 'docs'
 Requires-Dist: graphviz~=0.20; extra == 'docs'
-Requires-Dist: musify[build]; extra == 'docs'
+Requires-Dist: hatch; extra == 'docs'
 Requires-Dist: renku-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints<3.0,>=1.25; extra == 'docs'
 Requires-Dist: sphinxext-opengraph~=0.9; extra == 'docs'
 Requires-Dist: sphinx~=7.2; extra == 'docs'
+Requires-Dist: versioningit; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pycountry~=23.12; extra == 'test'
 Requires-Dist: pytest-mock~=3.12; extra == 'test'
 Requires-Dist: pytest-xdist~=3.5; extra == 'test'
 Requires-Dist: pytest~=8.0; extra == 'test'
 Requires-Dist: pyyaml~=6.0; extra == 'test'
 Requires-Dist: requests-mock~=1.11; extra == 'test'
```

