# Comparing `tmp/mongo_objects-1.0.19.tar.gz` & `tmp/mongo_objects-1.0.22.tar.gz`

## Comparing `mongo_objects-1.0.19.tar` & `mongo_objects-1.0.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/requirements.txt
--rw-r--r--   0        0        0    26853 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/conftest.py
--rw-r--r--   0        0        0    27835 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    31199 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    27066 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tests/test_proxy_combo.py
--rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tools/buildProject
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tools/runTests
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tools/setupPythonVenv
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/tools/updateRequirements
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/.hgignore
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/pyproject.toml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mongo_objects-1.0.19/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/requirements.txt
+-rw-r--r--   0        0        0    30263 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/src/mongo_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/conftest.py
+-rw-r--r--   0        0        0    27835 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    31199 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    30057 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_proxy_combo.py
+-rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/buildProject
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/runTests
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/setupPythonVenv
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/updateRequirements
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/.hgignore
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/README.md
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/pyproject.toml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/PKG-INFO
```

### Comparing `mongo_objects-1.0.19/src/mongo_objects.py` & `mongo_objects-1.0.22/src/mongo_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 ################################################################################
 # Custom exceptions
 ################################################################################
 
 class MongoObjectReadOnly( Exception ):
     pass
 
+class MongoObjectAuthFailed( Exception ):
+    pass
+
 
 ################################################################################
 # MongoDB document wrappers
 ################################################################################
 
 
 class MongoUserDict( UserDict ):
@@ -50,54 +53,116 @@
 
     def __init__( self, doc={}, readonly=False ):
         '''Initialize the custom UserDict object
         Flag readonly objects appropriately'''
         super().__init__( doc )
         self.readonly = readonly
 
+        # Authorize creating this object prior to returning to the user
+        if not self.authorize_init():
+            raise MongoObjectAuthFailed
+
+
+    # Authorization hooks()
+    # The user may call these hooks to authorize various CRUD operations
+    def authorize_init( self ):
+        '''Called after the document object is initialized but
+        before it is returned to the user.
+        If the return value is not truthy, an exception is raised.'''
+        return True
+
+    def authorize_delete( self ):
+        '''Called before the current document is deleted.
+        If the return value is not truthy, an exception is raised.'''
+        return True
+
+    @classmethod
+    def authorize_pre_read( cls ):
+        '''Called before a read operation is performed.
+        This is a class method as no data has been read and no
+        document object has been created.
+        If the return value is not truthy, an exception is raised.'''
+        return True
+
+    def authorize_read( self ):
+        '''Called after a document has been read but before the
+        data is returned to the user.
+        If the return value is not truthy, the data will
+        not be returned.
+
+        Note that if find_one() only inspects the first document
+        returned by the underlying MongoDB find_one() call. If the
+        document returned does not pass authorization, no attempt is
+        made to locate another matching document.'''
+        return True
+
+    def authorize_save( self ):
+        '''Called before the current document is saved.
+        If the return value is not truthy, an exception is raised.'''
+        return True
+
 
     @classmethod
     def collection( cls ):
         '''Return the collection object from the active database for the named collection'''
         return cls.database.get_collection( cls.collection_name )
 
 
     def delete( self ):
         '''Delete the current object
         Remove the id so save() will know this is a new object if we try to re-save.'''
         if '_id' in self:
+            # Authorize deleting this object
+            if not self.authorize_delete():
+                raise MongoObjectAuthFailed
             self.collection().find_one_and_delete( { '_id' : ObjectId( self['_id'] ) } )
             del self['_id']
 
 
     @classmethod
     def find( cls, filter={}, projection=None, readonly=False, **kwargs ):
         '''Return matching documents as instances of this class'''
+        # Authorize reading at all
+        if not cls.authorize_pre_read():
+            raise MongoObjectAuthFailed
+
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         for doc in cls.collection().find( filter, projection, **kwargs ):
-            yield cls(doc, readonly=readonly)
+            print( "STEP 4" )
+            obj = cls(doc, readonly=readonly)
+            # Authorize reading this particular document object before returning it
+            if obj.authorize_read():
+                yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=False, noMatch=None, **kwargs ):
         '''Return a single matching document as an instance of this class or None'''
