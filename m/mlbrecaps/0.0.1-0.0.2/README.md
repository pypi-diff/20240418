# Comparing `tmp/mlbrecaps-0.0.1.tar.gz` & `tmp/mlbrecaps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbrecaps-0.0.1.tar", last modified: Fri Mar 15 02:47:33 2024, max compression
+gzip compressed data, was "mlbrecaps-0.0.2.tar", last modified: Thu Apr 18 03:24:04 2024, max compression
```

## Comparing `mlbrecaps-0.0.1.tar` & `mlbrecaps-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-02-22 16:31:39.000000 mlbrecaps-0.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1916 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1414 2024-03-15 02:42:33.000000 mlbrecaps-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/mlbrecaps/
--rw-r--r--   0 root         (0) root         (0)      449 2024-03-15 02:38:27.000000 mlbrecaps-0.0.1/mlbrecaps/__init__.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-03-15 02:38:27.000000 mlbrecaps-0.0.1/mlbrecaps/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3477 2024-03-03 22:43:45.000000 mlbrecaps-0.0.1/mlbrecaps/clip.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-03-14 20:56:42.000000 mlbrecaps-0.0.1/mlbrecaps/clips.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/mlbrecaps/data/
--rw-r--r--   0 root         (0) root         (0)     1708 2024-02-15 22:21:47.000000 mlbrecaps-0.0.1/mlbrecaps/data/team-info.csv
--rw-r--r--   0 root         (0) root         (0)     1834 2024-03-03 22:25:47.000000 mlbrecaps-0.0.1/mlbrecaps/date.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-03-03 21:46:26.000000 mlbrecaps-0.0.1/mlbrecaps/date_generator.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-24 07:41:04.000000 mlbrecaps-0.0.1/mlbrecaps/date_range.py
--rw-r--r--   0 root         (0) root         (0)     5397 2024-03-14 16:27:02.000000 mlbrecaps-0.0.1/mlbrecaps/game.py
--rw-r--r--   0 root         (0) root         (0)     3027 2024-03-03 22:55:18.000000 mlbrecaps-0.0.1/mlbrecaps/game_generator.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-03-03 22:43:33.000000 mlbrecaps-0.0.1/mlbrecaps/play.py
--rw-r--r--   0 root         (0) root         (0)     3696 2024-03-03 22:53:09.000000 mlbrecaps-0.0.1/mlbrecaps/player.py
--rw-r--r--   0 root         (0) root         (0)     1791 2024-03-15 02:38:40.000000 mlbrecaps-0.0.1/mlbrecaps/scripts.py
--rw-r--r--   0 root         (0) root         (0)     1161 2024-03-14 16:25:47.000000 mlbrecaps-0.0.1/mlbrecaps/team.py
--rw-r--r--   0 root         (0) root         (0)     1613 2024-02-27 01:22:22.000000 mlbrecaps-0.0.1/mlbrecaps/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/mlbrecaps.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1916 2024-03-15 02:47:33.000000 mlbrecaps-0.0.1/mlbrecaps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2024-03-15 02:47:33.000000 mlbrecaps-0.0.1/mlbrecaps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-15 02:47:33.000000 mlbrecaps-0.0.1/mlbrecaps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-03-15 02:47:33.000000 mlbrecaps-0.0.1/mlbrecaps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-15 02:47:33.000000 mlbrecaps-0.0.1/mlbrecaps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-15 02:47:33.314724 mlbrecaps-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1051 2024-03-15 02:18:04.000000 mlbrecaps-0.0.1/setup.py
+drwxrwxr-x   0 karsten   (1000) karsten   (1000)        0 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1070 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/LICENSE.txt
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1936 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/PKG-INFO
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1414 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/README.md
+drwxrwxr-x   0 karsten   (1000) karsten   (1000)        0 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/mlbrecaps/
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)      449 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/__init__.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)      717 2024-03-28 02:13:28.000000 mlbrecaps-0.0.2/mlbrecaps/__main__.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     3476 2024-03-29 03:42:25.000000 mlbrecaps-0.0.2/mlbrecaps/clip.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     2321 2024-03-29 03:23:33.000000 mlbrecaps-0.0.2/mlbrecaps/clips.py
+drwxrwxr-x   0 karsten   (1000) karsten   (1000)        0 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/mlbrecaps/data/
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1707 2024-03-28 20:46:11.000000 mlbrecaps-0.0.2/mlbrecaps/data/team-info.csv
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1834 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/date.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1213 2024-03-28 02:14:39.000000 mlbrecaps-0.0.2/mlbrecaps/date_generator.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)      573 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/date_range.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     5762 2024-03-29 04:36:35.000000 mlbrecaps-0.0.2/mlbrecaps/game.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     3027 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/game_generator.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1834 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/play.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     3854 2024-03-29 05:03:57.000000 mlbrecaps-0.0.2/mlbrecaps/player.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1791 2024-03-26 15:32:52.000000 mlbrecaps-0.0.2/mlbrecaps/scripts.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1195 2024-03-29 02:58:02.000000 mlbrecaps-0.0.2/mlbrecaps/team.py
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1646 2024-03-29 04:36:10.000000 mlbrecaps-0.0.2/mlbrecaps/utils.py
+drwxrwxr-x   0 karsten   (1000) karsten   (1000)        0 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/mlbrecaps.egg-info/
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1936 2024-04-18 03:24:03.000000 mlbrecaps-0.0.2/mlbrecaps.egg-info/PKG-INFO
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)      516 2024-04-18 03:24:03.000000 mlbrecaps-0.0.2/mlbrecaps.egg-info/SOURCES.txt
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)        1 2024-04-18 03:24:03.000000 mlbrecaps-0.0.2/mlbrecaps.egg-info/dependency_links.txt
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)       92 2024-04-18 03:24:03.000000 mlbrecaps-0.0.2/mlbrecaps.egg-info/requires.txt
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)       10 2024-04-18 03:24:03.000000 mlbrecaps-0.0.2/mlbrecaps.egg-info/top_level.txt
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)       38 2024-04-18 03:24:04.127033 mlbrecaps-0.0.2/setup.cfg
+-rw-rw-r--   0 karsten   (1000) karsten   (1000)     1054 2024-04-18 03:22:56.000000 mlbrecaps-0.0.2/setup.py
```

### Comparing `mlbrecaps-0.0.1/LICENSE.txt` & `mlbrecaps-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/PKG-INFO` & `mlbrecaps-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mlbrecaps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that gathers information on given MLB games
 Home-page: https://github.com/MrRedwing/MLB-Recaps
 Author: Karsten Larson
 Author-email: karsten.larson.1@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
