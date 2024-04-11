# Comparing `tmp/mns-scheduler-1.0.1.9.tar.gz` & `tmp/mns-scheduler-1.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.1.9.tar", last modified: Tue Apr  2 15:21:15 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.2.0.tar", last modified: Thu Apr 11 14:05:04 2024, max compression
```

## Comparing `mns-scheduler-1.0.1.9.tar` & `mns-scheduler-1.0.2.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.371490 mns-scheduler-1.0.1.9/
--rw-rw-rw-   0        0        0       62 2024-04-02 15:21:15.371490 mns-scheduler-1.0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.342568 mns-scheduler-1.0.1.9/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.345560 mns-scheduler-1.0.1.9/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.1.9/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.346557 mns-scheduler-1.0.1.9/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20685 2024-04-02 12:30:14.000000 mns-scheduler-1.0.1.9/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.347555 mns-scheduler-1.0.1.9/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.348552 mns-scheduler-1.0.1.9/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.350546 mns-scheduler-1.0.1.9/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.350546 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.351544 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.352541 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10290 2024-03-21 16:17:01.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.353538 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8263 2024-03-22 07:44:40.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.354536 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     4996 2024-03-21 16:54:33.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.355533 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.357528 mns-scheduler-1.0.1.9/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.1.9/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.357528 mns-scheduler-1.0.1.9/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.358525 mns-scheduler-1.0.1.9/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.1.9/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.1.9/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.359522 mns-scheduler-1.0.1.9/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.360520 mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.361517 mns-scheduler-1.0.1.9/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.1.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.361517 mns-scheduler-1.0.1.9/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.361517 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.362514 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.363512 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.364509 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.365507 mns-scheduler-1.0.1.9/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.1.9/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.366504 mns-scheduler-1.0.1.9/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.1.9/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.369496 mns-scheduler-1.0.1.9/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7502 2024-04-02 12:30:14.000000 mns-scheduler-1.0.1.9/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.370493 mns-scheduler-1.0.1.9/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.9/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.1.9/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.1.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:21:15.370493 mns-scheduler-1.0.1.9/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-02 15:21:15.000000 mns-scheduler-1.0.1.9/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2948 2024-04-02 15:21:15.000000 mns-scheduler-1.0.1.9/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:21:15.000000 mns-scheduler-1.0.1.9/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-02 15:21:15.000000 mns-scheduler-1.0.1.9/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 15:21:15.371490 mns-scheduler-1.0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-02 15:20:14.000000 mns-scheduler-1.0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.823802 mns-scheduler-1.0.2.0/
+-rw-rw-rw-   0        0        0       62 2024-04-11 14:05:04.822805 mns-scheduler-1.0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.789894 mns-scheduler-1.0.2.0/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.791888 mns-scheduler-1.0.2.0/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.0/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.793883 mns-scheduler-1.0.2.0/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20271 2024-04-11 13:59:16.000000 mns-scheduler-1.0.2.0/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.793883 mns-scheduler-1.0.2.0/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.794880 mns-scheduler-1.0.2.0/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.796874 mns-scheduler-1.0.2.0/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.797871 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.798869 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.799866 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10180 2024-04-11 14:04:04.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.800864 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8263 2024-03-22 07:44:40.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.802858 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     4996 2024-03-21 16:54:33.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.803856 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.804853 mns-scheduler-1.0.2.0/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.0/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.805850 mns-scheduler-1.0.2.0/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.806848 mns-scheduler-1.0.2.0/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.0/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.0/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.807845 mns-scheduler-1.0.2.0/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.808843 mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.809840 mns-scheduler-1.0.2.0/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.810837 mns-scheduler-1.0.2.0/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.810837 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.811835 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.812832 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.813829 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.815823 mns-scheduler-1.0.2.0/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.0/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.816821 mns-scheduler-1.0.2.0/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.0/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.819813 mns-scheduler-1.0.2.0/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7502 2024-04-02 12:30:14.000000 mns-scheduler-1.0.2.0/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.821807 mns-scheduler-1.0.2.0/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.0/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.0/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:05:04.822805 mns-scheduler-1.0.2.0/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-11 14:05:04.000000 mns-scheduler-1.0.2.0/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2024-04-11 14:05:04.000000 mns-scheduler-1.0.2.0/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:05:04.000000 mns-scheduler-1.0.2.0/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 14:05:04.000000 mns-scheduler-1.0.2.0/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:05:04.823802 mns-scheduler-1.0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-11 14:04:49.000000 mns-scheduler-1.0.2.0/setup.py
```

### Comparing `mns-scheduler-1.0.1.9/README.md` & `mns-scheduler-1.0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.2.0/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         mongodb_util.save_mongo(company_info, 'company_info')
     except BaseException as e:
         logger.error("出现异常:{}", symbol)
 
     return company_info
 
 
-def sync_company_base_info(symbol):
+def sync_company_base_info(symbol_list):
     global result
     result = []
     create_index()
     east_money_stock_info = get_east_money_stock_info()
     east_money_stock_info = east_money_stock_info.loc[~(
         east_money_stock_info['symbol'].isin(company_constant_data_api.de_listed_stock_list))]
     east_money_stock_info = common_service_fun_api.exclude_ts_symbol(east_money_stock_info)
