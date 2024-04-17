# Comparing `tmp/hltv_async_api-0.5.1.tar.gz` & `tmp/hltv_async_api-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.5.1.tar", max compression
+gzip compressed data, was "hltv_async_api-0.5.2.tar", max compression
```

## Comparing `hltv_async_api-0.5.1.tar` & `hltv_async_api-0.5.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      124 2024-04-16 15:56:41.976763 hltv_async_api-0.5.1/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    37792 2024-04-16 15:56:13.528920 hltv_async_api-0.5.1/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.5.1/hltv_async_api/proxies.txt
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.1/LICENSE
--rw-r--r--   0        0        0      648 2024-04-16 15:56:41.983765 hltv_async_api-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.1/README.md
--rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-17 20:47:53.777052 hltv_async_api-0.5.2/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    38519 2024-04-17 20:40:49.329850 hltv_async_api-0.5.2/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.5.2/hltv_async_api/proxies.txt
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.2/LICENSE
+-rw-r--r--   0        0        0      648 2024-04-17 20:47:53.768948 hltv_async_api-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.2/README.md
+-rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.2/PKG-INFO
```

### Comparing `hltv_async_api-0.5.1/hltv_async_api/aiohltv.py` & `hltv_async_api-0.5.2/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,42 +288,46 @@
                         break
                     date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
 
                     for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
                         time_ = match.find('div', {'class': 'matchTime'}).text
                         rating = int(match['stars'])
                         if rating >= min_rating:
+                            id_ = 0
+                            t1_id = 0
+                            t2_id = 0
+                            team1 = 'TBD'
+                            team2 = 'TBD'
+
                             try:
-                                match_id_ = match.find('a')['href'].split('/')[2]
+                                id_ = match.find('a')['href'].split('/')[2]
                                 t1_id = match['team1']
                                 t2_id = match['team2']
                             except (IndexError, AttributeError, KeyError):
-                                t1_id = 0
-                                t2_id = 0
+                                pass
                             maps = match.find('div', {'class': 'matchMeta'}).text[-1:]
                             try:
                                 teams = match.find_all('div', {'class': 'matchTeamName text-ellipsis'})
 
                                 team1 = teams[0].text
                                 team2 = teams[1].text
                             except (IndexError, AttributeError):
-                                team1 = 'TBD'
-                                team2 = 'TBD'
+                                pass
 
                             try:
                                 event = match.find('div', {'class', 'matchEventName gtSmartphone-only'}).text
                             except AttributeError:
 
                                 try:
                                     event = match.find('span', {'class': 'line-clamp-3'}).text
                                 except AttributeError:
                                     event = ''
 
                             matches.append({
-                                'id': match_id_,
+                                'id': id_,
                                 'date': date_,
                                 'time': time_,
                                 'team1': team1,
                                 'team2': team2,
                                 't1_id': t1_id,
                                 't2_id': t2_id,
                                 'maps': maps,
@@ -396,15 +400,15 @@
                 elif map["r_team1"] == '13':
                     if len(map) != 1:
                         score2 += 1
                     else:
                         score2 = 13
                         score1 = int(map["r_team1"])
 
-        return match_id, score1, score2, status, maps, stats_
+        return {'id': match_id, 'score1': score1, 'score2': score2, 'status': status, 'maps': maps, 'stats': stats_}
 
     async def get_results(self, days: int = 1,
                           min_rating: int = 1,
                           max: int = 30,
                           featured: bool = True,
                           regular: bool = True) -> list[dict[str, Any]] | None:
         """returns a list of big event matches results"""
@@ -678,15 +682,15 @@
                     })
 
         return events
 
     async def get_event_info(self, event_id: str | int, event_title: str):
         # TODO ADD WINNER?
 
-        r = await self._fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
+        r = await self._fetch(f"https://hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
         if not r:
             return
 
         event_date_div = r.find('td', {'class', 'eventdate'}).find_all('span')
 
         event_start = self._normalize_date(event_date_div[0].text.split())
         event_end = self._normalize_date(event_date_div[1].text.split()[1:-1])
@@ -705,15 +709,22 @@
                 teams = []
                 for team in group.find_all('div', 'text-ellipsis'):
                     teams.append(team.find('a').text)
                 groups.append({group_name: teams})
         except AttributeError:
             groups = []
 
-        return event_id, event_title, event_start, event_end, prize, team_num, location, groups
+        return {'id': event_id,
+                'title': event_title,
+                'start': event_start,
+                'end': event_end,
+                'prize': prize,
+                'teams': team_num,
+                'location': location,
+                'group': groups}
 
     async def get_top_teams(self, max_teams=30):
         """
         returns a list of the top 1-30 teams
         :params:
         max_teams: int = 30
         :return:
@@ -765,15 +776,15 @@
                     'change': change,
                 })
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
         return teams
 
-    async def get_team_info(self, team_id: int | str, title: str) -> tuple | None:
+    async def get_team_info(self, team_id: int | str, title: str) -> dict[str, list[str]]:
         """
         Returns Information about team
         :params:
         team_id: int | str
         title: str
         :returns:
         (team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys) | None
@@ -787,32 +798,43 @@
 
             rank = '0'
             weeks = '0'
             age = '0'
             coach = ''
 
             for i, stat in enumerate(r.find_all('div', {'class': 'profile-team-stat'}), start=1):
-                if i == 1:
-                    rank = stat.find('a').text[1:]
-                elif i == 2:
-                    weeks = stat.find('span', {'class': 'right'}).text
-                elif i == 3:
-                    age = stat.find('span', {'class': 'right'}).text
-                elif i == 4:
-                    coach = stat.find('span', {'class': 'bold a-default'}).text[1:-1]
+                try:
+                    if i == 1:
+                        rank = stat.find('a').text[1:]
+                    elif i == 2:
+                        weeks = stat.find('span', {'class': 'right'}).text
+                    elif i == 3:
+                        age = stat.find('span', {'class': 'right'}).text
+                    elif i == 4:
+                        coach = stat.find('span', {'class': 'bold a-default'}).text[1:-1]
+                except AttributeError:
+                    pass
 
             last_trophy = None
-            total_trophys = None
+            total_trophies = None
             try:
                 last_trophy = r.find('div', {'class': 'trophyHolder'}).find('span')['title']
-                total_trophys = len(r.find_all('div', {'class': 'trophyHolder'}))
+                total_trophies = len(r.find_all('div', {'class': 'trophyHolder'}))
             except AttributeError:
                 pass
 
-            return team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys
+            return {'id': team_id,
+                    'title': title,
+                    'rank': rank,
+                    'players': players,
+                    'coach': coach,
+                    'age': age,
+                    'weekstop30': weeks,
+                    'last_trophy': last_trophy,
+                    'total_trophies': total_trophies}
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
     async def get_best_players(self, top=40):
         """
         returns a list of the top (1-40) players in top 20 at the year
         :params:
```

### Comparing `hltv_async_api-0.5.1/hltv_async_api/proxies.txt` & `hltv_async_api-0.5.2/hltv_async_api/proxies.txt`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.1/LICENSE` & `hltv_async_api-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.1/pyproject.toml` & `hltv_async_api-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.5.1"
+version = "0.5.2"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.5.1/README.md` & `hltv_async_api-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.1/PKG-INFO` & `hltv_async_api-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.5.1
+Version: 0.5.2
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