+        # Authorize reading at all
+        if not cls.authorize_pre_read():
+            raise MongoObjectAuthFailed
+
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
-            return cls(doc, readonly=readonly)
-        return None
+            obj = cls(doc, readonly=readonly)
+            # Authorize reading this particular document object before returning it
+            if obj.authorize_read():
+                return obj
+        return noMatch
 
 
     def getUniqueInteger( self, autosave=True ):
         '''Provide the next unique integer for this document.
         These integers are convenient for use as keys of subdocuments.
+        Start with 1; 0 is reserved for single proxy documents which don't have a key.
         By default, the document is saved.'''
         self.setdefault( '_lastUniqueInteger', 0 )
         self['_lastUniqueInteger'] += 1
         if autosave:
             self.save()
         return self['_lastUniqueInteger']
 
@@ -152,14 +217,18 @@
         1) Documents without an _id are inserted into the database; MongoDB will assign the ID
         2) If force is set, document will be saved regardless of update time or even if it exists.
            This is useful for upserting document from another database.
         3) Otherwise, only a document with this _id and _updated timestamp will be replaced.
            This protects against overwriting documents that have been updated elsewhere.
         '''
 
+        # authorize saving this document
+        if not self.authorize_save():
+            raise MongoObjectAuthFailed
+
         # refuse to save a read-only document
         if self.readonly:
             raise MongoObjectReadOnly( f"Can't save readonly object {type(self)} at {id(self)}" )
 
         # set updated timestamp
         # Note the original value in case we need to roll back
         addedUpdated = '_updated' not in self
@@ -247,31 +316,45 @@
         except Exception as e:
             raise Exception( 'PolymorphicMongoUserDict(): unable to register subclass' ) from e
 
 
     @classmethod
     def find( cls, filter={}, projection=None, readonly=False, **kwargs ):
         '''Return matching documents as appropriate subclass instances'''
+        # Authorize reading at all
+        if not cls.authorize_pre_read():
+            raise MongoObjectAuthFailed
+
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         for doc in cls.collection().find( filter, projection, **kwargs ):
-            yield cls.instantiate(doc, readonly=readonly)
+            obj = cls.instantiate(doc, readonly=readonly)
+            # Authorize reading this particular document object before returning it
+            if obj.authorize_read():
+                yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=False, noMatch=None, **kwargs ):
         '''Return a single matching document as the appropriate subclass or None'''
+        # Authorize reading at all
+        if not cls.authorize_pre_read():
+            raise MongoObjectAuthFailed
+
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
-            return cls.instantiate( doc, readonly=readonly )
-        return None
+            obj = cls.instantiate( doc, readonly=readonly )
+            # Authorize reading this particular document object before returning it
+            if obj.authorize_read():
+                return obj
+        return noMatch
 
 
     @classmethod
     def getSubclassByKey( cls, subclassKey ):
         '''Look up a subclass in the subclassMap by its subclassKey
         If the subclass can't be located, return the base class'''
         return cls.subclassMap.get( subclassKey, cls )
@@ -679,19 +762,14 @@
     within a parent MongoDB dictionary.
 
     This is really just AccessDictProxy with the parent MongoDB document as the container.
 
     Keys must be strings as required by MongoDB documents.
     '''
 
-    def getSubdocContainer( self ):
-        '''For a single subdocument dictionary, the container is the parent document.'''
-        return self.parent
-
-
     @classmethod
     def create( cls, parent, subdoc={}, key=None, autosave=True ):
         '''Add a new single subdocument dictionary to the parent object.
         No new key is auto-assigned as single subdocuments are assigned to fixed keys.
         The key can be defined in the class as "containerName"
         or overriden on the command line as "key".
         Return the new proxy object.
@@ -708,17 +786,31 @@
     def getProxies( cls, parent ):
         '''getProxies() doesn't make sense for single proxy use.
         This is a class method and we don't know the key, so
         we don't know which of the parent's subdocuments to return'''
         raise Exception( 'single proxy objects do not support getProxies()' )
 
 
+    def getSubdocContainer( self ):
+        '''For a single subdocument dictionary, the container is the parent document.'''
+        return self.parent
+
+
+    def id( self ):
+        '''Force the subdocument ID for single proxies to "0". We
+        can't use the actual key as we risk exposing the actual
+        dictionary key name.'''
+        return f"{self.parent.id()}{self.ultimateParent.subdocKeySep}0"
+
+
+
+
 
 
-class MongoSingleProxy( MongoBaseProxy, AccessSingleProxy ):
+class MongoSingleProxy( AccessSingleProxy, MongoBaseProxy ):
     '''Implement proxy object for a single subdocument dictionary'''
 
     @classmethod
     def getProxy( cls, parent, key=None ):
         '''Return a single proxy object. For non-polymorphic use,
         this simply calls __init__()'''
         if key is None:
