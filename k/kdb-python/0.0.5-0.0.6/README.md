# Comparing `tmp/kdb-python-0.0.5.tar.gz` & `tmp/kdb-python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdb-python-0.0.5.tar", last modified: Wed Sep 27 06:17:42 2023, max compression
+gzip compressed data, was "kdb-python-0.0.6.tar", last modified: Thu Apr 11 15:31:46 2024, max compression
```

## Comparing `kdb-python-0.0.5.tar` & `kdb-python-0.0.6.tar`

### file list

```diff
@@ -1,132 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.747340 kdb-python-0.0.5/
--rw-rw-rw-   0        0        0    11558 2022-11-30 15:14:57.000000 kdb-python-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      632 2023-09-27 06:17:42.744253 kdb-python-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-08-19 02:33:39.000000 kdb-python-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.048633 kdb-python-0.0.5/kdb/
--rw-rw-rw-   0        0        0     2628 2023-09-13 06:05:53.000000 kdb-python-0.0.5/kdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.120286 kdb-python-0.0.5/kdb/common/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/__init__.py
--rw-rw-rw-   0        0        0     3513 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/config_parser.py
--rw-rw-rw-   0        0        0     1494 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/constants.py
--rw-rw-rw-   0        0        0      738 2023-08-27 03:15:29.000000 kdb-python-0.0.5/kdb/common/encrypt_decrypt.py
--rw-rw-rw-   0        0        0    11111 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/mobile_manager.py
--rw-rw-rw-   0        0        0      995 2023-09-13 05:59:48.000000 kdb-python-0.0.5/kdb/common/profiles.py
--rw-rw-rw-   0        0        0     4355 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/properties.py
--rw-rw-rw-   0        0        0     1341 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/random_util.py
--rw-rw-rw-   0        0        0     1973 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/common/ssh_connection.py
--rw-rw-rw-   0        0        0    10540 2023-09-12 06:01:32.000000 kdb-python-0.0.5/kdb/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.120286 kdb-python-0.0.5/kdb/config/
--rw-rw-rw-   0        0        0      938 2023-09-13 05:51:34.000000 kdb-python-0.0.5/kdb/config/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-08-20 09:20:17.000000 kdb-python-0.0.5/kdb/config/device_list.py
--rw-rw-rw-   0        0        0      509 2023-08-27 03:26:08.000000 kdb-python-0.0.5/kdb/config/proxy_list.py
--rw-rw-rw-   0        0        0     1964 2023-09-13 05:52:41.000000 kdb-python-0.0.5/kdb/config/settings.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.120286 kdb-python-0.0.5/kdb/drivers/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:14:57.000000 kdb-python-0.0.5/kdb/drivers/__init__.py
--rw-rw-rw-   0        0        0      617 2023-08-20 02:00:17.000000 kdb-python-0.0.5/kdb/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.127395 kdb-python-0.0.5/kdb/report/
--rw-rw-rw-   0        0        0     9079 2023-08-09 11:22:10.000000 kdb-python-0.0.5/kdb/report/__init__.py
--rw-rw-rw-   0        0        0     6278 2023-09-13 05:59:48.000000 kdb-python-0.0.5/kdb/report/report_manager.py
--rw-rw-rw-   0        0        0     2374 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/report/test_case_log.py
--rw-rw-rw-   0        0        0      527 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/report/test_step_log.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.143030 kdb-python-0.0.5/kdb/scripts/
--rw-rw-rw-   0        0        0     4325 2023-08-27 04:07:08.000000 kdb-python-0.0.5/kdb/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.143030 kdb-python-0.0.5/kdb/unit_test/
--rw-rw-rw-   0        0        0        0 2023-08-19 09:46:05.000000 kdb-python-0.0.5/kdb/unit_test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.363463 kdb-python-0.0.5/kdb/unit_test/mobile/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/__init__.py
--rw-rw-rw-   0        0        0     4233 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_alert.py
--rw-rw-rw-   0        0        0     2712 2023-09-08 05:57:44.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_app.py
--rw-rw-rw-   0        0        0     1604 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_browser_navigation.py
--rw-rw-rw-   0        0        0     4544 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_check.py
--rw-rw-rw-   0        0        0     1694 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_click.py
--rw-rw-rw-   0        0        0      604 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_close_browser.py
--rw-rw-rw-   0        0        0     3697 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_cookies.py
--rw-rw-rw-   0        0        0      950 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_double_click.py
--rw-rw-rw-   0        0        0     3970 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_element_attribute.py
--rw-rw-rw-   0        0        0      892 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_execute_script.py
--rw-rw-rw-   0        0        0     1415 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_is_display.py
--rw-rw-rw-   0        0        0      660 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_open_url.py
--rw-rw-rw-   0        0        0     3711 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_press_keys.py
--rw-rw-rw-   0        0        0     2124 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_press_keys_and_click.py
--rw-rw-rw-   0        0        0     1536 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_select.py
--rw-rw-rw-   0        0        0     3587 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_start_browser.py
--rw-rw-rw-   0        0        0     1719 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_tap.py
--rw-rw-rw-   0        0        0     1926 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_update_text.py
--rw-rw-rw-   0        0        0     1017 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_text_on_page.py
--rw-rw-rw-   0        0        0      842 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_title.py
--rw-rw-rw-   0        0        0     1724 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_url_contains.py
--rw-rw-rw-   0        0        0     3486 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_video.py
--rw-rw-rw-   0        0        0     2092 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/mobile/test_window.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.410710 kdb-python-0.0.5/kdb/unit_test/no_driver/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/__init__.py
--rw-rw-rw-   0        0        0      207 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_command_line.py
--rw-rw-rw-   0        0        0     1133 2023-09-13 06:03:39.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_files.py
--rw-rw-rw-   0        0        0      364 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_global_var.py
--rw-rw-rw-   0        0        0     4523 2023-08-27 02:09:45.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_json_path.py
--rw-rw-rw-   0        0        0     1133 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_random.py
--rw-rw-rw-   0        0        0     3027 2023-07-24 16:46:01.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_requests.py
--rw-rw-rw-   0        0        0      905 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/no_driver/test_verify_string_contains.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.598171 kdb-python-0.0.5/kdb/unit_test/pc/
--rw-rw-rw-   0        0        0      550 2023-08-19 09:46:45.000000 kdb-python-0.0.5/kdb/unit_test/pc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.604687 kdb-python-0.0.5/kdb/unit_test/pc/page_object/
--rw-rw-rw-   0        0        0        0 2023-08-19 09:43:04.000000 kdb-python-0.0.5/kdb/unit_test/pc/page_object/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-08-19 17:40:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/page_object/signup.py
--rw-rw-rw-   0        0        0     3755 2023-09-13 17:04:07.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_alert.py
--rw-rw-rw-   0        0        0      942 2023-09-13 17:04:07.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_browser_navigation.py
--rw-rw-rw-   0        0        0     1382 2023-08-19 16:01:09.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_check.py
--rw-rw-rw-   0        0        0     1655 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_click.py
--rw-rw-rw-   0        0        0      633 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_close_browser.py
--rw-rw-rw-   0        0        0      536 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_context_click.py
--rw-rw-rw-   0        0        0     3697 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_cookies.py
--rw-rw-rw-   0        0        0      950 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_double_click.py
--rw-rw-rw-   0        0        0     3970 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_element_attribute.py
--rw-rw-rw-   0        0        0      949 2023-09-27 05:58:39.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_element_text.py
--rw-rw-rw-   0        0        0      892 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_execute_script.py
--rw-rw-rw-   0        0        0     1780 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_hover.py
--rw-rw-rw-   0        0        0     1649 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_is_display.py
--rw-rw-rw-   0        0        0      660 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_open_url.py
--rw-rw-rw-   0        0        0     3747 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_press_keys.py
--rw-rw-rw-   0        0        0     1468 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_press_keys_and_click.py
--rw-rw-rw-   0        0        0     1536 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_select.py
--rw-rw-rw-   0        0        0     6791 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_start_browser.py
--rw-rw-rw-   0        0        0     1209 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_uncheck.py
--rw-rw-rw-   0        0        0     1926 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_update_text.py
--rw-rw-rw-   0        0        0     1829 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_upload_file.py
--rw-rw-rw-   0        0        0     1020 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_verify_element_attribute.py
--rw-rw-rw-   0        0        0      864 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_verify_text_on_page.py
--rw-rw-rw-   0        0        0      851 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_verify_title.py
--rw-rw-rw-   0        0        0     1801 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_verify_url_contains.py
--rw-rw-rw-   0        0        0     3459 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_video.py
--rw-rw-rw-   0        0        0     2092 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/unit_test/pc/test_window.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.693016 kdb-python-0.0.5/kdb/webdriver/
--rw-rw-rw-   0        0        0       85 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.724876 kdb-python-0.0.5/kdb/webdriver/actions/
--rw-rw-rw-   0        0        0    27445 2023-09-25 06:06:44.000000 kdb-python-0.0.5/kdb/webdriver/actions/__init__.py
--rw-rw-rw-   0        0        0     2751 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/actions/alert.py
--rw-rw-rw-   0        0        0     1833 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/actions/cookies.py
--rw-rw-rw-   0        0        0     6653 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/actions/mobile_gestures.py
--rw-rw-rw-   0        0        0     4714 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/actions/video.py
--rw-rw-rw-   0        0        0     4724 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/alert.py
--rw-rw-rw-   0        0        0     3949 2023-09-13 06:03:39.000000 kdb-python-0.0.5/kdb/webdriver/common.py
--rw-rw-rw-   0        0        0     5825 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/cookies.py
--rw-rw-rw-   0        0        0     2763 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/files.py
--rw-rw-rw-   0        0        0     5744 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/json_path.py
--rw-rw-rw-   0        0        0    44874 2023-09-25 06:09:30.000000 kdb-python-0.0.5/kdb/webdriver/kdb_webdriver.py
--rw-rw-rw-   0        0        0    16450 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/kdb_webelement.py
--rw-rw-rw-   0        0        0     4762 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/keys.py
--rw-rw-rw-   0        0        0     2932 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/mobile_gestures.py
--rw-rw-rw-   0        0        0     1341 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/random.py
--rw-rw-rw-   0        0        0     9236 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/requests.py
--rw-rw-rw-   0        0        0    10706 2023-09-27 06:12:17.000000 kdb-python-0.0.5/kdb/webdriver/video.py
--rw-rw-rw-   0        0        0    10115 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/videoelement.py
--rw-rw-rw-   0        0        0    15884 2023-09-13 06:10:43.000000 kdb-python-0.0.5/kdb/webdriver/webdriver_generator.py
--rw-rw-rw-   0        0        0     5854 2022-11-30 15:15:00.000000 kdb-python-0.0.5/kdb/webdriver/windows.py
-drwxrwxrwx   0        0        0        0 2023-09-27 06:17:42.744253 kdb-python-0.0.5/kdb_python.egg-info/
--rw-rw-rw-   0        0        0      632 2023-09-27 06:17:42.000000 kdb-python-0.0.5/kdb_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-09-27 06:17:42.000000 kdb-python-0.0.5/kdb_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-27 06:17:42.000000 kdb-python-0.0.5/kdb_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-28 16:40:31.000000 kdb-python-0.0.5/kdb_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-09-27 06:17:42.000000 kdb-python-0.0.5/kdb_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      519 2023-09-17 09:56:04.000000 kdb-python-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-27 06:17:42.747340 kdb-python-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-09-08 15:07:17.000000 kdb-python-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.883787 kdb-python-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2022-11-30 15:14:57.000000 kdb-python-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      627 2024-04-11 15:31:46.883787 kdb-python-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-08-19 02:33:39.000000 kdb-python-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.349799 kdb-python-0.0.6/kdb/
+-rw-rw-rw-   0        0        0     2629 2023-10-25 16:24:34.000000 kdb-python-0.0.6/kdb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.413023 kdb-python-0.0.6/kdb/common/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/__init__.py
+-rw-rw-rw-   0        0        0     3513 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/config_parser.py
+-rw-rw-rw-   0        0        0     1494 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/constants.py
+-rw-rw-rw-   0        0        0      738 2023-08-27 03:15:29.000000 kdb-python-0.0.6/kdb/common/encrypt_decrypt.py
+-rw-rw-rw-   0        0        0    11731 2024-03-27 15:57:05.000000 kdb-python-0.0.6/kdb/common/mobile_manager.py
+-rw-rw-rw-   0        0        0      995 2023-09-13 05:59:48.000000 kdb-python-0.0.6/kdb/common/profiles.py
+-rw-rw-rw-   0        0        0     4355 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/properties.py
+-rw-rw-rw-   0        0        0     1341 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/random_util.py
+-rw-rw-rw-   0        0        0     1973 2022-11-30 15:14:57.000000 kdb-python-0.0.6/kdb/common/ssh_connection.py
+-rw-rw-rw-   0        0        0    10540 2023-09-12 06:01:32.000000 kdb-python-0.0.6/kdb/common/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.432065 kdb-python-0.0.6/kdb/config/
+-rw-rw-rw-   0        0        0      938 2023-09-13 05:51:34.000000 kdb-python-0.0.6/kdb/config/__init__.py
+-rw-rw-rw-   0        0        0     1964 2023-09-13 05:52:41.000000 kdb-python-0.0.6/kdb/config/settings.py
+-rw-rw-rw-   0        0        0      617 2023-08-20 02:00:17.000000 kdb-python-0.0.6/kdb/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.444074 kdb-python-0.0.6/kdb/report/
+-rw-rw-rw-   0        0        0     9079 2023-08-09 11:22:10.000000 kdb-python-0.0.6/kdb/report/__init__.py
+-rw-rw-rw-   0        0        0     6278 2023-09-13 05:59:48.000000 kdb-python-0.0.6/kdb/report/report_manager.py
+-rw-rw-rw-   0        0        0     2374 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/report/test_case_log.py
+-rw-rw-rw-   0        0        0      527 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/report/test_step_log.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.444074 kdb-python-0.0.6/kdb/scripts/
+-rw-rw-rw-   0        0        0     4325 2023-08-27 04:07:08.000000 kdb-python-0.0.6/kdb/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.459705 kdb-python-0.0.6/kdb/unit_test/
+-rw-rw-rw-   0        0        0        0 2023-08-19 09:46:05.000000 kdb-python-0.0.6/kdb/unit_test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.663807 kdb-python-0.0.6/kdb/unit_test/mobile/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/__init__.py
+-rw-rw-rw-   0        0        0     4233 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_alert.py
+-rw-rw-rw-   0        0        0     2712 2023-09-08 05:57:44.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_app.py
+-rw-rw-rw-   0        0        0     1604 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_browser_navigation.py
+-rw-rw-rw-   0        0        0     4544 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_check.py
+-rw-rw-rw-   0        0        0     1694 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_click.py
+-rw-rw-rw-   0        0        0      604 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_close_browser.py
+-rw-rw-rw-   0        0        0     3697 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_cookies.py
+-rw-rw-rw-   0        0        0      950 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_double_click.py
+-rw-rw-rw-   0        0        0     3970 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_element_attribute.py
+-rw-rw-rw-   0        0        0      892 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_execute_script.py
+-rw-rw-rw-   0        0        0     1415 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_is_display.py
+-rw-rw-rw-   0        0        0      660 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_open_url.py
+-rw-rw-rw-   0        0        0     3711 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_press_keys.py
+-rw-rw-rw-   0        0        0     2124 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_press_keys_and_click.py
+-rw-rw-rw-   0        0        0     1536 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_select.py
+-rw-rw-rw-   0        0        0     3587 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_start_browser.py
+-rw-rw-rw-   0        0        0     1719 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_tap.py
+-rw-rw-rw-   0        0        0     1926 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_update_text.py
+-rw-rw-rw-   0        0        0     1017 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_text_on_page.py
+-rw-rw-rw-   0        0        0      842 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_title.py
+-rw-rw-rw-   0        0        0     1724 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_url_contains.py
+-rw-rw-rw-   0        0        0     3486 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_video.py
+-rw-rw-rw-   0        0        0     2092 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/mobile/test_window.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.710666 kdb-python-0.0.6/kdb/unit_test/no_driver/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/__init__.py
+-rw-rw-rw-   0        0        0      207 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_command_line.py
+-rw-rw-rw-   0        0        0     1133 2023-09-13 06:03:39.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_files.py
+-rw-rw-rw-   0        0        0      364 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_global_var.py
+-rw-rw-rw-   0        0        0     4523 2023-08-27 02:09:45.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_json_path.py
+-rw-rw-rw-   0        0        0     1133 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_random.py
+-rw-rw-rw-   0        0        0     3027 2023-07-24 16:46:01.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_requests.py
+-rw-rw-rw-   0        0        0      905 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/no_driver/test_verify_string_contains.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.741966 kdb-python-0.0.6/kdb/unit_test/pc/
+-rw-rw-rw-   0        0        0      971 2023-10-15 11:36:53.000000 kdb-python-0.0.6/kdb/unit_test/pc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.741966 kdb-python-0.0.6/kdb/unit_test/pc/page_object/
+-rw-rw-rw-   0        0        0        0 2023-08-19 09:43:04.000000 kdb-python-0.0.6/kdb/unit_test/pc/page_object/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-08-19 17:40:00.000000 kdb-python-0.0.6/kdb/unit_test/pc/page_object/signup.py
+-rw-rw-rw-   0        0        0     3814 2023-10-16 16:34:37.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_alert.py
+-rw-rw-rw-   0        0        0      898 2023-10-16 16:35:56.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_browser_navigation.py
+-rw-rw-rw-   0        0        0     1842 2023-10-10 05:41:28.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_check_and_uncheck.py
+-rw-rw-rw-   0        0        0     1861 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_click.py
+-rw-rw-rw-   0        0        0      842 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_context_click.py
+-rw-rw-rw-   0        0        0     3697 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_cookies.py
+-rw-rw-rw-   0        0        0      950 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_double_click.py
+-rw-rw-rw-   0        0        0     3689 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_element_attribute.py
+-rw-rw-rw-   0        0        0      949 2023-09-27 05:58:39.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_element_text.py
+-rw-rw-rw-   0        0        0      827 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_execute_script.py
+-rw-rw-rw-   0        0        0     1378 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_hover.py
+-rw-rw-rw-   0        0        0     1476 2023-10-15 11:35:30.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_is_display.py
+-rw-rw-rw-   0        0        0     3561 2023-10-15 04:23:25.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_press_keys.py
+-rw-rw-rw-   0        0        0     1103 2023-10-15 02:31:38.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_press_keys_and_click.py
+-rw-rw-rw-   0        0        0     1346 2023-10-13 06:24:01.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_select.py
+-rw-rw-rw-   0        0        0     7154 2024-03-27 16:06:15.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_start_browser.py
+-rw-rw-rw-   0        0        0     1097 2023-10-10 05:37:13.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_update_text.py
+-rw-rw-rw-   0        0        0     1829 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_upload_file.py
+-rw-rw-rw-   0        0        0     1323 2023-10-10 05:37:13.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_verify_element_attribute.py
+-rw-rw-rw-   0        0        0      889 2023-10-10 05:37:13.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_verify_text_on_page.py
+-rw-rw-rw-   0        0        0      838 2023-10-10 05:37:13.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_verify_title.py
+-rw-rw-rw-   0        0        0     1618 2023-10-10 05:37:13.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_verify_url_contains.py
+-rw-rw-rw-   0        0        0     3459 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_video.py
+-rw-rw-rw-   0        0        0     1983 2023-10-16 16:45:30.000000 kdb-python-0.0.6/kdb/unit_test/pc/test_window.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.851940 kdb-python-0.0.6/kdb/webdriver/
+-rw-rw-rw-   0        0        0       85 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.883787 kdb-python-0.0.6/kdb/webdriver/actions/
+-rw-rw-rw-   0        0        0    28065 2023-10-15 04:20:35.000000 kdb-python-0.0.6/kdb/webdriver/actions/__init__.py
+-rw-rw-rw-   0        0        0     2751 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/actions/alert.py
+-rw-rw-rw-   0        0        0     1833 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/actions/cookies.py
+-rw-rw-rw-   0        0        0     6653 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/actions/mobile_gestures.py
+-rw-rw-rw-   0        0        0     4714 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/actions/video.py
+-rw-rw-rw-   0        0        0     4724 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/alert.py
+-rw-rw-rw-   0        0        0     3949 2023-09-13 06:03:39.000000 kdb-python-0.0.6/kdb/webdriver/common.py
+-rw-rw-rw-   0        0        0     5825 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/cookies.py
+-rw-rw-rw-   0        0        0     2763 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/files.py
+-rw-rw-rw-   0        0        0     5744 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/json_path.py
+-rw-rw-rw-   0        0        0    44870 2023-10-15 11:34:57.000000 kdb-python-0.0.6/kdb/webdriver/kdb_webdriver.py
+-rw-rw-rw-   0        0        0    16450 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/kdb_webelement.py
+-rw-rw-rw-   0        0        0     4918 2023-10-15 04:20:35.000000 kdb-python-0.0.6/kdb/webdriver/keys.py
+-rw-rw-rw-   0        0        0     2932 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/mobile_gestures.py
+-rw-rw-rw-   0        0        0     1341 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/random.py
+-rw-rw-rw-   0        0        0     9236 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/requests.py
+-rw-rw-rw-   0        0        0    10706 2023-09-27 06:12:17.000000 kdb-python-0.0.6/kdb/webdriver/video.py
+-rw-rw-rw-   0        0        0    10115 2022-11-30 15:15:00.000000 kdb-python-0.0.6/kdb/webdriver/videoelement.py
+-rw-rw-rw-   0        0        0    18840 2024-03-27 15:26:33.000000 kdb-python-0.0.6/kdb/webdriver/webdriver_generator.py
+-rw-rw-rw-   0        0        0     5854 2023-10-10 05:37:12.000000 kdb-python-0.0.6/kdb/webdriver/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:31:46.883787 kdb-python-0.0.6/kdb_python.egg-info/
+-rw-rw-rw-   0        0        0      627 2024-04-11 15:31:46.000000 kdb-python-0.0.6/kdb_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3633 2024-04-11 15:31:46.000000 kdb-python-0.0.6/kdb_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 15:31:46.000000 kdb-python-0.0.6/kdb_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-11 15:31:45.000000 kdb-python-0.0.6/kdb_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-04-11 15:31:46.000000 kdb-python-0.0.6/kdb_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      516 2024-04-11 15:31:39.000000 kdb-python-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 15:31:46.883787 kdb-python-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-09-08 15:07:17.000000 kdb-python-0.0.6/setup.py
```

### Comparing `kdb-python-0.0.5/LICENSE` & `kdb-python-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/PKG-INFO` & `kdb-python-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kdb-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation testing
 Home-page: https://github.com/Trucnt/kdb-core
 Author: Truc Nguyen
