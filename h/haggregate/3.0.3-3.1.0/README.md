# Comparing `tmp/haggregate-3.0.3.tar.gz` & `tmp/haggregate-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haggregate-3.0.3.tar", last modified: Tue Apr 16 20:05:17 2024, max compression
+gzip compressed data, was "haggregate-3.1.0.tar", last modified: Thu Apr 18 14:00:47 2024, max compression
```

## Comparing `haggregate-3.0.3.tar` & `haggregate-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1539 2024-04-16 20:04:26.000000 haggregate-3.0.3/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       23 2022-12-03 16:55:59.000000 haggregate-3.0.3/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:23.000000 haggregate-3.0.3/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3104 2024-04-16 20:05:17.310176 haggregate-3.0.3/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      736 2022-03-05 20:41:23.000000 haggregate-3.0.3/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3931 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     5163 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1230 2022-12-03 16:55:59.000000 haggregate-3.0.3/docs/copyright.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      174 2022-11-13 20:46:58.000000 haggregate-3.0.3/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8445 2022-03-05 20:41:23.000000 haggregate-3.0.3/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/haggregate/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      177 2024-04-16 20:04:41.000000 haggregate-3.0.3/haggregate/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3038 2024-04-16 20:02:25.000000 haggregate-3.0.3/haggregate/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4949 2022-12-03 06:06:47.000000 haggregate-3.0.3/haggregate/haggregate.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)   399470 2022-12-03 16:57:22.000000 haggregate-3.0.3/haggregate/regularize.c
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/haggregate.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3104 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      568 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-13 10:11:23.000000 haggregate-3.0.3/haggregate.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       30 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2024-04-16 20:05:17.000000 haggregate-3.0.3/haggregate.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-16 20:05:17.310176 haggregate-3.0.3/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3134 2024-04-16 20:04:26.000000 haggregate-3.0.3/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:05:17.310176 haggregate-3.0.3/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:23.000000 haggregate-3.0.3/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4867 2022-12-03 16:58:54.000000 haggregate-3.0.3/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    11181 2022-12-03 16:55:59.000000 haggregate-3.0.3/tests/test_haggregate.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7021 2022-12-03 16:55:59.000000 haggregate-3.0.3/tests/test_regularize.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1660 2024-04-18 13:58:43.000000 haggregate-3.1.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       23 2022-12-03 16:55:59.000000 haggregate-3.1.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:23.000000 haggregate-3.1.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3225 2024-04-18 14:00:47.637156 haggregate-3.1.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      736 2022-03-05 20:41:23.000000 haggregate-3.1.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/docs/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.633156 haggregate-3.1.0/docs/_build/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.633156 haggregate-3.1.0/docs/_build/html/
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/docs/_build/html/_static/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      286 2023-03-29 08:31:27.000000 haggregate-3.1.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7791 2021-06-13 20:22:59.000000 haggregate-3.1.0/docs/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 haggregate-3.1.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2023-03-29 08:31:27.000000 haggregate-3.1.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6705 2024-04-18 13:58:43.000000 haggregate-3.1.0/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     5163 2024-04-18 13:58:43.000000 haggregate-3.1.0/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1230 2022-12-03 16:55:59.000000 haggregate-3.1.0/docs/copyright.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:23.000000 haggregate-3.1.0/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      174 2022-11-13 20:46:58.000000 haggregate-3.1.0/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6234 2024-04-18 13:58:43.000000 haggregate-3.1.0/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/haggregate/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      177 2024-04-18 14:00:20.000000 haggregate-3.1.0/haggregate/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3272 2024-04-18 13:58:43.000000 haggregate-3.1.0/haggregate/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5044 2024-04-18 13:58:43.000000 haggregate-3.1.0/haggregate/haggregate.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   434727 2024-04-18 13:59:41.000000 haggregate-3.1.0/haggregate/regularize.c
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/haggregate.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3225 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      729 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-13 10:11:23.000000 haggregate-3.1.0/haggregate.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       30 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       11 2024-04-18 14:00:47.000000 haggregate-3.1.0/haggregate.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-18 14:00:47.637156 haggregate-3.1.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3134 2024-04-18 13:40:11.000000 haggregate-3.1.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-18 14:00:47.637156 haggregate-3.1.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:23.000000 haggregate-3.1.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6617 2024-04-18 13:58:43.000000 haggregate-3.1.0/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    11181 2022-12-03 16:55:59.000000 haggregate-3.1.0/tests/test_haggregate.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8934 2024-04-18 13:58:43.000000 haggregate-3.1.0/tests/test_regularize.py
```

### Comparing `haggregate-3.0.3/HISTORY.rst` & `haggregate-3.1.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+3.1.0 (2024-04-18)
+==================
+
+- Use different regularization modes for interval and instantaneous
+  variables.
+
 3.0.3 (2024-04-16)
 ==================
 
 - Allow htimeseries 7.
 
 3.0.2 (2023-12-20)
 ==================
```

### Comparing `haggregate-3.0.3/PKG-INFO` & `haggregate-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haggregate
-Version: 3.0.3
+Version: 3.1.0
 Summary: Aggregates htimeseries to larger steps
 Home-page: https://github.com/openmeteo/haggregate
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: haggregate
 Classifier: Development Status :: 4 - Beta
@@ -46,14 +46,20 @@
 * Documentation: https://haggregate.readthedocs.io.
 
 
 =======
 History
 =======
 
+3.1.0 (2024-04-18)
+==================
+
+- Use different regularization modes for interval and instantaneous
+  variables.
+
 3.0.3 (2024-04-16)
 ==================
 
 - Allow htimeseries 7.
 
 3.0.2 (2023-12-20)
 ==================
```

### Comparing `haggregate-3.0.3/README.rst` & `haggregate-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.3/docs/api.rst` & `haggregate-3.1.0/docs/api.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,28 @@
 ===
 API
 ===
 
-.. function:: haggregate.regularize(ts, new_date_flag="DATEINSERT")
+.. function:: haggregate.regularize(ts, new_date_flag="DATEINSERT", mode=haggregate.RegularizationMode.INTERVAL)
 
    Process *ts* (a HTimeseries_ object) and return a new time series
    (HTimeseries_ object), with a strict time step.
 
-   The source time series, *ts*, must not be an irregular time series;
-   it must have a time step, but this time step may have disturbances.
-   For example, it may be a ten-minute time series like this::
-
-       2008-02-07 10:10 10.54 
-       2008-02-07 10:20 10.71 
-       2008-02-07 10:41 10.93 
-       2008-02-07 10:50 11.10 
-       2008-02-07 11:00 11.23 
-
-   The above has a missing record (10:30) and a disturbance in the time
-   stamp of another record (10:41). :func:`regularize` would convert it
-   to this::
-
-       2008-02-07 10:10 10.54 
-       2008-02-07 10:20 10.71 
-       2008-02-07 10:30 empty
-       2008-02-07 10:40 10.93
-       2008-02-07 10:50 11.10 
-       2008-02-07 11:00 11.23 
-
-   That is, the result of :func:`regularize` is a time series with a
-   regular time step from beginning to end, with no missing records.
-
    *ts* must have the ``time_step`` attribute set (see HTimeseries_).
 
-   A **regular timestamp** is one that falls exactly on the round time
-   step; e.g. for a ten-minute step, regular timestamps are 10:10,
-   10:20, etc., whereas irregular timestamps are 10:11, 10:25, etc. For
-   hourly time step, regular timestamps end in :00.
-
-   The returned time series begins with the regular timestamp A which is
-   nearest to the timestamp of the first record of *ts*, and ends at the
-   timestamp B which is nearest to the last record of *ts*. Between A
-   and B, the returned time series contains records for all regular
-   timestamps, although some may be null.  The value and flags for each
-   record with timestamp *t* are determined as follows:
-
-   * If a record exists in *ts* and has timestamp *t*, that record's
-     value and flags are used.
-   * Otherwise, if a single not null record exists in *ts* such that its
-     timestamp is between ``t - time_step/2`` (inclusive) and ``t +
-     time_step/2`` (non-inclusive), then the value and flags of this
-     record are used (plus *new_date_flag*, explained below).
-   * Otherwise, the value is null and no flags are set.
-
-   Whenever the algorithm results in creating a non-null record whose
-   timestamp does not have an exact match in *ts*, the flag specified
-   by *new_date_flag* is raised in the destination record, unless
-   *new_date_flag* is the empty string.
-
    If an error occurs, such as *ts* not having the ``time_step``
    attribute, :exc:`RegularizeError` (or a sublcass) is raised.
 
-   If you think the algorithm is insufficient and you intend to extend
-   it with a more clever one that does interpolation, first check commit
-   67bceaa, which had one (or the difference with the next commit).
+   *mode* can be :attr:`RegularizationMode.INSTANTANEOUS` or
+   :attr:`RegularizationMode.INTERVAL` (:class:`RegularizationMode` is
+   an :class:`Enum` class in :module:`haggregate`). This affects the
+   algorithm used. See :ref:`regularization-algorithm` below. The
+   default is :attr:`RegularizationMode.INTERVAL` for backwards
+   compatibility reasons, but letting it use the default is
+   deprecated—you should always specify it.
 
 .. function:: haggregate.aggregate(ts, target_step, method[, min_count=None][, missing_flag][, target_timestamp_offset])
 
    Process *ts* (a HTimeseries_ object) and return a new time series
    (HTimeseries_ object), with the aggregated series.  "target_step" and
    "target_timestamp_offset" are pandas "frequency" strings (see
    :ref:`usage` for more).  *method* is "sum", "mean", "max" or "min".
@@ -80,8 +35,125 @@
    destination record is null; otherwise, the destination record is
    derived even though some records are missing.  In that case, the flag
    specified by *missing_flag* is raised in the destination record.
 
    If an error occurs, such as *ts* not having a strictly regular step,
    :exc:`AggregateError` (or a subclass) is raised.
 
+.. _regularization-algorithm:
+
+How regularization is performed
+===============================
+
+The source time series, *ts*, must not be an irregular time series;
+it must have a time step, but this time step may have disturbances.
+For example, it may be a ten-minute time series like this::
+
+      2008-02-07 10:10 10.54
+      2008-02-07 10:20 10.71
+      2008-02-07 10:41 10.93
+      2008-02-07 10:50 11.10
+      2008-02-07 11:00 11.23
+
+The above has a missing record (10:30) and a disturbance in the time
+stamp of another record (10:41). :func:`regularize` would convert it
+to this::
+
+      2008-02-07 10:10 10.54
+      2008-02-07 10:20 10.71
+      2008-02-07 10:30 empty
+      2008-02-07 10:40 10.93
+      2008-02-07 10:50 11.10
+      2008-02-07 11:00 11.23
+
+That is, the result of :func:`regularize` is a time series with a
+regular time step from beginning to end, with no missing records.
+
+Specifically, he returned time series begins with the regular timestamp
+A which is nearest to the timestamp of the first record of *ts*, and
+ends at the timestamp B which is nearest to the last record of *ts*.
+Between A and B, the returned time series contains records for all
+regular timestamps, although some may be null.
+
+The regularization does not perform any interpolation or otherwise
+modify the time series values; it only modifies the time stamps,
+leaving the values as is.  If you think the algorithm is insufficient
+and you intend to extend it with a more clever one that does
+interpolation, first check commit 67bceaa, which had one (or the
+difference with the next commit).
+
+A **regular timestamp** is one that falls exactly on the round time
+step; e.g. for a ten-minute step, regular timestamps are 10:10,
+10:20, etc., whereas irregular timestamps are 10:11, 10:25, etc. For
+hourly time step, regular timestamps end in :00.
+
+Instantaneous mode
+------------------
+
+When :samp:`{mode}=RegularizationMode.INSTANTANEOUS`, the value and
+flags for each resulting record with (regular) timestamp *t* are
+determined as follows:
+
+1. If a nonempty record exists in *ts* and has timestamp *t*, that
+   record's value and flags are used.
+2. Otherwise, if a not null record exists in *ts* such that its
+   timestamp is between ``t - time_step/2`` (inclusive) and ``t +
+   time_step/2`` (non-inclusive), then the value and flags of this
+   record (or the nearest such record, if there are more than one)
+   are used (plus *new_date_flag*, explained below).
+3. Otherwise, the value is null and no flags are set.
+
+Whenever the algorithm results in creating a non-null record whose
+timestamp does not have an exact match in *ts*, the flag specified
+by *new_date_flag* is raised in the destination record, unless
+*new_date_flag* is the empty string.
+
+Interval mode
+-------------
+
+When :samp:`{mode}=RegularizationMode.INTERVAL`, essentially the same
+rules are followed as for instantaneous, with these differences:
+
+ * Step (1) applies even if the source time series record is empty. For
+   example, consider these source records::
+
+      09:00 4.7
+      09:09 5.9
+      09:10 empty
+      09:20 3.1
+
+   In this case, the regularized time series will have an empty record at
+   09:10 rather than 5.9. (It would have 5.9 if a 09:10 record did not
+   exist at all in the source time series.)
+
+ * Step (2) applies only if there is exactly one record in the interval,
+   and it is not null. For example::
+
+      09:00 4.7
+      09:09 5.9
+      09:13 5.8
+      09:20 3.1
+
+   In this case, the resulting 09:10 record will be empty.
+
+Rationale for the different modes
+---------------------------------
+
+If the variable is cumulative, such as rainfall, the time series record
+indicates not what the value was in that time instant, but what happened
+in the preceding interval. So, in the last example, what is the meaning
+of the record ``09:13 5.8``? Does it mean that 5.8 mm of rain fell
+between 09:09 and 09:13? Or is it between 09:03 and 09:13? And if that
+is the case, why do we also have another record at 09:09? The situation
+is too fishy to allow a safe conclusion when aggregating automatically,
+and therefore we choose the conservative approach of marking 09:10 as
+null, effectively declaring that we don't know what happened at that
+time. Likewise, the existence of an empty record at 09:10 in the example
+of step (1) is an indication of something fishy happening.
+
+In instantaneous variables like temperature, the value of a record
+doesn't always refer to the indicated instant, but depends on how the
+measurement was made—sometimes it's the mean value of several samples
+taken in the preceding interval. One way or the other, there doesn't
+seem to be a reason to be too picky, so the rules are relaxed.
+
 .. _HTimeseries: https://github.com/openmeteo/htimeseries
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `haggregate-3.0.3/docs/conf.py` & `haggregate-3.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `haggregate-3.0.3/docs/copyright.rst` & `haggregate-3.1.0/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.3/docs/usage.rst` & `haggregate-3.1.0/docs/usage.rst`

 * *Files 18% similar despite different names*

```diff
@@ -156,75 +156,18 @@
    "max" and "min".
 
 .. _file format: https://github.com/openmeteo/htimeseries/#file-format
 
 How the aggregation is performed
 ================================
 
-The aggregation is performed in two steps:
-
-1. Regularization
------------------
-
-The source time series must not be entirely irregular; it must have a
-time step, but this time step may have disturbances.  For example, it
-may be a ten-minute time series like this::
-
-   2008-02-07 10:10 10.54 
-   2008-02-07 10:20 10.71 
-   2008-02-07 10:41 10.93 
-   2008-02-07 10:50 11.10 
-   2008-02-07 11:00 11.23 
-
-The above has a missing record (10:30) and a disturbance in the time
-stamp of another record (10:41). The first step of the process,
-regularization, would convert it to this::
-
-   2008-02-07 10:10 10.54 
-   2008-02-07 10:20 10.71 
-   2008-02-07 10:30 empty
-   2008-02-07 10:40 10.93
-   2008-02-07 10:50 11.10 
-   2008-02-07 11:00 11.23 
-
-That is, the result of regularization is a time series with a regular
-time step from beginning to end, with no missing records.
-
-A **regular timestamp** is one that falls exactly on the round time
-step; e.g. for a ten-minute step, regular timestamps are 10:10,
-10:20, etc., whereas irregular timestamps are 10:11, 10:25, etc. For
-hourly time step, regular timestamps end in :00.
-
-The regularization does not perform any interpolation or otherwise
-modify the time series values; it only modifies the time stamps, leaving
-the values as is.
-
-Specifically, the resulting regularized time series begins with the
-regular timestamp A which is nearest to the timestamp of the first
-record of the source time series, and ends at the timestamp B which is
-nearest to the last record of the source time series. Between A and B,
-the resulting time series contains records for all regular timestamps,
-although some may be empty.  The value and flags for each resulting
-record with (regular) timestamp *t* are determined as follows:
-
-* If a record exists in the source time series and has timestamp *t*,
-  that record's value and flags are used.
-* Otherwise, if a single nonempty record exists in the source time
-  series such that its timestamp is between ``t - time_step/2``
-  (inclusive) and ``t + time_step/2`` (non-inclusive), then the value
-  and flags of this record are used (plus ``DATEINSERT``, explained
-  below).
-* Otherwise, the value is empty and no flags are set.
-
-Whenever the algorithm results in creating a nonempty record whose
-timestamp does not have an exact match in the source time series, the
-``DATEINSERT`` flag is set in the destination record.
-
-2. Aggregation
---------------
+The aggregation is performed in two steps: Regularization and
+aggregation. For the regularization, see
+:ref:`regularization-algorithm`. The mode used is "instantaneous" for
+mean, and "interval" for sum, max and min.
 
 After regularization is complete, aggregation is trivial. The timestamp
 in an aggregated record is the end of the interval.
 
 For example, if you aggregate a ten-minute time series to hourly, the
 record with timestamp ``11:00`` is the average or sum or max or min of
 time stamps ``10:10``, ``10:20``, ..., ``10:50``, ``11:00``.
```

### Comparing `haggregate-3.0.3/haggregate/cli.py` & `haggregate-3.1.0/haggregate/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 import traceback
 
 import click
 from htimeseries import HTimeseries
 
-from haggregate import aggregate
+from haggregate import RegularizationMode, aggregate
 from haggregate.regularize import regularize
 
 
 @click.command()
 @click.argument("configfile")
 def main(configfile):
     """Create lower-step timeseries from higher-step ones"""
@@ -58,15 +58,19 @@
             source_filename = os.path.join(base_dir, section.get("source_file"))
             target_filename = os.path.join(base_dir, section.get("target_file"))
             method = section.get("method")
             with open(source_filename, newline="\n") as f:
                 ts = HTimeseries(
                     f, format=HTimeseries.FILE, default_tzinfo=dt.timezone.utc
                 )