@@ -61,7 +62,9 @@
 ### Contributing
 
 All contributions are welcomed to improve the mlbrecaps package. To contribute simply submit a pull request.
 
 ### License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+
```

### Comparing `mlbrecaps-0.0.1/README.md` & `mlbrecaps-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/clip.py` & `mlbrecaps-0.0.2/mlbrecaps/clip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 from bs4 import BeautifulSoup
 
 import requests
-import json
-import subprocess
+from pathlib import Path
 
 from .play import Play
 
+
 class Clip():
+    """A wrapper class for Play that allows for plays to be downloaded"""
 
-    def __init__(self, play: Play, broadcast_type: str | None=None):
+    def __init__(self, play: Play, broadcast_type: str | None = None):
         if not isinstance(play, Play):
             raise ValueError("Play must be a Play object")
 
         self._play: Play = play
 
-        match broadcast_type: # Enforce broad_type types
+        match broadcast_type:  # Enforce broad_type types
             case "HOME" | "AWAY" | None:
                 self.broadcast_type: str | None = broadcast_type
             case _:
-                raise ValueError("BroadcastType must be None, \"HOME\", or \"AWAY\"")
+                raise ValueError(
+                    "BroadcastType must be None, \"HOME\", or \"AWAY\"")
 
         self._clip_url: str = self.__generate()
 
     @property
     def clip_url(self) -> str:
         return self._clip_url
 
     def __str__(self) -> str:
         return self.clip_url
 
     @property
     def play(self) -> Play:
         return self._play
 
-    # gets the url of the clip to be downloaded from the savant clip
     def __get_url(self, site_url: str) -> str:
+        """
+        Gets the url of the clip to be downloaded from the savant clip
+        """
         # Get the savant site
         site: requests.Response = requests.get(site_url)
 
         # Find the video element of the savant clip, find the source url of the clip
-        soup= BeautifulSoup(site.text, features="lxml")
+        soup = BeautifulSoup(site.text, features="lxml")
         video_obj = soup.find("video", id="sporty")
 
         if not video_obj:
             return ""
 
         source = video_obj.find('source')
         clip_url: str = source.get('src')
 
         # Return the source url of the clip so it can be downloaded later
         return clip_url
 
-
-    # finds the savant clip based on the given at-bat information
-    # row must be a pandas dataframe row
     def __generate(self) -> str:
-        # load the given game's json file
-        game_json = self._play.game.game_json
+        """
+        Generates a savant clip based on the given at-bat information
+
+        Row must be a pandas dataframe row.
+        """
 
         # find the broadcast type so it's always corresponding
         # to the given batter's home team's broadcast
         if self.broadcast_type:
             broadcast_type = self.broadcast_type
         elif self._play.inning_topbot == "TOP":
             broadcast_type = "AWAY"
@@ -70,34 +74,35 @@
         # with the play id find the url for the savant clip
         site_url = f"https://baseballsavant.mlb.com/sporty-videos?playId={self._play.play_id}&videoType={broadcast_type}"
         clip_url = self.__get_url(site_url)
 
         # if the clip is alright return it
         if clip_url != "":
             return clip_url
-        
+
         # if the clip is screwed up then it was a national tv game
         # return the correct national tv clip url
         site_url = f"https://baseballsavant.mlb.com/sporty-videos?playId={self._play.play_id}&videoType=NETWORK"
         clip_url = self.__get_url(site_url)
 
         return clip_url
 
-    def download(self, path: str, verbose: bool =False) -> None:
-        # create response object 
-        # if a time out happens, try five more times before crashing the entire program
-        for z in range(5):
-            try:
-                r = requests.get(self._clip_url, stream=True, timeout=60) 
-                break
-            except requests.exceptions.Timeout:
-                print(f'Timeout has been raised. Link: {self._clip_url}')
+    def download(self, path: str | Path, verbose: bool = False) -> Path:
+        path = path if isinstance(path, Path) else Path(path)
+
+        # create response object
+        try:
+            r = requests.get(self._clip_url, stream=True, timeout=60)
+        except requests.exceptions.Timeout:
+            print(f'Timeout has been raised. Link: {self._clip_url}')
 
         # download the file to the specific location
         # honestly copied and pasted code, can't say much else
-        with open(path, 'wb') as f: 
-            for chunk in r.iter_content(chunk_size = 1024*1024): 
-                if chunk: 
-                    f.write(chunk) 
+        with open(path, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=1024*1024):
+                if chunk:
+                    f.write(chunk)
 
         if verbose:
-            print(f"Successfully downloaded: {path}")
+            print(f"Successfully downloaded: {path.absolute()}")
+
+        return path
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/clips.py` & `mlbrecaps-0.0.2/mlbrecaps/clips.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from typing import List, Literal
 from functools import singledispatchmethod
+from pathlib import Path
 
 from .play import Play
 from .game import Game
 from .clip import Clip
 from .utils import async_run
 
+
 class Clips():
-    def __init__(self, plays: List[Play] | Play, broadcast_type: Literal["HOME", "AWAY"] | None=None):
+    """Container class for working with and generating multiple clips from a list of plays"""
+
+    def __init__(self, plays: List[Play] | Play, broadcast_type: Literal["HOME", "AWAY"] | None = None):
         self.__set_plays(plays)
 
-        match broadcast_type: # Enforce broad_type types
+        match broadcast_type:  # Enforce broad_type types
             case "HOME" | "AWAY" | None:
                 self._broadcast_type: str | None = broadcast_type
             case _:
-                raise ValueError("BroadcastType must be None, \"HOME\", or \"AWAY\"")
+                raise ValueError(
+                    "BroadcastType must be None, \"HOME\", or \"AWAY\"")
 
         # Generate clip objects for each play passed
         self._clips = async_run(Clip, self._plays, self._broadcast_type)
 
     @singledispatchmethod
     def __set_plays(self, plays) -> None:
         raise ValueError("A Play or list of Play objects must be passed")
