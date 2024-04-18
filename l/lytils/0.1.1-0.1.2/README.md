# Comparing `tmp/lytils-0.1.1.tar.gz` & `tmp/lytils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytils-0.1.1.tar", max compression
+gzip compressed data, was "lytils-0.1.2.tar", max compression
```

## Comparing `lytils-0.1.1.tar` & `lytils-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.1/LICENSE
--rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.1/lytils/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.1/lytils/app.py
--rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.1/lytils/classes/__init__.py
--rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.1/lytils/classes/Regex.py
--rw-r--r--   0        0        0     1112 2023-10-18 01:09:58.336249 lytils-0.1.1/lytils/common.py
--rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.1/lytils/discord/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/discord/DiscordBot.py
--rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.1/lytils/email/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.1/lytils/email/Email.py
--rw-r--r--   0        0        0     1577 2024-04-10 19:47:10.141707 lytils-0.1.1/lytils/file.py
--rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.1/lytils/google_sheets/__init__.py
--rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.1/lytils/google_sheets/Column.py
--rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.1/lytils/google_sheets/format.py
--rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.1/lytils/google_sheets/GoogleSheets.py
--rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/google_sheets/helpers.py
--rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.1/lytils/google_sheets/Sheet.py
--rw-r--r--   0        0        0     7421 2024-04-10 19:21:06.136630 lytils-0.1.1/lytils/google_sheets/Tab.py
--rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.1/lytils/input.py
--rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.1/lytils/logging.py
--rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.1/lytils/print.py
--rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.1/lytils/regex.py
--rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.1/lytils/surfshark.py
--rw-r--r--   0        0        0      318 2024-04-12 07:11:04.872541 lytils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.1/README.md
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.2/LICENSE
+-rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.2/lytils/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.2/lytils/app.py
+-rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.2/lytils/classes/__init__.py
+-rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.2/lytils/classes/Regex.py
+-rw-r--r--   0        0        0     1112 2023-10-18 01:09:58.336249 lytils-0.1.2/lytils/common.py
+-rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.2/lytils/discord/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.2/lytils/discord/DiscordBot.py
+-rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.2/lytils/email/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.2/lytils/email/Email.py
+-rw-r--r--   0        0        0     1577 2024-04-10 19:47:10.141707 lytils-0.1.2/lytils/file.py
+-rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.2/lytils/google_sheets/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.2/lytils/google_sheets/Column.py
+-rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.2/lytils/google_sheets/format.py
+-rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.2/lytils/google_sheets/GoogleSheets.py
+-rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.2/lytils/google_sheets/helpers.py
+-rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.2/lytils/google_sheets/Sheet.py
+-rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.2/lytils/google_sheets/Tab.py
+-rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.2/lytils/input.py
+-rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.2/lytils/logging.py
+-rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.2/lytils/print.py
+-rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.2/lytils/regex.py
+-rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.2/lytils/surfshark.py
+-rw-r--r--   0        0        0      318 2024-04-18 01:08:19.709129 lytils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.2/README.md
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.2/PKG-INFO
```

### Comparing `lytils-0.1.1/LICENSE` & `lytils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/app.py` & `lytils-0.1.2/lytils/app.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/classes/Regex.py` & `lytils-0.1.2/lytils/classes/Regex.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/common.py` & `lytils-0.1.2/lytils/common.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/discord/DiscordBot.py` & `lytils-0.1.2/lytils/discord/DiscordBot.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/email/Email.py` & `lytils-0.1.2/lytils/email/Email.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/file.py` & `lytils-0.1.2/lytils/file.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/google_sheets/Column.py` & `lytils-0.1.2/lytils/google_sheets/Column.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/google_sheets/format.py` & `lytils-0.1.2/lytils/google_sheets/format.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/google_sheets/GoogleSheets.py` & `lytils-0.1.2/lytils/google_sheets/GoogleSheets.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/google_sheets/Tab.py` & `lytils-0.1.2/lytils/google_sheets/Tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,23 @@
         data = self.__tab.get_values()
         if len(data) > 1:
             return DataFrame(data[1:], columns=data[0])
         else:
             return DataFrame()
 
     # Get data from specific range
-    def get_range(self, range: str) -> DataFrame:
+    def get_range(self, range: str, headers: bool = True) -> DataFrame:
         data = self.__tab.get(range)
 
         if data:
-            headers = data.pop(0)  # Use the first row as headers
-            df = DataFrame(data, columns=headers)
+            if headers:
+                headers_row = data.pop(0)  # Use the first row as headers
+                df = DataFrame(data, columns=headers_row)
+            else:
+                df = DataFrame(data)
         else:
             df = DataFrame()
 
         df = df.fillna("")  # Replace None values with an empty string
         return df
 
     # Clear all data
```

### Comparing `lytils-0.1.1/lytils/input.py` & `lytils-0.1.2/lytils/input.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/logging.py` & `lytils-0.1.2/lytils/logging.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/print.py` & `lytils-0.1.2/lytils/print.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.1/lytils/surfshark.py` & `lytils-0.1.2/lytils/surfshark.py`

 * *Files identical despite different names*

