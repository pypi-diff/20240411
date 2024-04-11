# Comparing `tmp/auto-test-common-1.1.95.tar.gz` & `tmp/auto-test-common-1.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.95.tar", last modified: Wed Apr 10 05:37:15 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.96.tar", last modified: Wed Apr 10 07:09:20 2024, max compression
```

## Comparing `auto-test-common-1.1.95.tar` & `auto-test-common-1.1.96.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.451922 auto-test-common-1.1.95/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 05:37:15.452152 auto-test-common-1.1.95/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.408733 auto-test-common-1.1.95/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-10 05:37:15.000000 auto-test-common-1.1.95/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.409041 auto-test-common-1.1.95/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.95/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.410372 auto-test-common-1.1.95/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.95/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11697 2024-04-10 05:37:08.000000 auto-test-common-1.1.95/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.95/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.95/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.412708 auto-test-common-1.1.95/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.95/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.95/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.95/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.413578 auto-test-common-1.1.95/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.95/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.415927 auto-test-common-1.1.95/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.95/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    24716 2024-04-10 05:26:16.000000 auto-test-common-1.1.95/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    11152 2024-04-10 05:26:16.000000 auto-test-common-1.1.95/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.95/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.421605 auto-test-common-1.1.95/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.95/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.95/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.95/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.423965 auto-test-common-1.1.95/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.95/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.95/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.95/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.431038 auto-test-common-1.1.95/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.95/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.95/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.95/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.95/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.95/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.95/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.432009 auto-test-common-1.1.95/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.95/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.95/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.436957 auto-test-common-1.1.95/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.95/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.95/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.95/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.95/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.95/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.95/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 05:37:15.450230 auto-test-common-1.1.95/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.95/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.95/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.95/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.95/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.95/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.95/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12914 2024-04-10 05:37:08.000000 auto-test-common-1.1.95/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.95/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.95/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.95/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.95/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.95/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.95/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-10 05:37:15.453516 auto-test-common-1.1.95/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.95/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.945487 auto-test-common-1.1.96/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 07:09:20.945662 auto-test-common-1.1.96/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.895449 auto-test-common-1.1.96/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-10 07:09:20.000000 auto-test-common-1.1.96/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.895833 auto-test-common-1.1.96/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.96/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.898300 auto-test-common-1.1.96/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.96/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.96/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.96/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.96/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.901211 auto-test-common-1.1.96/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.96/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.96/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.96/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.902909 auto-test-common-1.1.96/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.96/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.907625 auto-test-common-1.1.96/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.96/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    24716 2024-04-10 05:26:16.000000 auto-test-common-1.1.96/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    11152 2024-04-10 05:26:16.000000 auto-test-common-1.1.96/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.96/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.914393 auto-test-common-1.1.96/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.96/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.96/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.96/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.916351 auto-test-common-1.1.96/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.96/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.96/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.96/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.924868 auto-test-common-1.1.96/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.96/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.96/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.96/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.96/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.96/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.96/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.926271 auto-test-common-1.1.96/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.96/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.96/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.932793 auto-test-common-1.1.96/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.96/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.96/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.96/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.96/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.96/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.96/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-10 07:09:20.943947 auto-test-common-1.1.96/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.96/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.96/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.96/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.96/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.96/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.96/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12914 2024-04-10 05:37:08.000000 auto-test-common-1.1.96/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.96/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.96/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.96/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.96/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.96/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.96/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-10 07:09:20.946695 auto-test-common-1.1.96/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.96/setup.py
```

### Comparing `auto-test-common-1.1.95/PKG-INFO` & `auto-test-common-1.1.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.95
+Version: 1.1.96
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.95/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.96/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.95
+Version: 1.1.96
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.95/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.96/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.96/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/autotest/base_requests.py` & `auto-test-common-1.1.96/common/autotest/base_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
                             content = FilePlugin.load_data(content['file'])
                     data = convert_json_bank(content, data)
                 data = DataProcess.handle_data(variable=data, _replace=_replace)
             else:
                 if 'body' in schemal_data:
                     schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                     content = schemal_body['body']
+                    if isinstance(content,dict):
+                        if 'file' in content:
+                            from common.plugin.file_plugin import FilePlugin
+                            content = FilePlugin.load_data(content['file'])
                     data = req_expr(content=content, data=data, _no_content=0)
             if 'format' in schemal_data:
                 if schemal_data['format'] == 'text':
                     data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
                 elif schemal_data['format'] == 'json':
                     data = DataProcess.handle_data(variable=data, _replace=_replace)
                 elif schemal_data['format'] == 'None':
