# Comparing `tmp/datewise-0.2.1.tar.gz` & `tmp/datewise-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datewise-0.2.1.tar", last modified: Wed Apr 17 08:28:26 2024, max compression
+gzip compressed data, was "datewise-0.2.2.tar", last modified: Thu Apr 18 20:31:11 2024, max compression
```

## Comparing `datewise-0.2.1.tar` & `datewise-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:28:26.286242 datewise-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 08:28:26.286242 datewise-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 08:28:08.000000 datewise-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:28:26.286242 datewise-0.2.1/datewise/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 08:28:08.000000 datewise-0.2.1/datewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-17 08:28:08.000000 datewise-0.2.1/datewise/datewise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:28:26.286242 datewise-0.2.1/datewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 08:28:26.000000 datewise-0.2.1/datewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 08:28:26.000000 datewise-0.2.1/datewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:28:26.000000 datewise-0.2.1/datewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 08:28:26.000000 datewise-0.2.1/datewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 08:28:26.000000 datewise-0.2.1/datewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:28:26.286242 datewise-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-17 08:28:08.000000 datewise-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:28:26.286242 datewise-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-17 08:28:08.000000 datewise-0.2.1/tests/test_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 20:31:11.683951 datewise-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 20:30:52.000000 datewise-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.679951 datewise-0.2.2/datewise/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-18 20:30:52.000000 datewise-0.2.2/datewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-04-18 20:30:52.000000 datewise-0.2.2/datewise/datewise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/datewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:31:11.000000 datewise-0.2.2/datewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:31:11.683951 datewise-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-18 20:30:52.000000 datewise-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:11.683951 datewise-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-18 20:30:52.000000 datewise-0.2.2/tests/test_functionality.py
```

### Comparing `datewise-0.2.1/PKG-INFO` & `datewise-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.2.1
+Version: 0.2.2
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.2.1/datewise/datewise.py` & `datewise-0.2.2/datewise/datewise.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
         if fmt:
 
             weekday = datetime.strptime(date, fmt).weekday()
 
             if weekend == False:
 
-                if weekday < 3:   
+                if weekday <= 3:   
 
                     date_week_end = (datetime.strptime(date, fmt) + timedelta(days=4 - weekday)).strftime(fmt)
                     return(f'Business Week ends: {date_week_end}')
                 
                 elif weekday == 4:
 
                     return('Today is the end of the business week.') 
@@ -446,15 +446,15 @@
             max_date = datetime.strptime(max_date, max_format)
 
             min_format = identify_date_format(end)
             min_date = datetime.strptime(min_date, min_format)
 
             days_between = []
 
-            if weekend:
+            if not weekend:
 
                 while max_date != min_date + timedelta(days=1):
 
                     max_date -= timedelta(days=1)
                     if max_date.weekday() < 5:
                         days_between.append(max_date.strftime(max_format))
                     else:
@@ -473,29 +473,29 @@
 
             if frequency == 'day':
 
                 return output
             
             elif frequency == 'week':
 
-                week_difference = len(days_between) / 7
+                if not weekend:
 
-                if type(week_difference) != int:
+                    week_difference = len(days_between) / 5 
+                    
+                    weeks = int(week_difference)
+                    days = len(days_between) % 5
 
-                    if weekend:
-                        
-                        weeks = int(week_difference)
-                        days = len(days_between) % 5
+                else:
 
-                    else:
+                    week_difference = len(days_between) / 7
 
-                        weeks = int(week_difference)
-                        days = len(days_between) % 7
+                    weeks = int(week_difference)
+                    days = len(days_between) % 7
 
-                return f"Difference between two dates is {weeks} week(s) and {days} days. If you want to see specific dates, switch to format='day'"
+                return f"Difference between two dates is {weeks} week(s) and {days} days. If you want to see specific dates, switch to format='day'" 
 
             elif frequency == 'month':
 
                 month_difference = len(days_between) / 30
 
                 if type(month_difference) != int:
```

### Comparing `datewise-0.2.1/datewise.egg-info/PKG-INFO` & `datewise-0.2.2/datewise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.2.1
+Version: 0.2.2
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datewise-0.2.1/setup.py` & `datewise-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datewise",
-    version="0.2.1",
+    version="0.2.2",
     description="Thesis Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://datewise.readthedocs.io/",
     author="Sebastian Gontkovic",
     author_email="sebascngont@gmail.com",
     license="MIT",