-Author-email: Truc Nguyen <trucnt88@gmail.com>
+Author-email: Trucnt <trucnt88@gmail.com>
 License: MIT
 Project-URL: home-page, https://github.com/Trucnt/kdb-demo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kdb-python-0.0.5/kdb/__init__.py` & `kdb-python-0.0.6/kdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 
 # cmd param
 ENV = 'production'  # dev, production
 BROWSER = 'chrome'
 PARAMS = []
 WORKSPACE = None
-PROFILE_NAME = None
+PROFILE_NAME = 'dev'
 APP_PATH = None
 
 # constant
 SESSION_ID = str(int(time.time())) + str(random.randrange(10000, 99999))
 
 XML_REPORT_FILE = 'xml_report_main.xml'
 APPIUM_LOCK_FILE = '~/.appium.lock'
```

### Comparing `kdb-python-0.0.5/kdb/common/config_parser.py` & `kdb-python-0.0.6/kdb/common/config_parser.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/constants.py` & `kdb-python-0.0.6/kdb/common/constants.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/encrypt_decrypt.py` & `kdb-python-0.0.6/kdb/common/encrypt_decrypt.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/mobile_manager.py` & `kdb-python-0.0.6/kdb/common/mobile_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+import json
 import logging
+import os
 import time
 from random import random
 
 from selenium.common.exceptions import TimeoutException, SessionNotCreatedException, InvalidArgumentException
 
 from kdb import APPIUM_LOCK_FILE
+from kdb import FolderSettings
 from kdb.common.constants import ErrorMessage, AppiumCommand
 from kdb.common.ssh_connection import SSH
 from kdb.common.utils import DeviceType
-from kdb.config import device_list
 from kdb.config.settings import MobileSettings
 
 _ssh = SSH(MobileSettings.HOST, MobileSettings.USERNAME, MobileSettings.PASSWORD)
 
 
+def _get_device_config(device_type):
+    """
+    get the device info by type from config file (mobile-devices.json)
+    """
+    with open(os.path.join(FolderSettings.CONFIG_DIR, 'mobile-devices.json')) as devices_file:
+        data = json.load(devices_file)
+    if not device_type or not data or not data['devices'][str(device_type).lower()]:
+        raise Exception("No device is found for %s." % device_type)
+    return data['devices'][str(device_type).lower()]
+
+
 def execute_ssh_command(command, new_connection=False, print_command=True):
     """
     Execute a command in server
     """
     if new_connection:
         new_ssh = SSH(MobileSettings.HOST, MobileSettings.USERNAME, MobileSettings.PASSWORD)
         return new_ssh.execute_command(command, print_command)
