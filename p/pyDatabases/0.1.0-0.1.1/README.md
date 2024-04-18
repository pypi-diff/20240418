# Comparing `tmp/pydatabases-0.1.0.tar.gz` & `tmp/pydatabases-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatabases-0.1.0.tar", last modified: Tue Apr 16 22:36:50 2024, max compression
+gzip compressed data, was "pydatabases-0.1.1.tar", last modified: Thu Apr 18 11:52:25 2024, max compression
```

## Comparing `pydatabases-0.1.0.tar` & `pydatabases-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.385957 pydatabases-0.1.0/
--rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      761 2024-04-16 22:36:50.384589 pydatabases-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.308069 pydatabases-0.1.0/pyDatabases/
--rw-rw-rw-   0        0        0       34 2024-04-15 19:36:01.000000 pydatabases-0.1.0/pyDatabases/__init__.py
--rw-rw-rw-   0        0        0    12902 2024-04-16 12:46:37.000000 pydatabases-0.1.0/pyDatabases/auxfuncs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.356879 pydatabases-0.1.0/pyDatabases/gpyDB/
--rw-rw-rw-   0        0        0      101 2024-04-16 22:30:11.000000 pydatabases-0.1.0/pyDatabases/gpyDB/__init__.py
--rw-rw-rw-   0        0        0    20423 2024-04-16 11:41:37.000000 pydatabases-0.1.0/pyDatabases/gpyDB/database.py
--rw-rw-rw-   0        0        0    23887 2024-04-16 22:23:52.000000 pydatabases-0.1.0/pyDatabases/gpyDB/gpyDB.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.372523 pydatabases-0.1.0/pyDatabases/simpleDB/
--rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.0/pyDatabases/simpleDB/__init__.py
--rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.0/pyDatabases/simpleDB/simpleDB.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:36:50.382919 pydatabases-0.1.0/pyDatabases.egg-info/
--rw-rw-rw-   0        0        0      761 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 22:36:50.000000 pydatabases-0.1.0/pyDatabases.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 22:36:50.386795 pydatabases-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-16 22:32:56.000000 pydatabases-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.473285 pydatabases-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2022-11-24 10:36:30.000000 pydatabases-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      761 2024-04-18 11:52:25.472073 pydatabases-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-16 22:31:17.000000 pydatabases-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.436880 pydatabases-0.1.1/pyDatabases/
+-rw-rw-rw-   0        0        0       34 2024-04-16 22:50:27.000000 pydatabases-0.1.1/pyDatabases/__init__.py
+-rw-rw-rw-   0        0        0    12902 2024-04-16 23:18:35.000000 pydatabases-0.1.1/pyDatabases/auxfuncs.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.461176 pydatabases-0.1.1/pyDatabases/gpyDB/
+-rw-rw-rw-   0        0        0      101 2024-04-16 22:30:11.000000 pydatabases-0.1.1/pyDatabases/gpyDB/__init__.py
+-rw-rw-rw-   0        0        0    20423 2024-04-18 07:18:37.000000 pydatabases-0.1.1/pyDatabases/gpyDB/database.py
+-rw-rw-rw-   0        0        0    24830 2024-04-18 11:47:33.000000 pydatabases-0.1.1/pyDatabases/gpyDB/gpyDB.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.467479 pydatabases-0.1.1/pyDatabases/simpleDB/
+-rw-rw-rw-   0        0        0       23 2024-04-05 12:13:25.000000 pydatabases-0.1.1/pyDatabases/simpleDB/__init__.py
+-rw-rw-rw-   0        0        0     6339 2024-04-15 19:40:03.000000 pydatabases-0.1.1/pyDatabases/simpleDB/simpleDB.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:52:25.469903 pydatabases-0.1.1/pyDatabases.egg-info/
+-rw-rw-rw-   0        0        0      761 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 11:52:25.000000 pydatabases-0.1.1/pyDatabases.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:52:25.474216 pydatabases-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-18 11:51:34.000000 pydatabases-0.1.1/setup.py
```

### Comparing `pydatabases-0.1.0/LICENSE` & `pydatabases-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.0/PKG-INFO` & `pydatabases-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.0/pyDatabases/auxfuncs.py` & `pydatabases-0.1.1/pyDatabases/auxfuncs.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.0/pyDatabases/gpyDB/database.py` & `pydatabases-0.1.1/pyDatabases/gpyDB/database.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.0/pyDatabases/gpyDB/gpyDB.py` & `pydatabases-0.1.1/pyDatabases/gpyDB/gpyDB.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from .database import *
 from gams.core.numpy import gams2numpy
 import os, pickle, openpyxl, io
 
 admissable_gpy_types = (pd.Series,pd.Index,int,float,str,np.generic,dict,gpy)
