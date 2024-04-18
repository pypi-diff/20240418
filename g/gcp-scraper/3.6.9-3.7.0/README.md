# Comparing `tmp/gcp-scraper-3.6.9.tar.gz` & `tmp/gcp-scraper-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-scraper-3.6.9.tar", last modified: Sat Apr 13 00:29:08 2024, max compression
+gzip compressed data, was "gcp-scraper-3.7.0.tar", last modified: Thu Apr 18 13:01:06 2024, max compression
```

## Comparing `gcp-scraper-3.6.9.tar` & `gcp-scraper-3.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:29:08.068861 gcp-scraper-3.6.9/
--rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.6.9/LICENSE
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-13 00:29:08.068689 gcp-scraper-3.6.9/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.6.9/README.md
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:29:08.067846 gcp-scraper-3.6.9/gcp_scraper.egg-info/
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-13 00:29:07.000000 gcp-scraper-3.6.9/gcp_scraper.egg-info/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-13 00:29:07.000000 gcp-scraper-3.6.9/gcp_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-13 00:29:07.000000 gcp-scraper-3.6.9/gcp_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-13 00:29:07.000000 gcp-scraper-3.6.9/gcp_scraper.egg-info/requires.txt
--rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-13 00:29:07.000000 gcp-scraper-3.6.9/gcp_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:29:08.054778 gcp-scraper-3.6.9/gscraper/
--rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-13 00:19:26.000000 gcp-scraper-3.6.9/gscraper/__init__.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:29:08.059536 gcp-scraper-3.6.9/gscraper/base/
--rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.6.9/gscraper/base/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    22817 2024-04-13 00:20:53.000000 gcp-scraper-3.6.9/gscraper/base/abstract.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.6.9/gscraper/base/gcloud.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    89284 2024-04-13 00:22:05.000000 gcp-scraper-3.6.9/gscraper/base/session.py
--rwxr-xr-x   0 cuz        (501) staff       (20)   117106 2024-04-13 00:28:06.000000 gcp-scraper-3.6.9/gscraper/base/spider.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.6.9/gscraper/base/types.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:29:08.067156 gcp-scraper-3.6.9/gscraper/utils/
--rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.6.9/gscraper/utils/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.6.9/gscraper/utils/cast.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.6.9/gscraper/utils/date.py
--rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.6.9/gscraper/utils/logs.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    69616 2024-04-13 00:20:03.000000 gcp-scraper-3.6.9/gscraper/utils/map.py
--rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-13 00:29:08.069440 gcp-scraper-3.6.9/setup.cfg
--rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.6.9/setup.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.203067 gcp-scraper-3.7.0/
+-rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.7.0/LICENSE
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-18 13:01:06.202779 gcp-scraper-3.7.0/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.7.0/README.md
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.198430 gcp-scraper-3.7.0/gcp_scraper.egg-info/
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-18 13:01:06.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/requires.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-18 13:01:05.000000 gcp-scraper-3.7.0/gcp_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.183237 gcp-scraper-3.7.0/gscraper/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-18 13:00:36.000000 gcp-scraper-3.7.0/gscraper/__init__.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.195134 gcp-scraper-3.7.0/gscraper/base/
+-rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.7.0/gscraper/base/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    22817 2024-04-13 00:20:53.000000 gcp-scraper-3.7.0/gscraper/base/abstract.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.7.0/gscraper/base/gcloud.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    89023 2024-04-18 12:57:21.000000 gcp-scraper-3.7.0/gscraper/base/session.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)   117188 2024-04-18 13:00:09.000000 gcp-scraper-3.7.0/gscraper/base/spider.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.7.0/gscraper/base/types.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-18 13:01:06.198098 gcp-scraper-3.7.0/gscraper/utils/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.7.0/gscraper/utils/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.7.0/gscraper/utils/cast.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.7.0/gscraper/utils/date.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.7.0/gscraper/utils/logs.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    69662 2024-04-18 12:54:00.000000 gcp-scraper-3.7.0/gscraper/utils/map.py
+-rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-18 13:01:06.204021 gcp-scraper-3.7.0/setup.cfg
+-rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.7.0/setup.py
```

### Comparing `gcp-scraper-3.6.9/LICENSE` & `gcp-scraper-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/PKG-INFO` & `gcp-scraper-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.9
+Version: 3.7.0
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.9/gcp_scraper.egg-info/PKG-INFO` & `gcp-scraper-3.7.0/gcp_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.9
+Version: 3.7.0
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.9/gscraper/base/abstract.py` & `gcp-scraper-3.7.0/gscraper/base/abstract.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/base/gcloud.py` & `gcp-scraper-3.7.0/gscraper/base/gcloud.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/base/session.py` & `gcp-scraper-3.7.0/gscraper/base/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from gscraper.base.types import is_array, allin_instance, is_str_array
 
 from gscraper.utils import isna, notna, exists
 from gscraper.utils.cast import cast_object, cast_str, cast_list, cast_tuple, cast_float, cast_int, cast_int1
 from gscraper.utils.date import now, today, get_date, get_date_pair, set_date, is_daily_frequency, get_date_range
 from gscraper.utils.logs import CustomLogger, dumps_data, log_exception, log_data
 from gscraper.utils.map import isna_plus, notna_plus, exists_one, howin, safe_apply, safe_len, get_scala, unique
