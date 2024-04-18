# Comparing `tmp/mns-scheduler-1.0.2.4.tar.gz` & `tmp/mns-scheduler-1.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.2.4.tar", last modified: Mon Apr 15 03:00:32 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.2.5.tar", last modified: Thu Apr 18 09:35:39 2024, max compression
```

## Comparing `mns-scheduler-1.0.2.4.tar` & `mns-scheduler-1.0.2.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.983014 mns-scheduler-1.0.2.4/
--rw-rw-rw-   0        0        0       62 2024-04-15 03:00:32.982017 mns-scheduler-1.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.949103 mns-scheduler-1.0.2.4/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.951098 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.4/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.953092 mns-scheduler-1.0.2.4/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20330 2024-04-11 14:07:31.000000 mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.954089 mns-scheduler-1.0.2.4/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.954089 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.957082 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.957082 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.958079 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.959077 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.961071 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8757 2024-04-15 03:00:19.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.962069 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.963066 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.965060 mns-scheduler-1.0.2.4/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.965060 mns-scheduler-1.0.2.4/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.966058 mns-scheduler-1.0.2.4/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.4/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.4/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.967056 mns-scheduler-1.0.2.4/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.968052 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.969049 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.970048 mns-scheduler-1.0.2.4/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.970048 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.971044 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.972042 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.973039 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.975034 mns-scheduler-1.0.2.4/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.976031 mns-scheduler-1.0.2.4/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.4/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.979024 mns-scheduler-1.0.2.4/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-12 05:21:45.000000 mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.981019 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:00:32.982017 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3014 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 03:00:32.000000 mns-scheduler-1.0.2.4/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 03:00:32.983014 mns-scheduler-1.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-15 03:00:19.000000 mns-scheduler-1.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.178888 mns-scheduler-1.0.2.5/
+-rw-rw-rw-   0        0        0       62 2024-04-18 09:35:39.178888 mns-scheduler-1.0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.145976 mns-scheduler-1.0.2.5/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.148968 mns-scheduler-1.0.2.5/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.5/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.149966 mns-scheduler-1.0.2.5/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20330 2024-04-17 00:31:02.000000 mns-scheduler-1.0.2.5/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.150963 mns-scheduler-1.0.2.5/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.151960 mns-scheduler-1.0.2.5/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.153955 mns-scheduler-1.0.2.5/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.153955 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.154952 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.156947 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.157944 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.159941 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.160936 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.162931 mns-scheduler-1.0.2.5/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.5/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.162931 mns-scheduler-1.0.2.5/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.163928 mns-scheduler-1.0.2.5/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.5/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.5/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.164925 mns-scheduler-1.0.2.5/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.165923 mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7332 2024-04-18 09:35:36.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.166920 mns-scheduler-1.0.2.5/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.167917 mns-scheduler-1.0.2.5/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.167917 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.168914 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.169912 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.170909 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.171907 mns-scheduler-1.0.2.5/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.5/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.172904 mns-scheduler-1.0.2.5/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.5/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.176893 mns-scheduler-1.0.2.5/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.2.5/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.177891 mns-scheduler-1.0.2.5/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.5/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13768 2024-04-16 14:08:50.000000 mns-scheduler-1.0.2.5/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:35:39.178888 mns-scheduler-1.0.2.5/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-18 09:35:39.000000 mns-scheduler-1.0.2.5/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3014 2024-04-18 09:35:39.000000 mns-scheduler-1.0.2.5/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:35:39.000000 mns-scheduler-1.0.2.5/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 09:35:39.000000 mns-scheduler-1.0.2.5/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 09:35:39.179885 mns-scheduler-1.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-18 09:35:36.000000 mns-scheduler-1.0.2.5/setup.py
```

### Comparing `mns-scheduler-1.0.2.4/README.md` & `mns-scheduler-1.0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.2.5/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.2.5/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.2.5/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.2.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,20 +43,24 @@
 
 
 def sync_k_line_info(str_day, symbol_list):
     result_k_line_list_df = None
     if symbol_list is not None:
         for symbol in symbol_list:
             try:
-                k_line_result = k_line_info_clean_impl.calculate_k_line_info(str_day, symbol)
-                save_k_line_data(symbol, str_day, k_line_result)
-                if result_k_line_list_df is None:
-                    result_k_line_list_df = result
-                else:
-                    result_k_line_list_df = pd.concat([result_k_line_list_df, k_line_result])
+                query = {'symbol': symbol}
+                company_info_df = mongodb_util.find_query_data('company_info', query)
+                if data_frame_util.is_not_empty(company_info_df):
+                    diff_days = list(company_info_df['diff_days'])[0]
+                    k_line_result = k_line_info_clean_impl.calculate_k_line_info(str_day, symbol, diff_days)
+                    save_k_line_data(symbol, str_day, k_line_result)
+                    if result_k_line_list_df is None:
+                        result_k_line_list_df = result
+                    else:
+                        result_k_line_list_df = pd.concat([result_k_line_list_df, k_line_result])
 
             except BaseException as e:
                 logger.error("k线同步错误:{},{},{}", str_day, symbol, e)
     else:
         result_k_line_list_df = multi_threaded_k_line_sync(str_day)
     logger.info("计算k线数据任务完成:{}", str_day)
     return result_k_line_list_df
```

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.2.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.2.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.4/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.2.5/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

