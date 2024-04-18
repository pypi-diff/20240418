# Comparing `tmp/com.castsoftware.uc.arg-1.7.2.tar.gz` & `tmp/com_castsoftware_uc_arg-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.arg-1.7.2.tar", last modified: Fri Mar 15 21:18:47 2024, max compression
+gzip compressed data, was "com_castsoftware_uc_arg-1.7.3.tar", last modified: Thu Apr 18 19:40:44 2024, max compression
```

## Comparing `com.castsoftware.uc.arg-1.7.2.tar` & `com_castsoftware_uc_arg-1.7.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 21:18:47.603641 com.castsoftware.uc.arg-1.7.2/
--rw-rw-rw-   0        0        0      918 2024-03-15 21:18:47.587665 com.castsoftware.uc.arg-1.7.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-15 21:18:47.202161 com.castsoftware.uc.arg-1.7.2/cast_arg/
--rw-rw-rw-   0        0        0     1429 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     8669 2024-02-14 14:50:20.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0      338 2023-12-20 18:51:05.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/apikey_test.py
--rw-rw-rw-   0        0        0     1004 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/cause.json
--rw-rw-rw-   0        0        0     7689 2024-02-05 21:42:15.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/config.py
--rw-rw-rw-   0        0        0    28245 2024-03-15 21:04:31.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/convert.py
--rw-rw-rw-   0        0        0      624 2023-08-25 16:17:25.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/keycloak_test.py
--rw-rw-rw-   0        0        0     1042 2024-02-05 15:11:37.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2024-03-15 21:18:47.488938 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0     6344 2023-11-28 18:25:50.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_benchmark.py
--rw-rw-rw-   0        0        0     4589 2024-02-12 18:04:52.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_cloud.py
--rw-rw-rw-   0        0        0     4567 2024-02-08 21:15:16.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_greenIt.py
--rw-rw-rw-   0        0        0     1326 2024-02-07 21:38:46.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_report.py
--rw-rw-rw-   0        0        0     9057 2024-02-20 14:45:39.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_summary.py
--rw-rw-rw-   0        0        0     3191 2023-12-27 13:33:57.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_grades.py
--rw-rw-rw-   0        0        0     1084 2024-01-05 20:20:49.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_overview.py
--rw-rw-rw-   0        0        0      890 2024-02-07 20:58:01.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_report.py
--rw-rw-rw-   0        0        0     4593 2024-03-15 19:02:18.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_sizing.py
--rw-rw-rw-   0        0        0     1780 2024-02-21 18:47:01.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_strengh_improvement.py
--rw-rw-rw-   0        0        0     3582 2024-03-15 20:51:57.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_tech_detail_table.py
--rw-rw-rw-   0        0        0     9012 2024-02-14 21:54:47.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    34636 2024-02-20 19:28:49.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/stats.py
--rw-rw-rw-   0        0        0    14091 2024-01-28 17:19:54.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/test copy.py
--rw-rw-rw-   0        0        0    11974 2024-01-29 19:02:47.000000 com.castsoftware.uc.arg-1.7.2/cast_arg/test.py
-drwxrwxrwx   0        0        0        0 2024-03-15 21:18:47.575636 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0      918 2024-03-15 21:18:46.000000 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2024-03-15 21:18:46.000000 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 21:18:46.000000 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-03-15 21:18:46.000000 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-15 21:18:46.000000 com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      806 2024-03-15 21:18:08.000000 com.castsoftware.uc.arg-1.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-15 21:18:47.603641 com.castsoftware.uc.arg-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.635631 com_castsoftware_uc_arg-1.7.3/
+-rw-rw-rw-   0        0        0      943 2024-04-18 19:40:44.590190 com_castsoftware_uc_arg-1.7.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.353321 com_castsoftware_uc_arg-1.7.3/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     8669 2024-02-14 14:50:20.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0      338 2023-12-20 18:51:05.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/apikey_test.py
+-rw-rw-rw-   0        0        0     1004 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     7689 2024-02-05 21:42:15.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/config.py
+-rw-rw-rw-   0        0        0    28200 2024-04-18 19:37:06.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/convert.py
+-rw-rw-rw-   0        0        0      624 2023-08-25 16:17:25.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/keycloak_test.py
+-rw-rw-rw-   0        0        0     1042 2024-02-05 15:11:37.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/main.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.496418 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/__init__.py
+-rw-rw-rw-   0        0        0     6344 2023-11-28 18:25:50.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_benchmark.py
+-rw-rw-rw-   0        0        0     4985 2024-04-12 21:15:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_cloud.py
+-rw-rw-rw-   0        0        0     4567 2024-02-08 21:15:16.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_greenIt.py
+-rw-rw-rw-   0        0        0     2344 2024-04-13 15:52:11.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_report.py
+-rw-rw-rw-   0        0        0    11293 2024-04-15 19:53:46.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_summary.py
+-rw-rw-rw-   0        0        0     3191 2023-12-27 13:33:57.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_grades.py
+-rw-rw-rw-   0        0        0     1084 2024-01-05 20:20:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_overview.py
+-rw-rw-rw-   0        0        0      890 2024-02-07 20:58:01.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_report.py
+-rw-rw-rw-   0        0        0     4593 2024-03-15 19:02:18.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_sizing.py
+-rw-rw-rw-   0        0        0     1780 2024-02-21 18:47:01.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_strengh_improvement.py
+-rw-rw-rw-   0        0        0     3582 2024-03-15 20:51:57.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_tech_detail_table.py
+-rw-rw-rw-   0        0        0     9012 2024-02-14 21:54:47.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    34636 2024-02-20 19:28:49.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/stats.py
+-rw-rw-rw-   0        0        0    14091 2024-01-28 17:19:54.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/test copy.py
+-rw-rw-rw-   0        0        0    11974 2024-01-29 19:02:47.000000 com_castsoftware_uc_arg-1.7.3/cast_arg/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:40:44.578467 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0      943 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      919 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 19:40:44.000000 com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      817 2024-04-18 19:39:27.000000 com_castsoftware_uc_arg-1.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:40:44.635631 com_castsoftware_uc_arg-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-06-15 16:10:33.000000 com_castsoftware_uc_arg-1.7.3/setup.py
```

### Comparing `com.castsoftware.uc.arg-1.7.2/PKG-INFO` & `com_castsoftware_uc_arg-1.7.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.7.2
+Version: 1.7.3
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Author-email: Nevin Kaplan <n.kaplan@castsoftware.com>, DD Assessment Team <Team.ddassessments@castsoftware.com>
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: documentation, https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: python-pptx==0.6.19
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.8
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: IPython
 Requires-Dist: requests
 Requires-Dist: Jinja2
 Requires-Dist: setuptools
