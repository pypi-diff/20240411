# Comparing `tmp/linktest-2.3.8.tar.gz` & `tmp/linktest-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.3.8.tar", last modified: Tue Apr  9 14:21:35 2024, max compression
+gzip compressed data, was "linktest-2.3.9.tar", last modified: Thu Apr 11 08:18:30 2024, max compression
```

## Comparing `linktest-2.3.8.tar` & `linktest-2.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-09 14:21:35.937568 linktest-2.3.8/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-09 14:21:35.937316 linktest-2.3.8/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-09 14:21:35.934511 linktest-2.3.8/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-09 14:18:58.000000 linktest-2.3.8/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-09 07:59:47.000000 linktest-2.3.8/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15820 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    32502 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8719 2024-04-09 08:55:17.000000 linktest-2.3.8/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104723 2024-04-09 09:00:24.000000 linktest-2.3.8/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7740 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-09 14:19:32.000000 linktest-2.3.8/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10111 2024-04-09 08:56:12.000000 linktest-2.3.8/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-09 06:45:08.000000 linktest-2.3.8/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-09 14:21:35.936981 linktest-2.3.8/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-09 14:21:35.000000 linktest-2.3.8/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1241 2024-04-09 14:21:35.000000 linktest-2.3.8/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-09 14:21:35.000000 linktest-2.3.8/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-09 14:21:35.000000 linktest-2.3.8/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-09 14:21:35.000000 linktest-2.3.8/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-09 14:21:35.937622 linktest-2.3.8/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-09 14:21:28.000000 linktest-2.3.8/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.535325 linktest-2.3.9/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-11 08:18:30.534953 linktest-2.3.9/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.532401 linktest-2.3.9/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-11 08:12:00.000000 linktest-2.3.9/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15820 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33851 2024-04-11 08:08:56.000000 linktest-2.3.9/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-10 09:42:36.000000 linktest-2.3.9/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104520 2024-04-11 07:37:54.000000 linktest-2.3.9/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7733 2024-04-11 08:10:09.000000 linktest-2.3.9/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-11 08:12:10.000000 linktest-2.3.9/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10727 2024-04-11 08:11:02.000000 linktest-2.3.9/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.534533 linktest-2.3.9/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1241 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-11 08:18:30.535388 linktest-2.3.9/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-11 08:18:24.000000 linktest-2.3.9/setup.py
```

### Comparing `linktest-2.3.8/linktest/appium_utils.py` & `linktest-2.3.9/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/auto_generate_testcase_list.py` & `linktest-2.3.9/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.3.9/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/base_testcase.py` & `linktest-2.3.9/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/clean_data.py` & `linktest-2.3.9/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/conver_xml_into_db.py` & `linktest-2.3.9/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/database_helper.py` & `linktest-2.3.9/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/date_utilities.py` & `linktest-2.3.9/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/doctor.py` & `linktest-2.3.9/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/framework_log.py` & `linktest-2.3.9/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/get_adb_devices.py` & `linktest-2.3.9/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/get_ios_devices_list.py` & `linktest-2.3.9/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/get_platform_info.py` & `linktest-2.3.9/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/get_project_info.py` & `linktest-2.3.9/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/html_report.py` & `linktest-2.3.9/linktest/html_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,15 +351,15 @@
             if len(failed_cases) > 0:
                 str_failed_testcase_names = ""
 
                 for failed_testcase in failed_cases:
                     str_failed_testcase_names += failed_testcase.__class__.__name__ + " "
 
                 str_failed_testcases = """
-                <button style='background-color: #DC3912; border: none; border-radius: 6px; margin-top: 2px; margin-left: 10%%;' 
+                <button style='background-color: #DC3912; border: none; border-radius: 6px; margin-top: 1px; margin-left: 10%%; width: 125px; height: 38px;' 
                 id="failed_testcase_names" class='failed_testcase_names'
                  data-clipboard-text="%s" onclick="copyFailedTestCase()">
                     <font color='white'>Copy Names of Failed Cases</font>
                 </button>
                 <script>
                     new Clipboard('.failed_testcase_names');
                 </script>
@@ -450,14 +450,21 @@
                                 "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> Log</font></a>" %
                                 failed_testcase.log_file_path)
                         except BaseException:
                             print(traceback.format_exc())
 
                         try:
                             if isinstance(failed_testcase, UITestCase):
+                                if failed_testcase.screenshot_index > 0:
+                                    for index in range(failed_testcase.screenshot_index):
+                                        report_file_handler.write(
+                                            "<a title='Screenshot%s' href='%s'> <font color='green'> - Screenshot_%s</font> </a>" %
+                                            (index + 1, "./" + failed_testcase.__module__.replace(".", "_") +
+                                             os.sep + failed_testcase.logger.name + os.sep + failed_testcase.logger.name +
+                                             "_" + str(index + 1) + "_screenshot.png", index + 1))
                                 report_file_handler.write(
                                     "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='click to see the Screenshot' href='%s'> <font color='#DC3912'> - Screenshot</font> </a>" %
                                     failed_testcase.screenshot)
                         except BaseException:
                             print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
@@ -482,15 +489,14 @@
                     report_file_handler.write("<font>")
                     if not hasattr(failed_testcase, "execution_time"):
                         failed_testcase.execution_time = ""
                     report_file_handler.write("%s" % failed_testcase.execution_time)
                     report_file_handler.write("</font>")
                     report_file_handler.write("</td></tr>")
                 report_file_handler.write("</table></td></tr></table>")
-            # report_file_handler.write("<br>")
 
             if len(passed_cases) > 0:
                 passed_testcase_table = """
                 <table align='center'>
                 <tr><td>
 
                 <table class='table table-hover' border='0'>
