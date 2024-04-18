# Comparing `tmp/simulation-schedule-1.2.3.tar.gz` & `tmp/simulation_schedule-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation-schedule-1.2.3.tar", last modified: Fri Apr 12 13:48:25 2024, max compression
+gzip compressed data, was "simulation_schedule-1.2.4.tar", last modified: Thu Apr 18 06:37:40 2024, max compression
```

## Comparing `simulation-schedule-1.2.3.tar` & `simulation_schedule-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423910 simulation-schedule-1.2.3/
--rw-r--r--   0 ruben      (501) staff       (20)     2012 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/AUTHORS.rst
--rw-r--r--   0 ruben      (501) staff       (20)     6542 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/HISTORY.rst
--rw-r--r--   0 ruben      (501) staff       (20)     1099 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/LICENSE.txt
--rw-r--r--   0 ruben      (501) staff       (20)      147 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/MANIFEST.in
--rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-12 13:48:25.423849 simulation-schedule-1.2.3/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)     2288 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/README.rst
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423129 simulation-schedule-1.2.3/schedule/
--rw-r--r--   0 ruben      (501) staff       (20)    33428 2024-04-12 13:47:40.000000 simulation-schedule-1.2.3/schedule/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)        0 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/schedule/py.typed
--rw-r--r--   0 ruben      (501) staff       (20)       93 2024-04-12 13:48:25.424091 simulation-schedule-1.2.3/setup.cfg
--rw-r--r--   0 ruben      (501) staff       (20)     1599 2024-04-12 13:48:14.000000 simulation-schedule-1.2.3/setup.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423667 simulation-schedule-1.2.3/simulation_schedule.egg-info/
--rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      305 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 ruben      (501) staff       (20)        1 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 ruben      (501) staff       (20)        9 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/top_level.txt
--rw-r--r--   0 ruben      (501) staff       (20)    46579 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/test_schedule.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-18 06:37:40.224286 simulation_schedule-1.2.4/
+-rw-r--r--   0 ruben      (501) staff       (20)     2012 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/AUTHORS.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     6542 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/HISTORY.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     1099 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/LICENSE.txt
+-rw-r--r--   0 ruben      (501) staff       (20)      147 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-18 06:37:40.224228 simulation_schedule-1.2.4/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)     2288 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/README.rst
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-18 06:37:40.223377 simulation_schedule-1.2.4/schedule/
+-rw-r--r--   0 ruben      (501) staff       (20)    33587 2024-04-18 06:37:00.000000 simulation_schedule-1.2.4/schedule/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/schedule/py.typed
+-rw-r--r--   0 ruben      (501) staff       (20)       93 2024-04-18 06:37:40.224485 simulation_schedule-1.2.4/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)     1599 2024-04-17 20:30:41.000000 simulation_schedule-1.2.4/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-18 06:37:40.223998 simulation_schedule-1.2.4/simulation_schedule.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-18 06:37:40.000000 simulation_schedule-1.2.4/simulation_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      305 2024-04-18 06:37:40.000000 simulation_schedule-1.2.4/simulation_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2024-04-18 06:37:40.000000 simulation_schedule-1.2.4/simulation_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        9 2024-04-18 06:37:40.000000 simulation_schedule-1.2.4/simulation_schedule.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)    46579 2024-04-09 16:00:45.000000 simulation_schedule-1.2.4/test_schedule.py
```

### Comparing `simulation-schedule-1.2.3/AUTHORS.rst` & `simulation_schedule-1.2.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.3/HISTORY.rst` & `simulation_schedule-1.2.4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.3/LICENSE.txt` & `simulation_schedule-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.3/PKG-INFO` & `simulation_schedule-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.3
+Version: 1.2.4
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.3
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.4
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simulation-schedule-1.2.3/README.rst` & `simulation_schedule-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.3/schedule/__init__.py` & `simulation_schedule-1.2.4/schedule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,22 +783,24 @@
             days_ahead = weekday - self.next_run.weekday()
             if days_ahead <= 0:  # Target day already happened this week
                 days_ahead += 7
             self.next_run += datetime.timedelta(days_ahead) - self.period
 
         # before we apply the .at() time, we need to normalize the timestamp
         # to ensure we change the time elements in the new timezone
+        original_day = self.next_run.day # Is required to check if the day has changed after applying the at_time
         if self.at_time_zone is not None:
             self.next_run = self.at_time_zone.normalize(self.next_run)
 
         if self.at_time is not None:
             if self.unit not in ("days", "hours", "minutes") and self.start_day is None:
                 raise ScheduleValueError("Invalid unit without specifying start day")
             kwargs = {"second": self.at_time.second, "microsecond": 0}
             if self.unit == "days" or self.start_day is not None:
+                kwargs["day"] = original_day
                 kwargs["hour"] = self.at_time.hour
             if self.unit in ["days", "hours"] or self.start_day is not None:
                 kwargs["minute"] = self.at_time.minute
 
             self.next_run = self.next_run.replace(**kwargs)  # type: ignore
 
             # Make sure we run at the specified time *today* (or *this hour*)
```

### Comparing `simulation-schedule-1.2.3/setup.py` & `simulation_schedule-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 from setuptools import setup
 
 
-SCHEDULE_VERSION = "1.2.3"
+SCHEDULE_VERSION = "1.2.4"
 SCHEDULE_DOWNLOAD_URL = "https://github.com/dbader/schedule/tarball/" + SCHEDULE_VERSION
 
 
 def read_file(filename):
     """
     Read a utf8 encoded text file and return its contents.
     """
```

### Comparing `simulation-schedule-1.2.3/simulation_schedule.egg-info/PKG-INFO` & `simulation_schedule-1.2.4/simulation_schedule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.3
+Version: 1.2.4
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.3
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.4
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simulation-schedule-1.2.3/test_schedule.py` & `simulation_schedule-1.2.4/test_schedule.py`

 * *Files identical despite different names*