+Requires-Dist: inflect
```

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/Effort.csv` & `com_castsoftware_uc_arg-1.7.3/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/actionPlan.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/actionPlan.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/cause.json` & `com_castsoftware_uc_arg-1.7.3/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/config.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/convert.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,22 +84,21 @@
                 StrengthImprovment()
             ]
         if config.hl_active:
             self.info("Collecting Highlight Data")
             hl = Highlight(hl_base_url=config.hl_url,hl_user=config.hl_user,hl_pswd=config.hl_password, \
                            hl_instance=config.hl_instance,hl_apps=config.hl_list)
             self.hl_portfolio_pages = [
-                HighlightSummary(self.day_rate)
+                HighlightSummary(self.day_rate,self._config.output,ppt=self._ppt)
             ]
             self.hl_pages = [
-                CloudMaturity(self._config.output,ppt=self._ppt),
+                CloudMaturity(),
                 GreenIt(),
                 HighlightSummary(self.day_rate),
-                HighlightBenchmark(),
-
+                HighlightBenchmark()
             ]
             self._hl_data = HLData(config,log_level=config.logging_highlight)
 
         #project level work
         app_cnt = len(config.application)
 
         # self.remove_proc_slides(self._generate_procs)
@@ -229,14 +228,18 @@
 
         """Highlight Portfolio level pages """
         if self._config.hl_active:
             for proc in self.hl_portfolio_pages:
                 proc.report(hl_list)
 
         self._ppt.replace_text('{app_cnt}',app_cnt)
+
+        from inflect import engine
+        self._ppt.replace_text('{app_cnt_as_word}',engine().number_to_words(app_cnt))
+
         for idx in range(0,app_cnt):
             # create instance of action plan class 
             self.ap = ActionPlan (app_list,self._aip_data,self._ppt,self._config.output,day_rate)
             fix_now_total=AIPStats(day_rate,logger_level=self._config.logging_generate)
             near_term_total=AIPStats(day_rate,logger_level=self._config.logging_generate)
             mid_long_term=AIPStats(day_rate,logger_level=self._config.logging_generate)
             summary_total=AIPStats(day_rate,logger_level=self._config.logging_generate)
@@ -247,27 +250,23 @@
             app_no = idx+1
             app_id = app_list[idx]
             hl_id = hl_list[idx]
             app_title = self._config.title_list[idx]
             self.info(f'********************* Working on pages for {app_title} ******************************')
             self._ppt.replace_text(f'{{app{app_no}_name}}',app_title)
 
-            if self._config.aip_active:
-                for proc in self.mri_pages:
-                    self.info(f'Generating {proc.description}')
-                    proc.run(app_id,app_no)
-
-            if self._config.hl_active:
-                for proc in self.hl_pages:
-                    proc.report(hl_id,app_no)
 
             if self._config.aip_active:
                 if self._aip_data.has_data(app_id):
                     self.info('Preparing AIP Data')
-                    #self.info(f'Working on {app_id} ({self._appl_title[app_id]})')
+
+                    #Run MRI pages
+                    for proc in self.mri_pages:
+                        self.info(f'Generating {proc.description}')
+                        proc.run(app_id,app_no)
 
                     self.info('Filling risk factors for the executive summary page')
                     # do risk factors for the executive summary page
                     risk_grades = self.each_risk_factor(self._aip_data,app_id, app_no)
                     self._ppt.replace_text(f'{{app{app_no}_high_risk_grade_names}}',list_to_text(risk_grades.index.values))
 
                     snapshot = self._aip_data.snapshot(app=app_id)
@@ -339,14 +338,17 @@
                             iso_Maintainaility = iso_df[iso_df.category == 'Maintainability' ]
                             iso_MaintainailityCall = iso_Maintainaility["count"].sum()
                             self._ppt.replace_text(f'{{app{app_no}_ISO_5055}}', round((iso_MaintainailityCall/(pourcentage_iso5055/2))*100,1))
                         except ValueError as ex:
                             self.warning(ex)                    
             #replaceHighlight application specific data
             if self._config.hl_active and self._hl_data.has_data(hl_id):
+                for proc in self.hl_pages:
+                    proc.report(hl_id,app_no)
+
                 try:
                     (oss_crit,oss_high,oss_med,lic,components) = self.oss_risk_assessment(hl_id,app_no,day_rate)
                     fix_now_total.add_effort(oss_crit.effort)
                     fix_now_total.add_violations(oss_crit.violations)
 
                     near_term_total.add_effort(oss_high.effort)
                     near_term_total.add_effort(oss_med.effort)
@@ -495,14 +497,15 @@
             self.warning('This application contains no critical violations')
 
     def oss_risk_assessment(self,hl_id,app_no,day_rate):
         self.info('Filling OSS risk assessment table')
         lic_df=self._hl_data.get_lic_info(hl_id)
         lic_df=self._hl_data.sort_lic_info(lic_df)
         oss_df=self._hl_data.get_cve_info(hl_id)
+        lic = LicenseStats(logger_level=self._config.logging_generate)
         # lic_summary = pd.DataFrame(columns=['License Type','Risk Factor','Component Count','Example'])
 
         oss_crit = OssStats(hl_id,day_rate,self._hl_data,'crit',logger_level=self._config.logging_generate)
         oss_crit_comp_tot = self._hl_data.get_cve_crit_comp_tot(hl_id)
 
         oss_high = OssStats(hl_id,day_rate,self._hl_data,'high',logger_level=self._config.logging_generate)
         oss_high_comp_tot = self._hl_data.get_cve_high_comp_tot(hl_id)
@@ -546,15 +549,14 @@
             lic_summary.sort_values(['risk','license','comp count'],inplace=True)
 
             #remove low and undefined records from the table
             lic_summary=lic_summary[lic_summary["risk"].str.contains("Low")==False]
             lic_summary=lic_summary[lic_summary["risk"].str.contains("Undefined")==False]
 
             # are there any records left?
-            lic = LicenseStats(logger_level=self._config.logging_generate)
             if not lic_summary.empty:
                 #modify the forground color
                 lic_summary.loc[lic_summary['risk']=='High','forground']='211,76,76'
                 lic_summary.loc[lic_summary['risk']=='Medium','forground']='127,127,127'
 
                 #update the powerpoint table
                 tbl_name = f'app{app_no}_hl_table_lic_risks'
@@ -569,16 +571,14 @@
 
                 # #add the high and medium license risk counts to the deck
                 # self._ppt.replace_text(f'{{app{app_no}_high_lic_tot}}',
                 #     lic_summary[lic_summary['risk']=='High']['comp count'].sum())
                 # self._ppt.replace_text(f'{{app{app_no}_med_lic_tot}}',
                 #     lic_summary[lic_summary['risk']=='Medium']['comp count'].sum())
 
-            lic.replace_text(self._ppt,app_no)
-        else:
-            lic = DataFrame()
+        lic.replace_text(self._ppt,app_no)
         return (oss_crit,oss_high,oss_med,lic,total_components)
```

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/keycloak_test.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/keycloak_test.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/main.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_benchmark.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_benchmark.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_cloud.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_cloud.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,36 +10,43 @@
 from sys import exc_info
 
 class CloudMaturity(HLPage):
 
     def report(self,app:str,app_no:int) -> bool:
         status = True
         try:
-            self.prefix = f'app{app_no}'
-            self.slide = self.ppt.get_slide(self.ppt.get_shape_by_name(f'{self.prefix}_CloudTechPieChart'))
+            self.tag_prefix = f'app{app_no}'
+            self.slide = self.ppt.get_slide(self.ppt.get_shape_by_name(f'{self.tag_prefix}_CloudTechPieChart'))
             metrics = self._get_metrics(app)
 
-            self.ppt.replace_text(f'{{{self.prefix}_hl_CloudIndex}}',round(self._get_metrics(app)['cloudReady']*100,2),slide=self.slide)
+            self.replace_text('CloudIndex',round(self._get_metrics(app)['cloudReady']*100,1),shape=True,slide=self.slide)
 
             # get the cloud data from the Highlight REST API
             data = self.get_data(app)
             #export it to excel
             self.create_excel(app,data,self._output)
 
-            self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_total_roadblocks}}',int(metrics['roadblocks']),slide=self.slide)
-            self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_total_blockers}}',round(metrics['blockers']*100,1),slide=self.slide)
-            self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_total_boosters}}',round(metrics['boosters']*100,1),slide=self.slide)
+            #this slide has tags that are both text embedded and shape named
+            for shape in [True,False]:
+                self.replace_text('cloud_total_roadblocks',int(metrics['roadblocks']),slide=self.slide,shape=shape)
+                self.replace_text('cloud_total_blockers',round(metrics['blockers']*100,1),slide=self.slide,shape=shape)
+                self.replace_text('cloud_total_boosters',round(metrics['boosters']*100,1),slide=self.slide,shape=shape)
+
+
+            # self.ppt.replace_text(f'{{{self.tag_prefix}_hl_cloud_total_roadblocks}}',int(metrics['roadblocks']),slide=self.slide)
+            # self.ppt.replace_text(f'{{{self.tag_prefix}_hl_cloud_total_blockers}}',round(metrics['blockers']*100,1),slide=self.slide)
+            # self.ppt.replace_text(f'{{{self.tag_prefix}_hl_cloud_total_boosters}}',round(metrics['boosters']*100,1),slide=self.slide)
             self.get_cloud_totals(data)
                 
             # update the techology chart
             agr = data[['Technology','NB Roadblocks']].groupby('Technology').aggregate('sum').reindex()