@@ -30,50 +43,53 @@
     Get the device(s) information from configuration file
     """
     device_name = str(device_name).lower()
     is_group = False
 
     if DeviceType.is_android(device_name):
         # android
+        android_list = _get_device_config(DeviceType.ANDROID)
         if DeviceType.ANDROID == device_name:
             is_group = True
             # android group
             # shuffling device_list.ANDROID
-            return is_group, dict(sorted(device_list.ANDROID.items(), key=lambda x: random()))
+            return is_group, dict(sorted(android_list.items(), key=lambda x: random()))
         else:
-            if device_list.ANDROID.get(device_name) is not None:
-                return is_group, device_list.ANDROID.get(device_name)
+            if android_list.get(device_name) is not None:
+                return is_group, android_list.get(device_name)
             else:
                 raise InvalidArgumentException(ErrorMessage.DEVICE_NOT_FOUND % device_name)
 
     elif DeviceType.is_ios(device_name):
         # ios
+        ios_list = _get_device_config(DeviceType.IOS)
         if DeviceType.IOS == device_name:
             # ios group
             is_group = True
             # shuffling device_list.IOS
-            return is_group, dict(sorted(device_list.IOS.items(), key=lambda x: random()))
+            return is_group, dict(sorted(ios_list.items(), key=lambda x: random()))
         else:
             # ios device
-            if device_list.IOS.get(device_name) is not None:
-                return is_group, device_list.IOS.get(device_name)
+            if ios_list.get(device_name) is not None:
+                return is_group, ios_list.get(device_name)
             else:
                 raise InvalidArgumentException(ErrorMessage.DEVICE_NOT_FOUND % device_name)
     else:
         # raise exception
         raise InvalidArgumentException(ErrorMessage.DEVICE_NOT_FOUND % device_name)
 
 
 def check_free_port(device_alias, device_info):
     """
     Check device's Appium port is running or not. In Simulator case, return False if we have one simulator running.
     """
     if DeviceType.is_simulator(device_alias):
         simulator_ports = ""
-        for device_key, device_value in device_list.SIMULATOR.items():
+        ios_list = _get_device_config(DeviceType.IOS)
+        for device_key, device_value in ios_list.items():
             simulator_ports += "," + str()
             result = execute_ssh_command(
                 AppiumCommand.GET_PROCESS_ID_BY_PORT % ("appium", device_value.get('appiumPort')), print_command=False)
             if len(result) > 0:
                 return False
         else:
             return True
@@ -146,15 +162,15 @@
         # find a device until time out
         while True:
             if created_lock_file:
                 # checking whether the given device name is group or single device
                 if is_group:
                     # running on a group device
                     for device_alias, device_value in device_info.items():
-                        # device_alias: is key (device_name) in device_list.py
+                        # device_alias: is key (device_name) in mobile-devices.json
                         result = start_appium(device_alias, device_value)
                         if result is not None:
                             return result
                 else:
                     # running a single device
                     result = start_appium(device_name, device_info)
                     if result is not None:
```

### Comparing `kdb-python-0.0.5/kdb/common/profiles.py` & `kdb-python-0.0.6/kdb/common/profiles.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/properties.py` & `kdb-python-0.0.6/kdb/common/properties.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/random_util.py` & `kdb-python-0.0.6/kdb/common/random_util.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/ssh_connection.py` & `kdb-python-0.0.6/kdb/common/ssh_connection.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/common/utils.py` & `kdb-python-0.0.6/kdb/common/utils.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/config/__init__.py` & `kdb-python-0.0.6/kdb/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/config/settings.py` & `kdb-python-0.0.6/kdb/config/settings.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/exceptions.py` & `kdb-python-0.0.6/kdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/report/__init__.py` & `kdb-python-0.0.6/kdb/report/__init__.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/report/report_manager.py` & `kdb-python-0.0.6/kdb/report/report_manager.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/report/test_case_log.py` & `kdb-python-0.0.6/kdb/report/test_case_log.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/report/test_step_log.py` & `kdb-python-0.0.6/kdb/report/test_step_log.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/scripts/__init__.py` & `kdb-python-0.0.6/kdb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_alert.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_alert.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_app.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_app.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_browser_navigation.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_browser_navigation.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_check.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_check.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_click.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_click.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_close_browser.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_close_browser.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_cookies.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_cookies.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_double_click.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_double_click.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_element_attribute.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_element_attribute.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_execute_script.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_execute_script.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_is_display.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_is_display.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_open_url.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_open_url.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_press_keys.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_press_keys.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_press_keys_and_click.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_press_keys_and_click.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_select.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_select.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_start_browser.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_start_browser.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_tap.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_tap.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_update_text.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_update_text.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_text_on_page.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_text_on_page.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_title.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_title.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_verify_url_contains.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_verify_url_contains.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_video.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_video.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/mobile/test_window.py` & `kdb-python-0.0.6/kdb/unit_test/mobile/test_window.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/no_driver/test_files.py` & `kdb-python-0.0.6/kdb/unit_test/no_driver/test_files.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/no_driver/test_json_path.py` & `kdb-python-0.0.6/kdb/unit_test/no_driver/test_json_path.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/no_driver/test_random.py` & `kdb-python-0.0.6/kdb/unit_test/no_driver/test_random.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/no_driver/test_requests.py` & `kdb-python-0.0.6/kdb/unit_test/no_driver/test_requests.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/no_driver/test_verify_string_contains.py` & `kdb-python-0.0.6/kdb/unit_test/no_driver/test_verify_string_contains.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/__init__.py` & `kdb-python-0.0.6/kdb/unit_test/pc/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
+def hidden_ads():
+    try:
+        kdb_driver.set_element_attribute("id=fixedban", 'style', 'display: none !important;', log=False, timeout=3)
+        kdb_driver.set_element_attribute("xpath=//footer", 'style', 'display: none !important;', log=False, timeout=3)
+        kdb_driver.execute_script("document.querySelectorAll('iframe').forEach(function(element) {element.remove();});")
+    except:
+        pass
+
+
 def login_unit_test_page():
     report.add_comment("Open Tiki.vn page")
     # start browser
     kdb_driver.start_browser()
     # load page for test
     kdb_driver.open_url('https://tiki.vn/')
 
     # update text
     # kdb_driver.update_text('id=user-name', 'standard_user')
     # kdb_driver.update_text('id=password', 'secret_sauce')
     # # click to the search button
     # kdb_driver.click('id=login-button')
-    kdb_driver.verify_text_on_page('Sản phẩm bán chạy')
+    kdb_driver.verify_text_on_page('Sản phẩm bán chạy')
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/page_object/signup.py` & `kdb-python-0.0.6/kdb/unit_test/pc/page_object/signup.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_alert.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from kdb import report
+from kdb.unit_test.pc import hidden_ads
 from kdb.webdriver import kdb_driver
 
 
 def alert_test():
     report.add_comment("Test alert")
     # start browser
     kdb_driver.start_browser()
     # load page for test.
     kdb_driver.open_url('https://demoqa.com/alerts')
+    hidden_ads()
     kdb_driver.screen_shot()
 
     # TODO: get, verify alert text and accept
     report.add_comment("get, verify alert text and accept")
     kdb_driver.click("id=alertButton")
     # get text in alert
     text_alert = kdb_driver.alert.get_text()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_browser_navigation.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_element_text.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def test_browser_nav():
-    # start browser
-    report.add_comment("Test browser navigation")
+def element_text_test():
+    report.add_comment("Test get the text of element")
     # start browser
     kdb_driver.start_browser()
-    # load page for test.
+    # load url home page
     kdb_driver.open_url('https://demoqa.com/text-box')
-    kdb_driver.screen_shot()
 
-    # click a left menu "Điện Gia Dụng"
-    # href="https://tiki.vn/dien-gia-dung/c1882"
-    kdb_driver.click("xpath=//a[@href='https://tiki.vn/dien-gia-dung/c1882']")
-    kdb_driver.verify_text_on_page("Back to products")
-    #  //a[@data-view-index='1']/span[@title='Điện Gia Dụng']
-    kdb_driver.screen_shot()
-    kdb_driver.back()
-    kdb_driver.verify_url_contains("https://www.saucedemo.com/inventory.html")
-    kdb_driver.screen_shot()
-    kdb_driver.forward()
-    kdb_driver.verify_text_on_page("Back to products")
+    # TODO in viewport
+    report.add_comment(">>> IN VIEWPORT")
+    # verify element text
+    submit_btn_text = kdb_driver.get_element_text("id=submit")
+    kdb_driver.verify_string_contains(submit_btn_text, 'Submit')
     kdb_driver.screen_shot()
 
+    # TODO out of viewport
+    report.add_comment(">>> OUT OF VIEWPORT")
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
+    # verify element text
+    submit_btn_text = kdb_driver.get_element_text("id=stateCity-wrapper")
+    kdb_driver.verify_string_contains(submit_btn_text, 'State and City')
+    kdb_driver.screen_shot()
 
+    # close browser
     kdb_driver.close_browser()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_click.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_double_click.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,26 @@
-import time
-
-import kdb
 from kdb import report
-from kdb.webdriver import kdb_driver, webdriver_generator
+from kdb.webdriver import kdb_driver
 
 
-def click_test():
-    report.add_comment("Test click")
+def double_click_test():
+    # add command to the report
+    report.add_comment("Test double_click keyword/api")
     # start browser
     kdb_driver.start_browser()
-    # load page for test.
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-
-    # TODO click an element in viewport
-    report.add_comment(">>> IN VIEWPORT")
-    # click to the "Contact us" link
-    kdb_driver.click("xpath=//div[@id='contact-link']/a")
-    # verify text to confirm click success
-    kdb_driver.verify_text_on_page('Customer service - Contact us')
-    kdb_driver.screen_shot()
-
-    # TODO click an element out of viewport
-    report.add_comment(">>> OUT OF VIEWPORT")
-    # load home page
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-    # click to the "submitNewsletter" button
-    kdb_driver.click("xpath=//button[@name='submitNewsletter']", timeout=5)
-    # verify text to confirm click success
-    kdb_driver.verify_text_on_page('Newsletter : Invalid email address.')
+    # loads login page in the current browser session.
+    kdb_driver.open_url('https://unixpapa.com/js/testmouse.html')
+    # verify textarea before
+    kdb_driver.verify_element_attribute('xpath=//textarea', 'value', 'dblclick', check_contains=True, reverse=True,
+                                        timeout=2)
+    # take screenshot
     kdb_driver.screen_shot()
+    # double click
+    kdb_driver.double_click('xpath=//tr/td[1]/a[1]')
 
-    # TODO click an element in iframe
-    report.add_comment(">>> IN IFRAME")
-    if kdb.BROWSER.lower() in webdriver_generator._FIREFOX_ALIAS:
-        time.sleep(5)
-    # click the "PrestaShop" link inside iframe
-    kdb_driver.click("xpath=//a[contains(@class, '_3-8_ lfloat')]", extra_time=1)
-    # switch to fb window
-    kdb_driver.windows.next()
-    # verify text to confirm click success
-    kdb_driver.verify_url_contains('facebook.com/prestashop')
+    # verify textarea after double click
+    kdb_driver.verify_element_attribute('xpath=//textarea', 'value', 'dblclick', check_contains=True, timeout=3)
+    # take screenshot
     kdb_driver.screen_shot()
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_context_click.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_context_click.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from kdb import report
+from kdb.unit_test.pc import hidden_ads
 from kdb.webdriver import kdb_driver
 
 
 def context_click_test():
     report.add_comment("Test context click keyword/api")
     # start browser
     kdb_driver.start_browser()
     # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-    # context click to "Contact us" link
-    kdb_driver.context_click('id=contact-link', extra_time=10)
-    # todo verifying
+    kdb_driver.open_url('https://demoqa.com/buttons')
+    hidden_ads()
 
-    # take screenshot
+    # TODO click an element in viewport
+    report.add_comment(">>> IN VIEWPORT")
+    kdb_driver.verify_text_on_page('You have done a right click', reverse=True, timeout=3)
+    kdb_driver.screen_shot()
+    # click to the "Click Me" button
+    kdb_driver.context_click("id=rightClickBtn")
+    # verify text to confirm right click success
+    kdb_driver.verify_text_on_page('You have done a right click')
     kdb_driver.screen_shot()
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_cookies.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_cookies.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_double_click.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_verify_text_on_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def double_click_test():
-    # add command to the report
-    report.add_comment("Test double_click keyword/api")
+def verify_text_on_page_test():
+    report.add_comment("Test verify text on page")
     # start browser
     kdb_driver.start_browser()
     # loads login page in the current browser session.
-    kdb_driver.open_url('https://unixpapa.com/js/testmouse.html')
-    # verify textarea before
-    kdb_driver.verify_element_attribute('xpath=//textarea', 'value', 'dblclick', check_contains=True, reverse=True,
-                                        timeout=2)
-    # take screenshot
-    kdb_driver.screen_shot()
-    # double click
-    kdb_driver.double_click('xpath=//tr/td[1]/a[1]')
+    kdb_driver.open_url('http://automationpractice.com/index.php')
 
-    # verify textarea after double click
-    kdb_driver.verify_element_attribute('xpath=//textarea', 'value', 'dblclick', check_contains=True, timeout=3)
-    # take screenshot
-    kdb_driver.screen_shot()
+    # verify text is displayed on web page
+    kdb_driver.verify_text_on_page('This Account has been suspended.')
+    # verify text not displayed in web page
+    kdb_driver.verify_text_on_page('This text not in page', reverse=True, timeout=2)
+
+    #
+    kdb_driver.open_url('https://demoqa.com/nestedframes')
+    # verify hidden text
+    kdb_driver.verify_text_on_page('Practice Form', reverse=True, timeout=2)
+    # verify text inside frame
+    kdb_driver.verify_text_on_page('Child Iframe')
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_element_attribute.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_element_attribute.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 from kdb import report
+from kdb.unit_test.pc import hidden_ads
 from kdb.webdriver import kdb_driver
 
 
 def element_attribute_test():
     attribute_value = 'text for set attribute'
     report.add_comment("Test get,set and verify attributes of element")
     # start browser
     kdb_driver.start_browser()
     # load url home page
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
+    hidden_ads()
 
     # TODO in viewport
     report.add_comment(">>> IN VIEWPORT")
     # verify element attribute before set attribute
-    kdb_driver.verify_element_attribute("id=search_query_top", 'value', attribute_value, reverse=True, timeout=3)
+    kdb_driver.verify_element_attribute("id=firstName", 'value', attribute_value, reverse=True, timeout=3)
     # set
-    kdb_driver.set_element_attribute("id=search_query_top", 'value', attribute_value)
+    kdb_driver.set_element_attribute("id=firstName", 'value', attribute_value)
     kdb_driver.screen_shot()
     # verify
-    kdb_driver.verify_element_attribute("id=search_query_top", 'value', attribute_value, timeout=3)
-    kdb_driver.verify_element_attribute("id=search_query_top", 'name', 'search_query', timeout=2)
-    kdb_driver.verify_element_attribute("id=search_query_top", 'name', 'ch_query', timeout=2, check_contains=True)
-    kdb_driver.verify_element_attribute("id=search_query_top", 'placeholder', 'Search', timeout=2)
+    kdb_driver.verify_element_attribute("id=firstName", 'value', attribute_value, timeout=3)
+    
+    kdb_driver.verify_element_attribute("id=firstName", 'placeholder', 'First Name', timeout=2)
     # get
-    autocomplete = kdb_driver.get_element_attribute("id=search_query_top", "autocomplete")
+    autocomplete = kdb_driver.get_element_attribute("id=firstName", "autocomplete")
+    assert autocomplete == 'off'
     # verify of get
-    kdb_driver.verify_element_attribute("id=search_query_top", 'autocomplete', autocomplete, timeout=2)
+    kdb_driver.verify_element_attribute("id=firstName", 'autocomplete', autocomplete, timeout=2)
     # verify before set
-    kdb_driver.verify_element_attribute("id=search_query_top", 'custom-attr', 'truc.nguyen', timeout=1, reverse=True)
+    kdb_driver.verify_element_attribute("id=firstName", 'custom-attr', 'truc.nguyen', timeout=1, reverse=True)
     # set
-    kdb_driver.set_element_attribute("id=search_query_top", 'custom-attr', 'truc.nguyen', timeout=3)
+    kdb_driver.set_element_attribute("id=firstName", 'custom-attr', 'truc.nguyen', timeout=3)
     # verify
-    kdb_driver.verify_element_attribute("id=search_query_top", 'custom-attr', 'truc.nguyen', timeout=2)
-    kdb_driver.verify_element_attribute("id=search_query_top", 'custom-attr', 'truc', timeout=2, check_contains=True)
+    kdb_driver.verify_element_attribute("id=firstName", 'custom-attr', 'truc.nguyen', timeout=2)
+    kdb_driver.verify_element_attribute("id=firstName", 'custom-attr', 'truc', timeout=2, check_contains=True)
     # get
-    custom = kdb_driver.get_element_attribute("id=search_query_top", "custom-attr")
+    custom = kdb_driver.get_element_attribute("id=firstName", "custom-attr")
     # verify of get
-    kdb_driver.verify_element_attribute("id=search_query_top", 'custom-attr', custom, timeout=2)
+    kdb_driver.verify_element_attribute("id=firstName", 'custom-attr', custom, timeout=2)
 
     # TODO out of viewport
     report.add_comment(">>> OUT OF VIEWPORT")
+    attribute_value = 'NCR'
     # verify element attribute before set attribute
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', attribute_value, reverse=True, timeout=2)
-    kdb_driver.set_element_attribute("id=newsletter-input", 'value', attribute_value)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'value', attribute_value, reverse=True, timeout=2)
+    kdb_driver.set_element_attribute("id=react-select-3-input", 'value', attribute_value)
     kdb_driver.screen_shot()
     # verify element attribute after set attribute
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', attribute_value)
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'class', 'inputNew form-control grey newsletter-input')
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'type', 'text')
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'size', '18')
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'value', attribute_value)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'type', 'text')
     # get element attribute after set attribute
-    input_value = kdb_driver.get_element_attribute("id=newsletter-input", "value")
+    input_value = kdb_driver.get_element_attribute("id=react-select-3-input", "value")
     # verify element attribute after get attribute
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', input_value)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'value', input_value)
     # verify before set
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'abc', input_value, reverse=True, timeout=2)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'abc', input_value, reverse=True, timeout=2)
     # set an element attribute
-    kdb_driver.set_element_attribute("id=newsletter-input", 'abc', "aaa")
+    kdb_driver.set_element_attribute("id=react-select-3-input", 'abc', "aaa")
     # verify
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'abc', input_value, reverse=True, timeout=2)
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'abc', 'aaa')
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'abc', 'a', check_contains=True)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'abc', input_value, reverse=True, timeout=2)
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'abc', 'aaa')
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'abc', 'a', check_contains=True)
     # get element attribute after set attribute
-    abc = kdb_driver.get_element_attribute("id=newsletter-input", "abc")
+    abc = kdb_driver.get_element_attribute("id=react-select-3-input", "abc")
     # verify
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'abc', abc, timeout=3)
-
+    kdb_driver.verify_element_attribute("id=react-select-3-input", 'abc', abc, timeout=3)
+    kdb_driver.screen_shot()
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_element_text.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_update_text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def element_text_test():
-    report.add_comment("Test get the text of element")
+def update_text_test():
+    report.add_comment("Test function update text")
     # start browser
     kdb_driver.start_browser()
-    # load url home page
-    kdb_driver.open_url('https://demoqa.com/text-box')
+    # load page for test
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
 
     # TODO in viewport
     report.add_comment(">>> IN VIEWPORT")
-    # verify element text
-    submit_btn_text = kdb_driver.get_element_text("id=submit")
-    kdb_driver.verify_string_contains(submit_btn_text, 'Submit')
+    # update text
+    kdb_driver.update_text('id=lastName', 'trucnt88')
+    # verify result
+    kdb_driver.verify_element_attribute('id=lastName', 'value', "trucnt88")
     kdb_driver.screen_shot()
-
-    # TODO out of viewport
-    report.add_comment(">>> OUT OF VIEWPORT")
-    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
-    # verify element text
-    submit_btn_text = kdb_driver.get_element_text("id=stateCity-wrapper")
-    kdb_driver.verify_string_contains(submit_btn_text, 'State and City')
+    # with slow
+    kdb_driver.update_text('id=userEmail', 'trucnt88@gmail.com', slow=True, timeout=5)
+    # verify
+    kdb_driver.verify_element_attribute('id=userEmail', 'value', 'trucnt88@gmail.com', timeout=2)
     kdb_driver.screen_shot()
+    # # with decrypt todo later
+    # kdb_driver.update_text('id=search_query_top', 'shirts slow extra', decrypt=True, timeout=5)
 
+    # TODO out of viewport
+    # report.add_comment(">>> OUT OF VIEWPORT")
+    # update text
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_execute_script.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_execute_script.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     kdb_driver.start_browser()
     # load page for test.
     kdb_driver.open_url('http://automationpractice.com/index.php')
     kdb_driver.screen_shot()
 
     # execute javascript command
     kdb_driver.execute_script(
-        "window.location = 'http://automationpractice.com/index.php?id_product=1&controller=product';")
+        "window.location = 'https://demoqa.com/automation-practice-form';")
     # verify text to confirm execute success
-    kdb_driver.verify_text_on_page('Fashion has been creating well-designed collections since 2010')
+    kdb_driver.verify_text_on_page('Student Registration Form')
     kdb_driver.screen_shot()
 
     # execute javascript command
     result = kdb_driver.execute_script("return 123;")
     # verify text to confirm execute success
     assert result == 123
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_hover.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_upload_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def hover_test():
-    report.add_comment("Hover to a web element")
+def upload_file_test():
+    # add command to the report
+    report.add_comment("Test upload_file keyword/api")
     # start browser
     kdb_driver.start_browser()
-    # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    # loads login page in the current browser session.
+    kdb_driver.open_url('https://davidwalsh.name/demo/multiple-file-upload.php')
 
-    # TODO out of viewport
-    report.add_comment(">>> OUT OF VIEWPORT")
-    # hover to web element
-    kdb_driver.hover("xpath=//*[@id='homefeatured']/li[7]/div")
-    # screen shot
-    kdb_driver.screen_shot()
-    # click to the button More
-    kdb_driver.click("xpath=//*[@id='homefeatured']/li[7]/div/div[2]/div[2]/a[2]")
-    # verify text after click
-    kdb_driver.verify_text_on_page('Printed chiffon knee length dress with tank straps. Deep v-neckline.')
-    # screen shot
+    # verify fileList before
+    kdb_driver.verify_text_on_page('No Files Selected', timeout=5)
+    # take screenshot
     kdb_driver.screen_shot()
 
-    # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    # upload single file
+    kdb_driver.upload_file('id=filesToUpload', 'Domains.txt')
 
-    # TODO in viewport
-    report.add_comment(">>> IN VIEWPORT")
-    # hover to web element
-    kdb_driver.hover("xpath=//*[@id='homefeatured']/li[1]/div", extra_time=1)
-    # screen shot
+    # verify fileList after upload single file
+    kdb_driver.verify_text_on_page('Domains.txt', timeout=5)
+    kdb_driver.verify_text_on_page('No Files Selected', reverse=True, timeout=1)
+    # take screenshot
     kdb_driver.screen_shot()
-    # verify text before click
-    kdb_driver.verify_text_on_page('Product successfully added to your shopping cart', reverse=True, timeout=2)
-    kdb_driver.verify_text_on_page('There is 1 item in your cart.', reverse=True, timeout=2)
-    # click to the Add to cart button
-    kdb_driver.click("xpath=//*[@id='homefeatured']/li[1]/div/div[2]/div[2]/a[1]")
-    # verify text after click
-    kdb_driver.verify_text_on_page('Product successfully added to your shopping cart')
-    kdb_driver.verify_text_on_page('There is 1 item in your cart.')
-    # screen shot
+
+    # upload single file
+    kdb_driver.upload_file('id=filesToUpload', 'ProductIDs.txt', timeout=2)
+
+    # verify fileList after upload single file
+    kdb_driver.verify_text_on_page('ProductIDs.txt', timeout=5)
+    kdb_driver.verify_text_on_page('Domains.txt', reverse=True, timeout=0)
+    kdb_driver.verify_text_on_page('No Files Selected', reverse=True, timeout=0)
+    # take screenshot
     kdb_driver.screen_shot()
 
+    # negative cases
+    try:
+        # not support multiple files
+        # the file_path is only accept str
+        kdb_driver.upload_file('id=filesToUpload', ('Domains.txt', 'ProductIDs.txt'), log=False)
+        assert False
+    except:
+        assert True
+    #
+    try:
+        # raise exception if file path is not exist
+        kdb_driver.upload_file('id=filesToUpload', 'file_not_found.txt', log=False)
+        assert False
+    except:
+        assert True
+
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_is_display.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_is_display.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from kdb import report
+from kdb.unit_test.pc import hidden_ads
 from kdb.webdriver import kdb_driver
 
 
 def is_display_test():
     report.add_comment("Test is display")
     # start browser
     kdb_driver.start_browser()
     # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
+    hidden_ads()
 
     # TODO element is NOT displayed
     # verify an element is not display
     is_displayed = kdb_driver.is_displayed("xpath=//*[@id='homefeatured']/li[1]/div/div[2]/div[2]/a[2]", reverse=True,
                                            timeout=5)
     assert is_displayed is True
     is_displayed = kdb_driver.is_displayed("xpath=//*[@id='homefeatured']/li[1]/div/div[2]/div[2]/a[2]", timeout=3)
     assert is_displayed is False
     # take screenshot
     kdb_driver.screen_shot()
 
     # TODO element is displayed
-    # hover to web element
-    kdb_driver.hover("xpath=//*[@id='homefeatured']/li[1]/div")
     # check a web element is display
-    is_displayed = kdb_driver.is_displayed("xpath=//*[@id='homefeatured']/li[1]/div/div[2]/div[2]/a[2]")
+    is_displayed = kdb_driver.is_displayed("id=state")
     assert is_displayed is True
-    is_displayed = kdb_driver.is_displayed("xpath=//*[@id='homefeatured']/li[1]/div/div[2]/div[2]/a[2]", timeout=3,
-                                           reverse=True)
+    is_displayed = kdb_driver.is_displayed("id=submit", timeout=3, reverse=True)
     assert is_displayed is False
 
     # TODO element not exists
     is_displayed = kdb_driver.is_displayed("id=not-exist", timeout=3)
     assert is_displayed is False
     is_displayed = kdb_driver.is_displayed("id=not-exist", timeout=3, reverse=True)
     assert is_displayed is True
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_open_url.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_browser_navigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from kdb import report
+from kdb.unit_test.pc import hidden_ads
 from kdb.webdriver import kdb_driver
 
 
-def open_url_test():
-    report.add_comment("Open url http://automationpractice.com/index.php")
+def test_browser_nav():
+    # start browser
+    report.add_comment("Test browser navigation")
     # start browser
     kdb_driver.start_browser()
+    # load page for test.
+    kdb_driver.open_url('https://demoqa.com/books')
+    hidden_ads()
 
-    # load page
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-    # verify title
-    kdb_driver.verify_title("My Store")
+    kdb_driver.click("xpath=//a[@href='/books?book=9781449325862']")
+    kdb_driver.verify_text_on_page("9781449325862")
+    kdb_driver.verify_text_on_page("Back To Book Store")
+    kdb_driver.verify_url_contains("/books?book=9781449325862")
     kdb_driver.screen_shot()
-
-    # load page
-    kdb_driver.open_url('http://automationpractice.com/index.php?controller=contact')
-    # verify title
-    kdb_driver.verify_title("Contact us - My Store")
+    kdb_driver.back()
+    kdb_driver.verify_url_contains("https://demoqa.com/books")
+    kdb_driver.screen_shot()
+    kdb_driver.forward()
+    kdb_driver.verify_text_on_page("Back To Book Store")
     kdb_driver.screen_shot()
 
-    # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_press_keys.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_press_keys.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+from selenium.webdriver import Keys
+
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
 def press_keys_test():
     report.add_comment("Test press keys keyword/api")
     # start browser
     kdb_driver.start_browser()
     # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-    # focus to input search
-    kdb_driver.click('id=search_query_top')
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
+
+    # focus to input
+    kdb_driver.click('id=lastName')
     # input search
-    kdb_driver.press_keys('shirts')
-    # take screenshot
-    kdb_driver.screen_shot()
+    kdb_driver.press_keys('trucnt88')
     # press enter
     kdb_driver.press_keys(kdb_driver.keys.ENTER)
-    # verify shirts show on page
-    kdb_driver.verify_text_on_page('"shirts"')
     # take screenshot
     kdb_driver.screen_shot()
+    # verify result
+    kdb_driver.verify_element_attribute('id=lastName', 'value', "trucnt88")
 
     # copy value in input search
-    kdb_driver.press_keys((kdb_driver.keys.CONTROL, 'a'), 'id=search_query_top', timeout=10)
+    kdb_driver.press_keys((kdb_driver.keys.CONTROL, 'a'), 'id=lastName', timeout=10)
     kdb_driver.press_keys((kdb_driver.keys.CONTROL, 'c'))
-    # paste value to newsletter
-    kdb_driver.press_keys((kdb_driver.keys.CONTROL, 'v'), 'id=newsletter-input')
+    # paste value to email
+    kdb_driver.press_keys((kdb_driver.keys.CONTROL, 'v'), 'id=userEmail')
+    # take screenshot
+    kdb_driver.screen_shot()
     # press enter
     kdb_driver.press_keys(kdb_driver.keys.ENTER)
-    # verify text on page
-    kdb_driver.verify_text_on_page("Newsletter : Invalid email address.")
+    # verify result
+    kdb_driver.verify_element_attribute('id=userEmail', 'value', "trucnt88")
 
     # input search
-    kdb_driver.press_keys('TRUC_NGUYEN', 'id=search_query_top')
+    kdb_driver.press_keys('TRUC_NGUYEN', 'id=firstName')
     # press keys
     kdb_driver.press_keys(kdb_driver.keys.LEFT)
     kdb_driver.press_keys(kdb_driver.keys.ARROW_LEFT)
     kdb_driver.press_keys(kdb_driver.keys.NUMPAD0)
     kdb_driver.press_keys(kdb_driver.keys.NUMPAD1)
     kdb_driver.press_keys(kdb_driver.keys.NUMPAD2)
     kdb_driver.press_keys(kdb_driver.keys.NUMPAD3)
@@ -63,29 +66,24 @@
     kdb_driver.press_keys(kdb_driver.keys.ADD)
     kdb_driver.press_keys(kdb_driver.keys.SEPARATOR)
     kdb_driver.press_keys(kdb_driver.keys.SUBTRACT)
     kdb_driver.press_keys(kdb_driver.keys.DECIMAL)
     kdb_driver.press_keys(kdb_driver.keys.DIVIDE)
 
     kdb_driver.press_keys(kdb_driver.keys.ENTER)
-    # verify text on page
-    kdb_driver.verify_text_on_page("T;=R UNGUY0123456789N*+,-./")
-    # verify url after search
-    kdb_driver.verify_url_contains("T%3B%3DR+UNGUY0123456789N*%2B%2C-.%2F")
+    # verify result
+    kdb_driver.verify_element_attribute('id=firstName', 'value', "T;=R UNGUY0123456789N*+,-./")
     kdb_driver.screen_shot()
 
     # focus to input search
-    kdb_driver.click('id=search_query_top')
+    kdb_driver.click('id=firstName')
     # focus to Cart
     kdb_driver.press_keys(kdb_driver.keys.TAB)
     kdb_driver.press_keys(kdb_driver.keys.TAB)
     # press enter
-    kdb_driver.press_keys(kdb_driver.keys.ENTER)
-    kdb_driver.screen_shot()
-    # verify url of shopping cart page
-    kdb_driver.verify_url_contains("controller=order")
-    # verify text on page
-    kdb_driver.verify_text_on_page("Your shopping cart is empty.")
+    kdb_driver.press_keys("trucnt88@gmail.com")
     kdb_driver.screen_shot()
+    # verify result
+    kdb_driver.verify_element_attribute('id=userEmail', 'value', "trucnt88@gmail.com")
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_press_keys_and_click.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_click.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+import time
+
+import kdb
 from kdb import report
-from kdb.webdriver import kdb_driver
+from kdb.unit_test.pc import hidden_ads
+from kdb.webdriver import kdb_driver, webdriver_generator
 
 
-def press_keys_and_click_test():
-    report.add_comment("Test press keys and click keyword/api")
+def click_test():
+    report.add_comment("Test click")
     # start browser
     kdb_driver.start_browser()
-    # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
-    # verify curent title
-    kdb_driver.verify_title("My Store")
-    # take screenshot
-    kdb_driver.screen_shot()
-    # Ctrl + click to "Contact us" link
-    kdb_driver.press_keys_and_click(kdb_driver.keys.CONTROL, 'id=contact-link', timeout=5)
-
-    # switch to the tab which open in above step
-    kdb_driver.windows.next()
-    # verify curent title
-    kdb_driver.verify_title("Contact us - My Store")
-    # take screenshot
+    # load page for test.
+    kdb_driver.open_url('https://demoqa.com/buttons')
+    hidden_ads()
+
+    # TODO click an element in viewport
+    report.add_comment(">>> IN VIEWPORT")
+    kdb_driver.verify_text_on_page('You have done a dynamic click', reverse=True, timeout=3)
     kdb_driver.screen_shot()
-    # Ctrl + click to "Sign in" link
-    kdb_driver.press_keys_and_click(kdb_driver.keys.CONTROL, 'xpath=//*[@class="login"]', extra_time=2)
-
-    # switch to the tab which open in above step
-    kdb_driver.windows.next()
-    # verify curent title
-    kdb_driver.verify_title("Login - My Store")
-    # take screenshot
+    # click to the "Click Me" button
+    kdb_driver.click("xpath=//button[text()='Click Me']")
+    # verify text to confirm click success
+    kdb_driver.verify_text_on_page('You have done a dynamic click')
     kdb_driver.screen_shot()
 
-    # Ctrl + click to invalid element
-    try:
-        kdb_driver.press_keys_and_click(kdb_driver.keys.CONTROL, 'xpath=//*[@class="invalid-locator"]', timeout=1,
-                                        log=False)
-        assert False
-    except:
-        assert True
+    # TODO click an element out of viewport
+    # report.add_comment(">>> OUT OF VIEWPORT")
+    # # load home page
+    # kdb_driver.open_url('http://automationpractice.com/index.php')
+    # # click to the "submitNewsletter" button
+    # kdb_driver.click("xpath=//button[@name='submitNewsletter']", timeout=5)
+    # # verify text to confirm click success
+    # kdb_driver.verify_text_on_page('Newsletter : Invalid email address.')
+    # kdb_driver.screen_shot()
+
+    # TODO click an element in iframe
+    # report.add_comment(">>> IN IFRAME")
+    # if kdb.BROWSER.lower() in webdriver_generator._FIREFOX_ALIAS:
+    #     time.sleep(5)
+    # # click the "PrestaShop" link inside iframe
+    # kdb_driver.click("xpath=//a[contains(@class, '_3-8_ lfloat')]", extra_time=1)
+    # # switch to fb window
+    # kdb_driver.windows.next()
+    # # verify text to confirm click success
+    # kdb_driver.verify_url_contains('facebook.com/prestashop')
+    # kdb_driver.screen_shot()
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_start_browser.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_start_browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,24 @@
         }
     })
     """
 
 
 def start_browser_test():
     report.add_comment("Start browser testing")
