# Comparing `tmp/datalibro_backend-1.0.9.tar.gz` & `tmp/datalibro_backend-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.0.9.tar", last modified: Mon Feb 26 08:37:49 2024, max compression
+gzip compressed data, was "datalibro_backend-1.1.0.tar", last modified: Wed Apr 17 08:55:21 2024, max compression
```

## Comparing `datalibro_backend-1.0.9.tar` & `datalibro_backend-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-02-26 08:37:49.984860 datalibro_backend-1.0.9/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.0.9/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-02-26 08:37:49.984620 datalibro_backend-1.0.9/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.0.9/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-02-26 08:37:49.983443 datalibro_backend-1.0.9/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.0.9/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    11571 2024-02-26 08:37:01.000000 datalibro_backend-1.0.9/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)     6994 2024-02-01 06:18:54.000000 datalibro_backend-1.0.9/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-02-26 08:37:49.984399 datalibro_backend-1.0.9/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-02-26 08:37:49.000000 datalibro_backend-1.0.9/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-02-26 08:37:49.000000 datalibro_backend-1.0.9/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-02-26 08:37:49.000000 datalibro_backend-1.0.9/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-02-26 08:37:49.000000 datalibro_backend-1.0.9/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-02-26 08:37:49.984918 datalibro_backend-1.0.9/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-02-26 08:37:30.000000 datalibro_backend-1.0.9/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.520815 datalibro_backend-1.1.0/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.1.0/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-17 08:55:21.520490 datalibro_backend-1.1.0/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.1.0/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.519128 datalibro_backend-1.1.0/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.1.0/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    14859 2024-04-17 07:52:04.000000 datalibro_backend-1.1.0/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     6994 2024-02-01 06:18:54.000000 datalibro_backend-1.1.0/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-04-17 08:55:21.520264 datalibro_backend-1.1.0/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-04-17 08:55:21.000000 datalibro_backend-1.1.0/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-04-17 08:55:21.520874 datalibro_backend-1.1.0/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-04-17 08:54:58.000000 datalibro_backend-1.1.0/setup.py
```

### Comparing `datalibro_backend-1.0.9/LICENSE.txt` & `datalibro_backend-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.0.9/PKG-INFO` & `datalibro_backend-1.1.0/datalibro_backend.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datalibro_backend
-Version: 1.0.9
+Name: datalibro-backend
+Version: 1.1.0
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.0.9/README.md` & `datalibro_backend-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.0.9/datalibro_backend/quality_check.py` & `datalibro_backend-1.1.0/datalibro_backend/quality_check.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,34 +65,70 @@
                         suggestion = f"{i} position of the table's name is {seperate_table[i]}. Please carefully check it!"
                         wrong_col.append(seperate_table[i])
                         right_sugg.append(suggestion)
             else:
                     suggestion = f"{i} position of the table's name is incorrect! Please find the suitable name for this position! The enums for {i} position are ('tb','bi','map')."
                     wrong_col.append(seperate_table[i])
                     right_sugg.append(suggestion)
-        data_frame = {'Wrong Column':wrong_col,"Optimized Suggestion":right_sugg}
+        data_frame = {'Wrong Part of Table Name':wrong_col,"Optimized Suggestion of Table Name":right_sugg}
         data = pd.DataFrame(data_frame)
         return data
                     
-
+    def check_column_name(self):
+        tb = self.table_name
+        sql = f"select COLUMN_NAME,COLUMN_TYPE,COLUMN_COMMENT from information_schema.columns where table_name= '{tb}';"
+        execution_query= dc.sql_query('cfg.yaml',self.database,sql)
+        wrong_col = []
+        right_sugg = []
+        for i in range(len(execution_query)):
+            col_name = execution_query['COLUMN_NAME'][i]
+            if ' ' in col_name :
+                suggestion = f"The column name {col_name} contains space. Please remove the space and double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+            elif col_name.lower() != col_name:
+                suggestion = f"The column name {col_name} is not in lower case. Please double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+            elif col_name.startswith(' '):
+                suggestion = f"The column name {col_name} starts with a space. Please remove the space and double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+            elif col_name.endswith(' '):
+                suggestion = f"The column name {col_name} ends with a space. Please remove the space and double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+            elif col_name.startswith('_'):
+                suggestion = f"The column name {col_name} starts with an underscore. Please remove the underscore and double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+            elif col_name.endswith('_'):
+                suggestion = f"The column name {col_name} ends with an underscore. Please remove the underscore and double check it!"
+                wrong_col.append(col_name)
+                right_sugg.append(suggestion)
+        data_frame = {'Table Name':tb,'Wrong Column Name':wrong_col,"Optimized Suggestion of Column Name":right_sugg}
+        data = pd.DataFrame(data_frame)
+        if len(data['Table Name'])<1:
+            return 'There is no wrong column name in the table!'
+        else:
+            return data
 
     def basic_info_tb(self):
         tb = self.table_name
         sql = f"describe {tb}"
         execution_query= dc.sql_query('cfg.yaml',self.database,sql)
         col_len = execution_query['Field'].apply('nunique')
         sql_2 = f"select count(*) as cnt from {tb}"
         execution_query_2= dc.sql_query('cfg.yaml',self.database,sql_2)
         count_len = execution_query_2['cnt'][0]
         tot_len = 'The table '+str(tb)+' has '+str(col_len)+' columns'+' and '+str(count_len)+' records'
         return tot_len
     
     def check_missing_value(self):
         tb = self.df