-from gscraper.utils.map import re_get, replace_map, startswith, endswith, arg_and, union, diff
+from gscraper.utils.map import concat, re_get, replace_map, startswith, endswith, arg_and, union, diff
 from gscraper.utils.map import iloc, is_same_length, unit_records, concat_array, transpose_array
 from gscraper.utils.map import kloc, is_single_path, hier_get, notna_dict, chain_dict, drop_dict
 from gscraper.utils.map import vloc, concat_df, safe_apply_df, match_df, to_dataframe, to_series
 from gscraper.utils.map import get_value, filter_data, set_data, isin_data, chain_exists, groupby_data, is_single_selector
 
 from abc import ABCMeta
 from ast import literal_eval
@@ -73,32 +73,30 @@
 __RENAME__ = "__RENAME__"
 __SPLIT__ = "__SPLIT__"
 __STAT__ = "__STAT__"
 __SUM__ = "__SUM__"
 __MAP__ = "__MAP__"
 __MISMATCH__ = "__MISMATCH__"
 
-ITER_INDEX = "__index"
-ITER_SUFFIX = lambda context: f"_{context[ITER_INDEX]}" if ITER_INDEX in context else str()
-ITER_MSG = lambda context: {ITER_INDEX: context[ITER_INDEX]} if ITER_INDEX in context else dict()
-ITER_TEXT = lambda text, context: f"{text}_{context[ITER_INDEX]}" if ITER_INDEX in context else text
+TZINFO = "Asia/Seoul"
+START, END = 0, 1
 
+TASK = "task"
+ITER_INDEX = "__index"
 COUNT_INDEX = "__i"
-_NESTED_SUFFIX = lambda context: \
-    f"[{context[COUNT_INDEX]}]" if (ITER_INDEX in context) and isinstance(context[ITER_INDEX], str) else f"-{context[COUNT_INDEX]}"
-_COUNT_SUFFIX = lambda context: _NESTED_SUFFIX(context) if COUNT_INDEX in context else str()
-
-_SCHEMA_SUFFIX = lambda context: f"_{context[SCHEMA_KEY]}" if SCHEMA_KEY in context else str()
-_FIELD_SUFFIX = lambda field: f"_{field[NAME]}" if NAME in field else str()
-_NAME_SUFFIX = lambda name: f"_{name}" if name else str()
-SUFFIX = lambda context, field=dict(), name=str(): \
-    _SCHEMA_SUFFIX(context) + _FIELD_SUFFIX(field) + _NAME_SUFFIX(name) + ITER_SUFFIX(context) + _COUNT_SUFFIX(context)
 
-TZINFO = None
-START, END = 0, 1
+def iter_task(context: Context, method=str(), sep='_', strict=True) -> str:
+    return concat(context.get(TASK), method, context.get(ITER_INDEX), sep=sep, strict=strict)
+
+def count_task(context: Context, method=str(), field: Field=dict(), name=str(), sep='_', strict=True) -> str:
+    if COUNT_INDEX in context:
+        count_index = f"[{context[COUNT_INDEX]}]" if isinstance(context.get(ITER_INDEX), str) else f"-{context[COUNT_INDEX]}"
+    else: count_index = None
+    args = (context.get(TASK), method, context.get(SCHEMA_KEY), field.get(NAME), name, context.get(ITER_INDEX), count_index)
+    return concat(*args, sep=sep, strict=strict)
 
 class UserInterrupt(Exception):
     ...
 
 class ForbiddenError(ValueError):
     ...
 