+    kdb.BROWSER = 'ed'
 
     # TODO start browser with default params
     report.add_comment(">>> Start browser with default parameters")
     kdb_driver.start_browser()
     # load page for test
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    kdb_driver.open_url('https://www.google.com/')
     if kdb.BROWSER.lower() in webdriver_generator._CHROME_ALIAS:
         # verify Chrome started as default
-        assert kdb_driver.execute_script("return !!window.chrome && !!window.chrome.webstore;") is True
+        assert kdb_driver.execute_script("return !!window.chrome;") is True
     elif kdb.BROWSER.lower() in webdriver_generator._FIREFOX_ALIAS:
         # verify Firefox started as default
         assert kdb_driver.execute_script("return typeof InstallTrigger !== 'undefined';") is True
     elif kdb.BROWSER.lower() in webdriver_generator._IE_ALIAS:
         # verify IE started as default
         assert kdb_driver.execute_script("return /*@cc_on!@*/false || !!document.documentMode;") is True
     kdb_driver.close_browser()
@@ -68,15 +69,22 @@
     report.add_comment(">>> Start browser with a given name")
     # chrome
     if kdb.BROWSER.lower() in webdriver_generator._CHROME_ALIAS:
         kdb_driver.start_browser('chrome')
         # load page for test
         kdb_driver.open_url('https://www.google.com/')
         # verify Chrome started as default