-    
+
     @__set_plays.register(list)
     def _(self, plays: List[Play]) -> None:
         if len(plays) == 0 or not isinstance(plays[0], Play):
             raise ValueError("A list of Play objects must be passed")
 
         self._plays: List[Play] = plays
 
@@ -42,10 +47,24 @@
     def clips(self) -> List[Clip]:
         return self._clips
 
     @property
     def broadcast_type(self) -> str:
         return self._broadcast_type
 
-    def download(self, path: str, verbose: bool=False) -> None:
-        paths = [f"{path}{index:03d}.mp4" for index in range(len(self._clips))]
-        async_run(Clip.download, self._clips, paths, verbose)
+    def download(self, dir_path: str | Path, verbose: bool = False) -> List[Path]:
+        """Download all clips into a single directory"""
+        # Convert path string to Path object
+        dir_path: Path = dir_path if isinstance(
+            dir_path, Path) else Path(dir_path)
+        dir_path.mkdir(exist_ok=True, parents=True)
+
+        # Get all paths for the mp4s
+        paths: List[Path] = [
+            dir_path / f"{index:04d}.mp4" for index in range(len(self._clips))]
+
+        # Create all paths in memory if they don't exist
+        for p in paths:
+            p.touch()
+
+        # Download all clips and return the download paths
+        return async_run(Clip.download, self._clips, paths, verbose)
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/data/team-info.csv` & `mlbrecaps-0.0.2/mlbrecaps/data/team-info.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Team ID,Code,File Code,Abbreviation,Name,Full Name,Brief Name
 108,ana,ana,LAA,LA Angels,Los Angeles Angels,Angels
-109,ari,ari,ARI,Arizona,Arizona Diamondbacks,D-backs
+109,ari,ari,AZ,Arizona,Arizona Diamondbacks,D-backs
 110,bal,bal,BAL,Baltimore,Baltimore Orioles,Orioles
 111,bos,bos,BOS,Boston,Boston Red Sox,Red Sox
 112,chn,chc,CHC,Chi Cubs,Chicago Cubs,Cubs
 113,cin,cin,CIN,Cincinnati,Cincinnati Reds,Reds
 114,cle,cle,CLE,Cleveland,Cleveland Guardians,Guardians
 115,col,col,COL,Colorado,Colorado Rockies,Rockies
 116,det,det,DET,Detroit,Detroit Tigers,Tigers
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/date.py` & `mlbrecaps-0.0.2/mlbrecaps/date.py`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/date_generator.py` & `mlbrecaps-0.0.2/mlbrecaps/date_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
 from copy import copy
 
 from .date import Date
 from .date_range import DateRange
 
+
 class DateGenerator():
+    """Static library for generating date objects"""
 
     @classmethod
     def today(cls) -> Date:
         obj = Date(datetime.now())
 
         return obj
 
@@ -46,8 +48,8 @@
 
         # check if it is still in the month then go one back
         while end_dt._date.month == month:
             end_dt.next()
 
         end_dt.prev()
 
-        return DateRange(start_dt, end_dt)
+        return DateRange(start_dt, end_dt)
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/date_range.py` & `mlbrecaps-0.0.2/mlbrecaps/date_range.py`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/game.py` & `mlbrecaps-0.0.2/mlbrecaps/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import pandas as pd
-import io
 import requests
 import json
 
 from functools import lru_cache, singledispatchmethod
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 from .team import Team
 from .date import Date
 from .player import Player
 from .play import Play
 from .utils import async_run, dataframe_from_url
 
+
 class Game():
 
     @lru_cache(maxsize=3)
     def __new__(cls, game_pk: int):
         return super().__new__(cls)
 
     def __init__(self, game_pk: int):
-        self._game_pk: int  = game_pk
-        self._game_data: pd.DataFrame | None = None
+        self._game_pk: int = game_pk
 
         # finds the url of the game based on the game_pk information stored in the at-bat data
         game_url = f"https://baseballsavant.mlb.com/gf?game_pk={self._game_pk}"
         game = requests.get(game_url)
 
         # load the given game's json file
         self._game_json = json.loads(game.text)
         self._away_json = self._game_json["team_away"]
         self._home_json = self._game_json["team_home"]
 
         # Get home/away and date