@@ -595,15 +593,15 @@
             self.save_data(save, prefix=CHECKPOINT_PATH+str(point).replace('.','_'), ext=ext)
         if self.interrupt and self._isin_log_list(point, self.interrupt):
             raise UserInterrupt(USER_INTERRUPT_MSG(where))
 
     def save_data(self, data: Data, prefix=str(), suffix="now", ext: Optional[TypeHint]=None):
         prefix = prefix if prefix else self.operation
         suffix = self.now("%Y%m%d%H%M%S") if suffix == "now" else suffix
-        file_name = '_'.join(filter(None, [prefix, suffix]))
+        file_name = concat(prefix, suffix, sep='_')
         ext = ext if ext else type(data)
         if is_dataframe_type(ext):
             self.save_dataframe(data, file_name+".xlsx")
         elif is_tag_type(ext):
             self.save_source(data, file_name+".html")
         else: self.save_json(data, file_name+".json")
 
@@ -1023,15 +1021,15 @@
         return flow
 
     def _init_flow(self, data: ResponseData, flow: Optional[Flow]=None, responseType: Optional[TypeHint]=None,
                     root: Optional[_KT]=None, discard=True, **context) -> Union[Data,Context]:
         root = self.get_root(root=root, **context)
         if root: data = get_value(data, root)
         flow = self.get_flow(flow=flow, **context)
-        self.checkpoint("map"+SUFFIX(context), where="init_flow", msg={"root":root, "data":data, "flow":flow}, save=data)
+        self.checkpoint(count_task(context, "map"), where="init_flow", msg={"root":root, "data":data, "flow":flow}, save=data)
         return data, dict(context, flow=flow, responseType=responseType, discard=discard)
 
     def _set_update_time_by_interval(self, __data: Data, date: Optional[dt.date]=None, datetime: Optional[dt.datetime]=None,
                                     interval: Timedelta=str(), **context) -> Data:
         updateDate = date if isinstance(date, dt.date) and is_daily_frequency(interval) else self.today()
         return self.set_update_time(__data, date=updateDate, datetime=datetime)
 
@@ -1059,15 +1057,15 @@
 
     def match(self, data: ResponseData, **context) -> bool:
         return True
 
     def _init_process(self, data: ResponseData, __base: Data, process: Process, responseType: Type, **context) -> Union[Data,bool]:
         if not (isinstance(process, Process) and isinstance(process[SCHEMA], Schema)): return data, False
         data = get_value(data, process[ROOT]) if ROOT in process else data
-        self.checkpoint("schema"+SUFFIX(context), where="init_process", msg={"data":data, "schema":process[SCHEMA]}, save=data)
+        self.checkpoint(count_task(context, "schema"), where="init_process", msg={"data":data, "schema":process[SCHEMA]}, save=data)
         if not isinstance(data, _get_response_type(responseType)):
             if not data: return data, False
             else: raise TypeError(INVALID_DATA_TYPE_MSG(data, context))
         data = self._merge_base(data, __base)
         __match = self._match_process(data, process, **context)
         if isinstance(__match, pd.DataFrame): return __match, True
         else: return data, __match
@@ -1121,15 +1119,15 @@
             __value = field[PATH]
         elif path_type == TUPLE:
             if isinstance(data, pd.DataFrame): __value = self._get_value_tuple_df(data, **field, context=context)
             else: __value = self._get_value_tuple(data, **field, context=context)
         elif (path_type == ITERATE) and (not isinstance(data, pd.DataFrame)):
             __value = self._get_value_iterate(data, **field, context=context)
         else: raise TypeError(INVALID_PATH_TYPE_MSG(field[PATH]))
-        self.checkpoint("field"+SUFFIX(context, field), where="map_field", msg={"value":__value, "field":field})
+        self.checkpoint(count_task(context, "field", field), where="map_field", msg={"value":__value, "field":field})
         return self._set_value(__base, __value, field, **context)
 
     def _get_value(self, data: ResponseData, path=list(), type: Optional[TypeHint]=None, default=None,
                     apply: Apply=dict(), match: Match=dict(), cast=False, strict=True, sep=str(), strip=True,
                     context: Context=dict(), name=str(), log=False, **field) -> _VT:
         if isinstance(data, pd.DataFrame):
             if match:
@@ -1353,21 +1351,21 @@
             return _toggle(match_df(data, match=(lambda x: exists(x, strict=strict)), all_cols=True), flip=flip)
         else: return _toggle(exists(__value, strict=strict), flip=flip)
 
     def _log_origin(self, __value: _VT, __object: Any, point: str, where: str, msg=dict(), context: Context=dict(),
                     field: Optional[Field]=dict(), name: Optional[str]=str(), log=False, **kwargs):
         if not log: return
         msg = dict({"value":__value, point:__object}, **msg)