-            self.ppt.update_chart(f'{self.prefix}_CloudTechPieChart',agr)
+            self.ppt.update_chart(f'{self.tag_prefix}_CloudTechPieChart',agr)
 
             data = data.drop(columns=['Files'])
-            self.ppt.update_table(f'{self.prefix}_CloudDetailTable',data,app,include_index=False)  
+            self.ppt.update_table(f'{self.tag_prefix}_CloudDetailTable',data,app,include_index=False)  
             pass      
         except Exception as ex:
             ex_type, ex_value, ex_traceback = exc_info()
             self.log.error(f'{ex_type.__name__}: {ex_value} while in {__class__}')
             status = False
 
         return status
@@ -66,29 +73,29 @@
 
     def get_cloud_totals(self,data:DataFrame) -> None:
         total = data.sum(numeric_only=True)
 
         total_effort=round(total['Effort'],1)
         total_blockers=round(total['NB Roadblocks'],0)
 
-        self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_total_effort}}',total_effort,slide=self.slide)
+        self.replace_text('cloud_total_effort',total_effort,slide=self.slide)
 
         #get the top tech and total occurences for it
         agr = data[['Technology','NB Roadblocks']]. \
             groupby('Technology').aggregate('sum'). \
             sort_values('NB Roadblocks',ascending=False)
 
         agr.iloc[:1] # get the first row (top language)
         df = agr.iloc[:1]
 