```

### Comparing `datewise-0.2.1/tests/test_functionality.py` & `datewise-0.2.2/tests/test_functionality.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,247 +528,247 @@
 # range_calculation
     
 def test1_date1_string_date2_string_range_calculation_weekend_false_frequncy_day():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test2_date1_string_date2_timestamp_range_calculation_weekend_false_frequncy_day():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test3_date1_timestamp_date2_datetime_range_calculation_weekend_false_frequncy_day():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test4_date1_string_date2_string_range_calculation_weekend_false_frequncy_week():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
 
 
 def test5_date1_string_date2_timestamp_range_calculation_weekend_false_frequncy_week():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
 
 
 def test6_date1_timestamp_date2_datetime_range_calculation_weekend_false_frequncy_week():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
 
 
 def test7_date1_string_date2_string_range_calculation_weekend_false_frequncy_month():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='month') ==  "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='month') ==  "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test8_date1_string_date2_timestamp_range_calculation_weekend_false_frequncy_month():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='month') == "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='month') == "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test9_date1_timestamp_date2_datetime_range_calculation_weekend_false_frequncy_month():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='month') == "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='month') == "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test10_date1_string_date2_string_range_calculation_weekend_false_frequncy_quarter():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test11_date1_string_date2_timestamp_range_calculation_weekend_false_frequncy_quarter():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test12_date1_timestamp_date2_datetime_range_calculation_weekend_false_frequncy_quarter():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test13_date1_string_date2_string_range_calculation_weekend_false_frequncy_year():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test14_date1_string_date2_timestamp_range_calculation_weekend_false_frequncy_year():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test15_date1_timestamp_date2_datetime_range_calculation_weekend_false_frequncy_year():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=False, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
 
 
 def test16_date1_string_date2_string_range_calculation_weekend_true_frequncy_day():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test17_date1_string_date2_timestamp_range_calculation_weekend_true_frequncy_day():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test18_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_day():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Business days between two dates are: ['2024-04-01', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-22', '2024-03-21', '2024-03-20']"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='day') == "Days between two dates are: ['2024-04-01', '2024-03-31', '2024-03-30', '2024-03-29', '2024-03-28', '2024-03-27', '2024-03-26', '2024-03-25', '2024-03-24', '2024-03-23', '2024-03-22', '2024-03-21', '2024-03-20']"
 
 
 def test19_date1_string_date2_string_range_calculation_weekend_true_frequncy_week():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
 
 
 def test20_date1_string_date2_timestamp_range_calculation_weekend_true_frequncy_week():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
 
 
 def test21_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_week():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 4 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='week') == "Difference between two dates is 1 week(s) and 6 days. If you want to see specific dates, switch to format='day'"
 
 
 def test22_date1_string_date2_string_range_calculation_weekend_true_frequncy_month():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='month') ==  "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='month') ==  "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test23_date1_string_date2_timestamp_range_calculation_weekend_true_frequncy_month():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='month') == "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='month') == "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test24_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_month():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='month') == "Difference between two dates is 0 month(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='month') == "Difference between two dates is 0 month(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test25_date1_string_date2_string_range_calculation_weekend_true_frequncy_quarter():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test26_date1_string_date2_timestamp_range_calculation_weekend_true_frequncy_quarter():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test27_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_quarter():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='quarter') == "Difference between two dates is 0 quarter(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test28_date1_string_date2_string_range_calculation_weekend_true_frequncy_year():
 
     start = '2024-03-19'
     end = '2024-04-02'
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test29_date1_string_date2_timestamp_range_calculation_weekend_true_frequncy_year():
 
     start = '2024-03-19'
     end =  pd.Timestamp('2024-04-02 12:30:00')
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test30_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_year():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
 
-    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 9 days. If you want to see specific dates, switch to format='day'"
+    assert range_calculation(start=start, end=end, weekend=True, frequency='year') == "Difference between two dates is 0 year(s) and 13 days. If you want to see specific dates, switch to format='day'"
 
 
 def test31_date1_timestamp_date2_datetime_range_calculation_weekend_true_frequncy_unknown():
 
     start = pd.Timestamp('2024-03-19 12:30:00')
     end = datetime(year=2024, month=4, day=2)
```