```

### Comparing `mongo_objects-1.0.19/tests/test_MongoDictProxy.py` & `mongo_objects-1.0.22/tests/test_MongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tests/test_MongoListProxy.py` & `mongo_objects-1.0.22/tests/test_MongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tests/test_MongoSingleProxy.py` & `mongo_objects-1.0.22/tests/test_MongoSingleProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,21 +721,21 @@
         # verify data location
         assert id( proxyA1.getSubdocContainer() ) == id( proxyA1.parent )
 
 
     def test_id( self, getSampleProxyA ):
         '''Test ID for single level proxy'''
         proxy = getSampleProxyA
-        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdocKeySep}0"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
         '''Test ID for two-level proxy'''
         proxy = getSampleProxyA1
-        assert proxy.id() == f"{proxy.ultimateParent.id()}{proxy.ultimateParent.subdocKeySep}{proxy.parent.key}{proxy.ultimateParent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.ultimateParent.id()}{proxy.ultimateParent.subdocKeySep}0{proxy.ultimateParent.subdocKeySep}0"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey, getSampleProxyA1Key ):
         '''Test initialization of single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
         keyA = getSampleProxyAKey
```

### Comparing `mongo_objects-1.0.19/tests/test_MongoUserDict.py` & `mongo_objects-1.0.22/tests/test_MongoUserDict.py`

 * *Files 22% similar despite different names*

```diff
@@ -271,14 +271,33 @@
         assert result.readonly is True
 
         # saving a readonly document produces an exception
         with pytest.raises( Exception ):
             result.save()
 
 
+    def test_save_no_auth( self, getPopulatedMMUDClass ):
+        '''Test attempting to save a document without authorization'''
+        class LocalMMUD( getPopulatedMMUDClass):
+            def authorize_save( self ):
+                return False
+
+        obj = LocalMMUD.find_one()
+        original = dict( obj )
+
+        # verify saving a document without authorization produces an exception
+        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+            obj.save()
+
+        # verify nothing was saved
+        assert obj['_updated'] == original['_updated']
+
+
+
+
 class TestDelete:
     '''Test MongoUserDict.delete() in its own database'''
 
     def test_delete( self, getMMUDClass, sampleData ):
         MMUD = getMMUDClass
 
         # save the first record
@@ -314,14 +333,34 @@
         # delete the object
         obj.delete()
 
         # verify the database document count hasn't changed
         assert count == MMUD.collection().count_documents( {} )
 
 
+    def test_delete_no_auth( self, getPopulatedMMUDClass ):
+        '''Test attempting to delete a document without authorization'''
+        class LocalMMUD( getPopulatedMMUDClass):
+            def authorize_delete( self ):
+                return False
+
+        obj = LocalMMUD.find_one()
+
+        # note the number of documents in the database
+        count = LocalMMUD.collection().count_documents( {} )
+
+        # verify deleting a document without authorization produces an exception
+        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+            obj.delete()
+
+        # verify the database document count hasn't changed
+        assert count == LocalMMUD.collection().count_documents( {} )
+
+
+
 
 class TestBasics:
     '''Test all other functionality of MongoUserDict'''
 
     def test_init( self, getMMUDClass, sampleData ):
         MMUD = getMMUDClass
         obj = MMUD( sampleData[0] )
@@ -346,14 +385,24 @@
     def test_init_empty_readonly( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD(readonly=True)
         assert len(obj.data) == 0
         assert obj.readonly is True
 
 
+    def test_init_no_auth( self, getMMUDClass, sampleData ):
+        class LocalMMUD( getMMUDClass):
+            def authorize_init( self ):
+                return False
+
+        # verify initializing a document without authorization produces an exception
+        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+            obj = LocalMMUD( sampleData[0] )
+
+
     def test_collection( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
         assert isinstance( MMUD.collection(), Collection )
 
 
     def test_find_all( self, getPopulatedMMUDClass, sampleData ):
         MMUD = getPopulatedMMUDClass
@@ -465,35 +514,92 @@
         result = list( MMUD.find( readonly=True ) )
 
         # verify all objects are marked readonly
         for x in result:
             assert x.readonly is True
 
 
+    def test_find_no_pre_auth( self, getPopulatedMMUDClass ):
+        '''Test attempting to read without pre-authorization'''
+        class LocalMMUD( getPopulatedMMUDClass ):
+            @classmethod
+            def authorize_pre_read( cls ):
+                return False
+
+        # verify reading documents without pre-read authorization produces an exception
+        # must convert to a list or the generator is never called
+        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+            list( LocalMMUD.find() )
+
+
+    def test_find_no_auth_1( self, getPopulatedMMUDClass ):
+        '''Test attempting to read without authorization'''
+        class LocalMMUD( getPopulatedMMUDClass):
+            def authorize_read( self ):
+                return False
+
+        # verify reading documents without read authorization produces an empty list
+        result = LocalMMUD.find()
+        assert len( list( result ) ) == 0
+
+
+    def test_find_no_auth_2( self, getPopulatedMMUDClass ):
+        '''Test attempting to read without authorization for certain objects'''
+
+        # first collect a list of object IDs
+        ids = [ x.id() for x in getPopulatedMMUDClass.find() ]
+
+        # create a class authorized to read all but the first ID
+        class LocalMMUD( getPopulatedMMUDClass):
+            def authorize_read( self ):
+                return self.id() != ids[0]
+
+        # read all documents with the new custom class
+        ids2 = [ x.id() for x in LocalMMUD.find() ]
+        # construct a list of all ids missing from the second find() call
+        diff = list( set(ids).difference( ids2 ) )
+        # verify that only ids[0] is missing (the ID excluded by authorize_read() )
+        assert len( diff ) == 1
+        assert diff[0] == ids[0]
+
+
     def test_find_one( self, getPopulatedMMUDClass ):
         '''Test returning a single (random) object'''
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one()
         assert isinstance( result, MMUD )
         assert '_id' in result
         assert '_created' in result
         assert '_updated' in result
         assert 'amount' in result
         assert 'name' in result
         assert result.readonly is False
 
 
     def test_find_one_none( self, getPopulatedMMUDClass ):
+        '''Verify a non-matching filter produces a None result'''
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' } )
 
         # verify that we found nothing
         assert result is None
 
 
+    def test_find_one_none_custom_return( self, getPopulatedMMUDClass ):
+        '''Verify a non-matching filter produces our custom "noMatch" result'''
+        MMUD = getPopulatedMMUDClass
+
+        class EmptyResponse( object ):
+            pass
+
+        result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' }, noMatch=EmptyResponse() )
+
+        assert isinstance( result, EmptyResponse )
+
+
     def test_find_one_filter( self, getPopulatedMMUDClass, sampleData ):
         '''Use a filter to find a specific single record, in this case, the third sample by name'''
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( { 'name' : sampleData[2]['name'] } )
 
         # verify that we found the right record
         assert result['name'] == sampleData[2]['name']
@@ -559,14 +665,37 @@
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( readonly=True )
 
         # verify object are marked readonly
         result.readonly is True
 
 
+    def test_find_one_no_pre_auth( self, getPopulatedMMUDClass ):
+        '''Test attempting to read without pre-authorization'''
+        class LocalMMUD( getPopulatedMMUDClass ):
+            @classmethod
+            def authorize_pre_read( cls ):
+                return False
+
+        # verify reading a document without pre-read authorization produces an exception
+        with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
+            LocalMMUD.find_one()
+
+
+    def test_find_one_no_auth( self, getPopulatedMMUDClass ):
+        '''Test attempting to read without authorization'''
+        class LocalMMUD( getPopulatedMMUDClass):
+            def authorize_read( self ):
+                return False
+
+        # verify reading documents without read authorization produces an empty list
+        result = LocalMMUD.find_one()
+        assert result is None
+
+
     def test_getUniqueInteger( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD()
         startTime = MMUD.utcnow()
 
         # verify new object doesn't have a _lastUniqueInteger
         # an _id, a created or an update time
```

### Comparing `mongo_objects-1.0.19/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.0.22/tests/test_PolymorphicMongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.0.22/tests/test_PolymorphicMongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.0.22/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tests/test_proxy_combo.py` & `mongo_objects-1.0.22/tests/test_proxy_combo.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tools/buildProject` & `mongo_objects-1.0.22/tools/buildProject`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tools/runTests` & `mongo_objects-1.0.22/tools/runTests`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/tools/setupPythonVenv` & `mongo_objects-1.0.22/tools/setupPythonVenv`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/pyproject.toml` & `mongo_objects-1.0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.19/PKG-INFO` & `mongo_objects-1.0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mongo_objects
-Version: 1.0.19
+Version: 1.0.22
 Summary: Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects.
 Project-URL: Homepage, https://headwaters.com.sg/pycon-2023
 Author-email: Jonathan Lindstrom <lindstrom.j@headwaters.com.sg>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

