# Comparing `tmp/nakalapycon-0.0.7.tar.gz` & `tmp/nakalapycon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakalapycon-0.0.7.tar", last modified: Tue Feb 14 16:10:28 2023, max compression
+gzip compressed data, was "nakalapycon-0.0.9.tar", last modified: Thu Apr 18 14:32:32 2024, max compression
```

## Comparing `nakalapycon-0.0.7.tar` & `nakalapycon-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 16:10:28.951473 nakalapycon-0.0.7/
--rw-rw-rw-   0        0        0    35780 2021-07-15 15:28:17.000000 nakalapycon-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     6978 2023-02-14 16:10:28.951473 nakalapycon-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6119 2022-11-15 09:59:42.000000 nakalapycon-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 16:10:28.821684 nakalapycon-0.0.7/nakalapycon/
-drwxrwxrwx   0        0        0        0 2023-02-14 16:10:28.946427 nakalapycon-0.0.7/nakalapycon/src/
--rw-rw-rw-   0        0        0     1790 2021-10-22 07:46:32.000000 nakalapycon-0.0.7/nakalapycon/src/NklResponse.py
--rw-rw-rw-   0        0        0     1601 2021-07-16 08:13:11.000000 nakalapycon-0.0.7/nakalapycon/src/NklTarget.py
--rw-rw-rw-   0        0        0     4540 2021-08-18 09:03:09.000000 nakalapycon-0.0.7/nakalapycon/src/constantes.py
-drwxrwxrwx   0        0        0        0 2023-02-14 16:10:28.861790 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/
--rw-rw-rw-   0        0        0     6978 2023-02-14 16:10:28.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-02-14 16:10:28.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 16:10:28.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-14 16:10:28.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/requires.txt
--rw-rw-rw-   0        0        0      161 2023-02-14 16:10:28.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      612 2022-11-18 09:46:38.000000 nakalapycon-0.0.7/nakalapycon/src/nakalapycon.py
--rw-rw-rw-   0        0        0    14686 2021-10-22 07:46:33.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Collections.py
--rw-rw-rw-   0        0        0    56518 2022-08-29 08:59:17.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Datas.py
--rw-rw-rw-   0        0        0    12963 2021-10-22 07:46:33.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Groups.py
--rw-rw-rw-   0        0        0     7218 2022-05-25 15:06:59.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Search.py
--rw-rw-rw-   0        0        0     2488 2021-10-22 07:46:33.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Users.py
--rw-rw-rw-   0        0        0    11488 2021-10-22 07:46:33.000000 nakalapycon-0.0.7/nakalapycon/src/nklAPI_Vocabularies.py
--rw-rw-rw-   0        0        0    10469 2021-10-22 09:17:41.000000 nakalapycon-0.0.7/nakalapycon/src/nklPullCorpus.py
--rw-rw-rw-   0        0        0     9012 2022-12-02 10:23:31.000000 nakalapycon-0.0.7/nakalapycon/src/nklUtils.py
--rw-rw-rw-   0        0        0       42 2023-02-14 16:10:28.951473 nakalapycon-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1998 2023-02-14 16:00:37.000000 nakalapycon-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:32:32.566246 nakalapycon-0.0.9/
+-rw-rw-rw-   0        0        0    35780 2021-07-15 15:28:17.000000 nakalapycon-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6978 2024-04-18 14:32:32.566246 nakalapycon-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6119 2022-11-15 09:59:42.000000 nakalapycon-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 14:32:32.543291 nakalapycon-0.0.9/nakalapycon/
+drwxrwxrwx   0        0        0        0 2024-04-18 14:32:32.564246 nakalapycon-0.0.9/nakalapycon/src/
+-rw-rw-rw-   0        0        0     1790 2021-10-22 07:46:32.000000 nakalapycon-0.0.9/nakalapycon/src/NklResponse.py
+-rw-rw-rw-   0        0        0     1601 2021-07-16 08:13:11.000000 nakalapycon-0.0.9/nakalapycon/src/NklTarget.py
+-rw-rw-rw-   0        0        0     4540 2021-08-18 09:03:09.000000 nakalapycon-0.0.9/nakalapycon/src/constantes.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:32:32.551404 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/
+-rw-rw-rw-   0        0        0     6978 2024-04-18 14:32:32.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-18 14:32:32.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:32:32.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 14:32:32.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      161 2024-04-18 14:32:32.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      612 2022-11-18 09:46:38.000000 nakalapycon-0.0.9/nakalapycon/src/nakalapycon.py
+-rw-rw-rw-   0        0        0    14686 2021-10-22 07:46:33.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Collections.py
+-rw-rw-rw-   0        0        0    56518 2022-08-29 08:59:17.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Datas.py
+-rw-rw-rw-   0        0        0    12963 2021-10-22 07:46:33.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Groups.py
+-rw-rw-rw-   0        0        0     7218 2022-05-25 15:06:59.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Search.py
+-rw-rw-rw-   0        0        0     2488 2021-10-22 07:46:33.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Users.py
+-rw-rw-rw-   0        0        0    11488 2021-10-22 07:46:33.000000 nakalapycon-0.0.9/nakalapycon/src/nklAPI_Vocabularies.py
+-rw-rw-rw-   0        0        0    11929 2024-04-18 14:01:53.000000 nakalapycon-0.0.9/nakalapycon/src/nklPullCorpus.py
+-rw-rw-rw-   0        0        0     9012 2022-12-02 10:23:31.000000 nakalapycon-0.0.9/nakalapycon/src/nklUtils.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:32:32.566246 nakalapycon-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1998 2024-04-18 14:31:55.000000 nakalapycon-0.0.9/setup.py
```

### Comparing `nakalapycon-0.0.7/LICENSE` & `nakalapycon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/PKG-INFO` & `nakalapycon-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakalapycon
-Version: 0.0.7
+Version: 0.0.9
 Summary: Librairie Python pour interagir avec Nakala (Nakala est un entrepôt de données de recherche en SHS développé par Huma-Num)
 Home-page: https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon
 Author: Michael Nauge
 Project-URL: Issues, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/issues
 Project-URL: CI, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/pipelines
 Project-URL: Changelog, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nakalapycon-0.0.7/README.md` & `nakalapycon-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/NklResponse.py` & `nakalapycon-0.0.9/nakalapycon/src/NklResponse.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/NklTarget.py` & `nakalapycon-0.0.9/nakalapycon/src/NklTarget.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/constantes.py` & `nakalapycon-0.0.9/nakalapycon/src/constantes.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/PKG-INFO` & `nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakalapycon
-Version: 0.0.7
+Version: 0.0.9
 Summary: Librairie Python pour interagir avec Nakala (Nakala est un entrepôt de données de recherche en SHS développé par Huma-Num)
 Home-page: https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon
 Author: Michael Nauge
 Project-URL: Issues, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/issues
 Project-URL: CI, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/pipelines
 Project-URL: Changelog, https://gitlab.huma-num.fr/mshs-poitiers/plateforme/nakalapycon/-/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nakalapycon.egg-info/SOURCES.txt` & `nakalapycon-0.0.9/nakalapycon/src/nakalapycon.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,12 @@
 nakalapycon/src/nklAPI_Datas.py
 nakalapycon/src/nklAPI_Groups.py
 nakalapycon/src/nklAPI_Search.py
 nakalapycon/src/nklAPI_Users.py
 nakalapycon/src/nklAPI_Vocabularies.py
 nakalapycon/src/nklPullCorpus.py
 nakalapycon/src/nklUtils.py
-nakalapycon/src/nakalapycon.egg-info/SOURCES.txt
+nakalapycon/src/nakalapycon.egg-info/PKG-INFO
+nakalapycon/src/nakalapycon.egg-info/SOURCES.txt
+nakalapycon/src/nakalapycon.egg-info/dependency_links.txt
+nakalapycon/src/nakalapycon.egg-info/requires.txt
+nakalapycon/src/nakalapycon.egg-info/top_level.txt
```

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nakalapycon.py` & `nakalapycon-0.0.9/nakalapycon/src/nakalapycon.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Collections.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Collections.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Datas.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Datas.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Groups.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Groups.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Search.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Search.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Users.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Users.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklAPI_Vocabularies.py` & `nakalapycon-0.0.9/nakalapycon/src/nklAPI_Vocabularies.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklPullCorpus.py` & `nakalapycon-0.0.9/nakalapycon/src/nklPullCorpus.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,81 +82,108 @@
 
                 dataUri = data["uri"]
                 dataUri = dataUri.replace('https://doi.org/','')
                 
                 print(dataUri,' ', data["status"])
                 
                 dataTitle = ""
+                #'linkedInCollection','dataIdentifier','uriData',
+                #'nkl_title','nkl_created','nkl_license','nkl_type', 
+                #'nkl_type_converted','creators_formated'
                 
                 dicRowData = {}
-                dicRowData['dataIdentifier'] = dataUri
-                dicRowData['uriData'] = nklTarget.BASE_URL+"/"+dataUri
-                dicRowData['linkedInCollection'] = "not yet available in nakalapycon"
+                dicRowData['linkedInCollection'] = ["not yet available in nakalapycon"]
+                dicRowData['dataIdentifier'] = [dataUri]
+                dicRowData['uriData'] = [nklTarget.BASE_URL+"/"+dataUri]
+                dicRowData['nkl_title'] = [""]
+                dicRowData['nkl_created'] = [""]
+                dicRowData['nkl_license'] = [""]
+                dicRowData['nkl_type'] = [""]
+                dicRowData['nkl_type_converted'] = [""]
+                dicRowData['creators_formated'] = [""]
+
                 
                 if 'collectionsIds' in data:
                     print(data["collectionsIds"])
                 
-                dicRowData['creators_formated'] = ""
                 
                 for meta in data['metas']:
                     #print(meta['value'], " ", meta['propertyUri'])
                     
                     if meta['propertyUri'] == 'http://nakala.fr/terms#title':
                         #print("title :", meta['value'])
                         dataTitle = meta['value']
-                        dicRowData['nkl_title'] = dataTitle
+                        dicRowData['nkl_title'] = [dataTitle]
                       
                     if meta['propertyUri'] == 'http://nakala.fr/terms#created':
-                        dicRowData['nkl_created'] = meta['value']
+                        dicRowData['nkl_created'] = [meta['value']]
                         
                     if meta['propertyUri'] == 'http://nakala.fr/terms#license':
-                        dicRowData['nkl_license'] = meta['value']
+                        dicRowData['nkl_license'] = [meta['value']]
                       
                     
                     if meta['propertyUri'] == "http://nakala.fr/terms#type":
-                        dicRowData['nkl_type'] = meta['value']
+                        dicRowData['nkl_type'] = [meta['value']]
                         
                         #dicRowData['nkl_type_converted'] = myConst.vocabTypeGetKeyByUri(meta['value'])  
-                        dicRowData['nkl_type_converted'] = ""  
+                        dicRowData['nkl_type_converted'] = [""]
                         
                     if meta['propertyUri'] == "http://nakala.fr/terms#creator":
                         
                         #les anciennes data nakala n'avait pas la meme structuration pour le type creator
                         if not (meta['value']==None):
                             
                             if isinstance(meta['value'], dict):
                                 formattedName = meta['value']['givenname']+" "+meta['value']['surname']
                                 
-                                if dicRowData['creators_formated'] == "":
-                                    dicRowData['creators_formated'] = formattedName
+                                if dicRowData['creators_formated'] == [""]:
+                                    dicRowData['creators_formated'] = [formattedName]
                                 else:
-                                    dicRowData['creators_formated'] += ", "+formattedName
+                                    dicRowData['creators_formated'][0] += ", "+formattedName
                             else:
-                                if dicRowData['creators_formated'] == "":
-                                    dicRowData['creators_formated'] = meta['value']
+                                if dicRowData['creators_formated'] == [""]:
+                                    dicRowData['creators_formated'] = [meta['value']]
                                 else:
-                                    dicRowData['creators_formated'] += ", "+meta['value']
-                                
+                                    dicRowData['creators_formated'][0] += ", "+meta['value']
                                 
-                        
-                dfData = dfData.append(dicRowData, ignore_index=True) 
+                             
+                #obsolete       
+                #dfData = dfData.append(dicRowData, ignore_index=True) 
+                dfRowData = pd.DataFrame(data=dicRowData)
+
+
+                dfData = pd.concat([dfData, dfRowData])
+                
                 
                 for file in data['files']:
                     #print(file['name'], file['extension'],file['size'],file['mime_type'],file['sha1'],file['embargoed'],file['description'])
                     #print(">> uriFile", myConst.API_URL+"/data/"+dataUri+"/"+file['sha1'])
-                    dicRowFile = file.copy()
-                    #dicRowFile = {}
-                    dicRowFile['linkedInData'] = dataUri
-                    dicRowFile['linkedInData_Title'] = dataTitle
-                    dicRowFile['uriData'] = nklTarget.BASE_URL+"/"+dataUri
-                    dicRowFile['uriFileDL'] = nklTarget.API_URL+"/data/"+dataUri+"/"+file['sha1']
-                    dicRowFile['uriFileEmbed'] = nklTarget.API_URL+"/embed/"+dataUri+"/"+file['sha1']
+                    #dicRowFile = file.copy()
+                    #'linkedInData','linkedInData_Title','uriData',
+                    #'name','uriFileDL','description','size','extension',
+                    #'sha1','mime_type','embargoed','uriFileEmbed'
                     
-                    dfFile = dfFile.append(dicRowFile, ignore_index=True)
-                        
+                    dicRowFile = {}
+                    dicRowFile['linkedInData'] = [dataUri]
+                    dicRowFile['linkedInData_Title'] = [dataTitle]
+                    dicRowFile['uriData'] = [nklTarget.BASE_URL+"/"+dataUri]
+                    dicRowFile['name'] = [file['name']]
+                    dicRowFile['uriFileDL'] = [nklTarget.API_URL+"/data/"+dataUri+"/"+file['sha1']]
+                    dicRowFile['description'] = [file['description']]
+                    dicRowFile['size'] = [file['size']]
+                    dicRowFile['extension'] = [file['extension']]
+                    dicRowFile['sha1'] = file['sha1']
+                    dicRowFile['mime_type'] = file['mime_type']
+                    dicRowFile['embargoed'] = file['embargoed']
+                    dicRowFile['uriFileEmbed'] = [nklTarget.API_URL+"/embed/"+dataUri+"/"+file['sha1']]
+                    
+                    #obsolete
+                    #dfFile = dfFile.append(dicRowFile, ignore_index=True)
+                    dfRowFile = pd.DataFrame(data=dicRowFile)
+                    dfFile = pd.concat([dfFile, dfRowFile])                        
         else:
             lastPage = 0
 
     
     return dfData, dfFile
```

### Comparing `nakalapycon-0.0.7/nakalapycon/src/nklUtils.py` & `nakalapycon-0.0.9/nakalapycon/src/nklUtils.py`

 * *Files identical despite different names*

### Comparing `nakalapycon-0.0.7/setup.py` & `nakalapycon-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 import setuptools
 
-VERSION = "0.0.7"
+VERSION = "0.0.9"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nakalapycon",                     # This is the name of the package
     version=VERSION,                        # The initial release version
```