@@ -142,22 +146,30 @@
         if 'assert' in schemal_data:
             if isinstance(temp,dict):
                 schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                 assertData = schemal_body['assert']
                 _assert = convert_json_bank(assertData, temp)
             else:
                 _assert = schemal_data['assert']
-            assert_response(res, _assert)
+            if str(_assert).find('*ResCode') >= 0:
+                assert_response(res, _assert)
+            else:
+                if DataProcess.isNotNull(get_system_key(Constant.RESPONSE_CODE)):
+                    ex_status_code = get_system_key(Constant.RESPONSE_CODE)
+                    allure_step(f'状态码检查', f'实际状态码: {res.status_code}小于{ex_status_code}')
+                    assert res.status_code <= int(ex_status_code)
+                assert_response(res, _assert)
+        else:
+            if DataProcess.isNotNull(get_system_key(Constant.RESPONSE_CODE)):
+                ex_status_code = get_system_key(Constant.RESPONSE_CODE)
+                allure_step(f'状态码检查', f'实际状态码: {res.status_code}小于{ex_status_code}')
+                assert res.status_code <= int(ex_status_code)
         if 'data' in schemal_data:
             databus = schemal_data['data']
             DataProcess.get_response_jpath(res, databus, schemal_key)
-        if DataProcess.isNotNull(get_system_key(Constant.RESPONSE_CODE)):
-            ex_status_code = get_system_key(Constant.RESPONSE_CODE)
-            allure_step(f'状态码检查', f'实际状态码: {res.status_code}小于{ex_status_code}')
-            assert res.status_code <= int(ex_status_code)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, schemal_data['method'], header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         return res
```

### Comparing `auto-test-common-1.1.95/common/autotest/handle_allure.py` & `auto-test-common-1.1.96/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/autotest/handle_assert.py` & `auto-test-common-1.1.96/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/common/api_driver.py` & `auto-test-common-1.1.96/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/common/constant.py` & `auto-test-common-1.1.96/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/common/test.py` & `auto-test-common-1.1.96/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/config/config.py` & `auto-test-common-1.1.96/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/data/data_process.py` & `auto-test-common-1.1.96/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/data/handle_common.py` & `auto-test-common-1.1.96/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/data/template_data.py` & `auto-test-common-1.1.96/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_db.py` & `auto-test-common-1.1.96/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_db_batch.py` & `auto-test-common-1.1.96/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_mongo.py` & `auto-test-common-1.1.96/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_mysqldb.py` & `auto-test-common-1.1.96/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_oracle.py` & `auto-test-common-1.1.96/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/db/handle_sqlserver.py` & `auto-test-common-1.1.96/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/driver/ui_page.py` & `auto-test-common-1.1.96/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/ReadFile.py` & `auto-test-common-1.1.96/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/handle_excel.py` & `auto-test-common-1.1.96/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/handle_file.py` & `auto-test-common-1.1.96/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/handle_reques.py` & `auto-test-common-1.1.96/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/handle_system.py` & `auto-test-common-1.1.96/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/file/handle_yaml.py` & `auto-test-common-1.1.96/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/mq/handle_rabbit.py` & `auto-test-common-1.1.96/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plat/ATF_platform.py` & `auto-test-common-1.1.96/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plat/jenkin_platform.py` & `auto-test-common-1.1.96/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plat/jira_platform.py` & `auto-test-common-1.1.96/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plat/mysql_platform.py` & `auto-test-common-1.1.96/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plat/service_platform.py` & `auto-test-common-1.1.96/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/allure_plugin.py` & `auto-test-common-1.1.96/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/assert_plugin.py` & `auto-test-common-1.1.96/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/atf_plugin.py` & `auto-test-common-1.1.96/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/data_bus.py` & `auto-test-common-1.1.96/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/data_plugin.py` & `auto-test-common-1.1.96/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/file_plugin.py` & `auto-test-common-1.1.96/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.96/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.96/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.96/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/template_plugin.py` & `auto-test-common-1.1.96/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.96/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.95/setup.py` & `auto-test-common-1.1.96/setup.py`

 * *Files identical despite different names*