-        self._home: Team = Team(self._game_json["home_team_data"]["abbreviation"])
-        self._away: Team = Team(self._game_json["away_team_data"]["abbreviation"])
+        self._home: Team = Team(
+            self._game_json["home_team_data"]["abbreviation"])
+        self._away: Team = Team(
+            self._game_json["away_team_data"]["abbreviation"])
         self._date: Date = Date(self._game_json["gameDate"])
 
         # Get both lineups
-        self._home_lineup: List[int] = self._game_json["home_lineup"]
-        self._away_lineup: List[int] = self._game_json["away_lineup"]
+        self._home_lineup_ids: List[int] = self._game_json["home_lineup"]
+        self._away_lineup_ids: List[int] = self._game_json["away_lineup"]
 
         # Get the final scores
         self._home_score: int = self._game_json["scoreboard"]["linescore"]["teams"]["home"]["runs"]
         self._away_score: int = self._game_json["scoreboard"]["linescore"]["teams"]["away"]["runs"]
-    
+
     @singledispatchmethod
     def road_status(self, team: Team) -> str:
         raise ValueError("team must be of type Team")
 
     @road_status.register(Team)
     def _(self, team: Team) -> str:
         if self._away == team:
@@ -69,24 +70,24 @@
 
     @property
     def away_score(self) -> int:
         return self._away_score
 
     @property
     def home_lineup(self) -> List[int]:
-        return self._home_lineup.copy()
+        return self._home_lineup_ids.copy()
 
     @property
     def away_lineup(self) -> List[int]:
-        return self._away_lineup.copy()
+        return self._away_lineup_ids.copy()
 
     def get_lineup(self, team) -> List[int]:
         if team == self._away:
-            return self.away_lineup()
-            
+            return self.away_lineup
+
         return self.home_lineup
 
     @property
     def game_pk(self) -> int:
         return self._game_pk
 
     @property
@@ -109,33 +110,36 @@
     def away_json(self):
         return self._away_json.copy()
 
     @property
     def home_json(self):
         return self._home_json.copy()
 
-    def get_highlights(self, plays:int =10, team: Optional[str]=None):
-        df = self.__get_data()
+    def get_highlights(self, plays: int = 10, team: Optional[str] = None) -> List[Play]:
+        """Gets the highlights of both, away, or home teams"""
+        df: pd.DataFrame = self.__get_data()
 
         if plays <= 0:
             raise ValueError("Plays must be greater than 0")
 
         if team is not None and team.upper() not in ["HOME", "AWAY"]:
             raise ValueError("Team must be None, \"HOME\", or \"AWAY\"")
 
         # extra logic for when a home or away team is specified
         key = None if team else abs
-        ascending = False if not team else (True, False)[team.lower() == "home"]
+        ascending = False if not team else (
+            True, False)[team.lower() == "home"]
 
         # removes all non-events (balls, strikes, etc.)
         # then sorts for highest win expectancy for either team
         # then only keeps the top plays
         # also make sure the plays are in chronological order of the game
         df = df[df.events.notnull()]
-        df = df.sort_values(by="delta_home_win_exp", key=key, ascending=ascending)
+        df = df.sort_values(by="delta_home_win_exp",
+                            key=key, ascending=ascending)
         df = df.head(plays)
         df = df.sort_values(by="pitch_number", ascending=True)
         df = df.sort_values(by="at_bat_number", ascending=True)
 
         rows = [row for index, row in df.iterrows()]
         return async_run(Play, self, rows)
 
@@ -146,24 +150,32 @@
         return self.get_highlights(plays, "away")
 
     def get_player_highlights(self, player: Player, plays: int):
         df = self.__get_data()
 
         is_home_player = player.player_id in self.home_lineup
 
