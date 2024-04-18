# Comparing `tmp/SplatStats-4.1.1.tar.gz` & `tmp/SplatStats-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-4.1.1.tar", last modified: Sat Mar  2 21:17:35 2024, max compression
+gzip compressed data, was "SplatStats-4.2.1.tar", last modified: Thu Apr 18 16:39:18 2024, max compression
```

## Comparing `SplatStats-4.1.1.tar` & `SplatStats-4.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-02 21:17:35.880934 SplatStats-4.1.1/
--rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 02:43:58.000000 SplatStats-4.1.1/LICENSE
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-03-02 21:17:35.880636 SplatStats-4.1.1/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6370 2024-02-19 02:43:58.000000 SplatStats-4.1.1/README.md
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-02 21:17:35.879124 SplatStats-4.1.1/SplatStats/
--rw-r--r--   0 chipdelmal   (501) staff       (20)    10828 2024-02-19 02:43:58.000000 SplatStats-4.1.1/SplatStats/Battle.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    11409 2024-02-28 02:56:43.000000 SplatStats-4.1.1/SplatStats/Player.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     3107 2024-02-28 03:12:16.000000 SplatStats-4.1.1/SplatStats/StatInk.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     2477 2024-02-19 02:43:58.000000 SplatStats-4.1.1/SplatStats/Team.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)      896 2024-02-19 02:43:58.000000 SplatStats-4.1.1/SplatStats/__init__.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)       21 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats/_version.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6148 2024-02-19 02:43:58.000000 SplatStats-4.1.1/SplatStats/auxiliary.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    14521 2024-02-21 04:08:00.000000 SplatStats-4.1.1/SplatStats/colors.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6156 2024-03-01 03:27:11.000000 SplatStats-4.1.1/SplatStats/constants.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     4137 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/files.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     8968 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/parsers.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    59659 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/plots.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1428 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/plotsAux.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1707 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/plotsTeam.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    13586 2024-03-02 19:09:10.000000 SplatStats-4.1.1/SplatStats/statInkConstants.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    10922 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/statInkPlots.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     8511 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/statInkStats.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    15022 2024-02-19 02:43:59.000000 SplatStats-4.1.1/SplatStats/stats.py
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-03-02 21:17:35.880018 SplatStats-4.1.1/SplatStats.egg-info/
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)      607 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)      159 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)       11 2024-03-02 21:17:35.000000 SplatStats-4.1.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-03-02 21:17:35.880994 SplatStats-4.1.1/setup.cfg
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1251 2024-02-19 02:43:59.000000 SplatStats-4.1.1/setup.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.706938 SplatStats-4.2.1/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 02:43:58.000000 SplatStats-4.2.1/LICENSE
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-18 16:39:18.706619 SplatStats-4.2.1/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6370 2024-02-19 02:43:58.000000 SplatStats-4.2.1/README.md
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.705056 SplatStats-4.2.1/SplatStats/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    10828 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/Battle.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    11409 2024-02-28 02:56:43.000000 SplatStats-4.2.1/SplatStats/Player.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     3107 2024-02-28 03:12:16.000000 SplatStats-4.2.1/SplatStats/StatInk.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     2477 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/Team.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      896 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/__init__.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       21 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats/_version.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6148 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/auxiliary.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    14521 2024-02-21 04:08:00.000000 SplatStats-4.2.1/SplatStats/colors.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6156 2024-03-01 03:27:11.000000 SplatStats-4.2.1/SplatStats/constants.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     4137 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/files.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    11074 2024-03-25 03:13:54.000000 SplatStats-4.2.1/SplatStats/parsers.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    59659 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plots.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1428 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plotsAux.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1707 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plotsTeam.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    13586 2024-03-07 23:48:07.000000 SplatStats-4.2.1/SplatStats/statInkConstants.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    10922 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/statInkPlots.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     8511 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/statInkStats.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    15022 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/stats.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.705894 SplatStats-4.2.1/SplatStats.egg-info/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      607 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      159 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       11 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-04-18 16:39:18.707007 SplatStats-4.2.1/setup.cfg
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1251 2024-02-19 02:43:59.000000 SplatStats-4.2.1/setup.py
```

### Comparing `SplatStats-4.1.1/LICENSE` & `SplatStats-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/PKG-INFO` & `SplatStats-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 4.1.1
+Version: 4.2.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-4.1.1/README.md` & `SplatStats-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/Battle.py` & `SplatStats-4.2.1/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/Player.py` & `SplatStats-4.2.1/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/StatInk.py` & `SplatStats-4.2.1/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/Team.py` & `SplatStats-4.2.1/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/__init__.py` & `SplatStats-4.2.1/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/auxiliary.py` & `SplatStats-4.2.1/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/colors.py` & `SplatStats-4.2.1/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/constants.py` & `SplatStats-4.2.1/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/files.py` & `SplatStats-4.2.1/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/parsers.py` & `SplatStats-4.2.1/SplatStats/parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -251,8 +251,47 @@
         playerHistory, 
         slicer=(lambda x: "{}/{:02d}".format(
             x.isocalendar().year, x.isocalendar().week
         ))
     ):
     dteSlice = playerHistory['datetime'].apply(slicer).copy()
     playerHistory.insert(3, 'DateGroup', dteSlice)