-        self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_top_tech}}',agr.index[0],slide=self.slide)
-        self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_top_tech_total}}',int(agr['NB Roadblocks'].iloc[0]),slide=self.slide)
+        self.replace_text('cloud_top_tech',agr.index[0],slide=self.slide)
+        self.replace_text('cloud_top_tech_total',int(agr['NB Roadblocks'].iloc[0]),slide=self.slide)
 
         #len(data[data['']])
-        self.ppt.replace_text(f'{{{self.prefix}_hl_cloud_top_tech_total}}',int(agr['NB Roadblocks'].iloc[0]),slide=self.slide)
+        self.replace_text('cloud_top_tech_total',int(agr['NB Roadblocks'].iloc[0]),slide=self.slide)
 
 
     def create_excel(self,app_name:str,data:DataFrame,output:str):
         file_name = abspath(f'{output}/Cloud-Maturity-{app_name}.xlsx')
         writer = ExcelWriter(file_name, engine='xlsxwriter')
         col_widths=[50,10,10,10,10,10,10]
         cloud_tab = format_table(writer,data,'Cloud Data',col_widths)
```

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_greenIt.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_greenIt.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_report.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 from cast_common.highlight import Highlight
 from cast_arg.powerpoint import PowerPoint
 from cast_common.logger import Logger,INFO
+from pandas import DataFrame
 
 
 class HLPage(Highlight):
 
     _ppt=None
     _log = None
     _output = None
+    _benchmark = None
+
+    _tag_prefix = None
 
     @property
     def ppt(self) -> PowerPoint:
         return HLPage._ppt
-    
+
+    @property
+    def tag_prefix(self) -> str:
+        if self._tag_prefix is None:
+            raise ValueError(f'tag prefix is not set')
+        return self._tag_prefix
+    @tag_prefix.setter
+    def tag_prefix(self,value):
+        self._tag_prefix=f'{value}_hl'
+   
     @property
     def output(self) -> str:
         return HLPage._output
     
+    @property
+    def log(self) -> str:
+        return HLPage._log
+    
+    @property
+    def ppt(self) -> str:
+        return HLPage._ppt
+        
     def __init__(self,output:str=None,ppt:PowerPoint=None,  
                  hl_user:str=None, hl_pswd:str=None,hl_basic_auth=None, hl_instance:int=0,
                  hl_apps:str=[],hl_tags:str=[], 
                  hl_base_url:str=None, 
                  log_level=INFO):
         
         if HLPage._log is None:
@@ -35,9 +56,22 @@
             if output is None:
                 raise AttributeError('output must be defined in the first instance of HLPage')
             else:
                 HLPage._output=output
 
         super().__init__(hl_user, hl_pswd,hl_basic_auth, hl_instance,hl_apps,hl_tags, hl_base_url, log_level)
 
+        if HLPage._benchmark is None:
+            HLPage._benchmark = DataFrame(self._get(r'/benchmark'))
+
+
+    def replace_text(self, item, data,shape=False,slide=None):
+        tag = f'{self.tag_prefix}_{item}'
+        self.log.debug(f'{tag}: {data}')
+        if shape:
+            # slide = PowerPoint.ppt._prs.slides[3]
+            PowerPoint.ppt.replace_textbox(tag,data,slide=slide)
+        else:
+            tag = f'{{{tag}}}'
+            PowerPoint.ppt.replace_text(tag,data,slide=slide)
```

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/hl_summary.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/hl_summary.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-
 from cast_common.highlight import Highlight