+g2np_ = gams2numpy.Gams2Numpy()
+dropattrs_ = ['database','ws','g2np','gmd']
 
 def sunion_empty(ls):
 	""" return empty set if the list of sets (ls) is empty"""
 	try:
 		return set.union(*ls)
 	except TypeError:
 		return set()
@@ -19,74 +21,112 @@
 		partitions = [int(x.rpartition(name+'__v')[-1]) for x in d if ifInt(x.rpartition(name+'__v')[-1])]
 		return name+'__v'+str(max(partitions)+1) if partitions else name+'__v1'
 
 def partitionDoms(s, ss):
 	return OrdSet.partition(OrdSet(getDomains(s)), OrdSet(getDomains(ss)))
 
 class GpyDB:
-	def __init__(self,pickle_path=None,ws=None,db=None,alias=None,**kwargs):
-		""" Init methods: 	(1) from file path to a pickle (fastest, only uses the kwargs 'ws','alias'), 
-							(2) db = GpyDB (fast, only uses the kwarg 'ws','alias'), 
-							(3) db = dict (fast, but does not check validity of attributes. only uses 'ws','alias'), 
-							(4) db ∈ {None, str, gams.GamsDatabase} (slower, but more robust. uses all kwargs except 'pickle_path'); """ 
-		if pickle_path is not None:
-			self.initFromPickle(pickle_path,ws=ws)
-		elif isinstance(db,dict):
-			self.updateWithWs(ws,db)
-		elif isinstance(db,GpyDB):
-			self.initFromGpyGB(db,ws=ws)
-		else:
-			self.initWs(ws)
-			self.g2np = gams2numpy.Gams2Numpy(self.ws.system_directory)
-			self.name = versionizeName(dictInit('name', 'rname',kwargs), self.ws._gams_databases)
-			self.exportSettings = {'dropattrs': ['database','ws','g2np','gmd'], 'data_folder': dictInit('data_folder',os.getcwd(),kwargs)}
-			self.initDbs(db)
-			self.gmd = readGmd(self.database, self.g2np)
-			self.series = SeriesDB(database=self.gmd())
-		self.updateAlias(alias=alias)
-
 	###################################################################################################
 	###									0: Pickling/load/export settings 							###
 	###################################################################################################
+	def __init__(self, obj = None, ws = None, alias = None, **kwargs):
+		getattr(self, f'init_{obj.__class__.__name__}')(obj, ws = ws, **kwargs)
+		self.updateAlias(alias=alias)
 
