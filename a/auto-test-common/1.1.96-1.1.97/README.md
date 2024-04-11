# Comparing `tmp/auto-test-common-1.1.96.tar.gz` & `tmp/auto-test-common-1.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.96.tar", last modified: Wed Apr 10 07:09:20 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.97.tar", last modified: Thu Apr 11 02:08:43 2024, max compression
```

## Comparing `auto-test-common-1.1.96.tar` & `auto-test-common-1.1.97.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.945487 auto-test-common-1.1.96/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 07:09:20.945662 auto-test-common-1.1.96/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.895449 auto-test-common-1.1.96/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.895833 auto-test-common-1.1.96/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.96/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.898300 auto-test-common-1.1.96/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.96/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.96/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.96/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.96/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.901211 auto-test-common-1.1.96/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.96/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.96/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.96/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.902909 auto-test-common-1.1.96/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.96/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.907625 auto-test-common-1.1.96/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.96/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    24716 2024-04-10 05:26:16.000000 auto-test-common-1.1.96/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    11152 2024-04-10 05:26:16.000000 auto-test-common-1.1.96/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.96/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.914393 auto-test-common-1.1.96/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.96/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.96/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.96/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.916351 auto-test-common-1.1.96/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.96/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.96/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.96/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.924868 auto-test-common-1.1.96/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.96/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.96/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.96/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.96/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.96/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.96/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.926271 auto-test-common-1.1.96/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.932793 auto-test-common-1.1.96/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.96/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.96/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.96/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.96/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.96/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.96/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.943947 auto-test-common-1.1.96/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.96/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.96/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.96/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.96/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.96/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.96/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12914 2024-04-10 05:37:08.000000 auto-test-common-1.1.96/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.96/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.96/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.96/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.96/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.96/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.96/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-10 07:09:20.946695 auto-test-common-1.1.96/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.96/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.197059 auto-test-common-1.1.97/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:08:43.197314 auto-test-common-1.1.97/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.152896 auto-test-common-1.1.97/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.153263 auto-test-common-1.1.97/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.97/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.156703 auto-test-common-1.1.97/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.97/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.97/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.97/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.97/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.160139 auto-test-common-1.1.97/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.97/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.97/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.97/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.161391 auto-test-common-1.1.97/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.97/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.163805 auto-test-common-1.1.97/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.97/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25465 2024-04-11 02:07:25.000000 auto-test-common-1.1.97/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    11208 2024-04-11 02:07:25.000000 auto-test-common-1.1.97/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.97/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.169469 auto-test-common-1.1.97/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.97/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.97/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.97/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.171572 auto-test-common-1.1.97/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.97/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.97/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.97/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.177582 auto-test-common-1.1.97/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.97/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.97/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.97/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.97/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.97/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.97/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.178565 auto-test-common-1.1.97/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.182523 auto-test-common-1.1.97/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.97/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.97/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.97/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.97/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.97/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.97/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.195823 auto-test-common-1.1.97/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.97/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.97/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.97/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.97/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.97/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.97/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.97/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.97/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.97/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.97/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.97/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.97/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.97/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 02:08:43.198888 auto-test-common-1.1.97/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.97/setup.py
```

### Comparing `auto-test-common-1.1.96/PKG-INFO` & `auto-test-common-1.1.97/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.96
+Version: 1.1.97
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.96/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.97/auto_test_common.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.96
+Version: 1.1.97
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.96/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.97/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.97/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/autotest/base_requests.py` & `auto-test-common-1.1.97/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/autotest/handle_allure.py` & `auto-test-common-1.1.97/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/autotest/handle_assert.py` & `auto-test-common-1.1.97/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/common/api_driver.py` & `auto-test-common-1.1.97/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/common/constant.py` & `auto-test-common-1.1.97/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/common/test.py` & `auto-test-common-1.1.97/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/config/config.py` & `auto-test-common-1.1.97/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/data/data_process.py` & `auto-test-common-1.1.97/common/data/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
     @classmethod
     def handle_data(cls, variable: str, jsonformat:bool=True, _replace:int=0) -> dict:
         """请求数据处理
         :param variable: 请求数据，传入的是可转换字典/json的字符串,其中可以包含变量表达式
         return 处理之后的json/dict类型的字典数据
         """
-        if variable == '':
+        if variable == '' or variable is None:
             return
         if isinstance(variable, str) and variable.find(".json",len(variable)-5) != -1:
             _path = path.join(TEST_DATA_PATH, variable, )
             with open(_path, "r") as json_file:
                 variable = json.load(json_file)
         data = req_expr(content=variable, data=cls.response_dict, _replace=_replace)
         if jsonformat:
@@ -381,51 +381,56 @@
     @classmethod
     def check_test_data(self, testdatas:list):
         _testDatas = []
         casename = "00000"
         caseno = "00000"
         try:
             for testdata in testdatas:
+                casename = "00000"
+                caseno = "00000"
                 if type(testdata) == dict:
-                    if Constant.CASE_TITLE in testdata:
+                    if Constant.CASE_TITLE in testdata and DataProcess.isNotNull(testdata[Constant.CASE_TITLE]):
                         temp = str(testdata[Constant.CASE_TITLE])
                         casename = format_caseName(temp)
-                    if Constant.CASE_NO in testdata:
+                    if Constant.CASE_NO in testdata and DataProcess.isNotNull(testdata[Constant.CASE_NO]):
                         caseno = str(testdata[Constant.CASE_NO])
                     if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
                         if casename != "00000" or caseno != "00000":
                             _testDatas.append(testdata)
                         else:
-                            logger.info("用例脚本文件未关联用例名称或者用例编号【未关联用例名称或者编号】")
+                            logger.warning(f"用例脚本文件未关联用例名称或者用例编号【检查用例】用例信息:{str(testdata)}")
                     else:
-                        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-                            cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-                            _list = ServicePlatForm.getCaseRun(cycleId, caseno, casename)
-                            if 'status' in _list:
-                                if _list['status'] == Constant.STATUS_PRE or _list['status'] == Constant.STATUS_AUTOTEST:
-                                    ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST_PARA, "")
-                                    #_caseInfo = ServicePlatForm.getCaseInfoByNameOrID(caseno, casename)
-                                    # testdata[Constant.CASE_NO] = _caseInfo['key']
-                                    # testdata[Constant.CASE_TITLE] = _caseInfo['summary']
-                                    testdata[Constant.CASE_NO] = caseno
-                                    testdata[Constant.CASE_TITLE] = casename
-                                    _testDatas.append(testdata)
-                                    print_debug(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 添加到执行队列')
+                        if casename != "00000" or caseno != "00000":
+                            if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
+                                cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
+                                _list = ServicePlatForm.getCaseRun(cycleId, caseno, casename)
+                                if 'status' in _list:
+                                    if _list['status'] == Constant.STATUS_PRE or _list['status'] == Constant.STATUS_AUTOTEST:
+                                        ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST_PARA, "")
+                                        #_caseInfo = ServicePlatForm.getCaseInfoByNameOrID(caseno, casename)
+                                        # testdata[Constant.CASE_NO] = _caseInfo['key']
+                                        # testdata[Constant.CASE_TITLE] = _caseInfo['summary']
+                                        testdata[Constant.CASE_NO] = caseno
+                                        testdata[Constant.CASE_TITLE] = casename
+                                        _testDatas.append(testdata)
+                                        print_debug(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 添加到执行队列')
+                                    else:
+                                        logger.info(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 无需添加执行队列')
                                 else:
-                                    logger.info(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 无需添加执行队列')
+                                    logger.info(f"获取周期中的测试用例信息异常【{cycleId},{caseno},{casename}】:{_list}")
                             else:
-                                logger.info(f"获取周期中的测试用例信息异常【{cycleId},{caseno},{casename}】:{_list}")
-                        else:
-                            if Constant.CASE_STATUS in testdata:
-                                if testdata[Constant.CASE_STATUS].strip() != '否':
+                                if Constant.CASE_STATUS in testdata:
+                                    if testdata[Constant.CASE_STATUS].strip() != '否':
+                                        _testDatas.append(testdata)
+                                else:
                                     _testDatas.append(testdata)
-                            else:
-                                _testDatas.append(testdata)
+                        else:
+                            logger.warning(f"用例脚本文件未关联用例名称或者用例编号【检查用例】用例信息:{str(testdata)}")
                 else:
-                    logger.info(f"不复合单条测试数据标准:{testdatas}")
+                    logger.warning(f"不复合单条测试数据标准:{testdatas}")
             print_debug("处理前参数化测试数据:" + str(_testDatas))
             return _testDatas
         except Exception as e:
             logger.info(f'检查数据中用例属性错误信息测试数据:{testdatas} 用例名称：{casename} 用例编号：{caseno} 异常信息:'+repr(e))
         return _testDatas
 
     @classmethod
@@ -496,21 +501,25 @@
     def list_dict_duplicate_removal_byKey(self, list_dict, key):
         """列表中嵌套字典，按字典中得某个键去重"""
         if list_dict is not None and list_dict.__len__() > 0:
             a = []
             a.append(list_dict[0])
             for dict in list_dict:
                 k = 0
-                for item in a:
-                    if key in dict and dict[key] != item[key]:
-                        k = k + 1
-                    else:
-                        break
-                    if k == len(a):
-                        a.append(dict)
+                if key not in dict or DataProcess.isNotNull(dict[key])==False:
+                    k = k + 1
+                    a.append(dict)
+                else:
+                    for item in a:
+                        if key in dict and dict[key] != item[key]:
+                            k = k + 1
+                        else:
+                            break
+                        if k == len(a):
+                            a.append(dict)
             return a
         else:
             return list_dict
 
     @classmethod
     def list_script_removal_byKey(self, list_dict, key):
         """列表中嵌套字典，按字典中得某个键去重"""
```

### Comparing `auto-test-common-1.1.96/common/data/handle_common.py` & `auto-test-common-1.1.97/common/data/handle_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,18 @@
 
 def convert_json_bank(content, data):
     _str = req_expr(content=content, data=data, _no_content=0)
     _str = _str.replace(Constant.DATA_NO_CONTENT + ",", '"' + Constant.DATA_NO_CONTENT + '",')
     #_json = json.loads(_str)
     from common.data.data_process import DataProcess
     _json = DataProcess.handle_data(_str)
-    return json.dumps(convert_json_dict(_json), ensure_ascii=False)
+    if _json is None:
+        return None
+    else:
+        return json.dumps(convert_json_dict(_json), ensure_ascii=False)
 
 
 if __name__ == '__main__':
     content="{'Service': {'Header': {'UsernameToken': {'Username': 'CA129', 'Password': '${Password}'}}, 'Body': {'systemcode': 'CA129', 'filtercondition': '', 'SOAHttpOption': 'GET', 'EsbJsonBody': {}}}}"
     data= {'Password':'f1021c74-88f6-4b29-811d-ac873bc55115'}
     from common.data.data_process import DataProcess
     data =convert_json_bank(content, data)
```

### Comparing `auto-test-common-1.1.96/common/data/template_data.py` & `auto-test-common-1.1.97/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_db.py` & `auto-test-common-1.1.97/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_db_batch.py` & `auto-test-common-1.1.97/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_mongo.py` & `auto-test-common-1.1.97/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_mysqldb.py` & `auto-test-common-1.1.97/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_oracle.py` & `auto-test-common-1.1.97/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/db/handle_sqlserver.py` & `auto-test-common-1.1.97/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/driver/ui_page.py` & `auto-test-common-1.1.97/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/ReadFile.py` & `auto-test-common-1.1.97/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/handle_excel.py` & `auto-test-common-1.1.97/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/handle_file.py` & `auto-test-common-1.1.97/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/handle_reques.py` & `auto-test-common-1.1.97/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/handle_system.py` & `auto-test-common-1.1.97/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/file/handle_yaml.py` & `auto-test-common-1.1.97/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/mq/handle_rabbit.py` & `auto-test-common-1.1.97/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plat/ATF_platform.py` & `auto-test-common-1.1.97/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plat/jenkin_platform.py` & `auto-test-common-1.1.97/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plat/jira_platform.py` & `auto-test-common-1.1.97/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plat/mysql_platform.py` & `auto-test-common-1.1.97/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plat/service_platform.py` & `auto-test-common-1.1.97/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/allure_plugin.py` & `auto-test-common-1.1.97/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/assert_plugin.py` & `auto-test-common-1.1.97/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/atf_plugin.py` & `auto-test-common-1.1.97/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/data_bus.py` & `auto-test-common-1.1.97/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/data_plugin.py` & `auto-test-common-1.1.97/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/file_plugin.py` & `auto-test-common-1.1.97/common/plugin/file_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,22 +65,25 @@
             excel_sheet = file_name_temp + "_" + sheet
             if DataProcess.isNotNull(get_system_key(Constant.SYNC_EXCEL_SHEET)):
                 if get_system_key(Constant.SYNC_EXCEL_SHEET).find(excel_sheet.strip()+";") < 0:
                     sync_excel_sheet = get_system_key(Constant.SYNC_EXCEL_SHEET) + ";" + excel_sheet.strip()+";"
                     logger.info(f"文件路径:{file_name_temp} Sheet:{sheet} 脚本用例文件开始同步")
                     set_system_key(Constant.SYNC_EXCEL_SHEET, sync_excel_sheet, True)
                     _list = excel_to_list(file_name_temp, sheet, _index)
+                    _list = DataProcess.check_test_data(_list)
                 else:
                     logger.info(f"文件路径:{file_name_temp} Sheet:{sheet} 脚本用例文已经被处理")
             else:
                 set_system_key(Constant.SYNC_EXCEL_SHEET,excel_sheet.strip()+";")
                 logger.info(f"文件路径:{file_name_temp} Sheet:{sheet} 脚本用例文件开始同步")
                 _list = excel_to_list(file_name_temp, sheet, _index)
+                _list = DataProcess.check_test_data(_list)
         else:
             _list = excel_to_list(file_name_temp, sheet, _index, _filter,  _replace, _checkData=True)
+            _list = DataProcess.check_test_data(_list)
             _list = DataProcess.list_dict_duplicate_removal_byKey(_list, Constant.CASE_TITLE)
             _list = DataProcess.list_dict_duplicate_removal_byKey(_list, Constant.CASE_NO)
             for _temp in _list:
                 for key in _temp.keys():
                     _fileName, _sheet, _filter = self.handle_excel_data(_temp[key],file_name,sheet)
                     if DataProcess.isNotNull(_fileName):
                         _subData = excel_to_list(path.join(file_path, _fileName), _sheet, _index, _filter, _replace, _checkData=False)
```

### Comparing `auto-test-common-1.1.96/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.97/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.97/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.97/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/template_plugin.py` & `auto-test-common-1.1.97/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.97/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.96/setup.py` & `auto-test-common-1.1.97/setup.py`

 * *Files identical despite different names*

