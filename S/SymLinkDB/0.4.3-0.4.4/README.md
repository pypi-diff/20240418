# Comparing `tmp/SymLinkDB-0.4.3.tar.gz` & `tmp/SymLinkDB-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymLinkDB-0.4.3.tar", last modified: Thu Apr 18 11:30:57 2024, max compression
+gzip compressed data, was "SymLinkDB-0.4.4.tar", last modified: Thu Apr 18 11:39:00 2024, max compression
```

## Comparing `SymLinkDB-0.4.3.tar` & `SymLinkDB-0.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.548551 SymLinkDB-0.4.3/
--rw-rw-rw-   0        0        0    36975 2024-04-18 11:30:57.540549 SymLinkDB-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.484514 SymLinkDB-0.4.3/SymLinkDB/
--rw-rw-rw-   0        0        0    46974 2024-04-18 11:29:44.000000 SymLinkDB-0.4.3/SymLinkDB/__init__.py
--rw-rw-rw-   0        0        0    46374 2024-04-18 11:25:11.000000 SymLinkDB-0.4.3/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py
--rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.3/SymLinkDB/document_code.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.460515 SymLinkDB-0.4.3/SymLinkDB/parts/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.532550 SymLinkDB-0.4.3/SymLinkDB/parts/cfd_backend/
--rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.3/SymLinkDB/parts/cfd_backend/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.3/SymLinkDB/parts/cfd_backend/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.540549 SymLinkDB-0.4.3/SymLinkDB/parts/memory_backend/
--rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.3/SymLinkDB/parts/memory_backend/__init__.py
--rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.3/SymLinkDB/parts/memory_backend/test.py
--rw-rw-rw-   0        0        0    11537 2024-03-26 07:32:05.000000 SymLinkDB-0.4.3/SymLinkDB/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:30:57.516540 SymLinkDB-0.4.3/SymLinkDB.egg-info/
--rw-rw-rw-   0        0        0    36975 2024-04-18 11:30:57.000000 SymLinkDB-0.4.3/SymLinkDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-18 11:30:57.000000 SymLinkDB-0.4.3/SymLinkDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:30:57.000000 SymLinkDB-0.4.3/SymLinkDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-18 11:30:57.000000 SymLinkDB-0.4.3/SymLinkDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2024-04-18 11:30:57.000000 SymLinkDB-0.4.3/SymLinkDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:30:57.548551 SymLinkDB-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-18 11:29:57.000000 SymLinkDB-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/
+-rw-rw-rw-   0        0        0    36975 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.248051 SymLinkDB-0.4.4/SymLinkDB/
+-rw-rw-rw-   0        0        0    46974 2024-04-18 11:38:15.000000 SymLinkDB-0.4.4/SymLinkDB/__init__.py
+-rw-rw-rw-   0        0        0    46374 2024-04-18 11:25:11.000000 SymLinkDB-0.4.4/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py
+-rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.4/SymLinkDB/document_code.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.214854 SymLinkDB-0.4.4/SymLinkDB/parts/
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.264128 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/
+-rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/
+-rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/test.py
+-rw-rw-rw-   0        0        0    11537 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.264128 SymLinkDB-0.4.4/SymLinkDB.egg-info/
+-rw-rw-rw-   0        0        0    36975 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-18 11:38:34.000000 SymLinkDB-0.4.4/setup.py
```

### Comparing `SymLinkDB-0.4.3/PKG-INFO` & `SymLinkDB-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.3
+Version: 0.4.4
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.3/README.md` & `SymLinkDB-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/__init__.py` & `SymLinkDB-0.4.4/SymLinkDB/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,16 +419,14 @@
 	def __init__(self, rec_id, table):
 		# レコードに関する情報の登録
 		self.id = rec_id
 		# 所属するtableに関する情報の登録
 		self.table = table
 		self.table_name = table.table_name
 		self.table_id = table.table_id
-		# link_infoのcache (rec[role]等のlink_set取得が重いため、高速化するためのキャッシュ)
-		self.link_info_cache = {}
 	# dataのgetter
 	@property
 	def data(self):
 		self.is_deleted(raise_err = True)	# 自身が削除済みかどうかを判定
 		return self.table.backend[("rec", self.table_id, self.id)]["data"]
 	# dataのsetter
 	@data.setter
@@ -450,15 +448,15 @@
 			del_search_idx(old_data, self.table.search_keys, self.table_id, self.id, self.table.backend)
 			# 検索インデックスの追加
 			add_search_idx(new_data, self.table.search_keys, self.table_id, self.id, self.table.backend)
 	# link_setの取得 [SymLinkDB]
 	def __getitem__(self, query):
 		self.is_deleted(raise_err = True)	# 自身が削除済みかどうかを判定
 		# クエリからlink情報取得 (キャッシュ化バージョン; クエリは「role名」または「関係名, role名」)
-		link_info = self.cached_link_info_getter(query)
+		link_info = self.table.cached_link_info_getter(query)
 		# LinkSetオブジェクトを作成して返す
 		return LinkSet(	# LinkSetクラス [SymLinkDB]
 			link_info["link_table_id"],	# link table ID
 			link_info["link_table_name"],	# link table名
 			subj_role_info = link_info["subj_role_info"],	# 自roleの情報
 			obj_role_info = link_info["obj_role_info"],	# 相手側roleの情報
 			rec = self)	# linkオブジェクト