-	def initFromPickle(self,pickle_path,ws=None):
-		with open(pickle_path,"rb") as file:
-			pickled_data=pickle.load(file)
-		self.updateWithWs(ws,pickled_data.__dict__)
-
-	def initFromGpyGB(self,db,ws=None):
-		self.updateWithWs(ws,db.__dict__)
-
-	def updateWithWs(self,ws,dict_):
-		if ws is None:
-			self.__dict__ = dict_
-		else:
-			self.__dict__ = {key: value for key,value in dict_.items() if key not in ('ws','database')}
-			self.initWs(ws)
-			self.name = versionizeName(self.name, self.ws._gams_databases) # update name of database if it is already used in the current ws.
-			self.initDbs(dict_['database'])
-
-	def initWs(self,ws):
-		if ws is None:
-			self.ws = gams.GamsWorkspace()
-		elif type(ws) is str:
-			self.ws = gams.GamsWorkspace(working_directory=ws)
-		elif isinstance(ws,gams.GamsWorkspace):
-			self.ws = ws
-		self.work_folder = self.ws.working_directory
+	def init_NoneType(self, noneObj, db = None, **kwargs):
+		getattr(self, f'initFromDb_{db.__class__.__name__}')(db, **kwargs)
+	def init_str(self, pickle_path, ws = None):
+		with open(pickle_path, "rb") as file:
+			p = pickle.load(file)
+		self.init_dict(p.__dict__, ws = noneInit(ws, p.work_folder))
+	def init_GpyDB(self, db, ws = None):
+		d = {k: v if k in dropattrs_ else deepcopy(v) for k,v in db.__dict__.items()} # copy all attributes
+		self.init_dict(d, ws = noneInit(ws, db.ws))
+
+	def init_dict(self, d, ws = None):
+		self.__dict__ = d
+		if ws is not None:
+			self.setWs(ws)
+			self.name = versionizeName(self.name, self.ws._gams_databases)
+			self.initDb(d['database'])
+
+	def init_GamsDatabase(self, db, ws = None, data_folder = None, dropattrs = None):
+		self.database = db
+		self.setWs(db.workspace)
+		self.name = db.name
+		self.g2np = g2np_
+		self.data_folder = noneInit(data_folder, os.getcwd())
+		self.dropattrs = noneInit(dropattrs, dropattrs_.copy())
+		self.gmd = readGmd(self.database, self.g2np)
+		self.series = SeriesDB(database = self.gmd())
+
+	def initFromDb_SeriesDB(self, series, **kwargs):
+		self.initFromDb_dict(series.database, **kwargs)
+	def initFromDb_dict(self, d, ws = None, name = "db", data_folder = None, dropattrs = None):
+		self.setWs(ws)
+		self.series = SeriesDB(database = d)
+		self.name = versionizeName(name, self.ws._gams_databases)
+		self.g2np = g2np_
+		self.data_folder = noneInit(data_folder, os.getcwd())
+		self.dropattrs = noneInit(dropattrs, dropattrs_.copy())
+		self.initDb(None)
+	def initFromDb_NoneType(self, db, **kwargs):
+		self.initFromDb_str(db, **kwargs)
+	def initFromDb_GamsDatabase(self, db, **kwargs):
+		self.initFromDb_str(db, **kwargs)
+	def initFromDb_str(self, db, ws = None, name = "db", data_folder = None, dropattrs = None):
+		self.setWs(ws)
+		self.name = versionizeName(name, self.ws._gams_databases)
+		self.g2np = g2np_
+		self.data_folder = noneInit(data_folder, os.getcwd())
+		self.dropattrs = noneInit(dropattrs, dropattrs_.copy())
+		self.initDb(db)
+		self.series = SeriesDB(database = self.gmd())
+
+	@staticmethod
+	def initFast(name, series = None, data_folder = None, dropattrs = None):
+		""" Initialize class without the gams related attributes """
+		class Empty:
+			def __init__(self): pass
+		obj = Empty()
+		obj.__class__ = GpyDB
+		obj.name = name
+		obj.data_folder = noneInit(data_folder, os.getcwd())
+		obj.dropattrs = noneInit(dropattrs, dropattrs_.copy())
+		obj.series = noneInit(series, SeriesDB())
+		return obj
 
-	def initDbs(self,db):
-		if db is None:
-			self.database = self.ws.add_database(database_name=self.name)
-		elif type(db) is str:
-			self.database = self.ws.add_database_from_gdx(db,database_name=self.name)
-		elif isinstance(db,gams.GamsDatabase):
-			self.database = self.ws.add_database(source_database=db,database_name=self.name)
-		elif isinstance(db,GpyDB):
-			self.database = self.ws.add_database(source_database=db.database,database_name=self.name)
+	def setWs(self, ws):
+		self.ws = self.initWs(ws)
+		self.work_folder = self.ws.working_directory
+	@staticmethod
+	def initWs(ws):
+		return getattr(GpyDB, f'initWs_{ws.__class__.__name__}')(ws)
+	@staticmethod
+	def initWs_str(ws):
+		return gams.GamsWorkspace(working_directory=ws)
+	@staticmethod
+	def initWs_NoneType(ws):
+		return gams.GamsWorkspace()
+	@staticmethod
+	def initWs_GamsWorkspace(ws):
+		return ws
+
+	def initDb(self, db):
+		getattr(self, f'initDb_{db.__class__.__name__}')(db)
+		self.gmd = readGmd(self.database, self.g2np)
+		return self.database
+	def initDb_NoneType(self, db):
+		self.database = self.ws.add_database(database_name=self.name)
+	def initDb_str(self, db):
+		self.database = self.ws.add_database_from_gdx(db, database_name=self.name)
+	def initDb_GamsDatabase(self, db):
+		self.database = self.ws.add_database(source_database = db, database_name = self.name)
+	def initDb_GpyDB(self, db):
+		self.database = self.ws.add_database(source_database=db.database, database_name=self.name)
 
 	def readAlias(self, alias = None):
 		if isinstance(alias, pd.MultiIndex):
 			return alias.set_names(['alias_set','alias_map2'])
 		else:
 			if alias is None:
 				alias = []
