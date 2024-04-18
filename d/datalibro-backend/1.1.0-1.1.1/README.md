# Comparing `tmp/datalibro_backend-1.1.0.tar.gz` & `tmp/datalibro_backend-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.1.0.tar", last modified: Wed Apr 17 08:55:21 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.1.tar", last modified: Thu Apr 18 06:03:03 2024, max compression
```

## Comparing `datalibro_backend-1.1.0.tar` & `datalibro_backend-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.520815 datalibro_backend-1.1.0/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.0/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-17 08:55:21.520490 datalibro_backend-1.1.0/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.0/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.519128 datalibro_backend-1.1.0/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.0/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    14859 2024-04-17 07:52:04.000000 datalibro_backend-1.1.0/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)     6994 2024-02-01 06:18:54.000000 datalibro_backend-1.1.0/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.520264 datalibro_backend-1.1.0/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-04-17 08:55:21.520874 datalibro_backend-1.1.0/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-04-17 08:54:58.000000 datalibro_backend-1.1.0/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:03:03.685833 datalibro_backend-1.1.1/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.1/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-18 06:03:03.685536 datalibro_backend-1.1.1/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.1/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:03:03.684155 datalibro_backend-1.1.1/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.1/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15308 2024-04-18 06:02:10.000000 datalibro_backend-1.1.1/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     6994 2024-02-01 06:18:54.000000 datalibro_backend-1.1.1/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-18 06:03:03.685335 datalibro_backend-1.1.1/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-18 06:03:03.000000 datalibro_backend-1.1.1/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-04-18 06:03:03.000000 datalibro_backend-1.1.1/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-04-18 06:03:03.000000 datalibro_backend-1.1.1/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-04-18 06:03:03.000000 datalibro_backend-1.1.1/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-04-18 06:03:03.685886 datalibro_backend-1.1.1/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-04-18 06:02:47.000000 datalibro_backend-1.1.1/setup.py
```

### Comparing `datalibro_backend-1.1.0/LICENSE.txt` & `datalibro_backend-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.0/PKG-INFO` & `datalibro_backend-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.1.0
+Version: 1.1.1
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.0/README.md` & `datalibro_backend-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.0/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.1/datalibro_backend/quality_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,21 +58,19 @@
                         right_sugg.append(suggestion)
                 elif i >1:
                     try:
                         suggestion = f"{i} position of the table's name is {seperate_table[i]}. The {i} position for this table should be {self.standard_name_ods[i]}. Please carefully check it!"
                         wrong_col.append(seperate_table[i])
                         right_sugg.append(suggestion)
                     except:
-                        suggestion = f"{i} position of the table's name is {seperate_table[i]}. Please carefully check it!"
-                        wrong_col.append(seperate_table[i])
-                        right_sugg.append(suggestion)
+                        pass
             else:
-                    suggestion = f"{i} position of the table's name is incorrect! Please find the suitable name for this position! The enums for {i} position are ('tb','bi','map')."
-                    wrong_col.append(seperate_table[i])
-                    right_sugg.append(suggestion)
+                suggestion = f"{i} position of the table's name is incorrect! Please find the suitable name for this position! The enums for {i} position are ('tb','bi','map')."
+                wrong_col.append(seperate_table[i])
+                right_sugg.append(suggestion)
         data_frame = {'Wrong Part of Table Name':wrong_col,"Optimized Suggestion of Table Name":right_sugg}
         data = pd.DataFrame(data_frame)
         return data
                     
     def check_column_name(self):
         tb = self.table_name
         sql = f"select COLUMN_NAME,COLUMN_TYPE,COLUMN_COMMENT from information_schema.columns where table_name= '{tb}';"
@@ -192,40 +190,51 @@
         df_cur = df.copy()
         df_cur = df_cur.loc[(df_cur[date_col]>= cur_start_date)&(df_cur[date_col]<= cur_end_date)]
         df_cur[checked_col] = df_cur[checked_col].astype('float')
         df_prev = df.copy()
         df_prev = df_prev.loc[(df_prev[date_col]>= prev_start_date)&(df_prev[date_col]<= prev_end_date)]
         df_prev[checked_col] = df_prev[checked_col].astype('float')
         count = 0