@@ -218,16 +218,16 @@
 
     # 将日期数值转换为日期时间格式
     east_money_stock_info['list_date_01'] = pd.to_datetime(east_money_stock_info['list_date'], format='%Y%m%d')
 
     # 开票啦实时数据
     kpl_real_time_quotes = kpl_real_time_quotes_api.get_kpl_real_time_quotes()
 
-    if symbol is not None:
-        east_money_stock_info = east_money_stock_info.loc[east_money_stock_info['symbol'] == symbol]
+    if symbol_list is not None:
+        east_money_stock_info = east_money_stock_info.loc[east_money_stock_info['symbol'].isin(symbol_list)]
     count = east_money_stock_info.shape[0]
     page_number = round(count / MAX_PAGE_NUMBER, 0) + 1
     page_number = int(page_number)
     threads = []
     # 创建多个线程来获取数据
     for page in range(page_number):  # 0到100页
         end_count = (page + 1) * MAX_PAGE_NUMBER
@@ -363,36 +363,25 @@
             kpl_best_choose_index_detail['first_plate_name'] = kpl_best_choose_index_detail[
                 'first_plate_name'].str.replace(' ', '')
 
             company_info_type.loc[:, 'kpl_plate_list_info'] = kpl_best_choose_index_detail.to_string(index=False)
     return company_info_type
 
 
-# 开盘公司信息更新
-def company_info_update():
-    east_money_stock_info = get_east_money_stock_info()
-    for company_one in east_money_stock_info.itertuples():
-        try:
-            sync_company_base_info(company_one.symbol)
-            fix_company_industry(company_one.symbol)
-            company_common_service_api.company_info_industry_cache_clear
-        except BaseException as e:
-            logger.error("出现异常:{}", e)
-
-
 def new_company_info_update():
     east_money_stock_info = get_east_money_stock_info()
     new_stock = common_service_fun_api.get_new_stock(east_money_stock_info)
     for company_one in new_stock.itertuples():
         try:
-            sync_company_base_info(company_one.symbol)
+            sync_company_base_info([company_one.symbol])
             fix_company_industry(company_one.symbol)
-            company_common_service_api.company_info_industry_cache_clear
+
         except BaseException as e:
             logger.error("出现异常:{}", e)
+    company_common_service_api.company_info_industry_cache_clear
 
 
 def save_sw_data(company_info_type):
     first_sw_info = company_info_type[[
         'first_sw_industry',
         'first_industry_code'
     ]].copy()
@@ -474,10 +463,11 @@
     # company_info_type = ths_stock_api.get_company_info_detail('836699')
     # sync_company_base_info()
     # fix_company_industry()
     # calculate_circu_ratio("601069")
     # sync_company_base_info()
     # 300293
     # sync_company_base_info(None)
+    new_company_info_update()
     sync_company_base_info(None)
     fix_company_industry(None)
     # group_by_industry()
```

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 mongodb_util = MongodbUtil('27017')
 import mns_common.api.msg.push_msg_api as push_msg_api
+import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
 
 max_concept_code = 886110
 
 order_fields = [
     "index",
     "symbol",
     "name",
@@ -130,29 +131,27 @@
         new_concept_symbol_df = new_concept_symbol_df.loc[~(
             new_concept_symbol_df['symbol'].isin(exist_concept_detail_symbol_list))]
         if new_concept_symbol_df.shape[0] > 0:
             mongodb_util.save_mongo(new_concept_symbol_df, 'ths_stock_concept_detail')
             # 保存到当日新增概念列表
             new_concept_symbol_df['concept_type'] = 'ths'
             mongodb_util.save_mongo(new_concept_symbol_df, 'today_new_concept_list')
-    update_company_info(new_concept_symbol_df, concept_code, concept_name, str_day)
+    update_company_info(new_concept_symbol_df)
     # 公司缓存信息清除
     company_common_service_api.company_info_industry_cache_clear()
 
 
 # 更新公司表信息 todo 清空cache 公司表中  common_service_fun_api.py  get_company_info_industry
-def update_company_info(new_concept_symbol_df, concept_code, concept_name, str_day):
+def update_company_info(new_concept_symbol_df):
     if new_concept_symbol_df.shape[0] > 0:
         symbol_list = list(new_concept_symbol_df['symbol'])
-        query = {'symbol': {'$in': symbol_list}}
-        new_values = {"$set": {"ths_concept_name": concept_name,
-                               "ths_concept_code": concept_code,
-                               "ths_concept_sync_day": str_day,
-                               }}
-        mongodb_util.update_many(query, new_values, 'company_info')
+        company_info_sync_api.sync_company_base_info(symbol_list)
+        company_info_sync_api.fix_company_industry(None)
+        # 公司缓存信息清除
+        company_common_service_api.company_info_industry_cache_clear()
 
 
 def update_null_name():
     query = {"_id": {'$gte': 886025}}
     ths_concept_list = mongodb_util.find_query_data('ths_concept_list', query)
     ths_concept_list = ths_concept_list.sort_values(by=['_id'], ascending=False)
```

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.2.0/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.2.0/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.2.0/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.2.0/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.2.0/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.9/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.2.0/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

