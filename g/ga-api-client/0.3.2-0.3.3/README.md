# Comparing `tmp/ga-api-client-0.3.2.tar.gz` & `tmp/ga_api_client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ga-api-client-0.3.2.tar", last modified: Tue Jan 23 00:59:31 2024, max compression
+gzip compressed data, was "ga_api_client-0.3.3.tar", last modified: Thu Apr 18 05:43:23 2024, max compression
```

## Comparing `ga-api-client-0.3.2.tar` & `ga_api_client-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-01-23 00:59:31.401259 ga-api-client-0.3.2/
--rw-r--r--   0 zam       (1001) zam       (1001)     1073 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/LICENSE
--rw-r--r--   0 zam       (1001) zam       (1001)     1044 2024-01-23 00:59:31.401259 ga-api-client-0.3.2/PKG-INFO
--rw-r--r--   0 zam       (1001) zam       (1001)      666 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/README.md
-drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-01-23 00:59:31.401259 ga-api-client-0.3.2/ga_api/
--rw-r--r--   0 zam       (1001) zam       (1001)      149 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/ga_api/__init__.py
--rw-r--r--   0 zam       (1001) zam       (1001)    12131 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/ga_api/field_tree.py
--rw-r--r--   0 zam       (1001) zam       (1001)    43531 2024-01-23 00:57:16.000000 ga-api-client-0.3.2/ga_api/ga_api_client.py
--rw-r--r--   0 zam       (1001) zam       (1001)     1726 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/ga_api/hyper_log_log.py
-drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-01-23 00:59:31.401259 ga-api-client-0.3.2/ga_api_client.egg-info/
--rw-r--r--   0 zam       (1001) zam       (1001)     1044 2024-01-23 00:59:31.000000 ga-api-client-0.3.2/ga_api_client.egg-info/PKG-INFO
--rw-r--r--   0 zam       (1001) zam       (1001)      323 2024-01-23 00:59:31.000000 ga-api-client-0.3.2/ga_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 zam       (1001) zam       (1001)        1 2024-01-23 00:59:31.000000 ga-api-client-0.3.2/ga_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 zam       (1001) zam       (1001)       44 2024-01-23 00:59:31.000000 ga-api-client-0.3.2/ga_api_client.egg-info/requires.txt
--rw-r--r--   0 zam       (1001) zam       (1001)        7 2024-01-23 00:59:31.000000 ga-api-client-0.3.2/ga_api_client.egg-info/top_level.txt
--rw-r--r--   0 zam       (1001) zam       (1001)       84 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/pyproject.toml
--rw-r--r--   0 zam       (1001) zam       (1001)      463 2024-01-23 00:59:31.405259 ga-api-client-0.3.2/setup.cfg
--rw-r--r--   0 zam       (1001) zam       (1001)       67 2024-01-04 03:35:08.000000 ga-api-client-0.3.2/setup.py
+drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-04-18 05:43:23.399331 ga_api_client-0.3.3/
+-rw-r--r--   0 zam       (1001) zam       (1001)     1073 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/LICENSE
+-rw-r--r--   0 zam       (1001) zam       (1001)     1044 2024-04-18 05:43:23.399331 ga_api_client-0.3.3/PKG-INFO
+-rw-r--r--   0 zam       (1001) zam       (1001)      666 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/README.md
+drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-04-18 05:43:23.399331 ga_api_client-0.3.3/ga_api/
+-rw-r--r--   0 zam       (1001) zam       (1001)      149 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/ga_api/__init__.py
+-rw-r--r--   0 zam       (1001) zam       (1001)    12131 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/ga_api/field_tree.py
+-rw-r--r--   0 zam       (1001) zam       (1001)    43545 2024-04-18 05:40:24.000000 ga_api_client-0.3.3/ga_api/ga_api_client.py
+-rw-r--r--   0 zam       (1001) zam       (1001)     1726 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/ga_api/hyper_log_log.py
+drwxr-xr-x   0 zam       (1001) zam       (1001)        0 2024-04-18 05:43:23.399331 ga_api_client-0.3.3/ga_api_client.egg-info/
+-rw-r--r--   0 zam       (1001) zam       (1001)     1044 2024-04-18 05:43:23.000000 ga_api_client-0.3.3/ga_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 zam       (1001) zam       (1001)      323 2024-04-18 05:43:23.000000 ga_api_client-0.3.3/ga_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zam       (1001) zam       (1001)        1 2024-04-18 05:43:23.000000 ga_api_client-0.3.3/ga_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zam       (1001) zam       (1001)       44 2024-04-18 05:43:23.000000 ga_api_client-0.3.3/ga_api_client.egg-info/requires.txt
+-rw-r--r--   0 zam       (1001) zam       (1001)        7 2024-04-18 05:43:23.000000 ga_api_client-0.3.3/ga_api_client.egg-info/top_level.txt
+-rw-r--r--   0 zam       (1001) zam       (1001)       84 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/pyproject.toml
+-rw-r--r--   0 zam       (1001) zam       (1001)      463 2024-04-18 05:43:23.399331 ga_api_client-0.3.3/setup.cfg
+-rw-r--r--   0 zam       (1001) zam       (1001)       67 2024-01-04 03:35:08.000000 ga_api_client-0.3.3/setup.py
```

### Comparing `ga-api-client-0.3.2/LICENSE` & `ga_api_client-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.3.2/PKG-INFO` & `ga_api_client-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-api-client
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.4
```

### Comparing `ga-api-client-0.3.2/README.md` & `ga_api_client-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.3.2/ga_api/field_tree.py` & `ga_api_client-0.3.3/ga_api/field_tree.py`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.3.2/ga_api/ga_api_client.py` & `ga_api_client-0.3.3/ga_api/ga_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,28 +606,28 @@
         self.pipeline = pipeline # pipeline object
         self.pid = await self._tenant.create_adhoc(self.pipeline)
         return self
 
     async def _read_point(self, ts, series, columns=None, refresh=True):
         if refresh:
             await self._tenant.create_adhoc(self.pipeline)
-        freq_str = f"{self.freq}S"
+        freq_str = f"{self.freq}sec"
         delta = pd.Timedelta(freq_str)
         start = pd.Timestamp(ts).floor(freq_str)
         end = start + delta
         table = await self._tenant.execute_adhoc(self.pid, _get_utc_timestamp(start), _get_utc_timestamp(end), series)
         kcol, mcol = _compute_kcol_mcol(self.pipeline)
         return pd.DataFrame(_translate_table(table, None, kcol, mcol), columns=columns)
 
     async def _read_range(self, dts, series, columns=None, refresh=True):
         if refresh:
             await self._tenant.create_adhoc(self.pipeline)
         tasks = []
         tsidx = []
-        freq_str = f"{self.freq}S"
+        freq_str = f"{self.freq}sec"
         rlts = None
         delta = pd.Timedelta(freq_str)
         for ts in dts:
             start = ts.floor(freq_str)
             end = start + delta
             coro = self._tenant.execute_adhoc(self.pid, _get_utc_timestamp(start), _get_utc_timestamp(end), series)
             tasks.append(asyncio.create_task(coro))
@@ -676,24 +676,24 @@
         """
         self._tenant = tenant
         self._dset = dset
         self.plid = plid
         self.conf = conf
 
     async def _read_point(self, ts, columns=None):
-        freq_str = f"{self._dset.conf['freq']}S"
+        freq_str = f"{self._dset.conf['freq']}sec"
         start = ts.floor(freq_str)
         table = await self._tenant.query_pipeline_data(self._dset.dsid, self.plid, _get_utc_timestamp(start))
         kcol, mcol = _compute_kcol_mcol(self.conf['pipeline'])
         return pd.DataFrame(_translate_table(table, None, kcol, mcol), columns=columns)
 
     async def _read_range(self, dts, columns=None):
         tasks = []
         tsidx = []
-        freq_str = f"{self._dset.conf['freq']}S"
+        freq_str = f"{self._dset.conf['freq']}sec"
         rlts = None
         for ts in dts:
             start = ts.floor(freq_str)
             coro = self._tenant.query_pipeline_data(self._dset.dsid, self.plid, _get_utc_timestamp(start))
             tasks.append(asyncio.create_task(coro))
             tsidx.append(start)
         try:
@@ -763,15 +763,15 @@
         Args:
             dts: pandas.DatetimeIndex or array-like.
             overwrite: True to force overwrite data on API server. Defaults to False.
 
         Returns:
             Patch result in frame.
         """
-        freq_str = f"{self.conf['freq']}S"
+        freq_str = f"{self.conf['freq']}sec"
         tasks = []
         tsidx = []
         rlts = None
         for ts in dts:
             start = ts.floor(freq_str)
             coro = self._tenant.patch_dataset_data(self.dsid, _get_utc_timestamp(start), overwrite)
             tasks.append(asyncio.create_task(coro))
@@ -791,15 +791,15 @@
 
         Args:
             dts: pandas.DatetimeIndex or array-like.
 
         Returns:
             Patch result in frame.
         """
-        freq_str = f"{self.conf['freq']}S"
+        freq_str = f"{self.conf['freq']}sec"
         tasks = []
         tsidx = []
         rlts = None
         for ts in dts:
             start = ts.floor(freq_str)
             coro = self._tenant.poll_dataset_data(self.dsid, _get_utc_timestamp(start))
             tasks.append(asyncio.create_task(coro))
@@ -820,15 +820,15 @@
         Args:
             ts: start time in pandas.Timestamp
             coro: coroutine to handle new data
 
         Returns:
             The created task
         """
-        freq_str = f"{self.conf['freq']}S"
+        freq_str = f"{self.conf['freq']}sec"
         next_ts = pd.Timestamp(ts).floor(freq_str)
         delta = pd.Timedelta(freq_str)
         return asyncio.create_task(self._monitor_loop(next_ts, delta, coro, *args))
 
     async def _monitor_loop(self, next_ts, delta, coro, *args):
         add_delta = True
         while True:
```

### Comparing `ga-api-client-0.3.2/ga_api/hyper_log_log.py` & `ga_api_client-0.3.3/ga_api/hyper_log_log.py`

 * *Files identical despite different names*

### Comparing `ga-api-client-0.3.2/ga_api_client.egg-info/PKG-INFO` & `ga_api_client-0.3.3/ga_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga-api-client
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.4
```