-    return playerHistory
+    return playerHistory
+
+
+def getAlliesEnemiesDataFrames(
+        battleRecords, player, teammates,
+        STATS=(
+            'main weapon', 'sub weapon', 'special weapon', 
+            'win', 'kill', 'death', 'assist', 'paint', 'special'
+        ),
+        BATTLE=('ko', 'matchType', 'duration', 'stage', 'festMatch')
+    ):
+    (aList, eList, nBattles) = ([], [], len(battleRecords))
+    for ix in range(nBattles):
+        bRecord = battleRecords[ix]
+        (allies, enemies) = (bRecord.alliedTeam, pd.concat(bRecord.enemyTeams))
+        if player not in set(allies['player name']):
+            continue
+        # Get battle stats ----------------------------------------------------
+        bttlStats = {s: bRecord.__getattribute__(s) for s in BATTLE}
+        # Get player row and outcome ------------------------------------------
+        plyrEntry = allies[allies['player name']==player]
+        plyrStats = {s: plyrEntry[s].values[0] for s in STATS}
+        # Get if team members are present -------------------------------------
+        allyPrsnt = {n: (n in set(allies['player name'])) for n in teammates}
+        enmyPrsnt = {n: (n in set(enemies['player name'])) for n in teammates}
+        # Assemble full dictionary --------------------------------------------
+        bDicts = [bttlStats, plyrStats, allyPrsnt]
+        aList.append({k: v for d in bDicts for k, v in d.items()})
+        # Assemble full dictionary --------------------------------------------
+        bDicts = [bttlStats, plyrStats, enmyPrsnt]
+        eList.append({k: v for d in bDicts for k, v in d.items()})
+    # Generate dataframe and clean --------------------------------------------
+    dfAllies = pd.DataFrame.from_dict(aList)
+    dfAllies = dfAllies[dfAllies['win']!='NA']
+    dfAllies['win'] = dfAllies['win'].map({'W': True, 'L': False})
+    dfEnemies = pd.DataFrame.from_dict(eList)
+    dfEnemies = dfEnemies[dfEnemies['win']!='NA']
+    dfEnemies['win'] = dfEnemies['win'].map({'W': True, 'L': False})
+    # Return dataframes -------------------------------------------------------
+    return {'allies': dfAllies, 'enemies': dfEnemies}
```

### Comparing `SplatStats-4.1.1/SplatStats/plots.py` & `SplatStats-4.2.1/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/plotsAux.py` & `SplatStats-4.2.1/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/plotsTeam.py` & `SplatStats-4.2.1/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/statInkConstants.py` & `SplatStats-4.2.1/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/statInkPlots.py` & `SplatStats-4.2.1/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/statInkStats.py` & `SplatStats-4.2.1/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats/stats.py` & `SplatStats-4.2.1/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-4.2.1/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 4.1.1
+Version: 4.2.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-4.1.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-4.2.1/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-4.1.1/setup.py` & `SplatStats-4.2.1/setup.py`

 * *Files identical despite different names*