@@ -553,14 +559,21 @@
                             "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp;&nbsp;Log</font> </a>" %
                             passed_testcase.log_file_path)
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if isinstance(passed_testcase, UITestCase):
+                            if getattr(passed_testcase, 'screenshot_index', 0):
+                                for index in range(passed_testcase.screenshot_index):
+                                    report_file_handler.write(
+                                        "<a title='Screenshot%s' href='%s'> <font color='green'> - Screenshot_%s</font> </a>" %
+                                        (index + 1, "./" + passed_testcase.__module__.replace(".", "_") +
+                                         os.sep + passed_testcase.logger.name + os.sep + passed_testcase.logger.name +
+                                         "_" + str(index+1) + "_screenshot.png", index + 1))
                             report_file_handler.write(
                                 "<a title='Screenshot' href='%s'> <font color='green'> - Screenshot</font> </a>" %
                                 passed_testcase.screenshot)
                     except BaseException:
                         traceback.print_exc()
                         print(traceback.format_exc())
```

### Comparing `linktest-2.3.8/linktest/logged_requests.py` & `linktest-2.3.9/linktest/logged_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             res = func(*args, **kw)
 
             if not hasattr(settings, "always_generate_curl") or settings.always_generate_curl is False:
                 if res.status_code == 200:
                     return res
 
             instance.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> cURL Start >>>>>>>>>>>>>>>>>>>>>>>>>")
-            instance.logger.info(curlify.to_curl(res.request))
+            instance.logger.info(os.linesep + curlify.to_curl(res.request) + os.linesep)
             instance.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< cURL End <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
             api_version = ""
             # 检查响应头部中的各种可能的版本信息
             api_version_keys = ["version", "Version", "VERSION",
                                 "API-Version", "API-VERSION", "api-version",
                                 "API-Version-Header", "api-version-header", "API-VERSION-HEADER"]
```

### Comparing `linktest-2.3.8/linktest/main.py` & `linktest-2.3.9/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1942,22 +1942,18 @@
         for testcase_executor in testcase_executor_list:
             time.sleep(0.5)
             testcase_executor.start()
 
         for testcase_executor in testcase_executor_list:
             testcase_executor.join()
 
-        if len(TestCaseExecutor.passed_testcases) > 0:
-            print("****************** TestCases Passed: %s, Total TestCases Executed: %s): ******************" % (
-                    len(TestCaseExecutor.passed_testcases), total_testcases_count))
+        print(os.linesep + "****************** TestCases Passed: %s, TestCases Failed: %s, Total TestCases Executed: %s ******************" % (
+                len(TestCaseExecutor.passed_testcases),len(TestCaseExecutor.failed_testcases), total_testcases_count))
 
         if len(TestCaseExecutor.failed_testcases) > 0:
-            print("****************** TestCases Failed: %s, Total TestCases Executed: %s: ******************" % (
-                    len(TestCaseExecutor.failed_testcases), total_testcases_count))
-
             failed_testcase_name_list = "%s" % os.linesep
 
             for tc in TestCaseExecutor.failed_testcases:
                 failed_testcase_name_list += tc.__class__.__name__ + os.linesep
 
             print("Failed TestCase List:")
             print(failed_testcase_name_list)