-        
         miss = []
         index = []
         for col in tb.columns:
             for i in range(len(tb[col])):
                 if tb[col][i] is None or tb[col][i] == '':
                     miss.append(col)
                     index.append(i)
@@ -114,25 +150,28 @@
             result = '主键唯一，无重复记录。'
         else:
             result = f'主键不唯一，有重复记录。主键记录数：{df_primary["primary_key_cnt"][0]}, 全表记录数：{df_primary["total_cnt"][0]}'
         return result
     
     def check_qc(self,notification='disabled',user_id = ''):
         result_1 = self.check_name_database()
-        result_2 = self.check_missing_value()
-        result_3 = self.basic_info_tb()
+        result_2 = self.check_column_name()
+        result_3 = self.check_missing_value()
+        result_4 = self.basic_info_tb()
         if notification !='disabled':
             content_1 = result_1
-            send_a = send_card_message_user(user_id,content =content_1,title='Name QC')  
+            send_a = send_card_message_user(user_id,content =content_1,title='Table Name of {self.table_name} QC')  
             content_2 = result_2
-            send_b = send_card_message_user(user_id,content = content_2,title=f'Missing Value of {self.table_name}')  
+            send_b = send_card_message_user(user_id,content = content_2,title=f'Column Name of {self.table_name} QC')  
             content_3 = result_3
-            send_c = send_card_message_user(user_id,content = content_3,title=f'Basic Info of {self.table_name}') 
+            send_c = send_card_message_user(user_id,content = content_3,title=f'Missing Value of {self.table_name}')  
+            content_4= result_4
+            send_d = send_card_message_user(user_id,content = content_4,title=f'Basic Info of {self.table_name}') 
         send = 'True'
-        if send_a['msg'] != 'ok' or send_b['msg'] !='ok' or send_c['msg'] !='ok':
+        if send_a['msg'] != 'ok' or send_b['msg'] !='ok' or send_c['msg'] !='ok' or send_d['msg'] !='ok':
             send = 'False'
         return send
         
     def check_strange_data(self,checked_col,date_col,x1='',cur_start_date='',cur_end_date='',prev_start_date='',prev_end_date='',notification='disabled',user_id = ''):
         df = self.df
         df[date_col] = df[date_col].apply(lambda x:(pd.to_datetime(x)).strftime('%Y-%m-%d'))
         today = (datetime.now()).strftime('%Y-%m-%d')
@@ -143,37 +182,46 @@
         else:
             cur_start_date = (pd.to_datetime(cur_start_date)).strftime('%Y-%m-%d')
             cur_end_date = (pd.to_datetime(cur_end_date)).strftime('%Y-%m-%d')
         if prev_start_date == '' and prev_end_date == '':
             prev_start_date = (pd.to_datetime(cur_start_date)- relativedelta(days=31)).strftime('%Y-%m-%d')
             prev_end_date = (pd.to_datetime(prev_start_date)+relativedelta(days = 30)).strftime('%Y-%m-%d')
                     
-        
         if x1 == '':
             x1 = 1.4
         
         df_cur = df.copy()
         df_cur = df_cur.loc[(df_cur[date_col]>= cur_start_date)&(df_cur[date_col]<= cur_end_date)]
         df_cur[checked_col] = df_cur[checked_col].astype('float')
         df_prev = df.copy()
         df_prev = df_prev.loc[(df_prev[date_col]>= prev_start_date)&(df_prev[date_col]<= prev_end_date)]
         df_prev[checked_col] = df_prev[checked_col].astype('float')
-        
+        count = 0
         if df_prev[checked_col].max() < df_cur[checked_col].min():