+from cast_arg.pages.hl_report import HLPage
 from cast_common.logger import Logger, INFO,DEBUG
 from cast_common.powerpoint import PowerPoint
 from cast_common.util import list_to_text,convert_LOC
 from pandas import concat,DataFrame
 from math import ceil
 
 from pandas import json_normalize
 from pptx.enum.shapes import MSO_SHAPE_TYPE
 
-class HighlightSummary(Highlight):
+class HighlightSummary(HLPage):
 
-    def __init__(self,day_rate:int):
-        super().__init__()
+    def __init__(self,day_rate:int,output:str=None,ppt:PowerPoint=None):
+        super().__init__(output=output,ppt=ppt)
         self._day_rate = day_rate
         pass        
 
-
     def report(self,app_name:str|list=None,app_no:int=0) -> bool:
         if type(app_name) is list:
             self.tag_prefix = 'port'
         else:
             self.tag_prefix = f'app{app_no}'
             app_name = [app_name]
-        self.tag_prefix = f'{self.tag_prefix}_hl'
-
 
         #create list of technolgies sorted by LOC in decending order
         tech_df = DataFrame()
         comp_total = 0
-        oss_cve_df = DataFrame()
+        # oss_cve_df = DataFrame()
         cloud_df = DataFrame()
         green_df = DataFrame()
 
         t_health=t_cloud=t_oss=t_green=0
         t_high_license = t_medium_license = t_low_license = t_license = 0
         low_health={}
         oss_cve_counts={}
         t_scores = self.calc_scores(app_name)
 
         scores = {}
 
+        oss={}
+        oss['cve']={}
+        oss['license']={}
         for app in app_name:
             df = self.get_technology(app)
             tech_df = concat([tech_df,df])
             #
 
             scores[app] = self.calc_scores([app])
 
@@ -54,20 +54,33 @@
             t_license += t_high_license + t_medium_license + t_low_license
 
             health = self.get_software_health_score(app)
             #save information to be used for ranking
             low_health[app]=health # save the health score for ranking
             
             comp_total += self.get_component_total(app)
-#            oss_score = self.get_software_oss_safty_score(app) 
-            cve_df=self.get_cve_critical(app)
-            if cve_df is not None:
-                oss_cve_counts[app]=len(cve_df['cve'].unique()) 
-                cve_df=cve_df['cve']
-                oss_cve_df = concat([oss_cve_df,cve_df])
+#            oss_score += self.get_software_oss_safty_score(app) 
+
+            """
+                get the Common Vulnerabilty and Exposue information by priority
+                
+                The highlight class has three methods get_cve_critical, get_cve_high
+                and get_cve_medum. (we don't care about the low priority items). Use 
+                them to retrieve the information and store it in a dictionary for later 
+                use.
+            """
+            for crit in ['critical','high','medium']:
+                mth = getattr(self,f'get_cve_{crit}')
+                df = mth(app)
+                if df is not None:
+                    if crit in oss['cve'].keys():
+                        oss['cve'][crit] = concat([oss['cve'][crit],df])
+                    else: 
+                        oss['cve'][crit] = df
+            pass
 
             df = self.get_cloud_detail(app)
             df = df[df['cloudRequirement.criticality'].isin(['Critical','High'])] 
             cloud_df = concat([cloud_df,df])
 
             green_df = concat([green_df,self.get_green_detail(app)])
             pass
@@ -84,44 +97,94 @@
             'effort':{'high':'minimal','medium':'medium','low':'considerable'},
             'risk':{'high':'low amount of','medium':'average','low':'very high'}
         }
 
         t_apps = len(app_name)
         for key in self.grades:
             score = t_scores[key] 
-            self.replace_text(f'{key}_score',score)
+            self.replace_text(f'{key}_score',score,shape=True)
 
             # calculate the "BEST" and "WORST" grades for each tile
             high=0
             low = 100
             for app in app_name:
                 a = scores[app]
                 g = a[key]
                 if g < low: low = g
                 if g > high: high = g
-            PowerPoint.ppt.replace_text(f'{{bm_worst_{key}_score}}',low)
-            PowerPoint.ppt.replace_text(f'{{bm_best_{key}_score}}',high)
-
-            threshold = self.grades[key]['threshold']
-            if len(threshold)>1:
-                if score < threshold[0]:
-                    hml = 'low'
-                elif score > threshold[1]:
-                    hml = 'high'
-                else:
-                    hml = 'medium'
-                color = self.get_hml_color(hml)
-                PowerPoint.ppt.fill_text_box_color(f'{self.tag_prefix}_{key}_tile',color)
 