-        df = df[df.events.notnull() & ((df.batter == player.player_id) | (df.pitcher == player.player_id))]
-        df = df.sort_values(by="delta_home_win_exp", key=None, ascending=is_home_player)
+        df = df[df.events.notnull() & ((df.batter == player.player_id)
+                                       | (df.pitcher == player.player_id))]
+        df = df.sort_values(by="delta_home_win_exp",
+                            key=None, ascending=is_home_player)
         df = df.sort_values(by="at_bat_number", ascending=True)
 
         if is_home_player:
             df = df[df["delta_home_win_exp"] >= 0]
         else:
             df = df[df["delta_home_win_exp"] <= 0]
 
         df = df.head(plays)
 
         rows = [row for index, row in df.iterrows()]
         return async_run(Play, self, rows)
 
+    @property
+    def homers(self) -> Dict[int, int]:
+        df: pd.DataFrame = self.__get_data()
+        df = df[df.events == "home_run"]
+
+        return df["batter"].value_counts().to_dict()
+
     def __str__(self) -> str:
         return f"{self._away.abbreviation} - {self._home.abbreviation}, Final: {self._away_score}-{self._home_score}, Date: {self._date}, GamePK: {self._game_pk}"
-
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/game_generator.py` & `mlbrecaps-0.0.2/mlbrecaps/game_generator.py`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/play.py` & `mlbrecaps-0.0.2/mlbrecaps/play.py`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/player.py` & `mlbrecaps-0.0.2/mlbrecaps/player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
 import pandas as pd
-import io
 import requests
 import json
+from functools import lru_cache
 
-from typing import List, Dict, Optional, TYPE_CHECKING
+from typing import List, TYPE_CHECKING
 if TYPE_CHECKING:
     from .game import Play
 
-from .date_generator import DateGenerator
+from .date import Date
 from .utils import async_run, dataframe_copy, dataframe_from_url
 
+
 class Player():
 
+    @lru_cache(maxsize=100)
+    def __new__(cls, player_id: int):
+        return super().__new__(cls)
+
     def __init__(self, player_id: int):
         self._player_id: int = player_id
 
         # Get player JSON information
         playerURL: str = f"https://statsapi.mlb.com/api/v1/people/{player_id}"
         playerContent = requests.get(playerURL)
         player_json = json.loads(playerContent.text)["people"][0]
@@ -28,15 +33,15 @@
 
         # Player's position
         self._primary_position: str = player_json["primaryPosition"]["name"]
         self._primary_position_abbr: str = player_json["primaryPosition"]["abbreviation"]
 
     def is_pitcher(self) -> bool:
         return self._primary_position_abbr == "P"
-    
+
     def is_batter(self) -> bool:
         return not self.is_pitcher()
 
     @property
     def position(self) -> str:
         return self._primary_position
 
