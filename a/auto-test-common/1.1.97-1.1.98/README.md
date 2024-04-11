# Comparing `tmp/auto-test-common-1.1.97.tar.gz` & `tmp/auto-test-common-1.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.97.tar", last modified: Thu Apr 11 02:08:43 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.98.tar", last modified: Thu Apr 11 02:38:40 2024, max compression
```

## Comparing `auto-test-common-1.1.97.tar` & `auto-test-common-1.1.98.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.197059 auto-test-common-1.1.97/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:08:43.197314 auto-test-common-1.1.97/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.152896 auto-test-common-1.1.97/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 02:08:42.000000 auto-test-common-1.1.97/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.153263 auto-test-common-1.1.97/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.97/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.156703 auto-test-common-1.1.97/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.97/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.97/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.97/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.97/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.160139 auto-test-common-1.1.97/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.97/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.97/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.97/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.161391 auto-test-common-1.1.97/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.97/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.163805 auto-test-common-1.1.97/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.97/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25465 2024-04-11 02:07:25.000000 auto-test-common-1.1.97/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    11208 2024-04-11 02:07:25.000000 auto-test-common-1.1.97/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.97/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.169469 auto-test-common-1.1.97/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.97/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.97/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.97/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.171572 auto-test-common-1.1.97/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.97/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.97/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.97/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.177582 auto-test-common-1.1.97/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.97/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.97/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.97/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.97/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.97/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.97/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.178565 auto-test-common-1.1.97/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.97/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.97/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.182523 auto-test-common-1.1.97/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.97/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.97/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.97/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.97/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.97/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.97/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:08:43.195823 auto-test-common-1.1.97/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.97/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.97/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.97/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.97/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.97/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.97/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.97/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.97/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.97/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.97/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.97/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.97/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.97/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 02:08:43.198888 auto-test-common-1.1.97/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.97/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.610955 auto-test-common-1.1.98/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:38:40.611098 auto-test-common-1.1.98/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.560502 auto-test-common-1.1.98/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.560914 auto-test-common-1.1.98/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.98/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.563144 auto-test-common-1.1.98/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.98/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.98/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.98/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.98/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.566218 auto-test-common-1.1.98/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.98/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.98/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.98/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.567148 auto-test-common-1.1.98/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.98/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.569349 auto-test-common-1.1.98/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.98/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25566 2024-04-11 02:38:06.000000 auto-test-common-1.1.98/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-1.1.98/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.98/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.574960 auto-test-common-1.1.98/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.98/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.98/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.98/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.576843 auto-test-common-1.1.98/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.98/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.98/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.98/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.585989 auto-test-common-1.1.98/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.98/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.98/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.98/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.98/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.98/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.98/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.587904 auto-test-common-1.1.98/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.598056 auto-test-common-1.1.98/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.98/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.98/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.98/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.98/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.98/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.98/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.609777 auto-test-common-1.1.98/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.98/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.98/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.98/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.98/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.98/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.98/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.98/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.98/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.98/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.98/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.98/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.98/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.98/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 02:38:40.611851 auto-test-common-1.1.98/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.98/setup.py
```

### Comparing `auto-test-common-1.1.97/PKG-INFO` & `auto-test-common-1.1.98/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.97
+Version: 1.1.98
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.97/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.98/auto_test_common.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.97
+Version: 1.1.98
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.97/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.98/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.98/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/autotest/base_requests.py` & `auto-test-common-1.1.98/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/autotest/handle_allure.py` & `auto-test-common-1.1.98/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/autotest/handle_assert.py` & `auto-test-common-1.1.98/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/common/api_driver.py` & `auto-test-common-1.1.98/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/common/constant.py` & `auto-test-common-1.1.98/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/common/test.py` & `auto-test-common-1.1.98/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/config/config.py` & `auto-test-common-1.1.98/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/data/data_process.py` & `auto-test-common-1.1.98/common/data/data_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,17 +572,19 @@
                 else:
                     actual = str(actual)
                 DataBus.set_key(_key,actual)
                 _value = DataBus.get_key(_key)
                 allure_step(f'接口返回【{v}】回填【{_key}】', f'回填数据:{_value}')
 
 if __name__ == '__main__':
-    _list=[{'script':'1111[2334]'},{'script':'1122//[2334]'},{'script':'1111[233334]'},{'script':'111/1111'},{'script':'1111'},{'script':'1111'}]
-    list = DataProcess.list_script_removal_byKey(_list,'script')
-    print(list)
+    # _list=[{'script':'1111[2334]'},{'script':'1122//[2334]'},{'script':'1111[233334]'},{'script':'111/1111'},{'script':'1111'},{'script':'1111'}]
+    # list = DataProcess.list_script_removal_byKey(_list,'script')
+    from common.plugin.data_bus import DataBus
+    DataBus.set_key('3333','')
+    print(DataBus.get_key('3333'))
```

### Comparing `auto-test-common-1.1.97/common/data/handle_common.py` & `auto-test-common-1.1.98/common/data/handle_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,28 +178,41 @@
     """
     把值设置到环境变量中
     :param str_key:
     :param str_value:
     :param _replace: 如果存在，是否替换原来的Key
     :return:
     """