-        self.checkpoint(f"[origin]_{point}"+SUFFIX(context, field, name), where=where, msg=msg)
+        self.checkpoint(count_task(context, f"[origin]_{point}", field, name), where=where, msg=msg)
 
     def _log_result(self, __result: _VT, __object: Any, point: str, where: str, msg=dict(), context: Context=dict(),
                     field: Optional[Field]=dict(), name: Optional[str]=str(), log=False, **kwargs):
         if not log: return
         msg = dict({"result":__result, point:__object}, **msg)
-        self.checkpoint(point+SUFFIX(context, field, name), where=where, msg=msg)
+        self.checkpoint(count_task(context, point, field, name), where=where, msg=msg)
 
 
 def _get_response_type(responseType: TypeHint) -> Type:
     if isinstance(responseType, Type): return responseType
     elif is_dict_type(responseType): return dict
     elif is_dataframe_type(responseType): return pd.DataFrame
     elif is_tag_type(responseType): return Tag
@@ -1457,15 +1455,15 @@
         elif is_tag_type(responseType): return self._map_tag_list(data, **context)
         else: return self._map_records(data, **context)
 
     def _groupby_data(self, data: ResponseData, groupby: Union[Dict[_KT,_KT],_KT], groupSize: NestedDict=dict(),
                     if_null: Literal["drop","pass"]="drop", hier=False, **context) -> Data:
         groups = groupby_data(data, by=groupby, if_null=if_null, hier=hier)
         log_msg = {"groups":list(groups.keys()), "groupSize":[safe_len(group) for group in groups.values()]}
-        self.checkpoint("group"+SUFFIX(context), where="groupby_data", msg=log_msg)
+        self.checkpoint(count_task(context, "group"), where="groupby_data", msg=log_msg)
         results = [self._map_sequence(__data, **dict(context, group=group, dataSize=groupSize.get(group)))
                     for group, __data in groups.items()]
         return chain_exists(results)
 
     ###################################################################
     ######################## Map Sequence Data ########################
     ###################################################################
@@ -1567,15 +1565,15 @@
             context = RESPONSE_CONTEXT(**REQUEST_CONTEXT(**self.from_locals(locals, drop, **context)))
             is_valid = self.is_valid_response(response)
             if notna(context.get("countPath")) and (ITER_INDEX in context):
                 self.iterateCount[context[ITER_INDEX]] = cast_int(get_value(response, context["countPath"]))
             if notna(context.get("returnPath")):
                 return get_value(response, context["returnPath"])
             data = func(self, response, *args, **context) if is_valid else init_origin(func)
-            self.checkpoint(ITER_TEXT("parse",context), where=func.__name__, msg={"data":data}, save=data)
+            self.checkpoint(iter_task(context, "parse"), where=func.__name__, msg={"data":data}, save=data)
             self.log_results(data, **context)
             return data
         return wrapper
 
     def is_valid_response(self, response: Any) -> bool:
         return True
```

### Comparing `gcp-scraper-3.6.9/gscraper/base/spider.py` & `gcp-scraper-3.7.0/gscraper/base/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from gscraper.base.abstract import CustomDict, OptionalDict, TypedRecords, Query, INVALID_OBJECT_TYPE_MSG
 from gscraper.base.abstract import UNIQUE_CONTEXT, TASK_CONTEXT, REQUEST_CONTEXT
 from gscraper.base.abstract import SESSION_CONTEXT, PROXY_CONTEXT, REDIRECT_CONTEXT
 
 from gscraper.base.session import BaseSession, Iterator, Parser
 from gscraper.base.session import UserInterrupt, ForbiddenError, ParseError
 from gscraper.base.session import Info, Schema, Field, Flow, Process
-from gscraper.base.session import ITER_INDEX, ITER_TEXT, ITER_MSG, PAGE_ITERATOR
+from gscraper.base.session import ITER_INDEX, PAGE_ITERATOR, iter_task
 from gscraper.base.gcloud import GoogleQueryReader, GoogleUploader, GoogleQueryList, GoogleUploadList
 from gscraper.base.gcloud import Account, fetch_gcloud_authorization, read_gcloud
 
 from gscraper.base.types import _KT, _PASS, Arguments, Context, LogLevel, TypeHint, EncryptedKey, DecryptedKey
 from gscraper.base.types import IndexLabel, Keyword, Pagination, Status, Unit, Range, DateFormat, Timedelta, Timezone
 from gscraper.base.types import Records, Data, MappedData, JsonData, RedirectData
 from gscraper.base.types import is_datetime_type, is_date_type, is_array, is_int_array