-                for t in text:
-                    self.replace_text(f'{key}_{t}',text[t][hml])
+            self.replace_text(f'bmw_{key}_score',low,shape=True)
+            self.replace_text(f'bmb_{key}_score',high,shape=True)
+            self.replace_text(f'bmi_{key}_score',round(self._benchmark.loc[key]['avg']*100,2),shape=True)
+
+            # is this grade score above, below or equal to the industry average?
+            bm = round(Highlight._benchmark.loc[key]['avg']*100,2)
+            score_bm_hml = 'equal'
+            if score > bm:
+                score_bm_hml = 'high'
+            elif score < bm: 
+                score_bm_hml = 'low'
+            self.replace_text(f'{key}_bm_hle',score_bm_hml)
+
+            if key == 'openSourceSafety':
+                hml_risk = self.get_get_software_oss_risk(score=score)
+                self.replace_text(f'{key}_hml_risk',hml)
+                self.replace_text(f'{key}_risk',hml)
+
+                hml_score={'high':'low','medium':'medium','low':'high'}
+                self.replace_text(f'{key}_hml_score',hml_score[hml_risk])
+
+                total_cves = 0
+                total_cmpnts_df = DataFrame(columns=['component'])
+                for key in oss['cve'].keys():
+                    eff = 0
+                    cmpnt_df=DataFrame()
+                    df = oss['cve'][key]
+                    if df is not None:
+                        cmpnt_df['component']=df['component']
+                        if not cmpnt_df.empty:
+                            total_cmpnts_df = concat([cmpnt_df,total_cmpnts_df])
+                            eff = ceil(len(cmpnt_df['component'].unique())/2)
+                        cnt = len(df['cve'].unique())
+                        total_cves += cnt
+
+                    self.replace_text(f'{key}_cve_total',cnt)
+                    self.replace_text(f'{key}_cve_effort',eff)
+                    pass
+    
+                self.replace_text('cve_total',total_cves)
+                total_eff = 0
+                if not total_cmpnts_df.empty:
+                    total_eff = ceil(len(total_cmpnts_df['component'].unique())/2)
+                    self.replace_text(f'{key}_total_cve_effort',total_eff)
+
+
+                
+                self.replace_text('high_license_total',f'{t_high_license:,}')
+                self.replace_text('oss_effort',ceil(total_cves/2))
+                
+
+
+                # oss_cve_counts[app]=len(cve_df['cve'].unique()) 
+                # cve_df=cve_df['cve']
+                # oss_cve_df = concat([oss_cve_df,cve_df])
+            else:
+                threshold = self.grades[key]['threshold']
+                if len(threshold)>1:
+                    if score < threshold[0]:
+                        hml = 'low'
+                    elif score > threshold[1]:
+                        hml = 'high'
+                    else:
+                        hml = 'medium'
+                    color = self.get_hml_color(hml)
+                    PowerPoint.ppt.fill_text_box_color(f'{self.tag_prefix}_{key}_tile',color)
 
-
-        # oss_risk = self.get_get_software_oss_risk(score=metrics['openSourceSafety'])
-        # self.replace_text('oss_risk',oss_risk)
+                    for t in text:
+                        self.replace_text(f'{key}_{t}',text[t][hml])
 
         self.replace_text('app_count',t_apps)
 
         tech_df = tech_df.groupby(['technology']).sum().reset_index()   \
             [['technology', 'totalLinesOfCode', 'totalFiles']]          \
             .sort_values(by=['totalLinesOfCode'],ascending=False)
 
@@ -133,34 +196,21 @@
         self.replace_text('total_loc',f'{total_loc} {unit}')
 
         total_files = int(tech_df['totalFiles'].sum())
         self.replace_text('total_files',f'{total_files:,}')
         self.replace_text('oss_total_components',f'{comp_total:,}')
         self.replace_text('oss_total_licenses',f'{t_license:,}')
 