-            regts = regularize(ts, new_date_flag="DATEINSERT")
+            if method == "mean":
+                regularization_mode = RegularizationMode.INSTANTANEOUS
+            else:
+                regularization_mode = RegularizationMode.INTERVAL
+            regts = regularize(ts, new_date_flag="DATEINSERT", mode=regularization_mode)
             aggts = aggregate(
                 regts,
                 target_step,
                 method,
                 min_count=min_count,
                 missing_flag=missing_flag,
                 target_timestamp_offset=target_timestamp_offset,
```

### Comparing `haggregate-3.0.3/haggregate/haggregate.py` & `haggregate-3.1.0/haggregate/haggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from enum import Enum
 
 import numpy as np
 import pandas as pd
 from htimeseries import HTimeseries
 
 methods = {
     "sum": pd.Series.sum,
@@ -142,7 +143,12 @@
     if not m:
         raise AggregateError(
             "The target timestamp offset can currently only be a number of minutes "
             "such as 1min"
         )
     sign = m.group(1) == "-" and -1 or 1
     return sign * int(m.group(2))
+
+
+class RegularizationMode(Enum):
+    INSTANTANEOUS = 1
+    INTERVAL = 2
```

### Comparing `haggregate-3.0.3/haggregate/regularize.c` & `haggregate-3.1.0/haggregate/regularize.c`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "CYTHON_TRACE",
                 "1"
             ]
         ],
         "depends": [
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/usr/lib/python3/dist-packages/numpy/core/include/numpy/arrayobject.h",
+            "/usr/lib/python3/dist-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/usr/lib/python3/dist-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/usr/lib/python3/dist-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/usr/lib/python3/dist-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/home/anthony/nosync/virtualenvs/rocc/lib/python3.9/site-packages/numpy/core/include"
+            "/usr/lib/python3/dist-packages/numpy/core/include"
         ],
         "name": "haggregate.regularize",
         "sources": [
             "haggregate/regularize.pyx"
         ]
     },
     "module_name": "haggregate.regularize"
@@ -775,14 +775,15 @@
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
+#include <math.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -1011,195 +1012,195 @@
 
 static const char *__pyx_f[] = {
   "haggregate/regularize.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1226,42 +1227,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1848,14 +1849,25 @@
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
                                                int is_list, int wraparound, int boundscheck);
 
+/* py_abs.proto */
+#if CYTHON_USE_PYLONG_INTERNALS
+static PyObject *__Pyx_PyLong_AbsNeg(PyObject *num);
+#define __Pyx_PyNumber_Absolute(x)\
+    ((likely(PyLong_CheckExact(x))) ?\
+         (likely(Py_SIZE(x) >= 0) ? (Py_INCREF(x), (x)) : __Pyx_PyLong_AbsNeg(x)) :\
+         PyNumber_Absolute(x))
+#else
+#define __Pyx_PyNumber_Absolute(x)  PyNumber_Absolute(x)
+#endif
+
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
@@ -2078,47 +2090,52 @@
 static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
 static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
+/* Module declarations from 'libc.math' */
+
 /* Module declarations from 'haggregate.regularize' */
 #define __Pyx_MODULE_NAME "haggregate.regularize"
 extern int __pyx_module_is_main_haggregate__regularize;
 int __pyx_module_is_main_haggregate__regularize = 0;
 
 /* Implementation of 'haggregate.regularize' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_max;
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ImportError;
 static const char __pyx_k_U[] = "U";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_t[] = "t";
-static const char __pyx_k__3[] = "";
-static const char __pyx_k__6[] = " ";
+static const char __pyx_k_RM[] = "RM";
+static const char __pyx_k__4[] = "";
+static const char __pyx_k__7[] = " ";
 static const char __pyx_k_dt[] = "dt";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_pd[] = "pd";
+static const char __pyx_k_ti[] = "ti";
 static const char __pyx_k_ts[] = "ts";
 static const char __pyx_k_tz[] = "tz";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_end[] = "end";
 static const char __pyx_k_len[] = "len";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_nan[] = "nan";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_utc[] = "utc";
 static const char __pyx_k_attr[] = "attr";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_freq[] = "freq";
 static const char __pyx_k_full[] = "full";
 static const char __pyx_k_main[] = "__main__";
+static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_unit[] = "unit";
 static const char __pyx_k_attrs[] = "attrs";
 static const char __pyx_k_count[] = "count";
@@ -2139,53 +2156,63 @@
 static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_vstack[] = "vstack";
 static const char __pyx_k_columns[] = "columns";
 static const char __pyx_k_comment[] = "comment";
 static const char __pyx_k_prepare[] = "__prepare__";
+static const char __pyx_k_INTERVAL[] = "INTERVAL";
 static const char __pyx_k_datetime[] = "datetime";
 static const char __pyx_k_location[] = "location";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_timezone[] = "timezone";
 static const char __pyx_k_ts_flags[] = "ts_flags";
 static const char __pyx_k_ts_index[] = "ts_index";
 static const char __pyx_k_variable[] = "variable";
 static const char __pyx_k_DataFrame[] = "DataFrame";
 static const char __pyx_k_Timedelta[] = "Timedelta";
+static const char __pyx_k_current_i[] = "current_i";
 static const char __pyx_k_metaclass[] = "__metaclass__";
+static const char __pyx_k_nearest_i[] = "nearest_i";
 static const char __pyx_k_precision[] = "precision";
 static const char __pyx_k_time_step[] = "time_step";
 static const char __pyx_k_to_offset[] = "to_offset";
 static const char __pyx_k_transpose[] = "transpose";
 static const char __pyx_k_ts_values[] = "ts_values";
 static const char __pyx_k_DATEINSERT[] = "DATEINSERT";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_date_range[] = "date_range";
 static const char __pyx_k_get_record[] = "_get_record";
+static const char __pyx_k_haggregate[] = "haggregate";
 static const char __pyx_k_regularize[] = "regularize";
 static const char __pyx_k_tz_convert[] = "tz_convert";
 static const char __pyx_k_HTimeseries[] = "HTimeseries";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_Regularized[] = "Regularized ";
 static const char __pyx_k_flags_dtype[] = "flags_dtype";
+static const char __pyx_k_get_nearest[] = "_get_nearest";
 static const char __pyx_k_htimeseries[] = "htimeseries";
 static const char __pyx_k_result_step[] = "result_step";
 static const char __pyx_k_timedelta64[] = "timedelta64";
 static const char __pyx_k_tz_localize[] = "tz_localize";
 static const char __pyx_k_previous_pos[] = "previous_pos";
 static const char __pyx_k_result_flags[] = "result_flags";
 static const char __pyx_k_result_index[] = "result_index";
 static const char __pyx_k_to_timedelta[] = "to_timedelta";
+static const char __pyx_k_INSTANTANEOUS[] = "INSTANTANEOUS";
 static const char __pyx_k_interval_type[] = "interval_type";
 static const char __pyx_k_new_date_flag[] = "new_date_flag";
 static const char __pyx_k_result_values[] = "result_values";
 static const char __pyx_k_RegularizeError[] = "RegularizeError";
+static const char __pyx_k_current_distance[] = "current_distance";
 static const char __pyx_k_max_flags_length[] = "max_flags_length";
+static const char __pyx_k_previous_distance[] = "previous_distance";
+static const char __pyx_k_RegularizationMode[] = "RegularizationMode";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_previous_nearest_i[] = "previous_nearest_i";
 static const char __pyx_k_haggregate_regularize[] = "haggregate.regularize";
 static const char __pyx_k_perform_regularization[] = "_perform_regularization";
 static const char __pyx_k_last_timestamp_of_result[] = "last_timestamp_of_result";
 static const char __pyx_k_first_timestamp_of_result[] = "first_timestamp_of_result";
 static const char __pyx_k_haggregate_regularize_pyx[] = "haggregate/regularize.pyx";
 static const char __pyx_k_pandas_tseries_frequencies[] = "pandas.tseries.frequencies";
 static const char __pyx_k_Created_by_regularizing_step_of[] = "Created by regularizing step of timeseries that had this comment:\n\n";
@@ -2193,76 +2220,88 @@
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_The_time_step_is_malformed_or_is[] = "The time step is malformed or is specified in months. Only time steps specified in minutes, hours or days are supported.";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static PyObject *__pyx_kp_u_Created_by_regularizing_step_of;
 static PyObject *__pyx_n_u_DATEINSERT;
 static PyObject *__pyx_n_s_DataFrame;
 static PyObject *__pyx_n_s_HTimeseries;
+static PyObject *__pyx_n_s_INSTANTANEOUS;
+static PyObject *__pyx_n_s_INTERVAL;
 static PyObject *__pyx_n_s_ImportError;
+static PyObject *__pyx_n_s_RM;
+static PyObject *__pyx_n_s_RegularizationMode;
 static PyObject *__pyx_n_s_RegularizeError;
 static PyObject *__pyx_kp_u_Regularized;
 static PyObject *__pyx_kp_u_The_source_time_series_does_not;
 static PyObject *__pyx_kp_u_The_time_step_is_malformed_or_is;
 static PyObject *__pyx_n_s_Timedelta;
 static PyObject *__pyx_n_u_U;
 static PyObject *__pyx_n_s_ValueError;
-static PyObject *__pyx_kp_u__3;
-static PyObject *__pyx_kp_u__6;
+static PyObject *__pyx_kp_u__4;
+static PyObject *__pyx_kp_u__7;
 static PyObject *__pyx_n_s_astype;
 static PyObject *__pyx_n_s_attr;
 static PyObject *__pyx_n_s_attrs;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_comment;
 static PyObject *__pyx_n_u_comment;
 static PyObject *__pyx_n_s_count;
+static PyObject *__pyx_n_s_current_distance;
+static PyObject *__pyx_n_s_current_i;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_date_range;
 static PyObject *__pyx_n_s_datetime;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_dt;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_first_timestamp_of_result;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_u_flags;
 static PyObject *__pyx_n_s_flags_dtype;
 static PyObject *__pyx_n_s_found;
 static PyObject *__pyx_n_s_freq;
 static PyObject *__pyx_n_s_full;
+static PyObject *__pyx_n_s_get_nearest;
 static PyObject *__pyx_n_s_get_record;
+static PyObject *__pyx_n_s_haggregate;
 static PyObject *__pyx_n_s_haggregate_regularize;
 static PyObject *__pyx_kp_s_haggregate_regularize_pyx;
 static PyObject *__pyx_n_s_htimeseries;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_u_interval_type;
 static PyObject *__pyx_n_s_last_timestamp_of_result;
 static PyObject *__pyx_n_s_len;
 static PyObject *__pyx_n_u_location;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_max;
 static PyObject *__pyx_n_s_max_flags_length;
 static PyObject *__pyx_n_s_metaclass;
+static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_nan;
+static PyObject *__pyx_n_s_nearest_i;
 static PyObject *__pyx_n_s_new_date_flag;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_object;
 static PyObject *__pyx_n_s_pandas;
 static PyObject *__pyx_n_s_pandas_tseries_frequencies;
 static PyObject *__pyx_n_s_pd;
 static PyObject *__pyx_n_s_perform_regularization;
 static PyObject *__pyx_n_u_precision;
 static PyObject *__pyx_n_s_prepare;
+static PyObject *__pyx_n_s_previous_distance;
+static PyObject *__pyx_n_s_previous_nearest_i;
 static PyObject *__pyx_n_s_previous_pos;
 static PyObject *__pyx_n_s_qualname;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_regularize;
 static PyObject *__pyx_n_s_result;
 static PyObject *__pyx_n_s_result_flags;
 static PyObject *__pyx_n_s_result_index;
@@ -2271,14 +2310,15 @@
 static PyObject *__pyx_n_s_round;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_str;
 static PyObject *__pyx_n_s_t;
 static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_ti;
 static PyObject *__pyx_n_s_time_step;
 static PyObject *__pyx_n_u_time_step;
 static PyObject *__pyx_n_s_timedelta64;
 static PyObject *__pyx_n_s_timezone;
 static PyObject *__pyx_n_u_timezone;
 static PyObject *__pyx_n_s_title;
 static PyObject *__pyx_n_u_title;
@@ -2295,58 +2335,66 @@
 static PyObject *__pyx_n_u_unit;
 static PyObject *__pyx_n_s_utc;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_u_value;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_u_variable;
 static PyObject *__pyx_n_s_vstack;
-static PyObject *__pyx_pf_10haggregate_10regularize_regularize(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_ts, PyObject *__pyx_v_new_date_flag); /* proto */
-static PyObject *__pyx_pf_10haggregate_10regularize_2_perform_regularization(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_result_index, PyArrayObject *__pyx_v_result_values, PyArrayObject *__pyx_v_result_flags, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag); /* proto */
-static PyObject *__pyx_pf_10haggregate_10regularize_4_get_record(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_t, long __pyx_v_result_step, CYTHON_UNUSED PyObject *__pyx_v_new_date_flag, int __pyx_v_previous_pos); /* proto */
+static PyObject *__pyx_pf_10haggregate_10regularize_regularize(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_ts, PyObject *__pyx_v_new_date_flag, PyObject *__pyx_v_mode); /* proto */
+static PyObject *__pyx_pf_10haggregate_10regularize_2_perform_regularization(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_result_index, PyArrayObject *__pyx_v_result_values, PyArrayObject *__pyx_v_result_flags, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag, int __pyx_v_mode); /* proto */
+static PyObject *__pyx_pf_10haggregate_10regularize_4_get_record(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_t, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag, int __pyx_v_previous_pos, int __pyx_v_mode); /* proto */
+static PyObject *__pyx_pf_10haggregate_10regularize_6_get_nearest(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_previous_nearest_i, int __pyx_v_current_i, PyArrayObject *__pyx_v_ts_index, CYTHON_UNUSED PyArrayObject *__pyx_v_ts_values, long __pyx_v_t, int __pyx_v_mode); /* proto */
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_1000;
-static PyObject *__pyx_codeobj_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
+static PyObject *__pyx_k_;
+static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_tuple__12;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_codeobj__2;
 static PyObject *__pyx_codeobj__5;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
 /* Late includes */
 
-/* "haggregate/regularize.pyx":16
+/* "haggregate/regularize.pyx":19
  * 
  * 
- * def regularize(ts, new_date_flag="DATEINSERT"):             # <<<<<<<<<<<<<<
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):             # <<<<<<<<<<<<<<
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10haggregate_10regularize_1regularize(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_10haggregate_10regularize_1regularize = {"regularize", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10haggregate_10regularize_1regularize, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_10haggregate_10regularize_1regularize(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_ts = 0;
   PyObject *__pyx_v_new_date_flag = 0;
+  PyObject *__pyx_v_mode = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("regularize (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts,&__pyx_n_s_new_date_flag,0};
-    PyObject* values[2] = {0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts,&__pyx_n_s_new_date_flag,&__pyx_n_s_mode,0};
+    PyObject* values[3] = {0,0,0};
     values[1] = ((PyObject *)__pyx_n_u_DATEINSERT);
+    values[2] = __pyx_k_;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -2357,46 +2405,55 @@
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_new_date_flag);
           if (value) { values[1] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
+          if (value) { values[2] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "regularize") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "regularize") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_ts = values[0];
     __pyx_v_new_date_flag = values[1];
+    __pyx_v_mode = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("regularize", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 16, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("regularize", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("haggregate.regularize.regularize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10haggregate_10regularize_regularize(__pyx_self, __pyx_v_ts, __pyx_v_new_date_flag);
+  __pyx_r = __pyx_pf_10haggregate_10regularize_regularize(__pyx_self, __pyx_v_ts, __pyx_v_new_date_flag, __pyx_v_mode);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10haggregate_10regularize_regularize(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_ts, PyObject *__pyx_v_new_date_flag) {
+static PyObject *__pyx_pf_10haggregate_10regularize_regularize(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_ts, PyObject *__pyx_v_new_date_flag, PyObject *__pyx_v_mode) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_v_attrs = NULL;
   PyObject *__pyx_v_attr = NULL;
   PyObject *__pyx_v_step = NULL;
   PyObject *__pyx_v_first_timestamp_of_result = NULL;
   PyObject *__pyx_v_last_timestamp_of_result = NULL;
   PyObject *__pyx_v_max_flags_length = NULL;
@@ -2427,116 +2484,116 @@
   int __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj_)
+  __Pyx_TraceFrameInit(__pyx_codeobj__2)
   __Pyx_RefNannySetupContext("regularize", 0);
-  __Pyx_TraceCall("regularize", __pyx_f[0], 16, 0, __PYX_ERR(0, 16, __pyx_L1_error));
+  __Pyx_TraceCall("regularize", __pyx_f[0], 19, 0, __PYX_ERR(0, 19, __pyx_L1_error));
 
-  /* "haggregate/regularize.pyx":18
- * def regularize(ts, new_date_flag="DATEINSERT"):
+  /* "haggregate/regularize.pyx":21
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):             # <<<<<<<<<<<<<<
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:
  */
-  __Pyx_TraceLine(18,0,__PYX_ERR(0, 18, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_time_step); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_TraceLine(21,0,__PYX_ERR(0, 21, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_time_step); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "haggregate/regularize.pyx":19
+    /* "haggregate/regularize.pyx":22
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):
  *         raise RegularizeError("The source time series does not specify a time step")             # <<<<<<<<<<<<<<
  *     try:
  *         pd.to_timedelta(to_offset(ts.time_step))
  */
-    __Pyx_TraceLine(19,0,__PYX_ERR(0, 19, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RegularizeError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_TraceLine(22,0,__PYX_ERR(0, 22, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RegularizeError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_The_source_time_series_does_not) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_The_source_time_series_does_not);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 19, __pyx_L1_error)
+    __PYX_ERR(0, 22, __pyx_L1_error)
 
-    /* "haggregate/regularize.pyx":18
- * def regularize(ts, new_date_flag="DATEINSERT"):
+    /* "haggregate/regularize.pyx":21
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):             # <<<<<<<<<<<<<<
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:
  */
   }
 
-  /* "haggregate/regularize.pyx":20
+  /* "haggregate/regularize.pyx":23
  *     if not hasattr(ts, "time_step"):
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:             # <<<<<<<<<<<<<<
  *         pd.to_timedelta(to_offset(ts.time_step))
  *     except ValueError:
  */
-  __Pyx_TraceLine(20,0,__PYX_ERR(0, 20, __pyx_L1_error))
+  __Pyx_TraceLine(23,0,__PYX_ERR(0, 23, __pyx_L1_error))
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_8);
     /*try:*/ {
 
-      /* "haggregate/regularize.pyx":21
+      /* "haggregate/regularize.pyx":24
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:
  *         pd.to_timedelta(to_offset(ts.time_step))             # <<<<<<<<<<<<<<
  *     except ValueError:
  *         raise RegularizeError(
  */
-      __Pyx_TraceLine(21,0,__PYX_ERR(0, 21, __pyx_L4_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L4_error)
+      __Pyx_TraceLine(24,0,__PYX_ERR(0, 24, __pyx_L4_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pd); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_to_timedelta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L4_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_to_timedelta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_to_offset); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 21, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_to_offset); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 21, __pyx_L4_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_4 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L4_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -2544,20 +2601,20 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L4_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "haggregate/regularize.pyx":20
+      /* "haggregate/regularize.pyx":23
  *     if not hasattr(ts, "time_step"):
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:             # <<<<<<<<<<<<<<
  *         pd.to_timedelta(to_offset(ts.time_step))
  *     except ValueError:
  */
     }
@@ -2569,882 +2626,889 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "haggregate/regularize.pyx":22
+    /* "haggregate/regularize.pyx":25
  *     try:
  *         pd.to_timedelta(to_offset(ts.time_step))
  *     except ValueError:             # <<<<<<<<<<<<<<
  *         raise RegularizeError(
  *             "The time step is malformed or is specified in months. Only time steps "
  */
-    __Pyx_TraceLine(22,0,__PYX_ERR(0, 22, __pyx_L6_except_error))
+    __Pyx_TraceLine(25,0,__PYX_ERR(0, 25, __pyx_L6_except_error))
     __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
     if (__pyx_t_12) {
       __Pyx_AddTraceback("haggregate.regularize.regularize", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_5, &__pyx_t_4) < 0) __PYX_ERR(0, 22, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_5, &__pyx_t_4) < 0) __PYX_ERR(0, 25, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "haggregate/regularize.pyx":23
+      /* "haggregate/regularize.pyx":26
  *         pd.to_timedelta(to_offset(ts.time_step))
  *     except ValueError:
  *         raise RegularizeError(             # <<<<<<<<<<<<<<
  *             "The time step is malformed or is specified in months. Only time steps "
  *             "specified in minutes, hours or days are supported."
  */
-      __Pyx_TraceLine(23,0,__PYX_ERR(0, 23, __pyx_L6_except_error))
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_RegularizeError); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 23, __pyx_L6_except_error)
+      __Pyx_TraceLine(26,0,__PYX_ERR(0, 26, __pyx_L6_except_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_RegularizeError); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 26, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_10, function);
         }
       }
       __pyx_t_9 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_11, __pyx_kp_u_The_time_step_is_malformed_or_is) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_kp_u_The_time_step_is_malformed_or_is);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 23, __pyx_L6_except_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 26, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_Raise(__pyx_t_9, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __PYX_ERR(0, 23, __pyx_L6_except_error)
+      __PYX_ERR(0, 26, __pyx_L6_except_error)
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "haggregate/regularize.pyx":20
+    /* "haggregate/regularize.pyx":23
  *     if not hasattr(ts, "time_step"):
  *         raise RegularizeError("The source time series does not specify a time step")
  *     try:             # <<<<<<<<<<<<<<
  *         pd.to_timedelta(to_offset(ts.time_step))
  *     except ValueError:
  */
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_XGIVEREF(__pyx_t_8);
     __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "haggregate/regularize.pyx":29
+  /* "haggregate/regularize.pyx":32
  * 
  *     # Set metadata of result
  *     result = HTimeseries()             # <<<<<<<<<<<<<<
  *     attrs = (
  *         "unit",
  */
-  __Pyx_TraceLine(29,0,__PYX_ERR(0, 29, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HTimeseries); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_TraceLine(32,0,__PYX_ERR(0, 32, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HTimeseries); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":31
+  /* "haggregate/regularize.pyx":34
  *     result = HTimeseries()
  *     attrs = (
  *         "unit",             # <<<<<<<<<<<<<<
  *         "timezone",
  *         "time_step",
  */
-  __Pyx_TraceLine(31,0,__PYX_ERR(0, 31, __pyx_L1_error))
-  __Pyx_INCREF(__pyx_tuple__2);
-  __pyx_v_attrs = __pyx_tuple__2;
+  __Pyx_TraceLine(34,0,__PYX_ERR(0, 34, __pyx_L1_error))
+  __Pyx_INCREF(__pyx_tuple__3);
+  __pyx_v_attrs = __pyx_tuple__3;
 
-  /* "haggregate/regularize.pyx":39
+  /* "haggregate/regularize.pyx":42
  *         "location",
  *     )
  *     for attr in attrs:             # <<<<<<<<<<<<<<
  *         setattr(result, attr, getattr(ts, attr, None))
  *     if hasattr(ts, "title"):
  */
-  __Pyx_TraceLine(39,0,__PYX_ERR(0, 39, __pyx_L1_error))
+  __Pyx_TraceLine(42,0,__PYX_ERR(0, 42, __pyx_L1_error))
   __pyx_t_4 = __pyx_v_attrs; __Pyx_INCREF(__pyx_t_4); __pyx_t_13 = 0;
   for (;;) {
     if (__pyx_t_13 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_13); __Pyx_INCREF(__pyx_t_5); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_13); __Pyx_INCREF(__pyx_t_5); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 42, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_attr, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "haggregate/regularize.pyx":40
+    /* "haggregate/regularize.pyx":43
  *     )
  *     for attr in attrs:
  *         setattr(result, attr, getattr(ts, attr, None))             # <<<<<<<<<<<<<<
  *     if hasattr(ts, "title"):
  *         result.title = "Regularized " + ts.title
  */
-    __Pyx_TraceLine(40,0,__PYX_ERR(0, 40, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_GetAttr3(__pyx_v_ts, __pyx_v_attr, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_TraceLine(43,0,__PYX_ERR(0, 43, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_GetAttr3(__pyx_v_ts, __pyx_v_attr, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_14 = PyObject_SetAttr(__pyx_v_result, __pyx_v_attr, __pyx_t_5); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_14 = PyObject_SetAttr(__pyx_v_result, __pyx_v_attr, __pyx_t_5); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "haggregate/regularize.pyx":39
+    /* "haggregate/regularize.pyx":42
  *         "location",
  *     )
  *     for attr in attrs:             # <<<<<<<<<<<<<<
  *         setattr(result, attr, getattr(ts, attr, None))
  *     if hasattr(ts, "title"):
  */
-    __Pyx_TraceLine(39,0,__PYX_ERR(0, 39, __pyx_L1_error))
+    __Pyx_TraceLine(42,0,__PYX_ERR(0, 42, __pyx_L1_error))
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":41
+  /* "haggregate/regularize.pyx":44
  *     for attr in attrs:
  *         setattr(result, attr, getattr(ts, attr, None))
  *     if hasattr(ts, "title"):             # <<<<<<<<<<<<<<
  *         result.title = "Regularized " + ts.title
  *     if hasattr(ts, "comment"):
  */
-  __Pyx_TraceLine(41,0,__PYX_ERR(0, 41, __pyx_L1_error))
-  __pyx_t_2 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_title); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_TraceLine(44,0,__PYX_ERR(0, 44, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_title); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "haggregate/regularize.pyx":42
+    /* "haggregate/regularize.pyx":45
  *         setattr(result, attr, getattr(ts, attr, None))
  *     if hasattr(ts, "title"):
  *         result.title = "Regularized " + ts.title             # <<<<<<<<<<<<<<
  *     if hasattr(ts, "comment"):
  *         result.comment = (
  */
-    __Pyx_TraceLine(42,0,__PYX_ERR(0, 42, __pyx_L1_error))
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_title); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_TraceLine(45,0,__PYX_ERR(0, 45, __pyx_L1_error))
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_title); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyNumber_Add(__pyx_kp_u_Regularized, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_kp_u_Regularized, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_title, __pyx_t_5) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_title, __pyx_t_5) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "haggregate/regularize.pyx":41
+    /* "haggregate/regularize.pyx":44
  *     for attr in attrs:
  *         setattr(result, attr, getattr(ts, attr, None))
  *     if hasattr(ts, "title"):             # <<<<<<<<<<<<<<
  *         result.title = "Regularized " + ts.title
  *     if hasattr(ts, "comment"):
  */
   }
 
-  /* "haggregate/regularize.pyx":43
+  /* "haggregate/regularize.pyx":46
  *     if hasattr(ts, "title"):
  *         result.title = "Regularized " + ts.title
  *     if hasattr(ts, "comment"):             # <<<<<<<<<<<<<<
  *         result.comment = (
  *             "Created by regularizing step of timeseries that had this comment:\n\n"
  */
-  __Pyx_TraceLine(43,0,__PYX_ERR(0, 43, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_comment); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_TraceLine(46,0,__PYX_ERR(0, 46, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_HasAttr(__pyx_v_ts, __pyx_n_u_comment); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "haggregate/regularize.pyx":46
+    /* "haggregate/regularize.pyx":49
  *         result.comment = (
  *             "Created by regularizing step of timeseries that had this comment:\n\n"
  *             + ts.comment             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __Pyx_TraceLine(46,0,__PYX_ERR(0, 46, __pyx_L1_error))
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_comment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __Pyx_TraceLine(49,0,__PYX_ERR(0, 49, __pyx_L1_error))
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_comment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_Created_by_regularizing_step_of, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_kp_u_Created_by_regularizing_step_of, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "haggregate/regularize.pyx":44
+    /* "haggregate/regularize.pyx":47
  *         result.title = "Regularized " + ts.title
  *     if hasattr(ts, "comment"):
  *         result.comment = (             # <<<<<<<<<<<<<<
  *             "Created by regularizing step of timeseries that had this comment:\n\n"
  *             + ts.comment
  */
-    __Pyx_TraceLine(44,0,__PYX_ERR(0, 44, __pyx_L1_error))
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_comment, __pyx_t_4) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+    __Pyx_TraceLine(47,0,__PYX_ERR(0, 47, __pyx_L1_error))
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_comment, __pyx_t_4) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "haggregate/regularize.pyx":43
+    /* "haggregate/regularize.pyx":46
  *     if hasattr(ts, "title"):
  *         result.title = "Regularized " + ts.title
  *     if hasattr(ts, "comment"):             # <<<<<<<<<<<<<<
  *         result.comment = (
  *             "Created by regularizing step of timeseries that had this comment:\n\n"
  */
   }
 
-  /* "haggregate/regularize.pyx":50
+  /* "haggregate/regularize.pyx":53
  * 
  *     # Return immediately if empty
  *     if len(ts.data) == 0:             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __Pyx_TraceLine(50,0,__PYX_ERR(0, 50, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_TraceLine(53,0,__PYX_ERR(0, 53, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_13 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_13 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_2 = ((__pyx_t_13 == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "haggregate/regularize.pyx":51
+    /* "haggregate/regularize.pyx":54
  *     # Return immediately if empty
  *     if len(ts.data) == 0:
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     # Determine first and last timestamps
  */
-    __Pyx_TraceLine(51,0,__PYX_ERR(0, 51, __pyx_L1_error))
+    __Pyx_TraceLine(54,0,__PYX_ERR(0, 54, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_result);
     __pyx_r = __pyx_v_result;
     goto __pyx_L0;
 
-    /* "haggregate/regularize.pyx":50
+    /* "haggregate/regularize.pyx":53
  * 
  *     # Return immediately if empty
  *     if len(ts.data) == 0:             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
   }
 
-  /* "haggregate/regularize.pyx":54
+  /* "haggregate/regularize.pyx":57
  * 
  *     # Determine first and last timestamps
  *     step = pd.Timedelta(ts.time_step)             # <<<<<<<<<<<<<<
  *     first_timestamp_of_result = ts.data.index[0].round(step)
  *     last_timestamp_of_result = ts.data.index[-1].round(step)
  */
-  __Pyx_TraceLine(54,0,__PYX_ERR(0, 54, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_TraceLine(57,0,__PYX_ERR(0, 57, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Timedelta); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Timedelta); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_9, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_step = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":55
+  /* "haggregate/regularize.pyx":58
  *     # Determine first and last timestamps
  *     step = pd.Timedelta(ts.time_step)
  *     first_timestamp_of_result = ts.data.index[0].round(step)             # <<<<<<<<<<<<<<
  *     last_timestamp_of_result = ts.data.index[-1].round(step)
  * 
  */
-  __Pyx_TraceLine(55,0,__PYX_ERR(0, 55, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_TraceLine(58,0,__PYX_ERR(0, 58, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_round); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_round); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_v_step) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_step);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_first_timestamp_of_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":56
+  /* "haggregate/regularize.pyx":59
  *     step = pd.Timedelta(ts.time_step)
  *     first_timestamp_of_result = ts.data.index[0].round(step)
  *     last_timestamp_of_result = ts.data.index[-1].round(step)             # <<<<<<<<<<<<<<
  * 
  *     # Transform all pandas information to plain numpy, which is way faster and is also
  */
-  __Pyx_TraceLine(56,0,__PYX_ERR(0, 56, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_TraceLine(59,0,__PYX_ERR(0, 59, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_3, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_3, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_round); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_round); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_v_step) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_step);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_last_timestamp_of_result = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":60
+  /* "haggregate/regularize.pyx":63
  *     # Transform all pandas information to plain numpy, which is way faster and is also
  *     # supported by numba and Cython
  *     max_flags_length = max(ts.data["flags"].str.len()) + 1 + len(new_date_flag)             # <<<<<<<<<<<<<<
  *     flags_dtype = "U" + str(max_flags_length)
  *     ts_index = ts.data.index.values.astype(long)
  */
-  __Pyx_TraceLine(60,0,__PYX_ERR(0, 60, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_TraceLine(63,0,__PYX_ERR(0, 63, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_len); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_len); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_max, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_5, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_13 = PyObject_Length(__pyx_v_new_date_flag); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_13 = PyObject_Length(__pyx_v_new_date_flag); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_max_flags_length = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "haggregate/regularize.pyx":61
+  /* "haggregate/regularize.pyx":64
  *     # supported by numba and Cython
  *     max_flags_length = max(ts.data["flags"].str.len()) + 1 + len(new_date_flag)
  *     flags_dtype = "U" + str(max_flags_length)             # <<<<<<<<<<<<<<
  *     ts_index = ts.data.index.values.astype(long)
  *     ts_values = ts.data["value"].values
  */
-  __Pyx_TraceLine(61,0,__PYX_ERR(0, 61, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_max_flags_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __Pyx_TraceLine(64,0,__PYX_ERR(0, 64, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_max_flags_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_n_u_U, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_n_u_U, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_flags_dtype = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":62
+  /* "haggregate/regularize.pyx":65
  *     max_flags_length = max(ts.data["flags"].str.len()) + 1 + len(new_date_flag)
  *     flags_dtype = "U" + str(max_flags_length)
  *     ts_index = ts.data.index.values.astype(long)             # <<<<<<<<<<<<<<
  *     ts_values = ts.data["value"].values
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)
  */
-  __Pyx_TraceLine(62,0,__PYX_ERR(0, 62, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_TraceLine(65,0,__PYX_ERR(0, 65, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, ((PyObject *)(&PyLong_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyLong_Type)));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_ts_index = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":63
+  /* "haggregate/regularize.pyx":66
  *     flags_dtype = "U" + str(max_flags_length)
  *     ts_index = ts.data.index.values.astype(long)
  *     ts_values = ts.data["value"].values             # <<<<<<<<<<<<<<
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)
  *     result_step = np.timedelta64(step).astype(int) * 1000
  */
-  __Pyx_TraceLine(63,0,__PYX_ERR(0, 63, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __Pyx_TraceLine(66,0,__PYX_ERR(0, 66, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_ts_values = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":64
+  /* "haggregate/regularize.pyx":67
  *     ts_index = ts.data.index.values.astype(long)
  *     ts_values = ts.data["value"].values
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)             # <<<<<<<<<<<<<<
  *     result_step = np.timedelta64(step).astype(int) * 1000
  *     result_index = pd.date_range(
  */
-  __Pyx_TraceLine(64,0,__PYX_ERR(0, 64, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_TraceLine(67,0,__PYX_ERR(0, 67, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_flags_dtype) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_flags_dtype);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_ts_flags = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":65
+  /* "haggregate/regularize.pyx":68
  *     ts_values = ts.data["value"].values
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)
  *     result_step = np.timedelta64(step).astype(int) * 1000             # <<<<<<<<<<<<<<
  *     result_index = pd.date_range(
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step
  */
-  __Pyx_TraceLine(65,0,__PYX_ERR(0, 65, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_TraceLine(68,0,__PYX_ERR(0, 68, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_timedelta64); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_timedelta64); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, __pyx_v_step) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_step);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_3, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_9, ((PyObject *)(&PyInt_Type)));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = PyNumber_Multiply(__pyx_t_5, __pyx_int_1000); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_9 = PyNumber_Multiply(__pyx_t_5, __pyx_int_1000); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_result_step = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "haggregate/regularize.pyx":66
+  /* "haggregate/regularize.pyx":69
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)
  *     result_step = np.timedelta64(step).astype(int) * 1000
  *     result_index = pd.date_range(             # <<<<<<<<<<<<<<
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step
  *     ).values
  */
-  __Pyx_TraceLine(66,0,__PYX_ERR(0, 66, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_pd); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_pd); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_date_range); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_date_range); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "haggregate/regularize.pyx":67
+  /* "haggregate/regularize.pyx":70
  *     result_step = np.timedelta64(step).astype(int) * 1000
  *     result_index = pd.date_range(
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step             # <<<<<<<<<<<<<<
  *     ).values
  *     result_values = np.full(len(result_index), np.nan, dtype=object)
  */
-  __Pyx_TraceLine(67,0,__PYX_ERR(0, 67, __pyx_L1_error))
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_TraceLine(70,0,__PYX_ERR(0, 70, __pyx_L1_error))
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_v_first_timestamp_of_result);
   __Pyx_GIVEREF(__pyx_v_first_timestamp_of_result);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_first_timestamp_of_result);
   __Pyx_INCREF(__pyx_v_last_timestamp_of_result);
   __Pyx_GIVEREF(__pyx_v_last_timestamp_of_result);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_last_timestamp_of_result);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_ts, __pyx_n_s_time_step); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_freq, __pyx_t_4) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_freq, __pyx_t_4) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":66
+  /* "haggregate/regularize.pyx":69
  *     ts_flags = ts.data["flags"].values.astype(flags_dtype)
  *     result_step = np.timedelta64(step).astype(int) * 1000
  *     result_index = pd.date_range(             # <<<<<<<<<<<<<<
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step
  *     ).values
  */
-  __Pyx_TraceLine(66,0,__PYX_ERR(0, 66, __pyx_L1_error))
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "haggregate/regularize.pyx":68
+  /* "haggregate/regularize.pyx":71
  *     result_index = pd.date_range(
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step
  *     ).values             # <<<<<<<<<<<<<<
  *     result_values = np.full(len(result_index), np.nan, dtype=object)
  *     result_flags = np.full(len(result_index), "", dtype=flags_dtype)
  */
-  __Pyx_TraceLine(68,0,__PYX_ERR(0, 68, __pyx_L1_error))
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_TraceLine(71,0,__PYX_ERR(0, 71, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_result_index = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "haggregate/regularize.pyx":69
+  /* "haggregate/regularize.pyx":72
  *         first_timestamp_of_result, last_timestamp_of_result, freq=ts.time_step
  *     ).values
  *     result_values = np.full(len(result_index), np.nan, dtype=object)             # <<<<<<<<<<<<<<
  *     result_flags = np.full(len(result_index), "", dtype=flags_dtype)
  * 
  */
-  __Pyx_TraceLine(69,0,__PYX_ERR(0, 69, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_TraceLine(72,0,__PYX_ERR(0, 72, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_full); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_full); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_13 = PyObject_Length(__pyx_v_result_index); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 69, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_13 = PyObject_Length(__pyx_v_result_index); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_5);
   __pyx_t_3 = 0;
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_result_values = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "haggregate/regularize.pyx":70
+  /* "haggregate/regularize.pyx":73
  *     ).values
  *     result_values = np.full(len(result_index), np.nan, dtype=object)
  *     result_flags = np.full(len(result_index), "", dtype=flags_dtype)             # <<<<<<<<<<<<<<
  * 
  *     # Do the job
  */
-  __Pyx_TraceLine(70,0,__PYX_ERR(0, 70, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_TraceLine(73,0,__PYX_ERR(0, 73, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_full); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_full); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_13 = PyObject_Length(__pyx_v_result_index); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_13 = PyObject_Length(__pyx_v_result_index); if (unlikely(__pyx_t_13 == ((Py_ssize_t)-1))) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_3);
-  __Pyx_INCREF(__pyx_kp_u__3);
-  __Pyx_GIVEREF(__pyx_kp_u__3);
-  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_kp_u__3);
+  __Pyx_INCREF(__pyx_kp_u__4);
+  __Pyx_GIVEREF(__pyx_kp_u__4);
+  PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_kp_u__4);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_flags_dtype) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_flags_dtype) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result_flags = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":73
+  /* "haggregate/regularize.pyx":76
  * 
  *     # Do the job
  *     _perform_regularization(             # <<<<<<<<<<<<<<
  *         result_index,
  *         result_values,
  */
-  __Pyx_TraceLine(73,0,__PYX_ERR(0, 73, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_perform_regularization); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_TraceLine(76,0,__PYX_ERR(0, 76, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_perform_regularization); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "haggregate/regularize.pyx":81
- *         ts_flags,
+  /* "haggregate/regularize.pyx":85
  *         result_step,
- *         new_date_flag,             # <<<<<<<<<<<<<<
+ *         new_date_flag,
+ *         mode.value,             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  __Pyx_TraceLine(81,0,__PYX_ERR(0, 81, __pyx_L1_error))
-  __pyx_t_9 = NULL;
+  __Pyx_TraceLine(85,0,__PYX_ERR(0, 85, __pyx_L1_error))
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_value); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_5 = NULL;
   __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_9, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 8+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    PyObject *__pyx_temp[10] = {__pyx_t_5, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag, __pyx_t_9};
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 9+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[9] = {__pyx_t_9, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 8+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    PyObject *__pyx_temp[10] = {__pyx_t_5, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag, __pyx_t_9};
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 9+__pyx_t_12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(8+__pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (__pyx_t_9) {
-      __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_9); __pyx_t_9 = NULL;
+    __pyx_t_10 = PyTuple_New(9+__pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    if (__pyx_t_5) {
+      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_v_result_index);
     __Pyx_GIVEREF(__pyx_v_result_index);
-    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_12, __pyx_v_result_index);
+    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_12, __pyx_v_result_index);
     __Pyx_INCREF(__pyx_v_result_values);
     __Pyx_GIVEREF(__pyx_v_result_values);
-    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_12, __pyx_v_result_values);
+    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_12, __pyx_v_result_values);
     __Pyx_INCREF(__pyx_v_result_flags);
     __Pyx_GIVEREF(__pyx_v_result_flags);
-    PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_12, __pyx_v_result_flags);
+    PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_12, __pyx_v_result_flags);
     __Pyx_INCREF(__pyx_v_ts_index);
     __Pyx_GIVEREF(__pyx_v_ts_index);
-    PyTuple_SET_ITEM(__pyx_t_5, 3+__pyx_t_12, __pyx_v_ts_index);
+    PyTuple_SET_ITEM(__pyx_t_10, 3+__pyx_t_12, __pyx_v_ts_index);
     __Pyx_INCREF(__pyx_v_ts_values);
     __Pyx_GIVEREF(__pyx_v_ts_values);
-    PyTuple_SET_ITEM(__pyx_t_5, 4+__pyx_t_12, __pyx_v_ts_values);
+    PyTuple_SET_ITEM(__pyx_t_10, 4+__pyx_t_12, __pyx_v_ts_values);
     __Pyx_INCREF(__pyx_v_ts_flags);
     __Pyx_GIVEREF(__pyx_v_ts_flags);
-    PyTuple_SET_ITEM(__pyx_t_5, 5+__pyx_t_12, __pyx_v_ts_flags);
+    PyTuple_SET_ITEM(__pyx_t_10, 5+__pyx_t_12, __pyx_v_ts_flags);
     __Pyx_INCREF(__pyx_v_result_step);
     __Pyx_GIVEREF(__pyx_v_result_step);
-    PyTuple_SET_ITEM(__pyx_t_5, 6+__pyx_t_12, __pyx_v_result_step);
+    PyTuple_SET_ITEM(__pyx_t_10, 6+__pyx_t_12, __pyx_v_result_step);
     __Pyx_INCREF(__pyx_v_new_date_flag);
     __Pyx_GIVEREF(__pyx_v_new_date_flag);
-    PyTuple_SET_ITEM(__pyx_t_5, 7+__pyx_t_12, __pyx_v_new_date_flag);
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_10, 7+__pyx_t_12, __pyx_v_new_date_flag);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_10, 8+__pyx_t_12, __pyx_t_9);
+    __pyx_t_9 = 0;
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":84
+  /* "haggregate/regularize.pyx":88
  *     )
  * 
  *     result.data = pd.DataFrame(             # <<<<<<<<<<<<<<
  *         index=result_index,
  *         columns=["value", "flags"],
  */
-  __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_pd); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "haggregate/regularize.pyx":85
+  /* "haggregate/regularize.pyx":89
  * 
  *     result.data = pd.DataFrame(
  *         index=result_index,             # <<<<<<<<<<<<<<
  *         columns=["value", "flags"],
  *         data=np.vstack((result_values, result_flags)).transpose(),
  */
-  __Pyx_TraceLine(85,0,__PYX_ERR(0, 85, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_index, __pyx_v_result_index) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_TraceLine(89,0,__PYX_ERR(0, 89, __pyx_L1_error))
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_index, __pyx_v_result_index) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
 
-  /* "haggregate/regularize.pyx":86
+  /* "haggregate/regularize.pyx":90
  *     result.data = pd.DataFrame(
  *         index=result_index,
  *         columns=["value", "flags"],             # <<<<<<<<<<<<<<
  *         data=np.vstack((result_values, result_flags)).transpose(),
  *     ).tz_localize(dt.timezone.utc).tz_convert(first_timestamp_of_result.tz)
  */
-  __Pyx_TraceLine(86,0,__PYX_ERR(0, 86, __pyx_L1_error))
-  __pyx_t_10 = PyList_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_TraceLine(90,0,__PYX_ERR(0, 90, __pyx_L1_error))
+  __pyx_t_5 = PyList_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_u_value);
   __Pyx_GIVEREF(__pyx_n_u_value);
-  PyList_SET_ITEM(__pyx_t_10, 0, __pyx_n_u_value);
+  PyList_SET_ITEM(__pyx_t_5, 0, __pyx_n_u_value);
   __Pyx_INCREF(__pyx_n_u_flags);
   __Pyx_GIVEREF(__pyx_n_u_flags);
-  PyList_SET_ITEM(__pyx_t_10, 1, __pyx_n_u_flags);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_columns, __pyx_t_10) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  PyList_SET_ITEM(__pyx_t_5, 1, __pyx_n_u_flags);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_columns, __pyx_t_5) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":87
+  /* "haggregate/regularize.pyx":91
  *         index=result_index,
  *         columns=["value", "flags"],
  *         data=np.vstack((result_values, result_flags)).transpose(),             # <<<<<<<<<<<<<<
  *     ).tz_localize(dt.timezone.utc).tz_convert(first_timestamp_of_result.tz)
  *     return result
  */
-  __Pyx_TraceLine(87,0,__PYX_ERR(0, 87, __pyx_L1_error))
-  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_TraceLine(91,0,__PYX_ERR(0, 91, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_vstack); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_vstack); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_INCREF(__pyx_v_result_values);
   __Pyx_GIVEREF(__pyx_v_result_values);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_v_result_values);
   __Pyx_INCREF(__pyx_v_result_flags);
   __Pyx_GIVEREF(__pyx_v_result_flags);
   PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_v_result_flags);
@@ -3457,136 +3521,136 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_16, function);
     }
   }
   __pyx_t_11 = (__pyx_t_17) ? __Pyx_PyObject_Call2Args(__pyx_t_16, __pyx_t_17, __pyx_t_15) : __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_15);
   __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_transpose); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_transpose); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_16))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_16);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_16, function);
     }
   }
-  __pyx_t_10 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_16);
+  __pyx_t_5 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_16, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_data, __pyx_t_10) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_data, __pyx_t_5) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "haggregate/regularize.pyx":84
+  /* "haggregate/regularize.pyx":88
  *     )
  * 
  *     result.data = pd.DataFrame(             # <<<<<<<<<<<<<<
  *         index=result_index,
  *         columns=["value", "flags"],
  */
-  __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "haggregate/regularize.pyx":88
+  /* "haggregate/regularize.pyx":92
  *         columns=["value", "flags"],
  *         data=np.vstack((result_values, result_flags)).transpose(),
  *     ).tz_localize(dt.timezone.utc).tz_convert(first_timestamp_of_result.tz)             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-  __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_tz_localize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_dt); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_TraceLine(92,0,__PYX_ERR(0, 92, __pyx_L1_error))
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_tz_localize); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_timezone); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_dt); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_timezone); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_utc); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_utc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_9)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_10);
+  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_tz_convert); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_tz_convert); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_first_timestamp_of_result, __pyx_n_s_tz); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_first_timestamp_of_result, __pyx_n_s_tz); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_10 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_10)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_10);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_10, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "haggregate/regularize.pyx":84
+  /* "haggregate/regularize.pyx":88
  *     )
  * 
  *     result.data = pd.DataFrame(             # <<<<<<<<<<<<<<
  *         index=result_index,
  *         columns=["value", "flags"],
  */
-  __Pyx_TraceLine(84,0,__PYX_ERR(0, 84, __pyx_L1_error))
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_TraceLine(88,0,__PYX_ERR(0, 88, __pyx_L1_error))
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_result, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "haggregate/regularize.pyx":89
+  /* "haggregate/regularize.pyx":93
  *         data=np.vstack((result_values, result_flags)).transpose(),
  *     ).tz_localize(dt.timezone.utc).tz_convert(first_timestamp_of_result.tz)
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_TraceLine(89,0,__PYX_ERR(0, 89, __pyx_L1_error))
+  __Pyx_TraceLine(93,0,__PYX_ERR(0, 93, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "haggregate/regularize.pyx":16
+  /* "haggregate/regularize.pyx":19
  * 
  * 
- * def regularize(ts, new_date_flag="DATEINSERT"):             # <<<<<<<<<<<<<<
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):             # <<<<<<<<<<<<<<
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
@@ -3618,15 +3682,15 @@
   __Pyx_XDECREF(__pyx_v_result_flags);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "haggregate/regularize.pyx":92
+/* "haggregate/regularize.pyx":96
  * 
  * 
  * def _perform_regularization(             # <<<<<<<<<<<<<<
  *     np.ndarray result_index,
  *     np.ndarray result_values,
  */
 
@@ -3638,27 +3702,30 @@
   PyArrayObject *__pyx_v_result_values = 0;
   PyArrayObject *__pyx_v_result_flags = 0;
   PyArrayObject *__pyx_v_ts_index = 0;
   PyArrayObject *__pyx_v_ts_values = 0;
   PyArrayObject *__pyx_v_ts_flags = 0;
   long __pyx_v_result_step;
   PyObject *__pyx_v_new_date_flag = 0;
+  int __pyx_v_mode;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_perform_regularization (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_result_index,&__pyx_n_s_result_values,&__pyx_n_s_result_flags,&__pyx_n_s_ts_index,&__pyx_n_s_ts_values,&__pyx_n_s_ts_flags,&__pyx_n_s_result_step,&__pyx_n_s_new_date_flag,0};
-    PyObject* values[8] = {0,0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_result_index,&__pyx_n_s_result_values,&__pyx_n_s_result_flags,&__pyx_n_s_ts_index,&__pyx_n_s_ts_values,&__pyx_n_s_ts_flags,&__pyx_n_s_result_step,&__pyx_n_s_new_date_flag,&__pyx_n_s_mode,0};
+    PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
@@ -3679,104 +3746,112 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result_index)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result_values)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 1); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 1); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 2); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 2); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 3); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 3); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_values)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 4); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 4); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 5); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 5); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result_step)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 6); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 6); __PYX_ERR(0, 96, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_new_date_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, 7); __PYX_ERR(0, 92, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 7); __PYX_ERR(0, 96, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, 8); __PYX_ERR(0, 96, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_perform_regularization") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_perform_regularization") < 0)) __PYX_ERR(0, 96, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 8) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 9) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+      values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
     }
     __pyx_v_result_index = ((PyArrayObject *)values[0]);
     __pyx_v_result_values = ((PyArrayObject *)values[1]);
     __pyx_v_result_flags = ((PyArrayObject *)values[2]);
     __pyx_v_ts_index = ((PyArrayObject *)values[3]);
     __pyx_v_ts_values = ((PyArrayObject *)values[4]);
     __pyx_v_ts_flags = ((PyArrayObject *)values[5]);
-    __pyx_v_result_step = __Pyx_PyInt_As_long(values[6]); if (unlikely((__pyx_v_result_step == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+    __pyx_v_result_step = __Pyx_PyInt_As_long(values[6]); if (unlikely((__pyx_v_result_step == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L3_error)
     __pyx_v_new_date_flag = ((PyObject*)values[7]);
+    __pyx_v_mode = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_mode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 8, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_perform_regularization", 1, 9, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 96, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("haggregate.regularize._perform_regularization", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_index), __pyx_ptype_5numpy_ndarray, 1, "result_index", 0))) __PYX_ERR(0, 93, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_values), __pyx_ptype_5numpy_ndarray, 1, "result_values", 0))) __PYX_ERR(0, 94, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_flags), __pyx_ptype_5numpy_ndarray, 1, "result_flags", 0))) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_index), __pyx_ptype_5numpy_ndarray, 1, "ts_index", 0))) __PYX_ERR(0, 96, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_values), __pyx_ptype_5numpy_ndarray, 1, "ts_values", 0))) __PYX_ERR(0, 97, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_flags), __pyx_ptype_5numpy_ndarray, 1, "ts_flags", 0))) __PYX_ERR(0, 98, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_new_date_flag), (&PyUnicode_Type), 1, "new_date_flag", 1))) __PYX_ERR(0, 100, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10haggregate_10regularize_2_perform_regularization(__pyx_self, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_index), __pyx_ptype_5numpy_ndarray, 1, "result_index", 0))) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_values), __pyx_ptype_5numpy_ndarray, 1, "result_values", 0))) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_result_flags), __pyx_ptype_5numpy_ndarray, 1, "result_flags", 0))) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_index), __pyx_ptype_5numpy_ndarray, 1, "ts_index", 0))) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_values), __pyx_ptype_5numpy_ndarray, 1, "ts_values", 0))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_flags), __pyx_ptype_5numpy_ndarray, 1, "ts_flags", 0))) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_new_date_flag), (&PyUnicode_Type), 1, "new_date_flag", 1))) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10haggregate_10regularize_2_perform_regularization(__pyx_self, __pyx_v_result_index, __pyx_v_result_values, __pyx_v_result_flags, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_result_step, __pyx_v_new_date_flag, __pyx_v_mode);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10haggregate_10regularize_2_perform_regularization(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_result_index, PyArrayObject *__pyx_v_result_values, PyArrayObject *__pyx_v_result_flags, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag) {
+static PyObject *__pyx_pf_10haggregate_10regularize_2_perform_regularization(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_result_index, PyArrayObject *__pyx_v_result_values, PyArrayObject *__pyx_v_result_flags, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag, int __pyx_v_mode) {
   int __pyx_v_i;
   int __pyx_v_previous_pos;
   long __pyx_v_t;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -3785,227 +3860,262 @@
   int __pyx_t_4;
   long __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
-  int __pyx_t_11;
-  PyObject *__pyx_t_12 = NULL;
-  PyObject *(*__pyx_t_13)(PyObject *);
+  PyObject *__pyx_t_11 = NULL;
+  int __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *(*__pyx_t_14)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__4)
+  __Pyx_TraceFrameInit(__pyx_codeobj__5)
   __Pyx_RefNannySetupContext("_perform_regularization", 0);
-  __Pyx_TraceCall("_perform_regularization", __pyx_f[0], 92, 0, __PYX_ERR(0, 92, __pyx_L1_error));
+  __Pyx_TraceCall("_perform_regularization", __pyx_f[0], 96, 0, __PYX_ERR(0, 96, __pyx_L1_error));
 
-  /* "haggregate/regularize.pyx":105
+  /* "haggregate/regularize.pyx":110
  *     cdef long t
  * 
  *     previous_pos = 0             # <<<<<<<<<<<<<<
  *     for i in range(result_index.size):
  *         t = result_index[i]
  */
-  __Pyx_TraceLine(105,0,__PYX_ERR(0, 105, __pyx_L1_error))
+  __Pyx_TraceLine(110,0,__PYX_ERR(0, 110, __pyx_L1_error))
   __pyx_v_previous_pos = 0;
 
-  /* "haggregate/regularize.pyx":106
+  /* "haggregate/regularize.pyx":111
  * 
  *     previous_pos = 0
  *     for i in range(result_index.size):             # <<<<<<<<<<<<<<
  *         t = result_index[i]
  *         result_values[i], result_flags[i], previous_pos = _get_record(
  */
-  __Pyx_TraceLine(106,0,__PYX_ERR(0, 106, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_result_index), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_TraceLine(111,0,__PYX_ERR(0, 111, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_result_index), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_2 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_2 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "haggregate/regularize.pyx":107
+    /* "haggregate/regularize.pyx":112
  *     previous_pos = 0
  *     for i in range(result_index.size):
  *         t = result_index[i]             # <<<<<<<<<<<<<<
  *         result_values[i], result_flags[i], previous_pos = _get_record(
- *             ts_index, ts_values, ts_flags, t, result_step, new_date_flag, previous_pos
+ *             ts_index,
  */
-    __Pyx_TraceLine(107,0,__PYX_ERR(0, 107, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_result_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __Pyx_TraceLine(112,0,__PYX_ERR(0, 112, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_result_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_t = __pyx_t_5;
 
-    /* "haggregate/regularize.pyx":108
+    /* "haggregate/regularize.pyx":113
  *     for i in range(result_index.size):
  *         t = result_index[i]
  *         result_values[i], result_flags[i], previous_pos = _get_record(             # <<<<<<<<<<<<<<
- *             ts_index, ts_values, ts_flags, t, result_step, new_date_flag, previous_pos
- *         )
+ *             ts_index,
+ *             ts_values,
  */
-    __Pyx_TraceLine(108,0,__PYX_ERR(0, 108, __pyx_L1_error))
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_get_record); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_get_record); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "haggregate/regularize.pyx":109
- *         t = result_index[i]
- *         result_values[i], result_flags[i], previous_pos = _get_record(
- *             ts_index, ts_values, ts_flags, t, result_step, new_date_flag, previous_pos             # <<<<<<<<<<<<<<
- *         )
- * 
+    /* "haggregate/regularize.pyx":117
+ *             ts_values,
+ *             ts_flags,
+ *             t,             # <<<<<<<<<<<<<<
+ *             result_step,
+ *             new_date_flag,
  */
-    __Pyx_TraceLine(109,0,__PYX_ERR(0, 109, __pyx_L1_error))
-    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __Pyx_TraceLine(117,0,__PYX_ERR(0, 117, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 117, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_v_result_step); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 109, __pyx_L1_error)
+
+    /* "haggregate/regularize.pyx":118
+ *             ts_flags,
+ *             t,
+ *             result_step,             # <<<<<<<<<<<<<<
+ *             new_date_flag,
+ *             previous_pos,
+ */
+    __Pyx_TraceLine(118,0,__PYX_ERR(0, 118, __pyx_L1_error))
+    __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_v_result_step); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 118, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_previous_pos); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L1_error)
+
+    /* "haggregate/regularize.pyx":120
+ *             result_step,
+ *             new_date_flag,
+ *             previous_pos,             # <<<<<<<<<<<<<<
+ *             mode,
+ *         )
+ */
+    __Pyx_TraceLine(120,0,__PYX_ERR(0, 120, __pyx_L1_error))
+    __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_previous_pos); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = NULL;
-    __pyx_t_11 = 0;
+
+    /* "haggregate/regularize.pyx":121
+ *             new_date_flag,
+ *             previous_pos,
+ *             mode,             # <<<<<<<<<<<<<<
+ *         )
+ * 
+ */
+    __Pyx_TraceLine(121,0,__PYX_ERR(0, 121, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_mode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = NULL;
+    __pyx_t_12 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_10)) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_10);
+        __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_11 = 1;
+        __pyx_t_12 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[8] = {__pyx_t_10, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), ((PyObject *)__pyx_v_ts_flags), __pyx_t_7, __pyx_t_8, __pyx_v_new_date_flag, __pyx_t_9};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_11, 7+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      PyObject *__pyx_temp[9] = {__pyx_t_11, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), ((PyObject *)__pyx_v_ts_flags), __pyx_t_7, __pyx_t_8, __pyx_v_new_date_flag, __pyx_t_9, __pyx_t_10};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_12, 8+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[8] = {__pyx_t_10, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), ((PyObject *)__pyx_v_ts_flags), __pyx_t_7, __pyx_t_8, __pyx_v_new_date_flag, __pyx_t_9};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_11, 7+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      PyObject *__pyx_temp[9] = {__pyx_t_11, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), ((PyObject *)__pyx_v_ts_flags), __pyx_t_7, __pyx_t_8, __pyx_v_new_date_flag, __pyx_t_9, __pyx_t_10};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_12, 8+__pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     {
-      __pyx_t_12 = PyTuple_New(7+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      if (__pyx_t_10) {
-        __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
+      __pyx_t_13 = PyTuple_New(8+__pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      if (__pyx_t_11) {
+        __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_11); __pyx_t_11 = NULL;
       }
       __Pyx_INCREF(((PyObject *)__pyx_v_ts_index));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_ts_index));
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, ((PyObject *)__pyx_v_ts_index));
+      PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_12, ((PyObject *)__pyx_v_ts_index));
       __Pyx_INCREF(((PyObject *)__pyx_v_ts_values));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_ts_values));
-      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, ((PyObject *)__pyx_v_ts_values));
+      PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_12, ((PyObject *)__pyx_v_ts_values));
       __Pyx_INCREF(((PyObject *)__pyx_v_ts_flags));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_ts_flags));
-      PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_11, ((PyObject *)__pyx_v_ts_flags));
+      PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_12, ((PyObject *)__pyx_v_ts_flags));
       __Pyx_GIVEREF(__pyx_t_7);
-      PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_11, __pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_12, __pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_8);
-      PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_11, __pyx_t_8);
+      PyTuple_SET_ITEM(__pyx_t_13, 4+__pyx_t_12, __pyx_t_8);
       __Pyx_INCREF(__pyx_v_new_date_flag);
       __Pyx_GIVEREF(__pyx_v_new_date_flag);
-      PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_11, __pyx_v_new_date_flag);
+      PyTuple_SET_ITEM(__pyx_t_13, 5+__pyx_t_12, __pyx_v_new_date_flag);
       __Pyx_GIVEREF(__pyx_t_9);
-      PyTuple_SET_ITEM(__pyx_t_12, 6+__pyx_t_11, __pyx_t_9);
+      PyTuple_SET_ITEM(__pyx_t_13, 6+__pyx_t_12, __pyx_t_9);
+      __Pyx_GIVEREF(__pyx_t_10);
+      PyTuple_SET_ITEM(__pyx_t_13, 7+__pyx_t_12, __pyx_t_10);
       __pyx_t_7 = 0;
       __pyx_t_8 = 0;
       __pyx_t_9 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_10 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
       PyObject* sequence = __pyx_t_1;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 108, __pyx_L1_error)
+        __PYX_ERR(0, 113, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
-        __pyx_t_9 = PyTuple_GET_ITEM(sequence, 2); 
+        __pyx_t_13 = PyTuple_GET_ITEM(sequence, 1); 
+        __pyx_t_10 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
         __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_12 = PyList_GET_ITEM(sequence, 1); 
-        __pyx_t_9 = PyList_GET_ITEM(sequence, 2); 
+        __pyx_t_13 = PyList_GET_ITEM(sequence, 1); 
+        __pyx_t_10 = PyList_GET_ITEM(sequence, 2); 
       }
       __Pyx_INCREF(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_12);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_13);
+      __Pyx_INCREF(__pyx_t_10);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      __pyx_t_9 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __pyx_t_10 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_8 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 108, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_13 = Py_TYPE(__pyx_t_8)->tp_iternext;
-      index = 0; __pyx_t_6 = __pyx_t_13(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
+      __pyx_t_14 = Py_TYPE(__pyx_t_9)->tp_iternext;
+      index = 0; __pyx_t_6 = __pyx_t_14(__pyx_t_9); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      index = 1; __pyx_t_12 = __pyx_t_13(__pyx_t_8); if (unlikely(!__pyx_t_12)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_12);
-      index = 2; __pyx_t_9 = __pyx_t_13(__pyx_t_8); if (unlikely(!__pyx_t_9)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_9);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_8), 3) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
-      __pyx_t_13 = NULL;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      index = 1; __pyx_t_13 = __pyx_t_14(__pyx_t_9); if (unlikely(!__pyx_t_13)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_13);
+      index = 2; __pyx_t_10 = __pyx_t_14(__pyx_t_9); if (unlikely(!__pyx_t_10)) goto __pyx_L5_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_10);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_9), 3) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_14 = NULL;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_13 = NULL;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_14 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 108, __pyx_L1_error)
+      __PYX_ERR(0, 113, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
 
-    /* "haggregate/regularize.pyx":108
+    /* "haggregate/regularize.pyx":113
  *     for i in range(result_index.size):
  *         t = result_index[i]
  *         result_values[i], result_flags[i], previous_pos = _get_record(             # <<<<<<<<<<<<<<
- *             ts_index, ts_values, ts_flags, t, result_step, new_date_flag, previous_pos
- *         )
+ *             ts_index,
+ *             ts_values,
  */
-    __Pyx_TraceLine(108,0,__PYX_ERR(0, 108, __pyx_L1_error))
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_9); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_result_values), __pyx_v_i, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
+    __pyx_t_12 = __Pyx_PyInt_As_int(__pyx_t_10); if (unlikely((__pyx_t_12 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_result_values), __pyx_v_i, __pyx_t_6, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_result_flags), __pyx_v_i, __pyx_t_12, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_v_previous_pos = __pyx_t_11;
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_result_flags), __pyx_v_i, __pyx_t_13, int, 1, __Pyx_PyInt_From_int, 0, 1, 1) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    __pyx_v_previous_pos = __pyx_t_12;
   }
 
-  /* "haggregate/regularize.pyx":92
+  /* "haggregate/regularize.pyx":96
  * 
  * 
  * def _perform_regularization(             # <<<<<<<<<<<<<<
  *     np.ndarray result_index,
  *     np.ndarray result_values,
  */
 
@@ -4015,25 +4125,26 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("haggregate.regularize._perform_regularization", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "haggregate/regularize.pyx":113
+/* "haggregate/regularize.pyx":125
  * 
  * 
  * def _get_record(             # <<<<<<<<<<<<<<
  *     np.ndarray ts_index,
  *     np.ndarray ts_values,
  */
 
@@ -4042,29 +4153,32 @@
 static PyMethodDef __pyx_mdef_10haggregate_10regularize_5_get_record = {"_get_record", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10haggregate_10regularize_5_get_record, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_10haggregate_10regularize_5_get_record(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_ts_index = 0;
   PyArrayObject *__pyx_v_ts_values = 0;
   PyArrayObject *__pyx_v_ts_flags = 0;
   long __pyx_v_t;
   long __pyx_v_result_step;
-  CYTHON_UNUSED PyObject *__pyx_v_new_date_flag = 0;
+  PyObject *__pyx_v_new_date_flag = 0;
   int __pyx_v_previous_pos;
+  int __pyx_v_mode;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_record (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts_index,&__pyx_n_s_ts_values,&__pyx_n_s_ts_flags,&__pyx_n_s_t,&__pyx_n_s_result_step,&__pyx_n_s_new_date_flag,&__pyx_n_s_previous_pos,0};
-    PyObject* values[7] = {0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts_index,&__pyx_n_s_ts_values,&__pyx_n_s_ts_flags,&__pyx_n_s_t,&__pyx_n_s_result_step,&__pyx_n_s_new_date_flag,&__pyx_n_s_previous_pos,&__pyx_n_s_mode,0};
+    PyObject* values[8] = {0,0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
@@ -4083,605 +4197,1167 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_index)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_values)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 1); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 1); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 2); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 2); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 3); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 3); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_result_step)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 4); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 4); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_new_date_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 5); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 5); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_previous_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, 6); __PYX_ERR(0, 113, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 6); __PYX_ERR(0, 125, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, 7); __PYX_ERR(0, 125, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_get_record") < 0)) __PYX_ERR(0, 113, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_get_record") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 8) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+      values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
     }
     __pyx_v_ts_index = ((PyArrayObject *)values[0]);
     __pyx_v_ts_values = ((PyArrayObject *)values[1]);
     __pyx_v_ts_flags = ((PyArrayObject *)values[2]);
-    __pyx_v_t = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_t == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
-    __pyx_v_result_step = __Pyx_PyInt_As_long(values[4]); if (unlikely((__pyx_v_result_step == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 118, __pyx_L3_error)
+    __pyx_v_t = __Pyx_PyInt_As_long(values[3]); if (unlikely((__pyx_v_t == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L3_error)
+    __pyx_v_result_step = __Pyx_PyInt_As_long(values[4]); if (unlikely((__pyx_v_result_step == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L3_error)
     __pyx_v_new_date_flag = ((PyObject*)values[5]);
-    __pyx_v_previous_pos = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_previous_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L3_error)
+    __pyx_v_previous_pos = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_previous_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 132, __pyx_L3_error)
+    __pyx_v_mode = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_mode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_get_record", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 113, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_get_record", 1, 8, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("haggregate.regularize._get_record", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_index), __pyx_ptype_5numpy_ndarray, 1, "ts_index", 0))) __PYX_ERR(0, 114, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_values), __pyx_ptype_5numpy_ndarray, 1, "ts_values", 0))) __PYX_ERR(0, 115, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_flags), __pyx_ptype_5numpy_ndarray, 1, "ts_flags", 0))) __PYX_ERR(0, 116, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_new_date_flag), (&PyUnicode_Type), 1, "new_date_flag", 1))) __PYX_ERR(0, 119, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10haggregate_10regularize_4_get_record(__pyx_self, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_t, __pyx_v_result_step, __pyx_v_new_date_flag, __pyx_v_previous_pos);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_index), __pyx_ptype_5numpy_ndarray, 1, "ts_index", 0))) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_values), __pyx_ptype_5numpy_ndarray, 1, "ts_values", 0))) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_flags), __pyx_ptype_5numpy_ndarray, 1, "ts_flags", 0))) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_new_date_flag), (&PyUnicode_Type), 1, "new_date_flag", 1))) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10haggregate_10regularize_4_get_record(__pyx_self, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_ts_flags, __pyx_v_t, __pyx_v_result_step, __pyx_v_new_date_flag, __pyx_v_previous_pos, __pyx_v_mode);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10haggregate_10regularize_4_get_record(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_t, long __pyx_v_result_step, CYTHON_UNUSED PyObject *__pyx_v_new_date_flag, int __pyx_v_previous_pos) {
+static PyObject *__pyx_pf_10haggregate_10regularize_4_get_record(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_ts_index, PyArrayObject *__pyx_v_ts_values, PyArrayObject *__pyx_v_ts_flags, long __pyx_v_t, long __pyx_v_result_step, PyObject *__pyx_v_new_date_flag, int __pyx_v_previous_pos, int __pyx_v_mode) {
   int __pyx_v_i;
   int __pyx_v_found;
   int __pyx_v_count;
+  int __pyx_v_nearest_i;
+  int __pyx_v_INTERVAL;
+  CYTHON_UNUSED int __pyx_v_INSTANTANEOUS;
   double __pyx_v_start;
   double __pyx_v_end;
+  PyObject *__pyx_v_ti = NULL;
   PyObject *__pyx_v_value = NULL;
   PyObject *__pyx_v_flags = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  long __pyx_t_2;
-  long __pyx_t_3;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  long __pyx_t_4;
+  long __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  long double __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  int __pyx_t_14;
+  PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceFrameInit(__pyx_codeobj__5)
+  __Pyx_TraceFrameInit(__pyx_codeobj__6)
   __Pyx_RefNannySetupContext("_get_record", 0);
-  __Pyx_TraceCall("_get_record", __pyx_f[0], 113, 0, __PYX_ERR(0, 113, __pyx_L1_error));
+  __Pyx_TraceCall("_get_record", __pyx_f[0], 125, 0, __PYX_ERR(0, 125, __pyx_L1_error));
 
-  /* "haggregate/regularize.pyx":125
+  /* "haggregate/regularize.pyx":136
+ * ):
+ *     cdef int i, found, count
+ *     cdef int nearest_i = -1             # <<<<<<<<<<<<<<
+ *     cdef int INTERVAL = RM.INTERVAL.value
+ *     cdef int INSTANTANEOUS = RM.INSTANTANEOUS.value
+ */
+  __Pyx_TraceLine(136,0,__PYX_ERR(0, 136, __pyx_L1_error))
+  __pyx_v_nearest_i = -1;
+
+  /* "haggregate/regularize.pyx":137
+ *     cdef int i, found, count
+ *     cdef int nearest_i = -1
+ *     cdef int INTERVAL = RM.INTERVAL.value             # <<<<<<<<<<<<<<
+ *     cdef int INSTANTANEOUS = RM.INSTANTANEOUS.value
+ * 
+ */
+  __Pyx_TraceLine(137,0,__PYX_ERR(0, 137, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INTERVAL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_INTERVAL = __pyx_t_3;
+
+  /* "haggregate/regularize.pyx":138
+ *     cdef int nearest_i = -1
+ *     cdef int INTERVAL = RM.INTERVAL.value
+ *     cdef int INSTANTANEOUS = RM.INSTANTANEOUS.value             # <<<<<<<<<<<<<<
+ * 
+ *     # Return the source record if it already exists
+ */
+  __Pyx_TraceLine(138,0,__PYX_ERR(0, 138, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INSTANTANEOUS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_INSTANTANEOUS = __pyx_t_3;
+
+  /* "haggregate/regularize.pyx":141
  * 
  *     # Return the source record if it already exists
  *     found = False             # <<<<<<<<<<<<<<
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] == t:
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):
  */
-  __Pyx_TraceLine(125,0,__PYX_ERR(0, 125, __pyx_L1_error))
+  __Pyx_TraceLine(141,0,__PYX_ERR(0, 141, __pyx_L1_error))
   __pyx_v_found = 0;
 
-  /* "haggregate/regularize.pyx":126
+  /* "haggregate/regularize.pyx":142
  *     # Return the source record if it already exists
  *     found = False
  *     for i in range(previous_pos, ts_index.size):             # <<<<<<<<<<<<<<
- *         if ts_index[i] == t:
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):
  *             found = True
  */
-  __Pyx_TraceLine(126,0,__PYX_ERR(0, 126, __pyx_L1_error))
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ts_index), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_TraceLine(142,0,__PYX_ERR(0, 142, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ts_index), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_2 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_4 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = __pyx_v_previous_pos; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
+  __pyx_t_5 = __pyx_t_4;
+  for (__pyx_t_3 = __pyx_v_previous_pos; __pyx_t_3 < __pyx_t_5; __pyx_t_3+=1) {
+    __pyx_v_i = __pyx_t_3;
 
-    /* "haggregate/regularize.pyx":127
+    /* "haggregate/regularize.pyx":143
  *     found = False
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] == t:             # <<<<<<<<<<<<<<
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):             # <<<<<<<<<<<<<<
  *             found = True
  *             break
  */
-    __Pyx_TraceLine(127,0,__PYX_ERR(0, 127, __pyx_L1_error))
-    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_TraceLine(143,0,__PYX_ERR(0, 143, __pyx_L1_error))
+    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 127, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 127, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (__pyx_t_7) {
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (__pyx_t_8) {
+    } else {
+      __pyx_t_6 = __pyx_t_8;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_8 = ((__pyx_v_mode == __pyx_v_INTERVAL) != 0);
+    if (!__pyx_t_8) {
+    } else {
+      __pyx_t_6 = __pyx_t_8;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_7 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_9 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_8 = ((!(isnan(__pyx_t_9) != 0)) != 0);
+    __pyx_t_6 = __pyx_t_8;
+    __pyx_L6_bool_binop_done:;
+    if (__pyx_t_6) {
 
-      /* "haggregate/regularize.pyx":128
+      /* "haggregate/regularize.pyx":144
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] == t:
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):
  *             found = True             # <<<<<<<<<<<<<<
  *             break
  *         if ts_index[i] > t:
  */
-      __Pyx_TraceLine(128,0,__PYX_ERR(0, 128, __pyx_L1_error))
+      __Pyx_TraceLine(144,0,__PYX_ERR(0, 144, __pyx_L1_error))
       __pyx_v_found = 1;
 
-      /* "haggregate/regularize.pyx":129
- *         if ts_index[i] == t:
+      /* "haggregate/regularize.pyx":145
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):
  *             found = True
  *             break             # <<<<<<<<<<<<<<
  *         if ts_index[i] > t:
  *             break
  */
-      __Pyx_TraceLine(129,0,__PYX_ERR(0, 129, __pyx_L1_error))
+      __Pyx_TraceLine(145,0,__PYX_ERR(0, 145, __pyx_L1_error))
       goto __pyx_L4_break;
 
-      /* "haggregate/regularize.pyx":127
+      /* "haggregate/regularize.pyx":143
  *     found = False
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] == t:             # <<<<<<<<<<<<<<
+ *         if ts_index[i] == t and (mode == INTERVAL or not isnan(ts_values[i])):             # <<<<<<<<<<<<<<
  *             found = True
  *             break
  */
     }
 
-    /* "haggregate/regularize.pyx":130
+    /* "haggregate/regularize.pyx":146
  *             found = True
  *             break
  *         if ts_index[i] > t:             # <<<<<<<<<<<<<<
  *             break
  *     if found:
  */
-    __Pyx_TraceLine(130,0,__PYX_ERR(0, 130, __pyx_L1_error))
-    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_6, __pyx_t_5, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_TraceLine(146,0,__PYX_ERR(0, 146, __pyx_L1_error))
+    __pyx_t_7 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_7, __pyx_t_2, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__pyx_t_7) {
+    if (__pyx_t_6) {
 
-      /* "haggregate/regularize.pyx":131
+      /* "haggregate/regularize.pyx":147
  *             break
  *         if ts_index[i] > t:
  *             break             # <<<<<<<<<<<<<<
  *     if found:
  *         return ts_values[i], ts_flags[i], i
  */
-      __Pyx_TraceLine(131,0,__PYX_ERR(0, 131, __pyx_L1_error))
+      __Pyx_TraceLine(147,0,__PYX_ERR(0, 147, __pyx_L1_error))
       goto __pyx_L4_break;
 
-      /* "haggregate/regularize.pyx":130
+      /* "haggregate/regularize.pyx":146
  *             found = True
  *             break
  *         if ts_index[i] > t:             # <<<<<<<<<<<<<<
  *             break
  *     if found:
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "haggregate/regularize.pyx":132
+  /* "haggregate/regularize.pyx":148
  *         if ts_index[i] > t:
  *             break
  *     if found:             # <<<<<<<<<<<<<<
  *         return ts_values[i], ts_flags[i], i
  * 
  */
-  __Pyx_TraceLine(132,0,__PYX_ERR(0, 132, __pyx_L1_error))
-  __pyx_t_7 = (__pyx_v_found != 0);
-  if (__pyx_t_7) {
+  __Pyx_TraceLine(148,0,__PYX_ERR(0, 148, __pyx_L1_error))
+  __pyx_t_6 = (__pyx_v_found != 0);
+  if (__pyx_t_6) {
 
-    /* "haggregate/regularize.pyx":133
+    /* "haggregate/regularize.pyx":149
  *             break
  *     if found:
  *         return ts_values[i], ts_flags[i], i             # <<<<<<<<<<<<<<
  * 
- *     # Otherwise get the nearby record, if it exists and is only one
+ *     # Otherwise get the nearby record, if it exists
  */
-    __Pyx_TraceLine(133,0,__PYX_ERR(0, 133, __pyx_L1_error))
+    __Pyx_TraceLine(149,0,__PYX_ERR(0, 149, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_flags), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 133, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_2 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_flags), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_2);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_7);
     __pyx_t_1 = 0;
-    __pyx_t_5 = 0;
-    __pyx_t_6 = 0;
-    __pyx_r = __pyx_t_8;
-    __pyx_t_8 = 0;
+    __pyx_t_2 = 0;
+    __pyx_t_7 = 0;
+    __pyx_r = __pyx_t_10;
+    __pyx_t_10 = 0;
     goto __pyx_L0;
 
-    /* "haggregate/regularize.pyx":132
+    /* "haggregate/regularize.pyx":148
  *         if ts_index[i] > t:
  *             break
  *     if found:             # <<<<<<<<<<<<<<
  *         return ts_values[i], ts_flags[i], i
  * 
  */
   }
 
-  /* "haggregate/regularize.pyx":136
+  /* "haggregate/regularize.pyx":152
  * 
- *     # Otherwise get the nearby record, if it exists and is only one
+ *     # Otherwise get the nearby record, if it exists
  *     start = t - result_step / 2             # <<<<<<<<<<<<<<
  *     end = t + result_step / 2
  *     count = 0
  */
-  __Pyx_TraceLine(136,0,__PYX_ERR(0, 136, __pyx_L1_error))
+  __Pyx_TraceLine(152,0,__PYX_ERR(0, 152, __pyx_L1_error))
   __pyx_v_start = (__pyx_v_t - (((double)__pyx_v_result_step) / 2.0));
 
-  /* "haggregate/regularize.pyx":137
- *     # Otherwise get the nearby record, if it exists and is only one
+  /* "haggregate/regularize.pyx":153
+ *     # Otherwise get the nearby record, if it exists
  *     start = t - result_step / 2
  *     end = t + result_step / 2             # <<<<<<<<<<<<<<
  *     count = 0
  *     for i in range(previous_pos, ts_index.size):
  */
-  __Pyx_TraceLine(137,0,__PYX_ERR(0, 137, __pyx_L1_error))
+  __Pyx_TraceLine(153,0,__PYX_ERR(0, 153, __pyx_L1_error))
   __pyx_v_end = (__pyx_v_t + (((double)__pyx_v_result_step) / 2.0));
 
-  /* "haggregate/regularize.pyx":138
+  /* "haggregate/regularize.pyx":154
  *     start = t - result_step / 2
  *     end = t + result_step / 2
  *     count = 0             # <<<<<<<<<<<<<<
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] >= start and ts_index[i] < end:
+ *         ti = ts_index[i]
  */
-  __Pyx_TraceLine(138,0,__PYX_ERR(0, 138, __pyx_L1_error))
+  __Pyx_TraceLine(154,0,__PYX_ERR(0, 154, __pyx_L1_error))
   __pyx_v_count = 0;
 
-  /* "haggregate/regularize.pyx":139
+  /* "haggregate/regularize.pyx":155
  *     end = t + result_step / 2
  *     count = 0
  *     for i in range(previous_pos, ts_index.size):             # <<<<<<<<<<<<<<
- *         if ts_index[i] >= start and ts_index[i] < end:
- *             count += 1
+ *         ti = ts_index[i]
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):
  */
-  __Pyx_TraceLine(139,0,__PYX_ERR(0, 139, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ts_index), __pyx_n_s_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_2 = __Pyx_PyInt_As_long(__pyx_t_8); if (unlikely((__pyx_t_2 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = __pyx_v_previous_pos; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
+  __Pyx_TraceLine(155,0,__PYX_ERR(0, 155, __pyx_L1_error))
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ts_index), __pyx_n_s_size); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_4 = __Pyx_PyInt_As_long(__pyx_t_10); if (unlikely((__pyx_t_4 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_5 = __pyx_t_4;
+  for (__pyx_t_3 = __pyx_v_previous_pos; __pyx_t_3 < __pyx_t_5; __pyx_t_3+=1) {
+    __pyx_v_i = __pyx_t_3;
 
-    /* "haggregate/regularize.pyx":140
+    /* "haggregate/regularize.pyx":156
  *     count = 0
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] >= start and ts_index[i] < end:             # <<<<<<<<<<<<<<
+ *         ti = ts_index[i]             # <<<<<<<<<<<<<<
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):
  *             count += 1
- *         if ts_index[i] >= end:
  */
-    __Pyx_TraceLine(140,0,__PYX_ERR(0, 140, __pyx_L1_error))
-    __pyx_t_8 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_start); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_8, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (__pyx_t_9) {
-    } else {
-      __pyx_t_7 = __pyx_t_9;
-      goto __pyx_L11_bool_binop_done;
-    }
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = PyObject_RichCompare(__pyx_t_5, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 140, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_7 = __pyx_t_9;
-    __pyx_L11_bool_binop_done:;
-    if (__pyx_t_7) {
+    __Pyx_TraceLine(156,0,__PYX_ERR(0, 156, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_XDECREF_SET(__pyx_v_ti, __pyx_t_10);
+    __pyx_t_10 = 0;
 
-      /* "haggregate/regularize.pyx":141
+    /* "haggregate/regularize.pyx":157
  *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] >= start and ts_index[i] < end:
+ *         ti = ts_index[i]
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):             # <<<<<<<<<<<<<<
+ *             count += 1
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
+ */
+    __Pyx_TraceLine(157,0,__PYX_ERR(0, 157, __pyx_L1_error))
+    __pyx_t_10 = PyFloat_FromDouble(__pyx_v_start); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_7 = PyObject_RichCompare(__pyx_v_ti, __pyx_t_10, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (__pyx_t_8) {
+    } else {
+      __pyx_t_6 = __pyx_t_8;
+      goto __pyx_L14_bool_binop_done;
+    }
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_end); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_10 = PyObject_RichCompare(__pyx_v_ti, __pyx_t_7, Py_LT); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    if (__pyx_t_8) {
+    } else {
+      __pyx_t_6 = __pyx_t_8;
+      goto __pyx_L14_bool_binop_done;
+    }
+    __pyx_t_8 = ((__pyx_v_mode == __pyx_v_INTERVAL) != 0);
+    if (!__pyx_t_8) {
+    } else {
+      __pyx_t_6 = __pyx_t_8;
+      goto __pyx_L14_bool_binop_done;
+    }
+    __pyx_t_10 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_9 = __pyx_PyFloat_AsDouble(__pyx_t_10); if (unlikely((__pyx_t_9 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_8 = ((!(isnan(__pyx_t_9) != 0)) != 0);
+    __pyx_t_6 = __pyx_t_8;
+    __pyx_L14_bool_binop_done:;
+    if (__pyx_t_6) {
+
+      /* "haggregate/regularize.pyx":158
+ *         ti = ts_index[i]
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):
  *             count += 1             # <<<<<<<<<<<<<<
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
  *         if ts_index[i] >= end:
- *             i -= 1
  */
-      __Pyx_TraceLine(141,0,__PYX_ERR(0, 141, __pyx_L1_error))
+      __Pyx_TraceLine(158,0,__PYX_ERR(0, 158, __pyx_L1_error))
       __pyx_v_count = (__pyx_v_count + 1);
 
-      /* "haggregate/regularize.pyx":140
- *     count = 0
- *     for i in range(previous_pos, ts_index.size):
- *         if ts_index[i] >= start and ts_index[i] < end:             # <<<<<<<<<<<<<<
+      /* "haggregate/regularize.pyx":159
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):
  *             count += 1
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)             # <<<<<<<<<<<<<<
  *         if ts_index[i] >= end:
+ *             i -= 1
+ */
+      __Pyx_TraceLine(159,0,__PYX_ERR(0, 159, __pyx_L1_error))
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_get_nearest); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_nearest_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_11 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_mode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_12);
+      __pyx_t_13 = NULL;
+      __pyx_t_14 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_7);
+        if (likely(__pyx_t_13)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+          __Pyx_INCREF(__pyx_t_13);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_7, function);
+          __pyx_t_14 = 1;
+        }
+      }
+      #if CYTHON_FAST_PYCALL
+      if (PyFunction_Check(__pyx_t_7)) {
+        PyObject *__pyx_temp[7] = {__pyx_t_13, __pyx_t_2, __pyx_t_1, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), __pyx_t_11, __pyx_t_12};
+        __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_14, 6+__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      } else
+      #endif
+      #if CYTHON_FAST_PYCCALL
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
+        PyObject *__pyx_temp[7] = {__pyx_t_13, __pyx_t_2, __pyx_t_1, ((PyObject *)__pyx_v_ts_index), ((PyObject *)__pyx_v_ts_values), __pyx_t_11, __pyx_t_12};
+        __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_14, 6+__pyx_t_14); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      } else
+      #endif
+      {
+        __pyx_t_15 = PyTuple_New(6+__pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_15);
+        if (__pyx_t_13) {
+          __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_13); __pyx_t_13 = NULL;
+        }
+        __Pyx_GIVEREF(__pyx_t_2);
+        PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_14, __pyx_t_2);
+        __Pyx_GIVEREF(__pyx_t_1);
+        PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_14, __pyx_t_1);
+        __Pyx_INCREF(((PyObject *)__pyx_v_ts_index));
+        __Pyx_GIVEREF(((PyObject *)__pyx_v_ts_index));
+        PyTuple_SET_ITEM(__pyx_t_15, 2+__pyx_t_14, ((PyObject *)__pyx_v_ts_index));
+        __Pyx_INCREF(((PyObject *)__pyx_v_ts_values));
+        __Pyx_GIVEREF(((PyObject *)__pyx_v_ts_values));
+        PyTuple_SET_ITEM(__pyx_t_15, 3+__pyx_t_14, ((PyObject *)__pyx_v_ts_values));
+        __Pyx_GIVEREF(__pyx_t_11);
+        PyTuple_SET_ITEM(__pyx_t_15, 4+__pyx_t_14, __pyx_t_11);
+        __Pyx_GIVEREF(__pyx_t_12);
+        PyTuple_SET_ITEM(__pyx_t_15, 5+__pyx_t_14, __pyx_t_12);
+        __pyx_t_2 = 0;
+        __pyx_t_1 = 0;
+        __pyx_t_11 = 0;
+        __pyx_t_12 = 0;
+        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_15, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_10); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 159, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_v_nearest_i = __pyx_t_14;
+
+      /* "haggregate/regularize.pyx":157
+ *     for i in range(previous_pos, ts_index.size):
+ *         ti = ts_index[i]
+ *         if ti >= start and ti < end and (mode == INTERVAL or not isnan(ts_values[i])):             # <<<<<<<<<<<<<<
+ *             count += 1
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
  */
     }
 
-    /* "haggregate/regularize.pyx":142
- *         if ts_index[i] >= start and ts_index[i] < end:
+    /* "haggregate/regularize.pyx":160
  *             count += 1
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
  *         if ts_index[i] >= end:             # <<<<<<<<<<<<<<
  *             i -= 1
  *             break
  */
-    __Pyx_TraceLine(142,0,__PYX_ERR(0, 142, __pyx_L1_error))
-    __pyx_t_8 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 142, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 142, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_8, __pyx_t_6, Py_GE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (__pyx_t_7) {
+    __Pyx_TraceLine(160,0,__PYX_ERR(0, 160, __pyx_L1_error))
+    __pyx_t_10 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_end); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_15 = PyObject_RichCompare(__pyx_t_10, __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_15); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_15); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+    if (__pyx_t_6) {
 
-      /* "haggregate/regularize.pyx":143
- *             count += 1
+      /* "haggregate/regularize.pyx":161
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
  *         if ts_index[i] >= end:
  *             i -= 1             # <<<<<<<<<<<<<<
  *             break
- *     if count != 1:
+ *     if count < 1 or (count > 1 and mode == INTERVAL):
  */
-      __Pyx_TraceLine(143,0,__PYX_ERR(0, 143, __pyx_L1_error))
+      __Pyx_TraceLine(161,0,__PYX_ERR(0, 161, __pyx_L1_error))
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "haggregate/regularize.pyx":144
+      /* "haggregate/regularize.pyx":162
  *         if ts_index[i] >= end:
  *             i -= 1
  *             break             # <<<<<<<<<<<<<<
- *     if count != 1:
+ *     if count < 1 or (count > 1 and mode == INTERVAL):
  *         return np.nan, "", i
  */
-      __Pyx_TraceLine(144,0,__PYX_ERR(0, 144, __pyx_L1_error))
-      goto __pyx_L9_break;
+      __Pyx_TraceLine(162,0,__PYX_ERR(0, 162, __pyx_L1_error))
+      goto __pyx_L12_break;
 
-      /* "haggregate/regularize.pyx":142
- *         if ts_index[i] >= start and ts_index[i] < end:
+      /* "haggregate/regularize.pyx":160
  *             count += 1
+ *             nearest_i = _get_nearest(nearest_i, i, ts_index, ts_values, t, mode)
  *         if ts_index[i] >= end:             # <<<<<<<<<<<<<<
  *             i -= 1
  *             break
  */
     }
   }
-  __pyx_L9_break:;
+  __pyx_L12_break:;
 
-  /* "haggregate/regularize.pyx":145
+  /* "haggregate/regularize.pyx":163
  *             i -= 1
  *             break
- *     if count != 1:             # <<<<<<<<<<<<<<
+ *     if count < 1 or (count > 1 and mode == INTERVAL):             # <<<<<<<<<<<<<<
  *         return np.nan, "", i
- *     value = ts_values[i]
+ *     value = ts_values[nearest_i]
  */
-  __Pyx_TraceLine(145,0,__PYX_ERR(0, 145, __pyx_L1_error))
-  __pyx_t_7 = ((__pyx_v_count != 1) != 0);
-  if (__pyx_t_7) {
+  __Pyx_TraceLine(163,0,__PYX_ERR(0, 163, __pyx_L1_error))
+  __pyx_t_8 = ((__pyx_v_count < 1) != 0);
+  if (!__pyx_t_8) {
+  } else {
+    __pyx_t_6 = __pyx_t_8;
+    goto __pyx_L20_bool_binop_done;
+  }
+  __pyx_t_8 = ((__pyx_v_count > 1) != 0);
+  if (__pyx_t_8) {
+  } else {
+    __pyx_t_6 = __pyx_t_8;
+    goto __pyx_L20_bool_binop_done;
+  }
+  __pyx_t_8 = ((__pyx_v_mode == __pyx_v_INTERVAL) != 0);
+  __pyx_t_6 = __pyx_t_8;
+  __pyx_L20_bool_binop_done:;
+  if (__pyx_t_6) {
 
-    /* "haggregate/regularize.pyx":146
+    /* "haggregate/regularize.pyx":164
  *             break
- *     if count != 1:
+ *     if count < 1 or (count > 1 and mode == INTERVAL):
  *         return np.nan, "", i             # <<<<<<<<<<<<<<
- *     value = ts_values[i]
- *     flags = ts_flags[i]
+ *     value = ts_values[nearest_i]
+ *     flags = ts_flags[nearest_i]
  */
-    __Pyx_TraceLine(146,0,__PYX_ERR(0, 146, __pyx_L1_error))
+    __Pyx_TraceLine(164,0,__PYX_ERR(0, 164, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 146, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6);
-    __Pyx_INCREF(__pyx_kp_u__3);
-    __Pyx_GIVEREF(__pyx_kp_u__3);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_kp_u__3);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_5);
-    __pyx_t_6 = 0;
-    __pyx_t_5 = 0;
-    __pyx_r = __pyx_t_8;
-    __pyx_t_8 = 0;
+    __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_15);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_nan); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+    __pyx_t_15 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_15);
+    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7);
+    __Pyx_INCREF(__pyx_kp_u__4);
+    __Pyx_GIVEREF(__pyx_kp_u__4);
+    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_kp_u__4);
+    __Pyx_GIVEREF(__pyx_t_15);
+    PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_15);
+    __pyx_t_7 = 0;
+    __pyx_t_15 = 0;
+    __pyx_r = __pyx_t_10;
+    __pyx_t_10 = 0;
     goto __pyx_L0;
 
-    /* "haggregate/regularize.pyx":145
+    /* "haggregate/regularize.pyx":163
  *             i -= 1
  *             break
- *     if count != 1:             # <<<<<<<<<<<<<<
+ *     if count < 1 or (count > 1 and mode == INTERVAL):             # <<<<<<<<<<<<<<
  *         return np.nan, "", i
- *     value = ts_values[i]
+ *     value = ts_values[nearest_i]
  */
   }
 
-  /* "haggregate/regularize.pyx":147
- *     if count != 1:
+  /* "haggregate/regularize.pyx":165
+ *     if count < 1 or (count > 1 and mode == INTERVAL):
  *         return np.nan, "", i
- *     value = ts_values[i]             # <<<<<<<<<<<<<<
- *     flags = ts_flags[i]
+ *     value = ts_values[nearest_i]             # <<<<<<<<<<<<<<
+ *     flags = ts_flags[nearest_i]
  *     if flags:
  */
-  __Pyx_TraceLine(147,0,__PYX_ERR(0, 147, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 147, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_v_value = __pyx_t_8;
-  __pyx_t_8 = 0;
+  __Pyx_TraceLine(165,0,__PYX_ERR(0, 165, __pyx_L1_error))
+  __pyx_t_10 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_values), __pyx_v_nearest_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_v_value = __pyx_t_10;
+  __pyx_t_10 = 0;
 
-  /* "haggregate/regularize.pyx":148
+  /* "haggregate/regularize.pyx":166
  *         return np.nan, "", i
- *     value = ts_values[i]
- *     flags = ts_flags[i]             # <<<<<<<<<<<<<<
+ *     value = ts_values[nearest_i]
+ *     flags = ts_flags[nearest_i]             # <<<<<<<<<<<<<<
  *     if flags:
  *         flags += " "
  */
-  __Pyx_TraceLine(148,0,__PYX_ERR(0, 148, __pyx_L1_error))
-  __pyx_t_8 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_flags), __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_v_flags = __pyx_t_8;
-  __pyx_t_8 = 0;
-
-  /* "haggregate/regularize.pyx":149
- *     value = ts_values[i]
- *     flags = ts_flags[i]
+  __Pyx_TraceLine(166,0,__PYX_ERR(0, 166, __pyx_L1_error))
+  __pyx_t_10 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_flags), __pyx_v_nearest_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_v_flags = __pyx_t_10;
+  __pyx_t_10 = 0;
+
+  /* "haggregate/regularize.pyx":167
+ *     value = ts_values[nearest_i]
+ *     flags = ts_flags[nearest_i]
  *     if flags:             # <<<<<<<<<<<<<<
  *         flags += " "
- *     flags += "DATEINSERT"
+ *     flags += new_date_flag
  */
-  __Pyx_TraceLine(149,0,__PYX_ERR(0, 149, __pyx_L1_error))
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_flags); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
-  if (__pyx_t_7) {
+  __Pyx_TraceLine(167,0,__PYX_ERR(0, 167, __pyx_L1_error))
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_flags); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (__pyx_t_6) {
 
-    /* "haggregate/regularize.pyx":150
- *     flags = ts_flags[i]
+    /* "haggregate/regularize.pyx":168
+ *     flags = ts_flags[nearest_i]
  *     if flags:
  *         flags += " "             # <<<<<<<<<<<<<<
- *     flags += "DATEINSERT"
+ *     flags += new_date_flag
  *     return value, flags, i + 1
  */
-    __Pyx_TraceLine(150,0,__PYX_ERR(0, 150, __pyx_L1_error))
-    __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_v_flags, __pyx_kp_u__6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 150, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_8);
-    __pyx_t_8 = 0;
-
-    /* "haggregate/regularize.pyx":149
- *     value = ts_values[i]
- *     flags = ts_flags[i]
+    __Pyx_TraceLine(168,0,__PYX_ERR(0, 168, __pyx_L1_error))
+    __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_flags, __pyx_kp_u__7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_10);
+    __pyx_t_10 = 0;
+
+    /* "haggregate/regularize.pyx":167
+ *     value = ts_values[nearest_i]
+ *     flags = ts_flags[nearest_i]
  *     if flags:             # <<<<<<<<<<<<<<
  *         flags += " "
- *     flags += "DATEINSERT"
+ *     flags += new_date_flag
  */
   }
 
-  /* "haggregate/regularize.pyx":151
+  /* "haggregate/regularize.pyx":169
  *     if flags:
  *         flags += " "
- *     flags += "DATEINSERT"             # <<<<<<<<<<<<<<
+ *     flags += new_date_flag             # <<<<<<<<<<<<<<
  *     return value, flags, i + 1
+ * 
  */
-  __Pyx_TraceLine(151,0,__PYX_ERR(0, 151, __pyx_L1_error))
-  __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_v_flags, __pyx_n_u_DATEINSERT); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_8);
-  __pyx_t_8 = 0;
+  __Pyx_TraceLine(169,0,__PYX_ERR(0, 169, __pyx_L1_error))
+  __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_flags, __pyx_v_new_date_flag); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF_SET(__pyx_v_flags, __pyx_t_10);
+  __pyx_t_10 = 0;
 
-  /* "haggregate/regularize.pyx":152
+  /* "haggregate/regularize.pyx":170
  *         flags += " "
- *     flags += "DATEINSERT"
+ *     flags += new_date_flag
  *     return value, flags, i + 1             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
-  __Pyx_TraceLine(152,0,__PYX_ERR(0, 152, __pyx_L1_error))
+  __Pyx_TraceLine(170,0,__PYX_ERR(0, 170, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __Pyx_PyInt_From_long((__pyx_v_i + 1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_10 = __Pyx_PyInt_From_long((__pyx_v_i + 1)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_15);
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_value);
+  PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_v_value);
   __Pyx_INCREF(__pyx_v_flags);
   __Pyx_GIVEREF(__pyx_v_flags);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_flags);
-  __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_8);
-  __pyx_t_8 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_v_flags);
+  __Pyx_GIVEREF(__pyx_t_10);
+  PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_t_10);
+  __pyx_t_10 = 0;
+  __pyx_r = __pyx_t_15;
+  __pyx_t_15 = 0;
   goto __pyx_L0;
 
-  /* "haggregate/regularize.pyx":113
+  /* "haggregate/regularize.pyx":125
  * 
  * 
  * def _get_record(             # <<<<<<<<<<<<<<
  *     np.ndarray ts_index,
  *     np.ndarray ts_values,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("haggregate.regularize._get_record", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_ti);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_flags);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "haggregate/regularize.pyx":173
+ * 
+ * 
+ * def _get_nearest(             # <<<<<<<<<<<<<<
+ *     int previous_nearest_i,
+ *     int current_i,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10haggregate_10regularize_7_get_nearest(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_10haggregate_10regularize_7_get_nearest = {"_get_nearest", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10haggregate_10regularize_7_get_nearest, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10haggregate_10regularize_7_get_nearest(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  int __pyx_v_previous_nearest_i;
+  int __pyx_v_current_i;
+  PyArrayObject *__pyx_v_ts_index = 0;
+  CYTHON_UNUSED PyArrayObject *__pyx_v_ts_values = 0;
+  long __pyx_v_t;
+  int __pyx_v_mode;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_get_nearest (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_previous_nearest_i,&__pyx_n_s_current_i,&__pyx_n_s_ts_index,&__pyx_n_s_ts_values,&__pyx_n_s_t,&__pyx_n_s_mode,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_previous_nearest_i)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_current_i)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, 1); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_index)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, 2); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts_values)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, 3); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, 4); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, 5); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_get_nearest") < 0)) __PYX_ERR(0, 173, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+    }
+    __pyx_v_previous_nearest_i = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_previous_nearest_i == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L3_error)
+    __pyx_v_current_i = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_current_i == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 175, __pyx_L3_error)
+    __pyx_v_ts_index = ((PyArrayObject *)values[2]);
+    __pyx_v_ts_values = ((PyArrayObject *)values[3]);
+    __pyx_v_t = __Pyx_PyInt_As_long(values[4]); if (unlikely((__pyx_v_t == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
+    __pyx_v_mode = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_mode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("_get_nearest", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 173, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("haggregate.regularize._get_nearest", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_index), __pyx_ptype_5numpy_ndarray, 1, "ts_index", 0))) __PYX_ERR(0, 176, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ts_values), __pyx_ptype_5numpy_ndarray, 1, "ts_values", 0))) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10haggregate_10regularize_6_get_nearest(__pyx_self, __pyx_v_previous_nearest_i, __pyx_v_current_i, __pyx_v_ts_index, __pyx_v_ts_values, __pyx_v_t, __pyx_v_mode);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10haggregate_10regularize_6_get_nearest(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_previous_nearest_i, int __pyx_v_current_i, PyArrayObject *__pyx_v_ts_index, CYTHON_UNUSED PyArrayObject *__pyx_v_ts_values, long __pyx_v_t, int __pyx_v_mode) {
+  PyObject *__pyx_v_current_distance = NULL;
+  PyObject *__pyx_v_previous_distance = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_TraceDeclarations
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_TraceFrameInit(__pyx_codeobj__8)
+  __Pyx_RefNannySetupContext("_get_nearest", 0);
+  __Pyx_TraceCall("_get_nearest", __pyx_f[0], 173, 0, __PYX_ERR(0, 173, __pyx_L1_error));
+
+  /* "haggregate/regularize.pyx":181
+ *     int mode,
+ * ):
+ *     if mode == RM.INTERVAL.value:             # <<<<<<<<<<<<<<
+ *         # In that case it doesn't really matter which is the nearest, so long as it's
+ *         # only one (which is checked elsewhere), so we return immediately.
+ */
+  __Pyx_TraceLine(181,0,__PYX_ERR(0, 181, __pyx_L1_error))
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INTERVAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__pyx_t_4) {
+
+    /* "haggregate/regularize.pyx":184
+ *         # In that case it doesn't really matter which is the nearest, so long as it's
+ *         # only one (which is checked elsewhere), so we return immediately.
+ *         return current_i             # <<<<<<<<<<<<<<
+ *     if previous_nearest_i < 0:
+ *         return current_i
+ */
+    __Pyx_TraceLine(184,0,__PYX_ERR(0, 184, __pyx_L1_error))
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_current_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "haggregate/regularize.pyx":181
+ *     int mode,
+ * ):
+ *     if mode == RM.INTERVAL.value:             # <<<<<<<<<<<<<<
+ *         # In that case it doesn't really matter which is the nearest, so long as it's
+ *         # only one (which is checked elsewhere), so we return immediately.
+ */
+  }
+
+  /* "haggregate/regularize.pyx":185
+ *         # only one (which is checked elsewhere), so we return immediately.
+ *         return current_i
+ *     if previous_nearest_i < 0:             # <<<<<<<<<<<<<<
+ *         return current_i
+ *     current_distance = abs(t - ts_index[current_i])
+ */
+  __Pyx_TraceLine(185,0,__PYX_ERR(0, 185, __pyx_L1_error))
+  __pyx_t_4 = ((__pyx_v_previous_nearest_i < 0) != 0);
+  if (__pyx_t_4) {
+
+    /* "haggregate/regularize.pyx":186
+ *         return current_i
+ *     if previous_nearest_i < 0:
+ *         return current_i             # <<<<<<<<<<<<<<
+ *     current_distance = abs(t - ts_index[current_i])
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])
+ */
+    __Pyx_TraceLine(186,0,__PYX_ERR(0, 186, __pyx_L1_error))
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_current_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "haggregate/regularize.pyx":185
+ *         # only one (which is checked elsewhere), so we return immediately.
+ *         return current_i
+ *     if previous_nearest_i < 0:             # <<<<<<<<<<<<<<
+ *         return current_i
+ *     current_distance = abs(t - ts_index[current_i])
+ */
+  }
+
+  /* "haggregate/regularize.pyx":187
+ *     if previous_nearest_i < 0:
+ *         return current_i
+ *     current_distance = abs(t - ts_index[current_i])             # <<<<<<<<<<<<<<
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])
+ *     if current_distance < previous_distance:
+ */
+  __Pyx_TraceLine(187,0,__PYX_ERR(0, 187, __pyx_L1_error))
+  __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_current_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_current_distance = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "haggregate/regularize.pyx":188
+ *         return current_i
+ *     current_distance = abs(t - ts_index[current_i])
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])             # <<<<<<<<<<<<<<
+ *     if current_distance < previous_distance:
+ *         return current_i
+ */
+  __Pyx_TraceLine(188,0,__PYX_ERR(0, 188, __pyx_L1_error))
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_t); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_ts_index), __pyx_v_previous_nearest_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyNumber_Absolute(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_previous_distance = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "haggregate/regularize.pyx":189
+ *     current_distance = abs(t - ts_index[current_i])
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])
+ *     if current_distance < previous_distance:             # <<<<<<<<<<<<<<
+ *         return current_i
+ *     else:
+ */
+  __Pyx_TraceLine(189,0,__PYX_ERR(0, 189, __pyx_L1_error))
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_current_distance, __pyx_v_previous_distance, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_4) {
+
+    /* "haggregate/regularize.pyx":190
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])
+ *     if current_distance < previous_distance:
+ *         return current_i             # <<<<<<<<<<<<<<
+ *     else:
+ *         return previous_nearest_i
+ */
+    __Pyx_TraceLine(190,0,__PYX_ERR(0, 190, __pyx_L1_error))
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_current_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+
+    /* "haggregate/regularize.pyx":189
+ *     current_distance = abs(t - ts_index[current_i])
+ *     previous_distance = abs(t - ts_index[previous_nearest_i])
+ *     if current_distance < previous_distance:             # <<<<<<<<<<<<<<
+ *         return current_i
+ *     else:
+ */
+  }
+
+  /* "haggregate/regularize.pyx":192
+ *         return current_i
+ *     else:
+ *         return previous_nearest_i             # <<<<<<<<<<<<<<
+ */
+  __Pyx_TraceLine(192,0,__PYX_ERR(0, 192, __pyx_L1_error))
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_previous_nearest_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "haggregate/regularize.pyx":173
+ * 
+ * 
+ * def _get_nearest(             # <<<<<<<<<<<<<<
+ *     int previous_nearest_i,
+ *     int current_i,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("haggregate.regularize._get_nearest", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_current_distance);
+  __Pyx_XDECREF(__pyx_v_previous_distance);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_TraceReturn(__pyx_r, 0);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4692,30 +5368,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[1], 734, 0, __PYX_ERR(1, 734, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_TraceLine(735,0,__PYX_ERR(1, 735, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4727,15 +5403,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4746,30 +5422,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[1], 737, 0, __PYX_ERR(1, 737, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_TraceLine(738,0,__PYX_ERR(1, 738, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4781,15 +5457,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4800,30 +5476,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[1], 740, 0, __PYX_ERR(1, 740, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_TraceLine(741,0,__PYX_ERR(1, 741, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4835,15 +5511,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4854,30 +5530,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[1], 743, 0, __PYX_ERR(1, 743, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_TraceLine(744,0,__PYX_ERR(1, 744, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4889,15 +5565,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4908,30 +5584,30 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[1], 746, 0, __PYX_ERR(1, 746, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_TraceLine(747,0,__PYX_ERR(1, 747, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4943,15 +5619,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -4962,63 +5638,63 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[1], 749, 0, __PYX_ERR(1, 749, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __Pyx_TraceLine(750,0,__PYX_ERR(1, 750, __pyx_L1_error))
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_TraceLine(751,0,__PYX_ERR(1, 751, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(753,0,__PYX_ERR(1, 753, __pyx_L1_error))
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -5029,15 +5705,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -5046,35 +5722,35 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[1], 928, 0, __PYX_ERR(1, 928, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   __Pyx_TraceLine(929,0,__PYX_ERR(1, 929, __pyx_L1_error))
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __Pyx_TraceLine(930,0,__PYX_ERR(1, 930, __pyx_L1_error))
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -5083,15 +5759,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -5103,70 +5779,70 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[1], 932, 0, __PYX_ERR(1, 932, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __Pyx_TraceLine(933,0,__PYX_ERR(1, 933, __pyx_L1_error))
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __Pyx_TraceLine(934,0,__PYX_ERR(1, 934, __pyx_L1_error))
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_TraceLine(935,0,__PYX_ERR(1, 935, __pyx_L1_error))
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_TraceLine(936,0,__PYX_ERR(1, 936, __pyx_L1_error))
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -5177,15 +5853,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5203,15 +5879,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[1], 940, 0, __PYX_ERR(1, 940, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   __Pyx_TraceLine(941,0,__PYX_ERR(1, 941, __pyx_L1_error))
@@ -5220,39 +5896,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __Pyx_TraceLine(942,0,__PYX_ERR(1, 942, __pyx_L3_error))
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __Pyx_TraceLine(943,0,__PYX_ERR(1, 943, __pyx_L5_except_error))
@@ -5260,47 +5936,47 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __Pyx_TraceLine(944,0,__PYX_ERR(1, 944, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5316,15 +5992,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5342,15 +6018,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[1], 946, 0, __PYX_ERR(1, 946, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   __Pyx_TraceLine(947,0,__PYX_ERR(1, 947, __pyx_L1_error))
@@ -5359,39 +6035,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __Pyx_TraceLine(948,0,__PYX_ERR(1, 948, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __Pyx_TraceLine(949,0,__PYX_ERR(1, 949, __pyx_L5_except_error))
@@ -5399,47 +6075,47 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __Pyx_TraceLine(950,0,__PYX_ERR(1, 950, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5455,15 +6131,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5481,15 +6157,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[1], 952, 0, __PYX_ERR(1, 952, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   __Pyx_TraceLine(953,0,__PYX_ERR(1, 953, __pyx_L1_error))
@@ -5498,39 +6174,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __Pyx_TraceLine(954,0,__PYX_ERR(1, 954, __pyx_L3_error))
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __Pyx_TraceLine(955,0,__PYX_ERR(1, 955, __pyx_L5_except_error))
@@ -5538,47 +6214,47 @@
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __Pyx_TraceLine(956,0,__PYX_ERR(1, 956, __pyx_L5_except_error))
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5594,15 +6270,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -5612,26 +6288,26 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[1], 966, 0, __PYX_ERR(1, 966, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(978,0,__PYX_ERR(1, 978, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -5641,15 +6317,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -5659,26 +6335,26 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[1], 981, 0, __PYX_ERR(1, 981, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(993,0,__PYX_ERR(1, 993, __pyx_L1_error))
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -5688,15 +6364,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -5704,26 +6380,26 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[1], 996, 1, __PYX_ERR(1, 996, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(1003,1,__PYX_ERR(1, 1003, __pyx_L1_error))
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -5732,15 +6408,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -5748,26 +6424,26 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[1], 1006, 1, __PYX_ERR(1, 1006, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_TraceLine(1010,1,__PYX_ERR(1, 1010, __pyx_L1_error))
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -5776,15 +6452,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5792,24 +6468,24 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[1], 1013, 1, __PYX_ERR(1, 1013, __pyx_L1_error));
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __Pyx_TraceLine(1017,1,__PYX_ERR(1, 1017, __pyx_L1_error))
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5868,76 +6544,88 @@
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_Created_by_regularizing_step_of, __pyx_k_Created_by_regularizing_step_of, sizeof(__pyx_k_Created_by_regularizing_step_of), 0, 1, 0, 0},
   {&__pyx_n_u_DATEINSERT, __pyx_k_DATEINSERT, sizeof(__pyx_k_DATEINSERT), 0, 1, 0, 1},
   {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
   {&__pyx_n_s_HTimeseries, __pyx_k_HTimeseries, sizeof(__pyx_k_HTimeseries), 0, 0, 1, 1},
+  {&__pyx_n_s_INSTANTANEOUS, __pyx_k_INSTANTANEOUS, sizeof(__pyx_k_INSTANTANEOUS), 0, 0, 1, 1},
+  {&__pyx_n_s_INTERVAL, __pyx_k_INTERVAL, sizeof(__pyx_k_INTERVAL), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+  {&__pyx_n_s_RM, __pyx_k_RM, sizeof(__pyx_k_RM), 0, 0, 1, 1},
+  {&__pyx_n_s_RegularizationMode, __pyx_k_RegularizationMode, sizeof(__pyx_k_RegularizationMode), 0, 0, 1, 1},
   {&__pyx_n_s_RegularizeError, __pyx_k_RegularizeError, sizeof(__pyx_k_RegularizeError), 0, 0, 1, 1},
   {&__pyx_kp_u_Regularized, __pyx_k_Regularized, sizeof(__pyx_k_Regularized), 0, 1, 0, 0},
   {&__pyx_kp_u_The_source_time_series_does_not, __pyx_k_The_source_time_series_does_not, sizeof(__pyx_k_The_source_time_series_does_not), 0, 1, 0, 0},
   {&__pyx_kp_u_The_time_step_is_malformed_or_is, __pyx_k_The_time_step_is_malformed_or_is, sizeof(__pyx_k_The_time_step_is_malformed_or_is), 0, 1, 0, 0},
   {&__pyx_n_s_Timedelta, __pyx_k_Timedelta, sizeof(__pyx_k_Timedelta), 0, 0, 1, 1},
   {&__pyx_n_u_U, __pyx_k_U, sizeof(__pyx_k_U), 0, 1, 0, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
+  {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+  {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
   {&__pyx_n_s_astype, __pyx_k_astype, sizeof(__pyx_k_astype), 0, 0, 1, 1},
   {&__pyx_n_s_attr, __pyx_k_attr, sizeof(__pyx_k_attr), 0, 0, 1, 1},
   {&__pyx_n_s_attrs, __pyx_k_attrs, sizeof(__pyx_k_attrs), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_comment, __pyx_k_comment, sizeof(__pyx_k_comment), 0, 0, 1, 1},
   {&__pyx_n_u_comment, __pyx_k_comment, sizeof(__pyx_k_comment), 0, 1, 0, 1},
   {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
+  {&__pyx_n_s_current_distance, __pyx_k_current_distance, sizeof(__pyx_k_current_distance), 0, 0, 1, 1},
+  {&__pyx_n_s_current_i, __pyx_k_current_i, sizeof(__pyx_k_current_i), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_date_range, __pyx_k_date_range, sizeof(__pyx_k_date_range), 0, 0, 1, 1},
   {&__pyx_n_s_datetime, __pyx_k_datetime, sizeof(__pyx_k_datetime), 0, 0, 1, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_dt, __pyx_k_dt, sizeof(__pyx_k_dt), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_first_timestamp_of_result, __pyx_k_first_timestamp_of_result, sizeof(__pyx_k_first_timestamp_of_result), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_u_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 1, 0, 1},
   {&__pyx_n_s_flags_dtype, __pyx_k_flags_dtype, sizeof(__pyx_k_flags_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_found, __pyx_k_found, sizeof(__pyx_k_found), 0, 0, 1, 1},
   {&__pyx_n_s_freq, __pyx_k_freq, sizeof(__pyx_k_freq), 0, 0, 1, 1},
   {&__pyx_n_s_full, __pyx_k_full, sizeof(__pyx_k_full), 0, 0, 1, 1},
+  {&__pyx_n_s_get_nearest, __pyx_k_get_nearest, sizeof(__pyx_k_get_nearest), 0, 0, 1, 1},
   {&__pyx_n_s_get_record, __pyx_k_get_record, sizeof(__pyx_k_get_record), 0, 0, 1, 1},
+  {&__pyx_n_s_haggregate, __pyx_k_haggregate, sizeof(__pyx_k_haggregate), 0, 0, 1, 1},
   {&__pyx_n_s_haggregate_regularize, __pyx_k_haggregate_regularize, sizeof(__pyx_k_haggregate_regularize), 0, 0, 1, 1},
   {&__pyx_kp_s_haggregate_regularize_pyx, __pyx_k_haggregate_regularize_pyx, sizeof(__pyx_k_haggregate_regularize_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_htimeseries, __pyx_k_htimeseries, sizeof(__pyx_k_htimeseries), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_u_interval_type, __pyx_k_interval_type, sizeof(__pyx_k_interval_type), 0, 1, 0, 1},
   {&__pyx_n_s_last_timestamp_of_result, __pyx_k_last_timestamp_of_result, sizeof(__pyx_k_last_timestamp_of_result), 0, 0, 1, 1},
   {&__pyx_n_s_len, __pyx_k_len, sizeof(__pyx_k_len), 0, 0, 1, 1},
   {&__pyx_n_u_location, __pyx_k_location, sizeof(__pyx_k_location), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_max, __pyx_k_max, sizeof(__pyx_k_max), 0, 0, 1, 1},
   {&__pyx_n_s_max_flags_length, __pyx_k_max_flags_length, sizeof(__pyx_k_max_flags_length), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
+  {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
+  {&__pyx_n_s_nearest_i, __pyx_k_nearest_i, sizeof(__pyx_k_nearest_i), 0, 0, 1, 1},
   {&__pyx_n_s_new_date_flag, __pyx_k_new_date_flag, sizeof(__pyx_k_new_date_flag), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
   {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
   {&__pyx_n_s_pandas_tseries_frequencies, __pyx_k_pandas_tseries_frequencies, sizeof(__pyx_k_pandas_tseries_frequencies), 0, 0, 1, 1},
   {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
   {&__pyx_n_s_perform_regularization, __pyx_k_perform_regularization, sizeof(__pyx_k_perform_regularization), 0, 0, 1, 1},
   {&__pyx_n_u_precision, __pyx_k_precision, sizeof(__pyx_k_precision), 0, 1, 0, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+  {&__pyx_n_s_previous_distance, __pyx_k_previous_distance, sizeof(__pyx_k_previous_distance), 0, 0, 1, 1},
+  {&__pyx_n_s_previous_nearest_i, __pyx_k_previous_nearest_i, sizeof(__pyx_k_previous_nearest_i), 0, 0, 1, 1},
   {&__pyx_n_s_previous_pos, __pyx_k_previous_pos, sizeof(__pyx_k_previous_pos), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_regularize, __pyx_k_regularize, sizeof(__pyx_k_regularize), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
   {&__pyx_n_s_result_flags, __pyx_k_result_flags, sizeof(__pyx_k_result_flags), 0, 0, 1, 1},
   {&__pyx_n_s_result_index, __pyx_k_result_index, sizeof(__pyx_k_result_index), 0, 0, 1, 1},
@@ -5946,14 +6634,15 @@
   {&__pyx_n_s_round, __pyx_k_round, sizeof(__pyx_k_round), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
   {&__pyx_n_s_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_ti, __pyx_k_ti, sizeof(__pyx_k_ti), 0, 0, 1, 1},
   {&__pyx_n_s_time_step, __pyx_k_time_step, sizeof(__pyx_k_time_step), 0, 0, 1, 1},
   {&__pyx_n_u_time_step, __pyx_k_time_step, sizeof(__pyx_k_time_step), 0, 1, 0, 1},
   {&__pyx_n_s_timedelta64, __pyx_k_timedelta64, sizeof(__pyx_k_timedelta64), 0, 0, 1, 1},
   {&__pyx_n_s_timezone, __pyx_k_timezone, sizeof(__pyx_k_timezone), 0, 0, 1, 1},
   {&__pyx_n_u_timezone, __pyx_k_timezone, sizeof(__pyx_k_timezone), 0, 1, 0, 1},
   {&__pyx_n_s_title, __pyx_k_title, sizeof(__pyx_k_title), 0, 0, 1, 1},
   {&__pyx_n_u_title, __pyx_k_title, sizeof(__pyx_k_title), 0, 1, 0, 1},
@@ -5973,96 +6662,108 @@
   {&__pyx_n_u_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 1, 0, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_u_variable, __pyx_k_variable, sizeof(__pyx_k_variable), 0, 1, 0, 1},
   {&__pyx_n_s_vstack, __pyx_k_vstack, sizeof(__pyx_k_vstack), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 22, __pyx_L1_error)
-  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 69, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_max = __Pyx_GetBuiltinName(__pyx_n_s_max); if (!__pyx_builtin_max) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 111, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "haggregate/regularize.pyx":31
+  /* "haggregate/regularize.pyx":34
  *     result = HTimeseries()
  *     attrs = (
  *         "unit",             # <<<<<<<<<<<<<<
  *         "timezone",
  *         "time_step",
  */
-  __pyx_tuple__2 = PyTuple_Pack(7, __pyx_n_u_unit, __pyx_n_u_timezone, __pyx_n_u_time_step, __pyx_n_u_interval_type, __pyx_n_u_variable, __pyx_n_u_precision, __pyx_n_u_location); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__3 = PyTuple_Pack(7, __pyx_n_u_unit, __pyx_n_u_timezone, __pyx_n_u_time_step, __pyx_n_u_interval_type, __pyx_n_u_variable, __pyx_n_u_precision, __pyx_n_u_location); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "haggregate/regularize.pyx":16
+  /* "haggregate/regularize.pyx":19
  * 
  * 
- * def regularize(ts, new_date_flag="DATEINSERT"):             # <<<<<<<<<<<<<<
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):             # <<<<<<<<<<<<<<
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):
  */
-  __pyx_tuple__9 = PyTuple_Pack(17, __pyx_n_s_ts, __pyx_n_s_new_date_flag, __pyx_n_s_result, __pyx_n_s_attrs, __pyx_n_s_attr, __pyx_n_s_step, __pyx_n_s_first_timestamp_of_result, __pyx_n_s_last_timestamp_of_result, __pyx_n_s_max_flags_length, __pyx_n_s_flags_dtype, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_result_step, __pyx_n_s_result_index, __pyx_n_s_result_values, __pyx_n_s_result_flags); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(2, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_regularize, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(18, __pyx_n_s_ts, __pyx_n_s_new_date_flag, __pyx_n_s_mode, __pyx_n_s_result, __pyx_n_s_attrs, __pyx_n_s_attr, __pyx_n_s_step, __pyx_n_s_first_timestamp_of_result, __pyx_n_s_last_timestamp_of_result, __pyx_n_s_max_flags_length, __pyx_n_s_flags_dtype, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_result_step, __pyx_n_s_result_index, __pyx_n_s_result_values, __pyx_n_s_result_flags); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_regularize, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 19, __pyx_L1_error)
 
-  /* "haggregate/regularize.pyx":92
+  /* "haggregate/regularize.pyx":96
  * 
  * 
  * def _perform_regularization(             # <<<<<<<<<<<<<<
  *     np.ndarray result_index,
  *     np.ndarray result_values,
  */
-  __pyx_tuple__10 = PyTuple_Pack(11, __pyx_n_s_result_index, __pyx_n_s_result_values, __pyx_n_s_result_flags, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_result_step, __pyx_n_s_new_date_flag, __pyx_n_s_i, __pyx_n_s_previous_pos, __pyx_n_s_t); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(8, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_perform_regularization, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(12, __pyx_n_s_result_index, __pyx_n_s_result_values, __pyx_n_s_result_flags, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_result_step, __pyx_n_s_new_date_flag, __pyx_n_s_mode, __pyx_n_s_i, __pyx_n_s_previous_pos, __pyx_n_s_t); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(9, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_perform_regularization, 96, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 96, __pyx_L1_error)
 
-  /* "haggregate/regularize.pyx":113
+  /* "haggregate/regularize.pyx":125
  * 
  * 
  * def _get_record(             # <<<<<<<<<<<<<<
  *     np.ndarray ts_index,
  *     np.ndarray ts_values,
  */
-  __pyx_tuple__11 = PyTuple_Pack(14, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_t, __pyx_n_s_result_step, __pyx_n_s_new_date_flag, __pyx_n_s_previous_pos, __pyx_n_s_i, __pyx_n_s_found, __pyx_n_s_count, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_value, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(7, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_get_record, 113, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(19, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_ts_flags, __pyx_n_s_t, __pyx_n_s_result_step, __pyx_n_s_new_date_flag, __pyx_n_s_previous_pos, __pyx_n_s_mode, __pyx_n_s_i, __pyx_n_s_found, __pyx_n_s_count, __pyx_n_s_nearest_i, __pyx_n_s_INTERVAL, __pyx_n_s_INSTANTANEOUS, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_ti, __pyx_n_s_value, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(8, 0, 19, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_get_record, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 125, __pyx_L1_error)
+
+  /* "haggregate/regularize.pyx":173
+ * 
+ * 
+ * def _get_nearest(             # <<<<<<<<<<<<<<
+ *     int previous_nearest_i,
+ *     int current_i,
+ */
+  __pyx_tuple__14 = PyTuple_Pack(8, __pyx_n_s_previous_nearest_i, __pyx_n_s_current_i, __pyx_n_s_ts_index, __pyx_n_s_ts_values, __pyx_n_s_t, __pyx_n_s_mode, __pyx_n_s_current_distance, __pyx_n_s_previous_distance); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(6, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_haggregate_regularize_pyx, __pyx_n_s_get_nearest, 173, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6423,28 +7124,28 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "haggregate/regularize.pyx":7
  * cimport numpy as np
  * import numpy as np
  * import pandas as pd             # <<<<<<<<<<<<<<
  * from htimeseries import HTimeseries
- * from pandas.tseries.frequencies import to_offset
+ * from libc.math cimport isnan
  */
   __Pyx_TraceLine(7,0,__PYX_ERR(0, 7, __pyx_L1_error))
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "haggregate/regularize.pyx":8
  * import numpy as np
  * import pandas as pd
  * from htimeseries import HTimeseries             # <<<<<<<<<<<<<<
+ * from libc.math cimport isnan
  * from pandas.tseries.frequencies import to_offset
- * 
  */
   __Pyx_TraceLine(8,0,__PYX_ERR(0, 8, __pyx_L1_error))
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_HTimeseries);
   __Pyx_GIVEREF(__pyx_n_s_HTimeseries);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_HTimeseries);
@@ -6453,262 +7154,305 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_HTimeseries); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_HTimeseries, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "haggregate/regularize.pyx":9
- * import pandas as pd
+  /* "haggregate/regularize.pyx":10
  * from htimeseries import HTimeseries
+ * from libc.math cimport isnan
  * from pandas.tseries.frequencies import to_offset             # <<<<<<<<<<<<<<
  * 
- * 
+ * from .haggregate import RegularizationMode as RM
  */
-  __Pyx_TraceLine(9,0,__PYX_ERR(0, 9, __pyx_L1_error))
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_TraceLine(10,0,__PYX_ERR(0, 10, __pyx_L1_error))
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_to_offset);
   __Pyx_GIVEREF(__pyx_n_s_to_offset);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_offset);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas_tseries_frequencies, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas_tseries_frequencies, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_to_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_to_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_offset, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_offset, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "haggregate/regularize.pyx":12
+ * from pandas.tseries.frequencies import to_offset
  * 
+ * from .haggregate import RegularizationMode as RM             # <<<<<<<<<<<<<<
  * 
- * class RegularizeError(Exception):             # <<<<<<<<<<<<<<
- *     pass
  * 
  */
   __Pyx_TraceLine(12,0,__PYX_ERR(0, 12, __pyx_L1_error))
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_RegularizationMode);
+  __Pyx_GIVEREF(__pyx_n_s_RegularizationMode);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_RegularizationMode);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_haggregate, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_RegularizationMode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RM, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "haggregate/regularize.pyx":15
+ * 
+ * 
+ * class RegularizeError(Exception):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+  __Pyx_TraceLine(15,0,__PYX_ERR(0, 15, __pyx_L1_error))
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_RegularizeError, __pyx_n_s_RegularizeError, (PyObject *) NULL, __pyx_n_s_haggregate_regularize, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_RegularizeError, __pyx_n_s_RegularizeError, (PyObject *) NULL, __pyx_n_s_haggregate_regularize, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RegularizeError, __pyx_t_1, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_RegularizeError, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RegularizeError, __pyx_t_4) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RegularizeError, __pyx_t_4) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "haggregate/regularize.pyx":16
+  /* "haggregate/regularize.pyx":19
  * 
  * 
- * def regularize(ts, new_date_flag="DATEINSERT"):             # <<<<<<<<<<<<<<
+ * def regularize(ts, new_date_flag="DATEINSERT", mode=RM.INTERVAL):             # <<<<<<<<<<<<<<
  *     # Sanity checks
  *     if not hasattr(ts, "time_step"):
  */
-  __Pyx_TraceLine(16,0,__PYX_ERR(0, 16, __pyx_L1_error))
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_1regularize, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_TraceLine(19,0,__PYX_ERR(0, 19, __pyx_L1_error))
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INTERVAL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_regularize, __pyx_t_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_k_ = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_1regularize, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_regularize, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "haggregate/regularize.pyx":92
+  /* "haggregate/regularize.pyx":96
  * 
  * 
  * def _perform_regularization(             # <<<<<<<<<<<<<<
  *     np.ndarray result_index,
  *     np.ndarray result_values,
  */
-  __Pyx_TraceLine(92,0,__PYX_ERR(0, 92, __pyx_L1_error))
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_3_perform_regularization, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_TraceLine(96,0,__PYX_ERR(0, 96, __pyx_L1_error))
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_3_perform_regularization, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_perform_regularization, __pyx_t_1) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_perform_regularization, __pyx_t_1) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "haggregate/regularize.pyx":113
+  /* "haggregate/regularize.pyx":125
  * 
  * 
  * def _get_record(             # <<<<<<<<<<<<<<
  *     np.ndarray ts_index,
  *     np.ndarray ts_values,
  */
-  __Pyx_TraceLine(113,0,__PYX_ERR(0, 113, __pyx_L1_error))
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_5_get_record, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_TraceLine(125,0,__PYX_ERR(0, 125, __pyx_L1_error))
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_5_get_record, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_record, __pyx_t_1) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "haggregate/regularize.pyx":173
+ * 
+ * 
+ * def _get_nearest(             # <<<<<<<<<<<<<<
+ *     int previous_nearest_i,
+ *     int current_i,
+ */
+  __Pyx_TraceLine(173,0,__PYX_ERR(0, 173, __pyx_L1_error))
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10haggregate_10regularize_7_get_nearest, NULL, __pyx_n_s_haggregate_regularize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_record, __pyx_t_1) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_nearest, __pyx_t_1) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "haggregate/regularize.pyx":1
  * # cython: language_level=3, linetrace=True             # <<<<<<<<<<<<<<
  * # distutils: define_macros=CYTHON_TRACE=1
  * 
  */
   __Pyx_TraceLine(1,0,__PYX_ERR(0, 1, __pyx_L1_error))
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
   __Pyx_TraceLine(734,0,__PYX_ERR(1, 734, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
   __Pyx_TraceLine(737,0,__PYX_ERR(1, 737, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
   __Pyx_TraceLine(740,0,__PYX_ERR(1, 740, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
   __Pyx_TraceLine(743,0,__PYX_ERR(1, 743, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
   __Pyx_TraceLine(746,0,__PYX_ERR(1, 746, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
   __Pyx_TraceLine(749,0,__PYX_ERR(1, 749, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
   __Pyx_TraceLine(928,0,__PYX_ERR(1, 928, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
   __Pyx_TraceLine(932,0,__PYX_ERR(1, 932, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
   __Pyx_TraceLine(940,0,__PYX_ERR(1, 940, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
   __Pyx_TraceLine(946,0,__PYX_ERR(1, 946, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
   __Pyx_TraceLine(952,0,__PYX_ERR(1, 952, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
   __Pyx_TraceLine(966,0,__PYX_ERR(1, 966, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
   __Pyx_TraceLine(981,0,__PYX_ERR(1, 981, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
   __Pyx_TraceLine(996,0,__PYX_ERR(1, 996, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
   __Pyx_TraceLine(1006,0,__PYX_ERR(1, 1006, __pyx_L1_error))
 
 
-  /* "../../../virtualenvs/rocc/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../../usr/lib/python3/dist-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
   __Pyx_TraceLine(1013,0,__PYX_ERR(1, 1013, __pyx_L1_error))
@@ -7705,15 +8449,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -8113,14 +8857,34 @@
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
+/* py_abs */
+#if CYTHON_USE_PYLONG_INTERNALS
+static PyObject *__Pyx_PyLong_AbsNeg(PyObject *n) {
+    if (likely(Py_SIZE(n) == -1)) {
+        return PyLong_FromLong(((PyLongObject*)n)->ob_digit[0]);
+    }
+#if CYTHON_COMPILING_IN_CPYTHON
+    {
+        PyObject *copy = _PyLong_Copy((PyLongObject*)n);
+        if (likely(copy)) {
+            __Pyx_SET_SIZE(copy, -Py_SIZE(copy));
+        }
+        return copy;
+    }
+#else
+    return PyNumber_Negative(n);
+#endif
+}
+#endif
+
 /* WriteUnraisableException */
 static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
                                   CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
                                   int full_traceback, CYTHON_UNUSED int nogil) {
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
```

### Comparing `haggregate-3.0.3/haggregate.egg-info/PKG-INFO` & `haggregate-3.1.0/haggregate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haggregate
-Version: 3.0.3
+Version: 3.1.0
 Summary: Aggregates htimeseries to larger steps
 Home-page: https://github.com/openmeteo/haggregate
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: haggregate
 Classifier: Development Status :: 4 - Beta
@@ -46,14 +46,20 @@
 * Documentation: https://haggregate.readthedocs.io.
 
 
 =======
 History
 =======
 
+3.1.0 (2024-04-18)
+==================
+
+- Use different regularization modes for interval and instantaneous
+  variables.
+
 3.0.3 (2024-04-16)
 ==================
 
 - Allow htimeseries 7.
 
 3.0.2 (2023-12-20)
 ==================
```

### Comparing `haggregate-3.0.3/setup.py` & `haggregate-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.3/tests/test_cli.py` & `haggregate-3.1.0/tests/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime as dt
 import textwrap
 from unittest import TestCase
 from unittest.mock import patch
 
 from click.testing import CliRunner
 
-from haggregate import cli
+from haggregate import RegularizationMode, cli
 
 
 class CliUsageErrorTestCase(TestCase):
     def setUp(self):
         runner = CliRunner()
         self.result = runner.invoke(cli.main, [])
 
@@ -56,15 +56,15 @@
         self.assertIn("No time series have been specified", self.result.output)
 
 
 class CliMixin:
     @patch("haggregate.cli.HTimeseries", **{"return_value": "my timeseries"})
     @patch("haggregate.cli.regularize", return_value="regularized timeseries")
     @patch("haggregate.cli.aggregate")
-    def setUp(self, mock_aggregate, mock_regularize, mock_htimeseries):
+    def _execute(self, mock_aggregate, mock_regularize, mock_htimeseries):
         self.mock_aggregate = mock_aggregate
         self.mock_regularize = mock_regularize
         self.mock_htimeseries = mock_htimeseries
         runner = CliRunner()
         with runner.isolated_filesystem():
             with open("config.ini", "w") as f:
                 f.write(self.configuration)
@@ -83,14 +83,17 @@
         [MyTimeseries]
         source_file = mytimeseries.hts
         target_file = aggregatedtimeseries.hts
         method = sum
         """
     )
 
+    def setUp(self):
+        self._execute()
+
     def test_exit_code(self):
         self.assertEqual(self.result.exit_code, 0)
 
     def test_read_source_file(self):
         self.assertEqual(self.mock_htimeseries.call_count, 1)
 
     def test_htimeseries_called_correctly(self):
@@ -98,15 +101,17 @@
         self.assertEqual(
             self.mock_htimeseries.call_args[1],
             {"format": self.mock_htimeseries.FILE, "default_tzinfo": dt.timezone.utc},
         )
 
     def test_regularize_called_correctly(self):
         self.mock_regularize.assert_called_once_with(
-            "my timeseries", new_date_flag="DATEINSERT"
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INTERVAL,
         )
 
     def test_aggregate_called_correctly(self):
         self.mock_aggregate.assert_called_once_with(
             "regularized timeseries",
             "D",
             "sum",
@@ -115,14 +120,64 @@
             target_timestamp_offset=None,
         )
 
     def test_wrote_target_file(self):
         self.assertEqual(self.mock_aggregate.return_value.write.call_count, 1)
 
 
+class RegularizationModeTestCase(CliMixin, TestCase):
+    def _run(self, method):
+        self.configuration = textwrap.dedent(
+            f"""\
+            [General]
+            target_step = D
+            min_count = 10
+            missing_flag = MISSING
+
+            [MyTimeseries]
+            source_file = mytimeseries.hts
+            target_file = aggregatedtimeseries.hts
+            method = {method}
+            """
+        )
+        self._execute()
+
+    def test_regularize_called_correctly_when_sum(self):
+        self._run("sum")
+        self.mock_regularize.assert_called_once_with(
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INTERVAL,
+        )
+
+    def test_regularize_called_correctly_when_mean(self):
+        self._run("mean")
+        self.mock_regularize.assert_called_once_with(
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INSTANTANEOUS,
+        )
+
+    def test_regularize_called_correctly_when_max(self):
+        self._run("max")
+        self.mock_regularize.assert_called_once_with(
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INTERVAL,
+        )
+
+    def test_regularize_called_correctly_when_min(self):
+        self._run("min")
+        self.mock_regularize.assert_called_once_with(
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INTERVAL,
+        )
+
+
 class CliWithTargetTimestampOffsetTestCase(CliMixin, TestCase):
     configuration = textwrap.dedent(
         """\
         [General]
         target_step = D
         target_timestamp_offset = 1min
         min_count = 10
@@ -131,23 +186,28 @@
         [MyTimeseries]
         source_file = mytimeseries.hts
         target_file = aggregatedtimeseries.hts
         method = sum
         """
     )
 
+    def setUp(self):
+        self._execute()
+
     def test_exit_code(self):
         self.assertEqual(self.result.exit_code, 0)
 
     def test_read_source_file(self):
         self.assertEqual(self.mock_htimeseries.call_count, 1)
 
     def test_regularize_called_correctly(self):
         self.mock_regularize.assert_called_once_with(
-            "my timeseries", new_date_flag="DATEINSERT"
+            "my timeseries",
+            new_date_flag="DATEINSERT",
+            mode=RegularizationMode.INTERVAL,
         )
 
     def test_aggregate_called_correctly(self):
         self.mock_aggregate.assert_called_once_with(
             "regularized timeseries",
             "D",
             "sum",
```

### Comparing `haggregate-3.0.3/tests/test_haggregate.py` & `haggregate-3.1.0/tests/test_haggregate.py`

 * *Files identical despite different names*

### Comparing `haggregate-3.0.3/tests/test_regularize.py` & `haggregate-3.1.0/tests/test_regularize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 import datetime as dt
+import math
 import textwrap
 from io import StringIO
 from unittest import TestCase
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     from backports.zoneinfo import ZoneInfo
 
 import numpy as np
 from htimeseries import HTimeseries
 
-from haggregate import RegularizeError, regularize
+from haggregate import RegularizationMode, RegularizeError, regularize
 
 
 class BadTimeStepTestCase(TestCase):
     def test_unspecified_time_step(self):
         ts = HTimeseries()
         msg = "The source time series does not specify a time step"
         with self.assertRaisesRegex(RegularizeError, msg):
-            regularize(ts)
+            regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_malformed_time_step(self):
         ts = HTimeseries()
         ts.time_step = "hello"
         msg = (
             "The time step is malformed or is specified in months. Only time steps "
             "specified in minutes, hours or days are supported."
         )
         with self.assertRaisesRegex(RegularizeError, msg):
-            regularize(ts)
+            regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_malformed_time_step2(self):
         ts = HTimeseries()
         ts.time_step = "5M"
         msg = (
             "The time step is malformed or is specified in months. Only time steps "
             "specified in minutes, hours or days are supported."
         )
         with self.assertRaisesRegex(RegularizeError, msg):
-            regularize(ts)
+            regularize(ts, mode=RegularizationMode.INTERVAL)
 
 
 class RegularizeTestCase(TestCase):
     def setUp(self):
         input = textwrap.dedent(
             """\
             2008-02-07 10:30,10.71,FLAG1
             2008-02-07 10:41,10.93,FLAG2
             2008-02-07 10:50,11.10,
             """
         )
         ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
         ts.time_step = "10min"
-        self.result = regularize(ts)
+        self.result = regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_length(self):
         self.assertEqual(len(self.result.data), 3)
 
     def test_timestamps_are_aware(self):
         self.assertEqual(self.result.data.index[0].utcoffset(), dt.timedelta(hours=2))
 
@@ -98,15 +99,15 @@
             2008-02-07 10:31,10.71,
             2008-02-07 10:40,10.93,
             2008-02-07 10:50,11.10,
             """
         )
         ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
         ts.time_step = "10min"
-        self.result = regularize(ts)
+        self.result = regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_length(self):
         self.assertEqual(len(self.result.data), 3)
 
     def test_value_1(self):
         self.assertAlmostEqual(
             self.result.data.loc["2008-02-07 10:30:00+0200"].value, 10.71
@@ -130,15 +131,15 @@
             2008-02-07 10:30,10.71,
             2008-02-07 10:40,10.93,
             2008-02-07 10:49,11.10,
             """
         )
         ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
         ts.time_step = "10min"
-        self.result = regularize(ts)
+        self.result = regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_length(self):
         self.assertEqual(len(self.result.data), 3)
 
     def test_value_1(self):
         self.assertAlmostEqual(
             self.result.data.loc["2008-02-07 10:30:00+0200"].value, 10.71
@@ -162,15 +163,15 @@
             2008-02-07 10:30,10.71,
             2008-02-07 10:51,11.10,
             2008-02-07 11:00,10.93,
             """
         )
         ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
         ts.time_step = "10min"
-        self.result = regularize(ts)
+        self.result = regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_length(self):
         self.assertEqual(len(self.result.data), 4)
 
     def test_value_1(self):
         self.assertAlmostEqual(
             self.result.data.loc["2008-02-07 10:30:00+0200"].value, 10.71
@@ -192,20 +193,64 @@
         )
 
 
 class RegularizeEmptyTestCase(TestCase):
     def setUp(self):
         ts = HTimeseries()
         ts.time_step = "10min"
-        self.result = regularize(ts)
+        self.result = regularize(ts, mode=RegularizationMode.INTERVAL)
 
     def test_length(self):
         self.assertEqual(len(self.result.data), 0)
 
 
+class RegularizeWithNullRecordTestCase(TestCase):
+    def setUp(self):
+        input = textwrap.dedent(
+            """\
+            2008-02-07 10:30,10.71,FLAG1
+            2008-02-07 10:40,,
+            2008-02-07 10:41,10.93,FLAG2
+            2008-02-07 10:50,11.10,
+            """
+        )
+        self.ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
+        self.ts.time_step = "10min"
+
+    def test_interval(self):
+        result = regularize(self.ts, mode=RegularizationMode.INTERVAL)
+        self.assertTrue(math.isnan(result.data.loc["2008-02-07 10:40"].value))
+
+    def test_instantaneous(self):
+        result = regularize(self.ts, mode=RegularizationMode.INSTANTANEOUS)
+        self.assertAlmostEqual(result.data.loc["2008-02-07 10:40"].value, 10.93)
+
+
+class NearestTestCase(TestCase):
+    def setUp(self):
+        input = textwrap.dedent(
+            """\
+            2008-02-07 10:30,10.71,FLAG1
+            2008-02-07 10:38,11.93,FLAG2
+            2008-02-07 10:41,10.93,FLAG2
+            2008-02-07 10:50,11.10,
+            """
+        )
+        self.ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
+        self.ts.time_step = "10min"
+
+    def test_interval(self):
+        result = regularize(self.ts, mode=RegularizationMode.INTERVAL)
+        self.assertTrue(math.isnan(result.data.loc["2008-02-07 10:40"].value))
+
+    def test_instantaneous(self):
+        result = regularize(self.ts, mode=RegularizationMode.INSTANTANEOUS)
+        self.assertAlmostEqual(result.data.loc["2008-02-07 10:40"].value, 10.93)
+
+
 class SetsMetadataTestCase(TestCase):
     def setUp(self):
         input = textwrap.dedent(
             """\
             2008-02-07 10:30,10.71,FLAG1
             2008-02-07 10:41,10.93,FLAG2
             2008-02-07 10:50,11.10,
@@ -213,15 +258,15 @@
         )
         self.ts = HTimeseries(StringIO(input), default_tzinfo=ZoneInfo("Etc/GMT-2"))
         self.ts.time_step = "10min"
         self.ts.title = "hello"
         self.ts.precision = 1
         self.ts.comment = "world"
         self.ts.timezone = "EET (+0200)"
-        self.result = regularize(self.ts)
+        self.result = regularize(self.ts, mode=RegularizationMode.INTERVAL)
 
     def test_sets_title(self):
         self.assertEqual(self.result.title, "Regularized hello")
 
     def test_sets_precision(self):
         self.assertEqual(self.result.precision, 1)
```

