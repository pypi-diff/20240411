# Comparing `tmp/auto-test-common-1.1.98.tar.gz` & `tmp/auto-test-common-1.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.98.tar", last modified: Thu Apr 11 02:38:40 2024, max compression
+gzip compressed data, was "auto-test-common-1.1.99.tar", last modified: Thu Apr 11 08:55:14 2024, max compression
```

## Comparing `auto-test-common-1.1.98.tar` & `auto-test-common-1.1.99.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.610955 auto-test-common-1.1.98/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:38:40.611098 auto-test-common-1.1.98/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.560502 auto-test-common-1.1.98/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 02:38:40.000000 auto-test-common-1.1.98/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.560914 auto-test-common-1.1.98/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.98/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.563144 auto-test-common-1.1.98/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.98/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.98/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.98/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.98/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.566218 auto-test-common-1.1.98/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.98/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7777 2024-04-10 02:04:34.000000 auto-test-common-1.1.98/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.98/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.567148 auto-test-common-1.1.98/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.98/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.569349 auto-test-common-1.1.98/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.98/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25566 2024-04-11 02:38:06.000000 auto-test-common-1.1.98/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-1.1.98/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.98/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.574960 auto-test-common-1.1.98/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.98/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.98/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.98/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.576843 auto-test-common-1.1.98/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.98/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.98/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.98/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.585989 auto-test-common-1.1.98/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.98/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.98/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.98/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.98/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.98/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.98/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.587904 auto-test-common-1.1.98/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.98/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.98/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.598056 auto-test-common-1.1.98/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.98/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.98/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.98/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.98/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.98/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.98/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 02:38:40.609777 auto-test-common-1.1.98/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.98/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.98/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.98/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.98/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.98/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.98/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.98/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.98/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.98/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.98/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.98/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.98/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.98/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 02:38:40.611851 auto-test-common-1.1.98/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.98/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.066594 auto-test-common-1.1.99/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 08:55:14.066709 auto-test-common-1.1.99/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.989069 auto-test-common-1.1.99/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.989996 auto-test-common-1.1.99/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.99/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.993699 auto-test-common-1.1.99/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.99/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.99/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.99/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.99/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.998256 auto-test-common-1.1.99/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.99/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7580 2024-04-11 08:54:57.000000 auto-test-common-1.1.99/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.99/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.999884 auto-test-common-1.1.99/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.99/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.009620 auto-test-common-1.1.99/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.99/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25566 2024-04-11 02:38:06.000000 auto-test-common-1.1.99/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-1.1.99/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.99/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.024995 auto-test-common-1.1.99/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.99/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.99/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.99/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.028067 auto-test-common-1.1.99/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.99/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.99/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.99/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.036513 auto-test-common-1.1.99/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.99/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.99/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.99/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.99/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.99/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.99/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.037822 auto-test-common-1.1.99/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.046427 auto-test-common-1.1.99/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.99/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.99/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.99/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.99/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.99/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.99/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.066069 auto-test-common-1.1.99/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.99/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.99/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.99/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.99/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.99/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.99/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.99/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.99/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.99/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.99/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.99/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.99/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.99/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 08:55:14.067330 auto-test-common-1.1.99/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.99/setup.py
```

### Comparing `auto-test-common-1.1.98/PKG-INFO` & `auto-test-common-1.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.98
+Version: 1.1.99
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.98/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-1.1.99/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.98
+Version: 1.1.99
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.98/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.1.99/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.1.99/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/autotest/base_requests.py` & `auto-test-common-1.1.99/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/autotest/handle_allure.py` & `auto-test-common-1.1.99/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/autotest/handle_assert.py` & `auto-test-common-1.1.99/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/common/api_driver.py` & `auto-test-common-1.1.99/common/common/api_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,16 +128,15 @@
                     _path = adjust_path(data[key])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         all_path = os.sep.join([TEST_FILE_PATH, _path])
                         from common.file.handle_system import adjust_path
                         all_path = adjust_path(all_path)
                         data[key] = (data[key], open(all_path, 'rb'))
                     else:
-                        loguru.Logger.warning('在file目录未找到上传文件【警告】')
-                        allure_step('在file目录未找到上传文件【文件检查】', _path)
+                        loguru.logger.warning('在file目录未找到上传文件【警告】')
                 elif isinstance(data[key], tuple):
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key][1])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         if data[key].__len__() == 3:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
@@ -145,15 +144,14 @@
                             data[key] = (data[key][0], open(all_path, 'rb'), data[key][2])
                         elif data[key].__len__() == 2:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
                             all_path = adjust_path(all_path)
                             data[key] = (data[key][0], open(all_path, 'rb'))
                     else:
-                        loguru.Logger.warning('在file目录未找到上传文件【警告】')
-                        allure_step('在file目录未找到上传文件【文件检查】',_path)
+                        loguru.logger.warning('在file目录未找到上传文件【警告】')
                 else:
                     data = data
         return data
```

### Comparing `auto-test-common-1.1.98/common/common/constant.py` & `auto-test-common-1.1.99/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/common/test.py` & `auto-test-common-1.1.99/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/config/config.py` & `auto-test-common-1.1.99/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/data/data_process.py` & `auto-test-common-1.1.99/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/data/handle_common.py` & `auto-test-common-1.1.99/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/data/template_data.py` & `auto-test-common-1.1.99/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_db.py` & `auto-test-common-1.1.99/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_db_batch.py` & `auto-test-common-1.1.99/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_mongo.py` & `auto-test-common-1.1.99/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_mysqldb.py` & `auto-test-common-1.1.99/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_oracle.py` & `auto-test-common-1.1.99/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/db/handle_sqlserver.py` & `auto-test-common-1.1.99/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/driver/ui_page.py` & `auto-test-common-1.1.99/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/ReadFile.py` & `auto-test-common-1.1.99/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/handle_excel.py` & `auto-test-common-1.1.99/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/handle_file.py` & `auto-test-common-1.1.99/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/handle_reques.py` & `auto-test-common-1.1.99/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/handle_system.py` & `auto-test-common-1.1.99/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/file/handle_yaml.py` & `auto-test-common-1.1.99/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/mq/handle_rabbit.py` & `auto-test-common-1.1.99/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plat/ATF_platform.py` & `auto-test-common-1.1.99/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plat/jenkin_platform.py` & `auto-test-common-1.1.99/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plat/jira_platform.py` & `auto-test-common-1.1.99/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plat/mysql_platform.py` & `auto-test-common-1.1.99/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plat/service_platform.py` & `auto-test-common-1.1.99/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/allure_plugin.py` & `auto-test-common-1.1.99/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/assert_plugin.py` & `auto-test-common-1.1.99/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/atf_plugin.py` & `auto-test-common-1.1.99/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/data_bus.py` & `auto-test-common-1.1.99/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/data_plugin.py` & `auto-test-common-1.1.99/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/file_plugin.py` & `auto-test-common-1.1.99/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/hooks_plugin.py` & `auto-test-common-1.1.99/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/pytest_playwright.py` & `auto-test-common-1.1.99/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/pytest_plugin.py` & `auto-test-common-1.1.99/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/template_plugin.py` & `auto-test-common-1.1.99/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/common/plugin/yaml_plugin.py` & `auto-test-common-1.1.99/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.98/setup.py` & `auto-test-common-1.1.99/setup.py`

 * *Files identical despite different names*