+        warning = pd.DataFrame(columns={'Warning'})
         if df_prev[checked_col].max() < df_cur[checked_col].min():
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of prev < min of current, the current date range of data is much higher than the previous date range, {df_prev[checked_col].max()}<{df_cur[checked_col].min()}, {checked_col} is out of range!"
+            result_1 = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of prev < min of current, the current date range of data is much higher than the previous date range, {df_prev[checked_col].max()}<{df_cur[checked_col].min()}, {checked_col} is out of range!"
+            warning_1 = pd.DataFrame({'Warning':[result_1]})
+            warning = pd.concat([warning,warning_1],axis=0)
         else:
             count += 1
         if df_cur[checked_col].max()/df_prev[checked_col].max() >= x1:
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of current / max of prev >= {x1}, the current date range of data is {x1} higher than the previous date range, {df_cur[checked_col].max()}/{df_prev[checked_col].max()}>={x1}, {checked_col} is out of range!"
+            result_2 = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of current / max of prev >= {x1}, the current date range of data is {x1} higher than the previous date range, {df_cur[checked_col].max()}/{df_prev[checked_col].max()}>={x1}, {checked_col} is out of range!"
+            warning_2 = pd.DataFrame({'Warning':[result_2]})
+            warning = pd.concat([warning,warning_2],axis=0)
         else:
             count += 1
         if df_prev[checked_col].min()/df_cur[checked_col].min() >= x1:
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev / min of current >= {x1}, the current date range of data is {x1} lower than the previous date range, {df_prev[checked_col].min()}/{df_cur[checked_col].min()}>={x1}, {checked_col} is out of range!"
+            result_3 = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev / min of current >= {x1}, the current date range of data is {x1} lower than the previous date range, {df_prev[checked_col].min()}/{df_cur[checked_col].min()}>={x1}, {checked_col} is out of range!"
+            warning_3 = pd.DataFrame({'Warning':[result_3]})
+            warning = pd.concat([warning,warning_3],axis=0)
         else:
             count += 1
         if  df_prev[checked_col].min() >df_cur[checked_col].max():
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev > max of current, the current date range of data is much lower than the previous date range, {df_prev[checked_col].min()}>{df_cur[checked_col].max()}, {checked_col} is out of range!"
+            result_4 = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev > max of current, the current date range of data is much lower than the previous date range, {df_prev[checked_col].min()}>{df_cur[checked_col].max()}, {checked_col} is out of range!"
+            warning_4 = pd.DataFrame({'Warning':[result_4]})
+            warning = pd.concat([warning,warning_4],axis=0)
         else:
             count += 1
         if  abs(df_cur[checked_col].median()) / abs(df_prev[checked_col].median()) >= x1:
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the median of current / median of prev >= {x1}, the current date range of median of data is {x1} higher than the previous date range, {df_cur[checked_col].median()}/{df_prev[checked_col].median()}>={x1}, {checked_col} is out of range!"
+            result_5 = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the median of current / median of prev >= {x1}, the current date range of median of data is {x1} higher than the previous date range, {df_cur[checked_col].median()}/{df_prev[checked_col].median()}>={x1}, {checked_col} is out of range!"
+            warning_5 = pd.DataFrame({'Warning':[result_5]})
+            warning = pd.concat([warning,warning_5],axis=0)
         else:
             count += 1
         if count == 5:
-            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, {checked_col} is in the range."
+            warning = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, {checked_col} is in the range."
         if notification != 'disabled':
-            content = result
+            content = warning
             send_message_user(user_id,content)  
-        return result
+        return warning
     def check_enum(self,enum_col):
         tb = self.df
         col_enum = tb.groupby(enum_col)[enum_col].count()
         result = f"The {enum_col} has following enums:{col_enum.index}. \n Please check carefully if the enums are complete!"
         return result
```

### Comparing `datalibro_backend-1.1.0/datalibro_backend/read_file.py` & `datalibro_backend-1.1.1/datalibro_backend/read_file.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.1.0/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.1/datalibro_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.1.0
+Version: 1.1.1
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.1.0/setup.py` & `datalibro_backend-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.1.0",
+  version="1.1.1",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