@@ -490,20 +488,14 @@
 		except:
 			return False
 	# 自身が削除済みかどうかを判定
 	def is_deleted(self, raise_err = False):
 		deleted = (self.id not in self.table)
 		if deleted is True and raise_err is True: raise Exception("[SymLinkDB error] This record is already deleted.")
 		return deleted
-	# クエリからlink情報取得 (キャッシュ化バージョン; クエリは「role名」または「関係名, role名」)
-	def cached_link_info_getter(self, query):
-		if query not in self.link_info_cache:
-			# role名あるいはrole名とlink table名からlink情報を取得
-			self.link_info_cache[query] = get_link_info(query, self.table_id, self.table.sldb.backend)
-		return self.link_info_cache[query]
 
 # dataが正しく検索キーを持っているか確認する
 def check_data_format(data, search_keys):
 	# 辞書形式でない場合はエラー
 	if type(data) != type({}):
 		raise Exception("[SymLinkDB error] Insert data in dictionary format into the table where the search_key is set.")
 	# search_keyを1つでも持たない場合はエラー
@@ -570,14 +562,16 @@
 		sldb	# 所属するsldbオブジェクト
 	):
 		self.table_name = table_name
 		self.table_id = table_id
 		self.search_keys = search_keys
 		self.backend = backend
 		self.sldb = sldb
+		# link_infoのcache (rec[role]等のlink_set取得が重いため、高速化するためのキャッシュ)
+		self.link_info_cache = {}
 	# レコードの新規作成 [SymLinkDB]
 	def create(self, data, links = None):
 		# dataが正しく検索キーを持っているか確認する
 		if self.search_keys is not None: check_data_format(data, self.search_keys)
 		# linksが省略された場合
 		if links is None: links = {}
 		# rec_idの発行
@@ -667,14 +661,20 @@
 		# recを取得して返す
 		return [self[rec_id] for rec_id in rec_id_ls]	# レコードの取得 [SymLinkDB]
 	# 文字列化 (その1, その2)
 	def __str__(self):
 		recs_str = gen_recs_str(self)	# レコード一覧を表した要約文字列の生成
 		return f"<SymLinkTable {self.table_name} recs = {recs_str} search_keys = {souts(self.search_keys, 3)} >"
 	def __repr__(self): return str(self)
+	# クエリからlink情報取得 (キャッシュ化バージョン; クエリは「role名」または「関係名, role名」)
+	def cached_link_info_getter(self, query):
+		if query not in self.link_info_cache:
+			# role名あるいはrole名とlink table名からlink情報を取得
+			self.link_info_cache[query] = get_link_info(query, self.table_id, self.sldb.backend)
+		return self.link_info_cache[query]
 
 # versionの書き換え
 def rewrite_data_version(backend, target_key, filter_condition, new_ver_str):
 	old_value = backend[target_key]
 	def rewriter(entity):
 		entity["data_version"] = new_ver_str
 		return entity
```

### Comparing `SymLinkDB-0.4.3/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py` & `SymLinkDB-0.4.4/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/document_code.py` & `SymLinkDB-0.4.4/SymLinkDB/document_code.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/parts/cfd_backend/__init__.py` & `SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/parts/cfd_backend/test.py` & `SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/parts/memory_backend/__init__.py` & `SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/parts/memory_backend/test.py` & `SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB/test.py` & `SymLinkDB-0.4.4/SymLinkDB/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.3/SymLinkDB.egg-info/PKG-INFO` & `SymLinkDB-0.4.4/SymLinkDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.3
+Version: 0.4.4
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.3/setup.py` & `SymLinkDB-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 5379 6d4c 696e 6b44  develop_SymLinkD
 000000c0: 422f 2229 2061 7320 703a 0d0a 0973 6574  B/") as p:...set
 000000d0: 7570 280d 0a09 096e 616d 6520 3d20 2253  up(....name = "S
 000000e0: 796d 4c69 6e6b 4442 222c 0d0a 0909 7665  ymLinkDB",....ve
-000000f0: 7273 696f 6e20 3d20 2230 2e34 2e33 222c  rsion = "0.4.3",
+000000f0: 7273 696f 6e20 3d20 2230 2e34 2e34 222c  rsion = "0.4.4",
 00000100: 0d0a 0909 6465 7363 7269 7074 696f 6e20  ....description 
 00000110: 3d20 2241 2067 7261 7068 2064 6174 6162  = "A graph datab
 00000120: 6173 6520 6368 6172 6163 7465 7269 7a65  ase characterize
 00000130: 6420 6279 2062 6964 6972 6563 7469 6f6e  d by bidirection
 00000140: 616c 206c 696e 6b73 2e20 4974 2061 6c6c  al links. It all
 00000150: 6f77 7320 666f 7220 696e 7475 6974 6976  ows for intuitiv
 00000160: 6520 6465 7369 676e 206f 6620 6461 7461  e design of data
```