-        assert kdb_driver.execute_script("return !!window.chrome && !!window.chrome.webstore;") is True
+        assert kdb_driver.execute_script("return !!window.chrome;") is True
+    # ms edge
+    elif kdb.BROWSER.lower() in webdriver_generator._EDGE_ALIAS:
+        kdb_driver.start_browser('edge')
+        # load page for test
+        kdb_driver.open_url('https://www.google.com/')
+        # verify Chrome started as default
+        assert kdb_driver.execute_script('return window.navigator.userAgent.indexOf("Edg") > -1;') is True
     # firefox
     elif kdb.BROWSER.lower() in webdriver_generator._FIREFOX_ALIAS:
         kdb_driver.start_browser('firefox')
         # load page for test
         kdb_driver.open_url('https://www.google.com/')
         # verify Chrome started as default
         assert kdb_driver.execute_script("return typeof InstallTrigger !== 'undefined';") is True
@@ -89,18 +97,19 @@
         assert kdb_driver.execute_script("return /*@cc_on!@*/false || !!document.documentMode;") is True
     # close browser
     kdb_driver.close_browser()
 
     # TODO start browser with proxy
     report.add_comment(">>> Start browser with proxy")
     # fr proxy
+    # https://free-proxy-list.net/
     kdb_driver.start_browser(proxy_name='fr')
     # loads login page in the current browser session.
     kdb_driver.open_url('https://www.google.com/')