-        if oss_cve_df.empty:
-            oss_crit_vio_total = 0
-        else:
-            try:
-                oss_crit_vio_total = len(oss_cve_df[0].unique())
-            except KeyError:
-                oss_crit_vio_total = 0
-
-        self.replace_text('critical_cve_total',f'{oss_crit_vio_total:,}')
-        self.replace_text('high_license_total',f'{t_high_license:,}')
-        self.replace_text('oss_effort',ceil(oss_crit_vio_total/2))
-
-        # cloud_hml = self.get_get_cloud_hml(score=t_cloud)
-        # if cloud_hml == 'high':
-        #     cloud_eff_lvl = 'minimal'
-        # elif cloud_hml == 'medium':
-        #     cloud_eff_lvl = 'some'
-        # else: 
-        #     cloud_eff_lvl = 'good amount of'
-        # self.replace_text('cloud_effort_level',cloud_eff_lvl)
+        # if oss_cve_df.empty:
+        #     oss_crit_vio_total = 0
+        # else:
+        #     try:
+        #         oss_crit_vio_total = len(oss_cve_df[0].unique())
+        #     except KeyError:
+        #         oss_crit_vio_total = 0
         
         boosters = len(cloud_df[cloud_df['cloudRequirement.ruleType']=='BOOSTER'])
         blockers = len(cloud_df[cloud_df['cloudRequirement.ruleType']=='BLOCKER'])
         self.replace_text('cloud_booster_total',boosters)
         self.replace_text('cloud_blocker_total',blockers)
 
         if green_df.empty:
@@ -193,18 +243,14 @@
             return (0,0,0,0)
         low_app = min(factor, key=factor.get)
         low_score = round(factor[low_app],1)
         high_app = max(factor, key=factor.get)
         high_score = round(factor[high_app],1)
         return (low_app,low_score,high_app,high_score)
 
-    def replace_text(self, item, data):
-        tag = f'{{{self.tag_prefix}_{item}}}'
-        self.log.debug(f'{tag}: {data}')
-        PowerPoint.ppt.replace_text(tag,data)
 
 # from os.path import abspath
 # from cast_common.util import format_table
 # from pandas import ExcelWriter
 
 # ppt = PowerPoint(r'E:\work\Decks\highlight-test.pptx',r'E:\work\Decks\test\highlight.pptx')
```

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_grades.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_grades.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_overview.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_overview.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_report.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_report.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_sizing.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_sizing.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_strengh_improvement.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_strengh_improvement.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/pages/mri_tech_detail_table.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/pages/mri_tech_detail_table.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/powerpoint.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/powerpoint.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/restCall.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/restCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/stats.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/stats.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/test copy.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/test copy.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/cast_arg/test.py` & `com_castsoftware_uc_arg-1.7.3/cast_arg/test.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/PKG-INFO` & `com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.7.2
+Version: 1.7.3
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Author-email: Nevin Kaplan <n.kaplan@castsoftware.com>, DD Assessment Team <Team.ddassessments@castsoftware.com>
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: documentation, https://github.com/CAST-Extend/com.castsoftware.uc.arg/wiki
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: python-pptx==0.6.19
-Requires-Dist: com.castsoftware.uc.python.common>=1.1.8
+Requires-Dist: com.castsoftware.uc.python.common>=1.1.11
 Requires-Dist: IPython
 Requires-Dist: requests
 Requires-Dist: Jinja2
 Requires-Dist: setuptools
+Requires-Dist: inflect
```

### Comparing `com.castsoftware.uc.arg-1.7.2/com.castsoftware.uc.arg.egg-info/SOURCES.txt` & `com_castsoftware_uc_arg-1.7.3/com.castsoftware.uc.arg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.7.2/pyproject.toml` & `com_castsoftware_uc_arg-1.7.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name='com.castsoftware.uc.arg'
 description="Assessment Report Generator (ARG)"
-version='1.7.2' #prod version
+version='1.7.3' #prod version
 authors= [
     {name="Nevin Kaplan",email="n.kaplan@castsoftware.com"},
     {name="DD Assessment Team",email="Team.ddassessments@castsoftware.com"}
 ]
 readme="README.md"
-dependencies = ['pandas', 'python-pptx==0.6.19', 'com.castsoftware.uc.python.common>=1.1.8', 'IPython', 'requests', 'Jinja2','setuptools']
+dependencies = ['pandas', 'python-pptx==0.6.19', 'com.castsoftware.uc.python.common>=1.1.11', 'IPython', 'requests', 'Jinja2','setuptools','inflect']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.6"
 [project.urls]
```