@@ -71,37 +76,39 @@
         Gets pandas dataframe information on all their homerun plays
         """
         return f"https://baseballsavant.mlb.com/statcast_search/csv?hfPT=&hfAB=home%5C.%5C.run%7C&hfGT=R%7C&hfPR=hit%5C.%5C.into%5C.%5C.play%7C&hfZ=&hfStadium=&hfBBL=&hfNewZones=&hfPull=&hfC=&hfSea={season}%7C&hfSit=&player_type=batter&hfOuts=&hfOpponent=&pitcher_throws=&batter_stands=&hfSA=&game_date_gt=&game_date_lt=&hfMo=&hfTeam=&home_road=&hfRO=&position=&hfInfield=&hfOutfield=&hfInn=&hfBBT=&batters_lookup%5B%5D={self._player_id}&hfFlag=&metric_1=&group_by=name&min_pitches=0&min_results=0&min_pas=0&sort_col=pitches&player_event_sort=api_p_release_speed&sort_order=desc&type=details&player_id={self._player_id}"
 
     # Encapsulates mutable data by making a copy
     @dataframe_copy
     def get_homerun_data(self, season: int) -> pd.DataFrame:
-        return self.__get_homerun_data(season)
+        df: pd.DataFrame = self.__get_homerun_data(season)
+        df = df.sort_values("game_date")
+        return df
 
     def get_homerun_count(self, season: int) -> int:
         return len(self.__get_homerun_data(season).index)
 
-    def get_homeruns(self, season: int | Date) -> List[Play]:
+    def get_homeruns(self, season: int) -> List[Play]:
         from .game import Play, Game
 
         homerun_data = self.__get_homerun_data(season)
-        # homerun_data.to_csv("./homeruns.csv")
-
-        # if date:
-            # homerun_data = homerun_data[homerun_data[]]
 
         games: List[Game] = async_run(Game, list(homerun_data["game_pk"]))
         rows = [row for index, row in homerun_data.iterrows()]
 
         return async_run(Play, games, rows)[::-1]
 
+    @classmethod
+    def generate_players(cls, player_ids: List[int]) -> List[Player]:
+        return async_run(cls, player_ids)
+
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, Player):
             return False
 
-        return self._player_id == other._player_id
+        return self._player_id == o._player_id
 
     def __hash__(self) -> int:
-        return self._player_id
+        return hash(self._player_id)
 
     def __str__(self) -> str:
-        return f"{self.__class__}@PlayerID={self._player_id}:FirstName={self._first_name}:LastName={self._last_name}"
+        return f"{self.__class__}@PlayerID={self._player_id}:FirstName={self._first_name}:LastName={self._last_name}"
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps/scripts.py` & `mlbrecaps-0.0.2/mlbrecaps/scripts.py`

 * *Files identical despite different names*

### Comparing `mlbrecaps-0.0.1/mlbrecaps/utils.py` & `mlbrecaps-0.0.2/mlbrecaps/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,56 +4,62 @@
 import pandas as pd
 
 import itertools
 import functools
 
 from typing import Any, List, Tuple
 
+
 def async_run(func: callable, *args: Any | List[Any]) -> List[Any]:
     # Makes all arguments into lists
     try:
         max_length = max(len(x) for x in args if isinstance(x, list))
     except ValueError:
         raise ValueError("At least one argument must be a list")
 
-    repeated_args = [arg if isinstance(arg, list) else list(itertools.repeat(arg, max_length)) for arg in args]
+    repeated_args = [arg if isinstance(arg, list) else list(
+        itertools.repeat(arg, max_length)) for arg in args]
 
     # Ensure all list arguments are of the same length
     if not all(len(i) == len(repeated_args[0]) for i in repeated_args):
         raise ValueError("Argument arrays must all be of the same length")
 
     async def create(*args: List[Any]):
         return func(*args)
 
     async def generate() -> List[Any]:
-        tasks = [asyncio.create_task(create(*args)) for args in zip(*repeated_args)]
+        tasks = [asyncio.create_task(create(*args))
+                 for args in zip(*repeated_args)]
 
         await asyncio.gather(*tasks)
         return [task.result() for task in tasks]
 
     return asyncio.run(generate())
 
+
 def copy_cache(func):
     func = functools.cache(func)
 
     def wrapper(*args, **kwargs):
         return func.copy()
 
     return wrapper
 
+
 def dataframe_copy(func):
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs).copy()
 
     return wrapper
 
-def dataframe_from_url(func, use_cache: bool=True):
+
+def dataframe_from_url(func, use_cache: bool = True):
     if use_cache:
         func = functools.cache(func)
 
     def wrapper(*args, **kwargs):
         url: str = func(*args, **kwargs)
         csv: bytes = requests.get(url).content
 
         return pd.read_csv(io.StringIO(csv.decode('utf-8')))
 
-    return wrapper
+    return wrapper
```

### Comparing `mlbrecaps-0.0.1/mlbrecaps.egg-info/PKG-INFO` & `mlbrecaps-0.0.2/mlbrecaps.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mlbrecaps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package that gathers information on given MLB games
 Home-page: https://github.com/MrRedwing/MLB-Recaps
 Author: Karsten Larson
 Author-email: karsten.larson.1@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
@@ -61,7 +62,9 @@
 ### Contributing
 
 All contributions are welcomed to improve the mlbrecaps package. To contribute simply submit a pull request.
 
 ### License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+
```

### Comparing `mlbrecaps-0.0.1/setup.py` & `mlbrecaps-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
-	long_description = f.read()
+    long_description = f.read()
 
 setup(
     name="mlbrecaps",
-    version="0.0.1",
+    version="0.0.2",
     description="Package that gathers information on given MLB games",
     packages=find_packages(include=["mlbrecaps"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrRedwing/MLB-Recaps",
     author="Karsten Larson",
     author_email="karsten.larson.1@gmail.com",
```