-    kdb_driver.verify_text_on_page("France")
+    kdb_driver.verify_text_on_page("Français")
     kdb_driver.screen_shot()
     kdb_driver.close_browser()
     # br proxy
     kdb_driver.start_browser(proxy_name='br')
     # loads login page in the current browser session.
     kdb_driver.open_url('https://www.google.com/')
     kdb_driver.verify_text_on_page("Brasil")
@@ -141,14 +150,14 @@
 
     # TODO start browser with proxy and private_mode
     report.add_comment(">>> Start browser with proxy and private_mode")
     kdb_driver.start_browser(proxy_name='fr', private_mode=True)
     # loads login page in the current browser session.
     kdb_driver.open_url('https://www.google.com/')
     # verify proxy
-    kdb_driver.verify_text_on_page("France")
+    kdb_driver.verify_text_on_page("France", timeout=3)
     # verify private mode
     kdb_driver.execute_script(script_verify_private_mode)
     kdb_driver.verify_element_attribute("id=lst-ib", 'value', 'true', timeout=5)
     kdb_driver.screen_shot()
     # close browser
     kdb_driver.close_browser()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_upload_file.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_press_keys_and_click.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,33 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def upload_file_test():
-    # add command to the report
-    report.add_comment("Test upload_file keyword/api")
+def press_keys_and_click_test():
+    report.add_comment("Test press keys and click keyword/api")
     # start browser
     kdb_driver.start_browser()
-    # loads login page in the current browser session.
-    kdb_driver.open_url('https://davidwalsh.name/demo/multiple-file-upload.php')
-
-    # verify fileList before
-    kdb_driver.verify_text_on_page('No Files Selected', timeout=5)
-    # take screenshot
-    kdb_driver.screen_shot()
-
-    # upload single file
-    kdb_driver.upload_file('id=filesToUpload', 'Domains.txt')
-
-    # verify fileList after upload single file
-    kdb_driver.verify_text_on_page('Domains.txt', timeout=5)
-    kdb_driver.verify_text_on_page('No Files Selected', reverse=True, timeout=1)
+    # load page for test
+    kdb_driver.open_url('https://demoqa.com/books')
     # take screenshot
     kdb_driver.screen_shot()
+    # Ctrl + click to "Contact us" link
+    kdb_driver.press_keys_and_click(kdb_driver.keys.CONTROL, "xpath=//a[@href='/books?book=9781449325862']", timeout=5)
 
-    # upload single file
-    kdb_driver.upload_file('id=filesToUpload', 'ProductIDs.txt', timeout=2)
-
-    # verify fileList after upload single file
-    kdb_driver.verify_text_on_page('ProductIDs.txt', timeout=5)
-    kdb_driver.verify_text_on_page('Domains.txt', reverse=True, timeout=0)
-    kdb_driver.verify_text_on_page('No Files Selected', reverse=True, timeout=0)
+    # switch to the tab which open in above step
+    kdb_driver.windows.next()
+    # verify
+    kdb_driver.verify_text_on_page("9781449325862")
+    kdb_driver.verify_text_on_page("Back To Book Store")
     # take screenshot
     kdb_driver.screen_shot()
 
-    # negative cases
-    try:
-        # not support multiple files
-        # the file_path is only accept str
-        kdb_driver.upload_file('id=filesToUpload', ('Domains.txt', 'ProductIDs.txt'), log=False)
-        assert False
-    except:
-        assert True
-    #
+    # Ctrl + click to invalid element
     try:
-        # raise exception if file path is not exist
-        kdb_driver.upload_file('id=filesToUpload', 'file_not_found.txt', log=False)
+        kdb_driver.press_keys_and_click(kdb_driver.keys.CONTROL, 'xpath=//*[@class="invalid-locator"]', timeout=1,
+                                        log=False)
         assert False
     except:
         assert True
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_verify_element_attribute.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_verify_element_attribute.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,18 +5,25 @@
 
 def test_verify_element_attribute():
     # start browser
     report.add_comment("Test get attribute element")
     kdb_driver.start_browser(kdb.BROWSER)
     # load url home page
     kdb_driver.open_url('http://automationpractice.com/index.php')
-    kdb_driver.set_element_attribute("id=newsletter-input", 'value', "text for set attribute")
+    kdb_driver.verify_element_attribute("id=dynamicProviderLink", 'title', "webmaster@automationpractice.com")
+    kdb_driver.verify_element_attribute("id=dynamicProviderLink", 'title', "trucnt88@gmail.com", reverse=True,
+                                        timeout=2)
     kdb_driver.screen_shot()
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', "text for set attribute")
-    input_value = kdb_driver.get_element_attribute("id=newsletter-input", "value")
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', input_value, extra_time=5)
 
-    kdb_driver.set_element_attribute("id=newsletter-input", 'value', "text for set attribute set again")
+    #
+    kdb_driver.open_url('https://demoqa.com/automation-practice-form')
+    kdb_driver.set_element_attribute("id=firstName", 'value', "trucnt88")
     kdb_driver.screen_shot()
-    kdb_driver.verify_element_attribute("id=newsletter-input", 'value', input_value, reverse=True, timeout=5)
+    kdb_driver.verify_element_attribute("id=firstName", 'value', "trucnt88")
+    input_value = kdb_driver.get_element_attribute("id=firstName", "value")
+    kdb_driver.verify_element_attribute("id=firstName", 'value', input_value)
+
+    kdb_driver.set_element_attribute("id=firstName", 'value', "text for set attribute set again")
+    kdb_driver.screen_shot()
+    kdb_driver.verify_element_attribute("id=firstName", 'value', input_value, reverse=True, timeout=5)
 
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_verify_text_on_page.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_hover.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 from kdb import report
 from kdb.webdriver import kdb_driver
 
 
-def verify_text_on_page_test():
-    report.add_comment("Test verify text on page")
+def hover_test():
+    report.add_comment("Hover to a web element")
     # start browser
     kdb_driver.start_browser()
-    # loads login page in the current browser session.
-    kdb_driver.open_url('http://automationpractice.com/index.php')
+    # load page for test
+    kdb_driver.open_url('https://www.toolsqa.com/selenium-training/')
 
-    # verify text is displayed on web page
-    kdb_driver.verify_text_on_page('Best Sellers')
-    # verify text not displayed in web page
-    kdb_driver.verify_text_on_page('This text not in page', reverse=True, timeout=2)
-    # verify hidden text
-    kdb_driver.verify_text_on_page('Product successfully added to your shopping cart', reverse=True, timeout=2)
-    # verify text inside frame
-    kdb_driver.verify_text_on_page('Be the first of your friends to like this')
+    # TODO in of viewport
+    report.add_comment(">>> IN OF VIEWPORT")
+    # hover to web element
+    kdb_driver.click("xpath=//a[@class='navbar__tutorial-menu']")
+    kdb_driver.verify_text_on_page("Appium Studio", reverse=True, timeout=2)
+    mobile_test_locator = "xpath=//nav[@class='mega-menu']//descendant::div/ul/li[4]"
+    kdb_driver.hover(mobile_test_locator)
+    # screen shot
+    kdb_driver.screen_shot()
+    kdb_driver.verify_text_on_page("Appium Studio")
+    kdb_driver.verify_element_attribute(mobile_test_locator, "class", "active")
+
+    #
+    kdb_driver.verify_text_on_page("JMeter", reverse=True, timeout=2)
+    non_function_test_locator = "xpath=//nav[@class='mega-menu']//descendant::div/ul/li[8]"
+    kdb_driver.hover(non_function_test_locator)
+    # screen shot
+    kdb_driver.screen_shot()
+    kdb_driver.verify_text_on_page("JMeter")
+    kdb_driver.verify_element_attribute(non_function_test_locator, "class", "active")
+
+    # TODO out viewport
+    # report.add_comment(">>> OUT VIEWPORT")
 
     # close browser
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_verify_title.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_verify_title.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 def verify_title_test():
     report.add_comment("Test verify title")
     # start browser
     kdb_driver.start_browser()
     # loads page
     kdb_driver.open_url('http://automationpractice.com/index.php')
-    # Verify title is My Store
-    kdb_driver.verify_title('My Store')
+    # Verify title is Account Suspended
+    kdb_driver.verify_title('Account Suspended')
     # Verify title is not Women - My Store
     kdb_driver.verify_title('Women - My Store', reverse=True, timeout=2)
     kdb_driver.screen_shot()
-    # click to the button WOMEN
-    kdb_driver.click("xpath=//*[@id='block_top_menu']/ul/li[1]/a")
-    # Verify title is Women - My Store
-    kdb_driver.verify_title('Women - My Store')
+
+    #
+    kdb_driver.open_url("https://demoqa.com/books?book=9781449325862")
+    # Verify title is DEMOQA
+    kdb_driver.verify_title('DEMOQA')
     # Verify title is not My Store
-    kdb_driver.verify_title('My Store', reverse=True, timeout=2)
+    kdb_driver.verify_title('Account Suspended', reverse=True, timeout=2)
     kdb_driver.screen_shot()
     kdb_driver.close_browser()
```

### Comparing `kdb-python-0.0.5/kdb/unit_test/pc/test_video.py` & `kdb-python-0.0.6/kdb/unit_test/pc/test_video.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/actions/__init__.py` & `kdb-python-0.0.6/kdb/webdriver/actions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.wait import WebDriverWait
 
 from kdb.common.encrypt_decrypt import EncryptDecrypt
 from kdb.common.utils import TimeUtil, WebDriverUtil, FileUtil
 from kdb.webdriver.actions.mobile_gestures import swipe, Direction, scroll_to_element, scroll_to_top
-from kdb.webdriver.keys import KEYS_MAPPING, is_special_key, is_modifier_key
+from kdb.webdriver.keys import KEYS_MAPPING, is_special_key, is_modifier_key, Keys
 
 #
 NOT_FOUND_ELEMENT = '<<NOT_FOUND_ELEMENT>>'
 
 # locators prefix
 LOCATOR_ID_PREFIX = "id="
 LOCATOR_XPATH_PREFIX = "xpath="
@@ -256,25 +256,38 @@
 
 def check(driver, element, extra_time):
     """
     Check ON action
     """
     TimeUtil.sleep(extra_time)
     if not element.is_selected():
-        element.click()
+        # element.click()
+        _click_element_include_hidden(element)
     return True
 
 
+def _click_element_include_hidden(element):
+    """
+    Click on its parent element if it hidden, otherwise, click on it
+    """
+    if element.is_displayed() and element.is_enabled():
+        element.click()
+    else:
+        # click on parent of element if it hidden
+        element.find_element(By.XPATH, "./..").click()
+
+
 def uncheck(driver, element, extra_time):
     """
     Check OFF action
     """
     TimeUtil.sleep(extra_time)
     if element.is_selected():