-    if _replace:
-        if str_value is not None and isinstance(str_value, str):
-            os.environ[str_key.lower().strip()] = str_value.strip()
-        if str_value is not None and isinstance(str_value, dict):
-            os.environ[str_key.lower().strip()] = str(str_value)
-            os.environ[(str_key + Constant.DATA_TYPE).lower().strip()] = Constant.DATA_DIC
-    else:
-        _old = get_system_key(str_key)
-        if _old is None:
+    try:
+        if _replace:
             if str_value is not None and isinstance(str_value, str):
                 os.environ[str_key.lower().strip()] = str_value.strip()
-            if str_value is not None and isinstance(str_value, dict):
+            elif str_value is not None and isinstance(str_value, dict):
                 os.environ[str_key.lower().strip()] = str(str_value)
                 os.environ[(str_key + Constant.DATA_TYPE).lower().strip()] = Constant.DATA_DIC
+            elif str_value is not None and isinstance(str_value, list):
+                os.environ[str_key.lower().strip()] = str(str_value)
+                os.environ[(str_key + Constant.DATA_TYPE).lower().strip()] = Constant.DATA_LIST
+            elif str_value is not None:
+                os.environ[str_key.lower().strip()] = str(str_value)
+        else:
+            _old = get_system_key(str_key)
+            if _old is None:
+                if str_value is not None and isinstance(str_value, str):
+                    os.environ[str_key.lower().strip()] = str_value.strip()
+                elif str_value is not None and isinstance(str_value, dict):
+                    os.environ[str_key.lower().strip()] = str(str_value)
+                    os.environ[(str_key + Constant.DATA_TYPE).lower().strip()] = Constant.DATA_DIC
+                elif str_value is not None and isinstance(str_value, list):
+                    os.environ[str_key.lower().strip()] = str(str_value)
+                    os.environ[(str_key + Constant.DATA_TYPE).lower().strip()] = Constant.DATA_LIST
+                elif str_value is not None:
+                    os.environ[str_key.lower().strip()] = str(str_value)
+    except Exception as e:
+        logger.warning(f'保存DataBus中数据异常KEY:{str_key} Value:{str_value} 异常信息:' + repr(e))
 
 
 
 def print_databus_info(_key,_desc):
     _value = get_system_key(_key)
     if _value is not None:
         logger.info(f'{_desc}:{_value}')
```

### Comparing `auto-test-common-1.1.97/common/data/template_data.py` & `auto-test-common-1.1.98/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_db.py` & `auto-test-common-1.1.98/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_db_batch.py` & `auto-test-common-1.1.98/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_mongo.py` & `auto-test-common-1.1.98/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_mysqldb.py` & `auto-test-common-1.1.98/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_oracle.py` & `auto-test-common-1.1.98/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/db/handle_sqlserver.py` & `auto-test-common-1.1.98/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/driver/ui_page.py` & `auto-test-common-1.1.98/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/ReadFile.py` & `auto-test-common-1.1.98/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/handle_excel.py` & `auto-test-common-1.1.98/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/handle_file.py` & `auto-test-common-1.1.98/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/handle_reques.py` & `auto-test-common-1.1.98/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/handle_system.py` & `auto-test-common-1.1.98/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/file/handle_yaml.py` & `auto-test-common-1.1.98/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/mq/handle_rabbit.py` & `auto-test-common-1.1.98/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plat/ATF_platform.py` & `auto-test-common-1.1.98/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plat/jenkin_platform.py` & `auto-test-common-1.1.98/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plat/jira_platform.py` & `auto-test-common-1.1.98/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plat/mysql_platform.py` & `auto-test-common-1.1.98/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plat/service_platform.py` & `auto-test-common-1.1.98/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/allure_plugin.py` & `auto-test-common-1.1.98/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/assert_plugin.py` & `auto-test-common-1.1.98/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/atf_plugin.py` & `auto-test-common-1.1.98/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/data_bus.py` & `auto-test-common-1.1.98/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/data_plugin.py` & `auto-test-common-1.1.98/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/file_plugin.py` & `auto-test-common-1.1.98/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.98/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.98/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.98/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/template_plugin.py` & `auto-test-common-1.1.98/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.98/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.97/setup.py` & `auto-test-common-1.1.98/setup.py`

 * *Files identical despite different names*