@@ -18,15 +18,15 @@
 from gscraper.utils import notna
 from gscraper.utils.cast import cast_list, cast_tuple, cast_int, cast_datetime_format
 from gscraper.utils.date import get_date_pair, get_datetime_pair
 from gscraper.utils.logs import log_encrypt, log_messages, log_response, log_client, log_data
 from gscraper.utils.map import to_array, align_array, transpose_array, unit_array, get_scala, union, inter, diff
 from gscraper.utils.map import kloc, notna_dict, drop_dict, split_dict
 from gscraper.utils.map import vloc, apply_records, to_dataframe, convert_data, rename_data, filter_data
-from gscraper.utils.map import exists_one, unique, chain_exists, between_data, join, re_get
+from gscraper.utils.map import exists_one, unique, chain_exists, between_data, concat, re_get
 from gscraper.utils.map import convert_dtypes as _convert_dtypes
 
 from abc import ABCMeta, abstractmethod
 from http.cookies import SimpleCookie
 from requests.cookies import RequestsCookieJar
 from urllib.parse import quote, urlencode, urlparse
 import asyncio
@@ -137,21 +137,21 @@
 ###################################################################
 
 HEADERS = {
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "ko-KR,ko;q=0.9,en-US;q=0.8,en;q=0.7",
     "Connection": "keep-alive",
-    "sec-ch-ua": '"Chromium";v="116", "Not)A;Brand";v="24", "Google Chrome";v="116"',
+    "sec-ch-ua": '"Google Chrome";v="123", "Not:A-Brand";v="8", "Chromium";v="123"',
     "sec-ch-ua-mobile": "?0",
     "sec-ch-ua-platform": '"Windows"',
     "Sec-Fetch-Dest": "empty",
     "Sec-Fetch-Mode": "cors",
     "Sec-Fetch-Site": "same-origin",
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36",
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
 }
 
 
 def get_content_type(content_type=str(), urlencoded=False, utf8=False) -> str:
     if urlencoded or content_type == "urlencoded":
         __type = "application/x-www-form-urlencoded"
     elif content_type == "json": __type = "application/json"
@@ -822,26 +822,27 @@
     def fetch(self, *args, **context) -> Data:
         ...
 
     def validate_request(func):
         @functools.wraps(func)
         def wrapper(self: Spider, *args, locals: Dict=dict(), drop: _KT=list(), **context):
             context = self._encode_messages(*args, **self.from_locals(locals, drop, **context))
