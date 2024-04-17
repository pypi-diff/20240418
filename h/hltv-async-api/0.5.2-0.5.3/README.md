# Comparing `tmp/hltv_async_api-0.5.2.tar.gz` & `tmp/hltv_async_api-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.5.2.tar", max compression
+gzip compressed data, was "hltv_async_api-0.5.3.tar", max compression
```

## Comparing `hltv_async_api-0.5.2.tar` & `hltv_async_api-0.5.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      124 2024-04-17 20:47:53.777052 hltv_async_api-0.5.2/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    38519 2024-04-17 20:40:49.329850 hltv_async_api-0.5.2/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.5.2/hltv_async_api/proxies.txt
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.2/LICENSE
--rw-r--r--   0        0        0      648 2024-04-17 20:47:53.768948 hltv_async_api-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.2/README.md
--rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-17 22:10:26.232259 hltv_async_api-0.5.3/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    38403 2024-04-17 22:10:04.481202 hltv_async_api-0.5.3/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.3/LICENSE
+-rw-r--r--   0        0        0      648 2024-04-17 22:10:26.247497 hltv_async_api-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.3/README.md
+-rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.3/PKG-INFO
```

### Comparing `hltv_async_api-0.5.2/hltv_async_api/aiohltv.py` & `hltv_async_api-0.5.3/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,15 @@
                                 'maps': maps,
                                 'rating': rating,
                                 'event': event
                             })
 
         except AttributeError:
             return None
+
         return matches
 
     async def get_match_info(self, match_id: str | int, team1: str, team2: str, event_title: str, stats: bool = True):
         r = await self._fetch(f"https://www.hltv.org/matches/{str(match_id)}/"
                               f"{team1.replace(' ', '-')}-vs-"
                               f"{team2.replace(' ', '-')}-"
                               f"{event_title.replace(' ', '-')}")
@@ -435,21 +436,21 @@
                 event = res.find('span', class_='event-name').text
 
                 scores = res.find("td", class_="result-score").text.strip().split('-')
                 s_t1 = scores[0].strip()
                 s_t2 = scores[1].strip()
 
                 results.append({
-                            'id': match_id,
-                            'team1': team1,
-                            'team2': team2,
-                            'score1': s_t1,
-                            'score2': s_t2,
-                            'rating': rating,
-                            'event': event,
+                    'id': match_id,
+                    'team1': team1,
+                    'team2': team2,
+                    'score1': s_t1,
+                    'score2': s_t2,
+                    'rating': rating,
+                    'event': event,
                 })
 
         if regular:
 
             n = 0
 
             for i, date_div in enumerate(r.find_all('div', class_='results-sublist')[1:], start=1):
@@ -477,37 +478,38 @@
                         event = res.find('span', class_='event-name').text
 
                         scores = res.find("td", class_="result-score").text.strip().split('-')
                         s_t1 = scores[0].strip()
                         s_t2 = scores[1].strip()
 
                         results.append({
-                                    'id': match_id,
-                                    'date': date_,
-                                    'team1': team1,
-                                    'team2': team2,
-                                    'score1': s_t1,
-                                    'score2': s_t2,
-                                    'rating': rating,
-                                    'event': event,
+                            'id': match_id,
+                            'date': date_,
+                            'team1': team1,
+                            'team2': team2,
+                            'score1': s_t1,
+                            'score2': s_t2,
+                            'rating': rating,
+                            'event': event,
                         })
 
                         n += 1
 
         return results
 
     async def get_event_results(self, event: int | str, days: int = 1, max_: int = 10) -> list[dict[str, Any]] | None:
         r = await self._fetch("https://www.hltv.org/results?event=" + str(event))
         if not r:
             return
 
         match_results = []
 
         n = 0
-        for i, result in enumerate(r.find("div", {'class', 'results-holder'}).find_all("div", {'class', 'results-sublist'}), start=1):
+        for i, result in enumerate(
+                r.find("div", {'class', 'results-holder'}).find_all("div", {'class', 'results-sublist'}), start=1):
             if i > days or n > max_:
                 break
             date = self.__normalize_date(result.find("span", class_="standard-headline").text.strip())
             for match in result.find_all("a", class_="a-reset"):
                 if n > max_:
                     break
                 id_ = match['href'].split('/')[2]
@@ -941,15 +943,16 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv(debug=True, timeout=1, max_delay=5, true_session=True, use_proxy=True, proxy_list=['', ''])
-    print(await hltv.get('matches', 2371201, 'res-regional-series-3-latam', 'IMPERIAL', 'MIBR'))
+    hltv = Hltv(debug=True, timeout=1, max_delay=5, true_session=True, use_proxy=True, proxy_path='proxies.txt',
+                proxy_protocol='http')
+    print(await hltv.get_matches())
 
     await hltv.close_session()
 
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.5.2/LICENSE` & `hltv_async_api-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.2/pyproject.toml` & `hltv_async_api-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.5.2"
+version = "0.5.3"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.5.2/README.md` & `hltv_async_api-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.2/PKG-INFO` & `hltv_async_api-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.5.2
+Version: 0.5.3
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