-            result = f"compare with the {prev_start_date}-{prev_end_date}, the current date range of data is much higher than the previous date range, {df_prev[checked_col].max()}<{df_cur[checked_col].min()}, {checked_col} is out of range!"
-        elif df_cur[checked_col].max()/df_prev[checked_col].max() >= x1:
-            result = f"compare with the {prev_start_date}-{prev_end_date}, the current date range of data is {x1} higher than the previous date range, {df_cur[checked_col].max()}/{df_prev[checked_col].max()}>={x1}, {checked_col} is out of range!"
-        elif df_prev[checked_col].min()/df_cur[checked_col].min() >= x1:
-            result = f"compare with the {prev_start_date}-{prev_end_date}, the current date range of data is {x1} lower than the previous date range, {df_prev[checked_col].min()}/{df_cur[checked_col].min()}>={x1}, {checked_col} is out of range!"
-        elif  df_prev[checked_col].min() >df_cur[checked_col].max():
-            result = f"compare with the {prev_start_date}-{prev_end_date}, the current date range of data is much lower than the previous date range, {df_prev[checked_col].min()}>{df_cur[checked_col].max()}, {checked_col} is out of range!"
-        elif  abs(df_cur[checked_col].median()) / abs(df_prev[checked_col].median()) >= x1:
-            result = f"compare with the {prev_start_date}-{prev_end_date}, the current date range of median of data is {x1} higher than the previous date range, {df_cur[checked_col].median()}/{df_prev[checked_col].median()}>={x1}, {checked_col} is out of range!"
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of prev < min of current, the current date range of data is much higher than the previous date range, {df_prev[checked_col].max()}<{df_cur[checked_col].min()}, {checked_col} is out of range!"
+        else:
+            count += 1
+        if df_cur[checked_col].max()/df_prev[checked_col].max() >= x1:
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the max of current / max of prev >= {x1}, the current date range of data is {x1} higher than the previous date range, {df_cur[checked_col].max()}/{df_prev[checked_col].max()}>={x1}, {checked_col} is out of range!"
+        else:
+            count += 1
+        if df_prev[checked_col].min()/df_cur[checked_col].min() >= x1:
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev / min of current >= {x1}, the current date range of data is {x1} lower than the previous date range, {df_prev[checked_col].min()}/{df_cur[checked_col].min()}>={x1}, {checked_col} is out of range!"
+        else:
+            count += 1
+        if  df_prev[checked_col].min() >df_cur[checked_col].max():
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the min of prev > max of current, the current date range of data is much lower than the previous date range, {df_prev[checked_col].min()}>{df_cur[checked_col].max()}, {checked_col} is out of range!"
+        else:
+            count += 1
+        if  abs(df_cur[checked_col].median()) / abs(df_prev[checked_col].median()) >= x1:
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, checking with the median of current / median of prev >= {x1}, the current date range of median of data is {x1} higher than the previous date range, {df_cur[checked_col].median()}/{df_prev[checked_col].median()}>={x1}, {checked_col} is out of range!"
         else:
-            result = f"compare with the {prev_start_date}-{prev_end_date}, {checked_col} is in the range."
+            count += 1
+        if count == 5:
+            result = f"Current date range {cur_start_date}-{cur_end_date}, comparing with the {prev_start_date}-{prev_end_date}, {checked_col} is in the range."
         if notification != 'disabled':
             content = result
             send_message_user(user_id,content)  
         return result
     def check_enum(self,enum_col):
         tb = self.df
         col_enum = tb.groupby(enum_col)[enum_col].count()
@@ -184,23 +232,23 @@
     def check_missing_date(self,date_col='',start_date='',end_date='',notification='disabled',user_id=''):
         tb = self.df
         date_tb = self.date_df
         date_tb = date_tb.rename(columns = {'date':'date_map'})
         if date_col =='':
             date_col = self.date_col
         tb[date_col] = pd.to_datetime(tb[date_col]).apply(lambda x:x.strftime('%Y-%m-%d'))
-        if start_date == '':
-            date_tb = date_tb[date_tb['date_map']>=tb[date_col].min()]
-        elif start_date!= '' and end_date !='':
-            date_tb = date_tb.loc[(date_tb['date_map']>=start_date)&(date_tb['date_map']<=end_date)]
-        elif start_date !='' and end_date =='':
-            date_tb = date_tb.loc[(date_tb['date_map']>=start_date)]
-        elif start_date == '' and end_date != '':
-            date_tb = date_tb.loc[(date_tb['date_map']<=end_date)]
-        date_check = date_tb.merge(tb[date_col],left_on = 'date_map',right_on = date_col,how='left')
+        if start_date =='':
+            date_tb = date_tb[date_tb['date_map']>=tb[date_col].min()].reset_index(drop=True)
+        elif start_date !='':
+            date_tb = date_tb[date_tb['date_map']>=start_date].reset_index(drop=True)
+        if end_date !='':
+            date_tb = date_tb[date_tb['date_map']<=end_date].reset_index(drop=True)
+        data_list = tb[[date_col]].drop_duplicates()
+        date_tb['date_map'] = pd.to_datetime(date_tb['date_map']).apply(lambda x:x.strftime('%Y-%m-%d'))
+        date_check = date_tb.merge(data_list,left_on = 'date_map',right_on = date_col,how='left')
         date_check_miss = date_check[date_check[date_col].isna()].reset_index(drop=True)
         miss_date = pd.unique(date_check_miss['date_map'])
         length = date_check_miss['date_map'].apply('nunique')
         result  = f"In {self.table_name} : The {date_col} has {length} missing dates.\n The missing dates are \n {miss_date}"
         if notification !='disabled':
             send_card = send_card_message_user(user_id,content =result,title='Missing Date QC')
```

### Comparing `datalibro_backend-1.0.9/datalibro_backend/read_file.py` & `datalibro_backend-1.1.0/datalibro_backend/read_file.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.0.9/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datalibro-backend
-Version: 1.0.9
+Name: datalibro_backend
+Version: 1.1.0
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.0.9/setup.py` & `datalibro_backend-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.0.9",
+  version="1.1.0",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