@@ -98,40 +138,35 @@
 			self.series['alias_'] = alias
 		else:
 			self.series['alias_'] = self('alias_').union(alias)
 		self.series['alias_set'] = self('alias_').get_level_values('alias_set').unique()
 		self.series['alias_map2'] = self('alias_').get_level_values('alias_map2').unique()
 
 	def __getstate__(self):
-		if 'database' not in self.exportSettings['dropattrs']:
-			self.database.export(self.exportSettings['data_folder']+'\\'+self.name+'.gdx')
-		return {key: value for key,value in self.__dict__.items() if key not in (self.exportSettings['dropattrs']+['database'])}
+		if 'database' not in self.dropattrs:
+			self.database.export(os.path.join(self.data_folder,self.name))
+		return {key: value for key,value in self.__dict__.items() if key not in (self.dropattrs+['database'])}
 
 	def __setstate__(self,dict_):
+		""" Don't include ws. Don't include db. """
 		self.__dict__ = dict_
-		try:
-			self.ws = gams.GamsWorkspace(working_directory=self.work_folder)
-		except FileNotFoundError:
-			self.ws = gams.GamsWorkspace(working_directory=os.getcwd())
-		self.g2np = gams2numpy.Gams2Numpy(self.ws.system_directory)
-		if 'database' not in self.exportSettings['dropattrs']:
-			self.database = self.ws.add_database_from_gdx(os.path.join(self.exportSettings['data_folder'],self.name+'.gdx'))
-		else:
-			self.database = self.ws.add_database()
-		if 'gmd' in self.exportSettings['dropattrs']:
-			self.gmd = readGmd(self.database, self.g2np)
-		if 'series' in self.exportSettings['dropattrs']:
-			self.series = SeriesDB(database=self.gmd())
-	
+		self.g2np = g2np_
+		if not os.path.exists(self.work_folder):
+			self.work_folder = os.getcwd()
+		self.database = None if 'database' in self.dropattrs else os.path.join(self.data_folder, f'{self.name}.gdx')
+
 	def export(self,name=None,repo=None):
 		name = self.name if name is None else name
-		repo = self.exportSettings['data_folder'] if repo is None else repo
-		with open(repo+'\\'+name, "wb") as file:
+		repo = self.data_folder if repo is None else repo
+		with open(os.path.join(repo,name), "wb") as file:
 			pickle.dump(self,file)
 
+	def copy(self, ws = None, **kwargs):
+		return GpyDB(obj = self, ws = ws, **kwargs)
+
 	###################################################################################################
 	###								1: Properties and base methods 									###
 	###################################################################################################
 
 	def __iter__(self):
 		return self.series.__iter__()
 
@@ -156,16 +191,14 @@
 	@property
 	def symbols(self):
 		return self.series.database
 
 	def getTypes(self,types):
 		return {symbol.name: symbol for symbol in self.series if symbol.type in types}
 
-	def copy(self):
-		return deepcopy(self)
 
 	###################################################################################################
 	###									2: Dealing with aliases			 							###
 	###################################################################################################
 
 	@property
 	def aliasDict(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydatabases-0.1.0/pyDatabases/simpleDB/simpleDB.py` & `pydatabases-0.1.1/pyDatabases/simpleDB/simpleDB.py`

 * *Files identical despite different names*

### Comparing `pydatabases-0.1.0/pyDatabases.egg-info/PKG-INFO` & `pydatabases-0.1.1/pyDatabases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDatabases
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small collection of database classes based primarily pandas, secondarily scipy and GAMS.
 Home-page: https://github.com/ChampionApe/pyDatabases
 Author: Rasmus K. Skjødt Berg
 Author-email: rasmus.kehlet.berg@econ.ku.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
```

### Comparing `pydatabases-0.1.0/setup.py` & `pydatabases-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
   long_description = file.read()
 
 setuptools.setup(
   name="pyDatabases",
-  version="0.1.0",
+  version="0.1.1",
   author="Rasmus K. Skjødt Berg",
   author_email="rasmus.kehlet.berg@econ.ku.dk",
   description="Small collection of database classes based primarily pandas, secondarily scipy and GAMS.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ChampionApe/pyDatabases",
   packages=setuptools.find_packages(),
```