-        element.click()
+        # element.click()
+        _click_element_include_hidden(element)
     return True
 
 
 def verify_state(driver, element, checked, extra_time):
     """
     Returns whether the element is selected.
 
@@ -475,31 +488,42 @@
             time.sleep(1)
         elif WebDriverUtil.is_mobile_app(driver):
             swipe(driver, direction=Direction.DOWN)
         else:
             time.sleep(0.5)
 
 
+def _get_key(key):
+    """
+    Get selenium's keys
+    @param:
+        key: kdb.webdriver.Keys
+    """
+    if Keys.CONTROL == key or Keys.COMMAND == key:
+        key = Keys.get_cmd_ctrl_key()
+    return KEYS_MAPPING.get(key)
+
+
 def press_keys(driver, element, keys, extra_time, slow=False):
     """
     Press keys on keyboard
     """
     TimeUtil.sleep(extra_time)
     # press keys to an element
     if element is not None:
         convert_keys = ()
         if isinstance(keys, tuple):
             for k in keys:
                 if is_special_key(k):
-                    convert_keys += (KEYS_MAPPING.get(k),)
+                    convert_keys += (_get_key(k),)
                 else:
                     convert_keys += (k,)
         else:
             if is_special_key(keys):
-                convert_keys = KEYS_MAPPING.get(keys)
+                convert_keys = _get_key(keys)
             else:
                 convert_keys = keys
         if slow:
             for key in keys:
                 element.send_keys(key)
                 time.sleep(1)
         else:
@@ -509,31 +533,32 @@
         actions = ActionChains(driver)
         # perform combination keys
         if isinstance(keys, tuple):
             # perform key_down, click actions and send keys
             for k in keys:
                 # send key down
                 if is_modifier_key(k):
-                    actions.key_down(KEYS_MAPPING.get(k))
+                    actions.key_down(_get_key(k))
                 # send special keys to an element
                 elif is_special_key(k):
-                    actions.send_keys(KEYS_MAPPING.get(k))
+                    actions.send_keys(_get_key(k))
                 # send keys as a string to an element
                 else:
                     actions.send_keys(k)
             # perform key_up
             for k in keys:
                 if is_modifier_key(k):
-                    actions.key_up(KEYS_MAPPING.get(k))
+                    actions.key_up(_get_key(k))
             actions.perform()
         # send keys as a string or a special key
         elif isinstance(keys, str):
             # send special key
             if is_special_key(keys):
-                actions.send_keys(KEYS_MAPPING.get(keys))
+                actions.send_keys(_get_key(keys))
+                actions.perform()
             # send keys as a string
             else:
                 if slow:
                     for key in keys:
                         actions = ActionChains(driver)
                         actions.send_keys(key)
                         actions.perform()
@@ -558,43 +583,43 @@
     actions = ActionChains(driver)
     # perform combination keys
     if isinstance(keys, tuple):
         # perform key_down, click actions and send keys
         for k in keys:
             # send key down
             if is_modifier_key(k):
-                actions.key_down(KEYS_MAPPING.get(k))
+                actions.key_down(_get_key(k))
             # send special keys to an element
             elif is_special_key(k):
-                actions.send_keys_to_element(element, KEYS_MAPPING.get(k))
+                actions.send_keys_to_element(element, _get_key(k))
             # send keys as a string to an element
             else:
                 actions.send_keys_to_element(element, k)
         # click
         actions.click(element)
         # perform key_up
         for k in keys:
             if is_modifier_key(k):
-                actions.key_up(KEYS_MAPPING.get(k))
+                actions.key_up(_get_key(k))
     # send keys as a string
     elif isinstance(keys, str):
         # send key down
         if is_modifier_key(keys):
-            actions.key_down(KEYS_MAPPING.get(keys))
+            actions.key_down(_get_key(keys))
         # send special keys to an element
         elif is_special_key(keys):
-            actions.send_keys_to_element(element, KEYS_MAPPING.get(keys))
+            actions.send_keys_to_element(element, _get_key(keys))
         # send keys as a string to an element
         else:
             actions.send_keys_to_element(element, keys)
         # click
         actions.click(element)
         # perform key_up
         if is_modifier_key(keys):
-            actions.key_up(KEYS_MAPPING.get(keys))
+            actions.key_up(_get_key(keys))
     # raise exception if keys is not string and not tuple
     else:
         raise InvalidArgumentException("The keys (%s) must be string or tuple" % str(keys))
     actions.perform()
     return True
```

### Comparing `kdb-python-0.0.5/kdb/webdriver/actions/alert.py` & `kdb-python-0.0.6/kdb/webdriver/actions/alert.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/actions/cookies.py` & `kdb-python-0.0.6/kdb/webdriver/actions/cookies.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/actions/mobile_gestures.py` & `kdb-python-0.0.6/kdb/webdriver/actions/mobile_gestures.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/actions/video.py` & `kdb-python-0.0.6/kdb/webdriver/actions/video.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/alert.py` & `kdb-python-0.0.6/kdb/webdriver/alert.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/common.py` & `kdb-python-0.0.6/kdb/webdriver/common.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/cookies.py` & `kdb-python-0.0.6/kdb/webdriver/cookies.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/files.py` & `kdb-python-0.0.6/kdb/webdriver/files.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/json_path.py` & `kdb-python-0.0.6/kdb/webdriver/json_path.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/kdb_webdriver.py` & `kdb-python-0.0.6/kdb/webdriver/kdb_webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
                                            reverse)
             report_passed_test_step(self.is_displayed.__name__, args_passed, start_time,
                                     "Result is %s." % str(is_displayed))
             return is_displayed
         except NoSuchElementException:
             if reverse is True:
                 report_passed_test_step(self.is_displayed.__name__, args_passed, start_time,
-                                        "Element was not displayed.")
+                                        "Element was displayed.")
                 return True
             else:
                 warn_msg = "The element(%s) is not found."
                 report_warning_test_step(self.is_displayed.__name__, args_passed, start_time, warn_msg % locator)
                 return False
         except Exception as ex:
             report_failed_test_step(self._driver, self.is_displayed.__name__, args_passed, start_time, str(ex))
```

### Comparing `kdb-python-0.0.5/kdb/webdriver/kdb_webelement.py` & `kdb-python-0.0.6/kdb/webdriver/kdb_webelement.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/keys.py` & `kdb-python-0.0.6/kdb/webdriver/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from selenium.webdriver.common.keys import Keys as SeleniumKeys
 
+from kdb.common.utils import OS
+
 
 class Keys:
     """
     Set of special keys.
     """
 
     NULL = '<keys.NULL>'
@@ -70,14 +72,18 @@
     F10 = '<keys.F10>'
     F11 = '<keys.F11>'
     F12 = '<keys.F12>'
 
     META = '<keys.META>'
     COMMAND = '<keys.COMMAND>'
 
+    @staticmethod
+    def get_cmd_ctrl_key():
+        return Keys.COMMAND if OS.is_mac_platform() else Keys.CONTROL
+
 
 MODIFIER_KEYS = (
     Keys.SHIFT,
     Keys.LEFT_SHIFT,
     Keys.CONTROL,
     Keys.LEFT_CONTROL,
     Keys.ALT,
```

### Comparing `kdb-python-0.0.5/kdb/webdriver/mobile_gestures.py` & `kdb-python-0.0.6/kdb/webdriver/mobile_gestures.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/random.py` & `kdb-python-0.0.6/kdb/webdriver/random.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/requests.py` & `kdb-python-0.0.6/kdb/webdriver/requests.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/video.py` & `kdb-python-0.0.6/kdb/webdriver/video.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/videoelement.py` & `kdb-python-0.0.6/kdb/webdriver/videoelement.py`

 * *Files identical despite different names*

### Comparing `kdb-python-0.0.5/kdb/webdriver/webdriver_generator.py` & `kdb-python-0.0.6/kdb/webdriver/webdriver_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,167 @@
+import json
 import logging
 import os
 import random
 import time
 
 from appium import webdriver
 # Options are only available since client version 2.3.0
 # If you use an older client then switch to desired_capabilities
 # instead: https://github.com/appium/python-client/pull/720
 from appium.options.android import UiAutomator2Options
 from appium.options.ios import XCUITestOptions
 from selenium.common.exceptions import InvalidArgumentException, TimeoutException
 from selenium.webdriver import Proxy
 from selenium.webdriver.chrome.options import Options as ChromeOptions
-from selenium.webdriver.chrome.webdriver import WebDriver as ChromeDriver
 from selenium.webdriver.chrome.service import Service as ChromeService
+from selenium.webdriver.chrome.webdriver import WebDriver as ChromeDriver
+from selenium.webdriver.common.proxy import ProxyType
+from selenium.webdriver.edge.options import Options as EdgeOptions
+from selenium.webdriver.edge.service import Service as EdgeService
+from selenium.webdriver.edge.webdriver import WebDriver as EdgeDriver
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
+from selenium.webdriver.firefox.service import Service as FirefoxService
 from selenium.webdriver.firefox.webdriver import WebDriver as FirefoxDriver
 from selenium.webdriver.ie.options import Options as IEOptions, ElementScrollBehavior
+from selenium.webdriver.ie.service import Service as IEService
 from selenium.webdriver.ie.webdriver import WebDriver as IEDriver
+# https://github.com/SergeyPirogov/webdriver_manager
+from webdriver_manager.chrome import ChromeDriverManager
+from webdriver_manager.firefox import GeckoDriverManager
+from webdriver_manager.microsoft import EdgeChromiumDriverManager, IEDriverManager
 
 import kdb
 from kdb import FolderSettings
 from kdb.common.config_parser import ConfigParser
 from kdb.common.constants import ErrorMessage
 from kdb.common.mobile_manager import MobileManager, get_device_info
 from kdb.common.utils import DeviceType, WebDriverUtil, OS, CommandLine, FileUtil
-from kdb.config import proxy_list
-from kdb.config.settings import ChromeSettings, FirefoxSettings, DriverSettings, IESettings
+from kdb.config.settings import ChromeSettings, FirefoxSettings, DriverSettings, IESettings, EdgeSettings
 
 
-def _create_proxy(proxy_name):
+def _get_proxy(proxy_name):
+    """
+    get a proxy from config
+    """
+    with open(os.path.join(FolderSettings.CONFIG_DIR, 'proxies.json')) as proxies_file:
+        data = json.load(proxies_file)
+    if not proxy_name or not data or not data['proxies'][str(proxy_name).lower()]:
+        raise Exception("No proxy is found for %s." % proxy_name)
+    return data['proxies'][str(proxy_name).lower()]
+
+
+def _create_proxy(proxy_name) -> Proxy:
     """
     create a Proxy from config
     """
     # get a proxy from config
-    proxy_config = proxy_list.PROXYS.get(str(proxy_name).lower())
-    if proxy_name is None or proxy_config is None:
-        raise Exception("No proxy is found for %s" % proxy_name)
+    proxy_config = _get_proxy(proxy_name)
+    # if proxy_name is None or proxy_config is None:
+    #     raise Exception("No proxy is found for %s" % proxy_name)
 
     host = proxy_config.get('proxy')
-    proxy = {'proxyType': 'manual', 'ftpProxy': host, 'httpProxy': host, 'sslProxy': host}
+    proxy = {'proxyType': ProxyType.MANUAL, 'httpProxy': host, 'sslProxy': host}
 
-    if proxy_config.get('username') is not None and proxy_config.get('password') is not None:
+    if proxy_config.get('noProxy'):
+        proxy['noProxy'] = proxy_config.get('noProxy')
+    if proxy_config.get('username') and proxy_config.get('password'):
         proxy['socksProxy'] = host
-        proxy['username'] = proxy_config.get('username')
-        proxy['password'] = proxy_config.get('password')
+        proxy['socksUsername'] = proxy_config.get('username')
+        proxy['socksPassword'] = proxy_config.get('password')
 
     return Proxy(proxy)
 
 
 _CHROME_ALIAS = {"ch", "chrome"}
+_EDGE_ALIAS = {"ed", "edge", "msedge"}
 _FIREFOX_ALIAS = {"ff", "firefox"}
 _IE_ALIAS = {"ie", "internetexplorer"}
 
 
 def _create_chrome_driver(proxy_name=None, private_mode=False):
     # 1. create chromeOption
     chrome_options = ChromeOptions()
     # 2. set ChromeOption attribute from config (e.g. proxy, --maximize, etc)
     chrome_options.add_argument('start-maximized')
+    # bypass the message "your connection is not private" on non-secure page
+    chrome_options.add_argument('--ignore-ssl-errors=yes')
+    chrome_options.add_argument('--ignore-certificate-errors')
     # chrome_options.add_argument("--start-maximized")
     # chrome_options.add_argument('headless')
     if private_mode:
         chrome_options.add_argument('incognito')
     # 3. add proxy
-    if proxy_name is not None:
-        proxy = _create_proxy(proxy_name)  # todo proxy sẽ dc set ở ChromeOption
+    if proxy_name:
+        # https://www.zenrows.com/blog/selenium-proxy#how-to-set-selenium-proxy
+        # proxy = _get_proxy(proxy_name)
+        # chrome_options.add_argument(f'--proxy-server={proxy}')
+        proxy: Proxy = _create_proxy(proxy_name)
+        chrome_options.proxy = proxy
+        #
+        # chrome_options.add_argument('--proxy-server=%s' % '173.192.21.89:80')
     # 4. create ChromeService
-    service = ChromeService(executable_path=ChromeSettings.DRIVER_PATH,
-                            log_output=os.path.join(FolderSettings.LOG_DIR, ChromeSettings.DRIVER_NAME + ".log"))
+    service = ChromeService(
+        # executable_path=ChromeSettings.DRIVER_PATH,
+        executable_path=ChromeDriverManager().install(),
+        log_output=os.path.join(FolderSettings.LOG_DIR, ChromeSettings.DRIVER_NAME + ".log"))
     # 5. create ChromeDriver
     chrome_driver = ChromeDriver(service=service, options=chrome_options)
 
     return chrome_driver
 
 
+def _create_edge_driver(proxy_name=None, private_mode=False):
+    # 1. create EdgeOption
+    options = EdgeOptions()
+    # 2. set EdgeOption attribute from config (e.g. proxy, --maximize, etc)
+    options.add_argument('start-maximized')
+    # bypass the message "your connection is not private" on non-secure page
+    options.add_argument('--ignore-ssl-errors=yes')
+    options.add_argument('--ignore-certificate-errors')
+    if private_mode:
+        options.add_argument('incognito')
+    # 3. add proxy
+    if proxy_name:
+        proxy: Proxy = _create_proxy(proxy_name)
+        options.proxy = proxy
+    # 4. create EdgeService
+    service = EdgeService(
+        executable_path=EdgeChromiumDriverManager().install(),
+        log_output=os.path.join(FolderSettings.LOG_DIR, EdgeSettings.DRIVER_NAME + ".log"))
+    # 5. create EdgeDriver
+    edge_driver = EdgeDriver(service=service, options=options)
+
+    return edge_driver
+
+
 def _create_firefox_driver(proxy_name=None, private_mode=False):
     # create options instance
     options = FirefoxOptions()
     # set browser mode
     if private_mode:
         options.add_argument('-private')
     # set log level
     # options.log.level = 'trace'
-    # convert options to desired_capabilities
-    desired_capabilities = options.to_capabilities()
     # set proxy
     if proxy_name is not None:
-        proxy = _create_proxy(proxy_name)
-        proxy.add_to_capabilities(desired_capabilities)
+        proxy: Proxy = _create_proxy(proxy_name)
+        options.proxy = proxy
+        # options.set_preference('network.proxy.type', 1)
+        # options.set_preference('network.proxy.http', 'proxy_host')
+        # options.set_preference('network.proxy.http_port', 8080)
+    #
+    service = FirefoxService(
+        # executable_path=FirefoxSettings.DRIVER_PATH,
+        executable_path=GeckoDriverManager().install(),
+        log_output=os.path.join(FolderSettings.LOG_DIR, FirefoxSettings.DRIVER_NAME + ".log"),
+        # service_args=['--log', 'debug']
+    )
 
-    return FirefoxDriver(executable_path=FirefoxSettings.DRIVER_PATH, desired_capabilities=desired_capabilities,
-                         log_path=os.path.join(FolderSettings.LOG_DIR, FirefoxSettings.DRIVER_NAME + ".log"))
+    return FirefoxDriver(options=options, service=service)
 
 
 def check_ie_running():
     """
     Check just run single IE instance on a VM
     :return:
     """
@@ -168,22 +234,26 @@
 
     # Indicates whether to skip the check that the browser's zoom level is set to 100%.
     ie_options.ignore_zoom_level = True
     # TODO: persistent_hover not effect/work
     # Persistent hovering is achieved by continuously firing mouse over events at the last location
     # the mouse cursor has been moved to.
     ie_options.persistent_hover = True
-    # parse option to Capabilities using to add proxy
-    ie_capabilities = ie_options.to_capabilities()
     # set proxy
     if proxy_name is not None:
         proxy = _create_proxy(proxy_name)
-        proxy.add_to_capabilities(ie_capabilities)
-    return IEDriver(executable_path=IESettings.DRIVER_PATH, capabilities=ie_capabilities, port=IESettings.RUNNING_PORT,
-                    service_log_path=os.path.join(FolderSettings.LOG_DIR, IESettings.DRIVER_NAME + ".log"))
+        ie_options.proxy = proxy
+    #
+    service = IEService(
+        executable_path=IEDriverManager().install(),
+        port=IESettings.RUNNING_PORT,
+        log_output=os.path.join(FolderSettings.LOG_DIR, IESettings.DRIVER_NAME + ".log"),
+    )
+
+    return IEDriver(options=ie_options, service=service)
 
 
 def _create_android_driver(driver_name, app_path=None, full_reset=False, custom_opts=None):
     if kdb.ENV == 'dev':
         # get device info from config file
         is_group, device_info = get_device_info(driver_name)
         device_info = device_info['android_emulator-5555']
@@ -244,31 +314,33 @@
             "The %s driver is only run on MAC machine. Please check your server's OS." % driver_name)
     device_info = MobileManager.start_appium_server(driver_name)
     # remove lock file
     MobileManager.remove_lock_file()
 
     logging.info("Starting Safari browser on %s..." % device_info.get('deviceName'))
     #
-    desired_caps = {"automationName": "xcuitest",  # case-insensitively
+    options = XCUITestOptions()
+    #
+    desired_caps = {"appium:automationName": "xcuitest",  # case-insensitively
                     "platformName": "iOS",
                     # platformVersion: This capability is used for device autodetection if udid is not provided
-                    "platformVersion": device_info.get('platformVersion'),
+                    "appium:platformVersion": device_info.get('platformVersion'),
                     # Consider setting udid for real devices and use this one for Simulator selection instead
-                    "deviceName": device_info.get('deviceName'),
-                    "udid": device_info.get('udid'),
-                    "newCommandTimeout": DriverSettings.DRIVER_NEW_COMMAND_TIMEOUT,
+                    "appium:deviceName": device_info.get('deviceName'),
+                    "appium:udid": device_info.get('udid'),
+                    "appium:newCommandTimeout": DriverSettings.DRIVER_NEW_COMMAND_TIMEOUT,
                     "wdaLocalPort": device_info.get('wdaLocalPort'),
                     # todo: webkitDebugProxyPort is only necessary for Appium below version 1.15.
                     "webkitDebugProxyPort": device_info.get('webkitDebugProxyPort'),  # todo
                     "clearSystemFiles": True,  # Delete any generated files at the end of a session. Default to false.
                     "shouldUseSingletonTestManager": False,
                     # Get JSON source from WDA and transform it to XML on the Appium server side. Defaults to false
                     'useJSONSource': True,
                     'preventWDAAttachments': True,
-                    'fullReset': full_reset,
+                    'appium:fullReset': full_reset,
                     'sendKeyStrategy': 'oneByOne',
                     # simulator caps
                     "shutdownOtherSimulators": True, 'safariAllowPopups': True,
                     'safariIgnoreFraudWarning': True,
                     'safariOpenLinksInBackground': True, 'reduceMotion': True,
                     # todo
                     # 'useNewWDA': True,  # useNewWDA: Real devices require WebDriverAgent client to run for as long as possible without reinstall/restart
@@ -277,15 +349,15 @@
                     }
 
     if app_path is None:
         desired_caps['browserName'] = 'safari'
     else:
         desired_caps['app'] = FileUtil.get_absolute_path(app_path)
 
-    return webdriver.Remote(device_info.get('hubURL'), desired_caps)
+    return webdriver.Remote(device_info.get('hubURL'), options=options)
 
 
 def create_driver(driver_name="chrome", proxy_name=None, private_mode=False, app_path=None, full_reset=False):
     """
     create a webdriver
     :param driver_name:
     :param proxy_name:
@@ -294,14 +366,16 @@
     :param full_reset:
     :return: WebDriver
     """
     driver_name = str(driver_name).lower().strip()
     # create web driver depend driver_name
     if driver_name in _CHROME_ALIAS:
         driver = _create_chrome_driver(proxy_name, private_mode)
+    elif driver_name in _EDGE_ALIAS:
+        driver = _create_edge_driver(proxy_name, private_mode)
     elif driver_name in _FIREFOX_ALIAS:
         driver = _create_firefox_driver(proxy_name, private_mode)
     elif driver_name in _IE_ALIAS:
         driver = _create_ie_driver(proxy_name, private_mode)
     elif DeviceType.is_android(driver_name):
         driver = _create_android_driver(driver_name, app_path=app_path, full_reset=full_reset)
     elif DeviceType.is_ios(driver_name):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kdb-python-0.0.5/kdb/webdriver/windows.py` & `kdb-python-0.0.6/kdb/webdriver/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         start_time = log_start(self.next.__name__, args_passed, log)
         try:
             # get next window handle
             next_window = self._get_window(timeout, 1)
             # switch to next window handle
             self._driver.switch_to.window(next_window)
             report_passed_test_step(self.next.__name__, args_passed, start_time,
-                                    InfoMessage.ACTION_SUCCESS % "Switch to main windows")
+                                    InfoMessage.ACTION_SUCCESS % "Switch to next windows")
         except Exception as ex:
             report_failed_test_step(self._driver, self.next.__name__, args_passed, start_time, str(ex))
 
     def previous(self, timeout=DriverSettings.DRIVER_IMPLICITLY_WAIT, log=True):
         """
         Switch to previous windows
         """
```

### Comparing `kdb-python-0.0.5/kdb_python.egg-info/PKG-INFO` & `kdb-python-0.0.6/kdb_python.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kdb-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation testing
 Home-page: https://github.com/Trucnt/kdb-core
 Author: Truc Nguyen
-Author-email: Truc Nguyen <trucnt88@gmail.com>
+Author-email: Trucnt <trucnt88@gmail.com>
 License: MIT
 Project-URL: home-page, https://github.com/Trucnt/kdb-demo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `kdb-python-0.0.5/kdb_python.egg-info/SOURCES.txt` & `kdb-python-0.0.6/kdb_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 kdb/common/mobile_manager.py
 kdb/common/profiles.py
 kdb/common/properties.py
 kdb/common/random_util.py
 kdb/common/ssh_connection.py
 kdb/common/utils.py
 kdb/config/__init__.py
-kdb/config/device_list.py
-kdb/config/proxy_list.py
 kdb/config/settings.py
-kdb/drivers/__init__.py
 kdb/report/__init__.py
 kdb/report/report_manager.py
 kdb/report/test_case_log.py
 kdb/report/test_step_log.py
 kdb/scripts/__init__.py
 kdb/unit_test/__init__.py
 kdb/unit_test/mobile/__init__.py
@@ -56,31 +53,28 @@
 kdb/unit_test/no_driver/test_json_path.py
 kdb/unit_test/no_driver/test_random.py
 kdb/unit_test/no_driver/test_requests.py
 kdb/unit_test/no_driver/test_verify_string_contains.py
 kdb/unit_test/pc/__init__.py
 kdb/unit_test/pc/test_alert.py
 kdb/unit_test/pc/test_browser_navigation.py
-kdb/unit_test/pc/test_check.py
+kdb/unit_test/pc/test_check_and_uncheck.py
 kdb/unit_test/pc/test_click.py
-kdb/unit_test/pc/test_close_browser.py
 kdb/unit_test/pc/test_context_click.py
 kdb/unit_test/pc/test_cookies.py
 kdb/unit_test/pc/test_double_click.py
 kdb/unit_test/pc/test_element_attribute.py
 kdb/unit_test/pc/test_element_text.py
 kdb/unit_test/pc/test_execute_script.py
 kdb/unit_test/pc/test_hover.py
 kdb/unit_test/pc/test_is_display.py
-kdb/unit_test/pc/test_open_url.py
 kdb/unit_test/pc/test_press_keys.py
 kdb/unit_test/pc/test_press_keys_and_click.py
 kdb/unit_test/pc/test_select.py
 kdb/unit_test/pc/test_start_browser.py
-kdb/unit_test/pc/test_uncheck.py
 kdb/unit_test/pc/test_update_text.py
 kdb/unit_test/pc/test_upload_file.py
 kdb/unit_test/pc/test_verify_element_attribute.py
 kdb/unit_test/pc/test_verify_text_on_page.py
 kdb/unit_test/pc/test_verify_title.py
 kdb/unit_test/pc/test_verify_url_contains.py
 kdb/unit_test/pc/test_video.py
```

### Comparing `kdb-python-0.0.5/setup.py` & `kdb-python-0.0.6/setup.py`

 * *Files identical despite different names*