-            self.checkpoint(ITER_TEXT("request",context), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
+            self.checkpoint(iter_task(context, "request"), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
             response = func(self, **self._validate_session(context))
-            self.checkpoint(ITER_TEXT("response",context), where=func.__name__, msg={"response":response}, save=response)
+            self.checkpoint(iter_task(context, "response"), where=func.__name__, msg={"response":response}, save=response)
             return response
         return wrapper
 
     def _encode_messages(self, method: str, url: str, messages: Dict=dict(), params=None, encode: Optional[bool]=None,
                         data=None, json=None, headers=None, cookies=str(), *args, **context) -> Context:
         url, params = self.encode_params(url, params, encode=encode)
         if headers and cookies: headers["Cookie"] = str(cookies)
         messages = messages if messages else notna_dict(params=params, data=data, json=json, headers=headers)
-        self.logger.debug(log_messages(**ITER_MSG(context), **messages, dump=self.logJson))
+        iter_context = {ITER_INDEX: context[ITER_INDEX]} if ITER_INDEX in context else dict()
+        self.logger.debug(log_messages(**iter_context, **messages, dump=self.logJson))
         return dict(context, method=method, url=url, messages=messages)
 
     def _validate_session(self, context: Context) -> Context:
         if not (("session" in context) and isinstance(context["session"], requests.Session)):
             context["session"] = requests
         return context
 
@@ -1284,17 +1285,17 @@
     async def fetch(self, *args, **context) -> Data:
         ...
 
     def validate_request(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSpider, *args, locals: Dict=dict(), drop: _KT=list(), **context):
             context = self._encode_messages(*args, **self.from_locals(locals, drop, **context))
-            self.checkpoint(ITER_TEXT("request",context), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
+            self.checkpoint(iter_task(context, "request"), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
             response = await func(self, **self._validate_session(context))
-            self.checkpoint(ITER_TEXT("response",context), where=func.__name__, msg={"response":response}, save=response)
+            self.checkpoint(iter_task(context, "response"), where=func.__name__, msg={"response":response}, save=response)
             return response
         return wrapper
 
     def _validate_session(self, context: Context) -> Context:
         if not (("session" in context) and isinstance(context["session"], aiohttp.ClientSession)):
             raise RequestInterrupt(MISSING_CLIENT_SESSION_MSG)
         return context
@@ -1482,20 +1483,19 @@
 
     ###################################################################
     ########################## Fetch Request ##########################
     ###################################################################
 
     def validate_request(func):
         @functools.wraps(func)
-        def wrapper(self: Spider, *args, locals: Dict=dict(), drop: _KT=list(), **context):
+        def wrapper(self: Spider, *args, locals: Dict=dict(), drop: _KT=list(), origin=str(), **context):
             context = self._encode_messages(*args, **self.from_locals(locals, drop, **context))
-            origin = context.get("origin")
-            self.checkpoint(join(origin,"request",sep='_'), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
-            response = func(self, **context)
-            self.checkpoint(join(origin,"response",sep='_'), where=func.__name__, msg={"response":response}, save=response)
+            self.checkpoint(concat(origin, "request", sep='_'), where=func.__name__, msg=dict(url=context["url"], **context["messages"]))
+            response = func(self, origin=origin, **context)
+            self.checkpoint(concat(origin, "response", sep='_'), where=func.__name__, msg={"response":response}, save=response)
             return response
         return wrapper
 
     @validate_request
     def request_url(self, method: str, url: str, messages: Dict=dict(),
                     params=None, encode: Optional[bool]=None, data=None, json=None,
                     headers=None, cookies=str(), *args, origin=str(), allow_redirects=True, **context):
@@ -1559,15 +1559,15 @@
                     headers=None, cookies=str(), *args, origin=str(), allow_redirects=True, features="html.parser", **context) -> Tag:
         with self.request(method, url, **messages, allow_redirects=allow_redirects, verify=self.ssl) as response:
             self.logger.info(log_response(response, url=url, origin=origin))
             self.logger.debug(log_messages(cookies=self.get_cookies(encode=False), origin=origin, dump=self.logJson))
             return BeautifulSoup(response.text, features)
 
     def log_response_text(self, response: requests.Response, origin=str()):
-        self.checkpoint(join(origin,"text",sep='_'), where=origin, msg={"response":response.text}, save=response)
+        self.checkpoint(concat(origin, "text", sep='_'), where=origin, msg={"response":response.text}, save=response)
 
 
 class LoginCookie(LoginSpider):
     operation = "login"
 
     def __init__(self, cookies=str(), **context):
         requests.Session.__init__(self)
```

### Comparing `gcp-scraper-3.6.9/gscraper/base/types.py` & `gcp-scraper-3.7.0/gscraper/base/types.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/utils/__init__.py` & `gcp-scraper-3.7.0/gscraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/utils/cast.py` & `gcp-scraper-3.7.0/gscraper/utils/cast.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/utils/date.py` & `gcp-scraper-3.7.0/gscraper/utils/date.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/utils/logs.py` & `gcp-scraper-3.7.0/gscraper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.9/gscraper/utils/map.py` & `gcp-scraper-3.7.0/gscraper/utils/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1159,16 +1159,16 @@
     else: return sorted(data, reverse=(not asc))
 
 
 ###################################################################
 ############################## String #############################
 ###################################################################
 
-def join(*args: str, sep=',') -> str:
-    return sep.join(list(filter(None, args)))
+def concat(*args: str, sep=',', strict=True) -> str:
+    return sep.join([str(__s) for __s in args if notna(__s, strict=strict)])
 
 
 def re_get(pattern: RegexFormat, string: str, default=str(), index: Optional[int]=0) -> Union[str,List[str]]:
     __pattern = pattern if isinstance(pattern, re.Pattern) else re.compile(pattern)
     if not isinstance(index, int): return __pattern.findall(string)
     catch = __pattern.search(string)
     return __pattern.search(string).groups()[index] if catch else default
```

### Comparing `gcp-scraper-3.6.9/setup.py` & `gcp-scraper-3.7.0/setup.py`

 * *Files identical despite different names*