@@ -2035,15 +2031,15 @@
                             rerun_flag=1 if settings.RERUN_FLAG else 0
                         )
             except BaseException:
                 traceback.print_exc()
             finally:
                 pass
 
-        print(os.linesep + "=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
+        print("=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
 
         if hasattr(settings, "COPY_REPORT_TO_SPECIFIED_PATH"):
             if settings.COPY_REPORT_TO_SPECIFIED_PATH is True:
                 if not hasattr(settings, "SPECIFIED_REPORT_PATH") or not hasattr(settings, "SPECIFIED_REPORT_HOST_IP") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PORT") or not hasattr(settings,
                                                                                               "SPECIFIED_REPORT_HOST_USERNAME") \
                         or not hasattr(settings, "SPECIFIED_REPORT_HOST_PASSWORD"):
```

### Comparing `linktest-2.3.8/linktest/memory_usage.py` & `linktest-2.3.9/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/re_func.py` & `linktest-2.3.9/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/run.py` & `linktest-2.3.9/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/run_testcase_thread.py` & `linktest-2.3.9/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/scp_report_to_specified_path.py` & `linktest-2.3.9/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/selenium_helper.py` & `linktest-2.3.9/linktest/selenium_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     browser = webdriver.Chrome(chrome_options=chrome_options)
                 else:
                     # TODO: remove below hardcode ".webrtc.", instead of providing the BROWSER_OPTION in setting/__init__.py
                     if ui_testcase.__module__.find(".webrtc.") == -1:
                         # browser = webdriver.Chrome()
 
                         # 使用 WebDriverWrapper 替换原来的 webdriver 实例
-                        browser = WebDriverWrapper(ui_testcase.logger)
+                        browser = WebDriverWrapper(ui_testcase)
                     else:
                         chrome_options.add_argument("--use-fake-device-for-media-stream")
                         chrome_options.add_argument("--use-fake-ui-for-media-stream")
                         chrome_options.add_argument("--incognito")
 
                         if platform.system() == "Darwin":
                             pass
```

### Comparing `linktest-2.3.8/linktest/timeout_thread.py` & `linktest-2.3.9/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/ui_testcase.py` & `linktest-2.3.9/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/update_config.py` & `linktest-2.3.9/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest/webdriver_wrapper.py` & `linktest-2.3.9/linktest/webdriver_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
    - get
    - find_element
    - find_elements
    - execute_script
 
    根据需要，您可以继续为其他 webdriver 方法添加日志记录功能，只需在 WebDriverWrapper 类中重写这些方法并调用 _log_action() 即可。
 """
+import os
 import typing
 from typing import List
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from selenium.webdriver.common.by import By
@@ -169,16 +170,17 @@
         self._log_action("__hash__")
         return self.element.__hash__()
 
     # todo:可以继续封装 WebElement 的其他方法
 
 
 class WebDriverWrapper(Chrome):
-    def __init__(self, logger, *args, **kwargs):
-        self.logger = logger
+    def __init__(self, ui_testcase, *args, **kwargs):
+        self.logger = ui_testcase.logger
+        self.ui_testcase = ui_testcase
         super().__init__(*args, **kwargs)
 
     def _log_action(self, action, *args):
         msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
         self.logger.info(msg)
 
     def get(self, url):
@@ -298,8 +300,20 @@
         self._log_action("set_script_timeout", time_to_wait)
         super().set_script_timeout(time_to_wait)
 
     def set_page_load_timeout(self, time_to_wait: float) -> None:
         self._log_action("set_page_load_timeout", time_to_wait)
         super().set_page_load_timeout(time_to_wait)
 
+    def save_screenshot(self, filename=None) -> bool:
+        if filename is None:
+            if not getattr(self.ui_testcase, 'screenshot_index', False):
+                setattr(self.ui_testcase, 'screenshot_index', 1)
+            else:
+                self.ui_testcase.screenshot_index += 1
+
+            filename = self.ui_testcase.full_tc_folder + os.sep + self.logger.name + "_" + str(self.ui_testcase.screenshot_index) + "_screenshot.png"
+
+        self._log_action("save_screenshot", filename)
+        return super().save_screenshot(filename)
+
     # todo 可以继续在此处添加其他 WebDriver 方法的日志记录功能
```

### Comparing `linktest-2.3.8/linktest/xml_report.py` & `linktest-2.3.9/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.8/linktest.egg-info/SOURCES.txt` & `linktest-2.3.9/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

