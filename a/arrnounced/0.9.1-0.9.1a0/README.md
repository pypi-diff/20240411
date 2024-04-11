# Comparing `tmp/arrnounced-0.9.1.tar.gz` & `tmp/arrnounced-0.9.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrnounced-0.9.1.tar", last modified: Thu Apr 11 18:44:00 2024, max compression
+gzip compressed data, was "arrnounced-0.9.1a0.tar", max compression
```

## Comparing `arrnounced-0.9.1.tar` & `arrnounced-0.9.1a0.tar`

### file list

```diff
@@ -1,69 +1,48 @@
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.316747 arrnounced-0.9.1/
--rw-r--r--   0 klnt      (1000) users      (984)     4199 2024-04-11 18:44:00.316747 arrnounced-0.9.1/PKG-INFO
--rw-r--r--   0 klnt      (1000) users      (984)     3373 2024-04-09 14:37:36.000000 arrnounced-0.9.1/README.md
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.312747 arrnounced-0.9.1/arrnounced/
--rw-r--r--   0 klnt      (1000) users      (984)       22 2024-04-11 18:42:57.000000 arrnounced-0.9.1/arrnounced/__init__.py
--rw-r--r--   0 klnt      (1000) users      (984)     5562 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/announce_parser.py
--rw-r--r--   0 klnt      (1000) users      (984)     8871 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/announcement.py
--rw-r--r--   0 klnt      (1000) users      (984)     5103 2024-04-11 14:06:02.000000 arrnounced-0.9.1/arrnounced/backend.py
--rwxr-xr-x   0 klnt      (1000) users      (984)     2646 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/cli.py
--rw-r--r--   0 klnt      (1000) users      (984)    10364 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/config.py
--rw-r--r--   0 klnt      (1000) users      (984)     4249 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/db.py
--rw-r--r--   0 klnt      (1000) users      (984)     1080 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/eventloop_utils.py
--rw-r--r--   0 klnt      (1000) users      (984)     7026 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/irc.py
--rw-r--r--   0 klnt      (1000) users      (984)     2832 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/irc_modes.py
--rw-r--r--   0 klnt      (1000) users      (984)     1172 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/log.py
--rw-r--r--   0 klnt      (1000) users      (984)     2879 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/manager.py
--rw-r--r--   0 klnt      (1000) users      (984)     2709 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/message_handler.py
--rw-r--r--   0 klnt      (1000) users      (984)     1434 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/session_provider.py
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.312747 arrnounced-0.9.1/arrnounced/templates/
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.308747 arrnounced-0.9.1/arrnounced/templates/assets/
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.308747 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.312747 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/css/
--rw-r--r--   0 klnt      (1000) users      (984)   131226 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.312747 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/
--rw-r--r--   0 klnt      (1000) users      (984)    20127 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 klnt      (1000) users      (984)   108738 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 klnt      (1000) users      (984)    45404 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 klnt      (1000) users      (984)    23424 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 klnt      (1000) users      (984)    18028 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.312747 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/js/
--rw-r--r--   0 klnt      (1000) users      (984)    37045 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.316747 arrnounced-0.9.1/arrnounced/templates/assets/css/
--rw-r--r--   0 klnt      (1000) users      (984)      357 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/index.css
--rw-r--r--   0 klnt      (1000) users      (984)      349 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/status.css
--rw-r--r--   0 klnt      (1000) users      (984)     1740 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/styles.min.css
--rw-r--r--   0 klnt      (1000) users      (984)     7518 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/toastr.css
--rw-r--r--   0 klnt      (1000) users      (984)     6740 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/toastr.min.css
--rw-r--r--   0 klnt      (1000) users      (984)     2243 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/css/user.css
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.316747 arrnounced-0.9.1/arrnounced/templates/assets/js/
--rw-r--r--   0 klnt      (1000) users      (984)      704 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/common.js
--rw-r--r--   0 klnt      (1000) users      (984)     4437 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/index.js
--rw-r--r--   0 klnt      (1000) users      (984)    97162 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/jquery.min.js
--rw-r--r--   0 klnt      (1000) users      (984)     6543 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/jquery.twbsPagination.min.js
--rw-r--r--   0 klnt      (1000) users      (984)       13 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/logs.js
--rw-r--r--   0 klnt      (1000) users      (984)      857 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/script.min.js
--rw-r--r--   0 klnt      (1000) users      (984)     1845 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/settings.js
--rw-r--r--   0 klnt      (1000) users      (984)     5536 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/assets/js/toastr.js
--rw-r--r--   0 klnt      (1000) users      (984)     4815 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/index.html
--rw-r--r--   0 klnt      (1000) users      (984)     1800 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/login.html
--rw-r--r--   0 klnt      (1000) users      (984)     2550 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/templates/logs.html
--rw-r--r--   0 klnt      (1000) users      (984)     7033 2024-04-11 14:06:02.000000 arrnounced-0.9.1/arrnounced/templates/status.html
--rw-r--r--   0 klnt      (1000) users      (984)     8162 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/tracker.py
--rw-r--r--   0 klnt      (1000) users      (984)     6801 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/tracker_xml_config.py
--rw-r--r--   0 klnt      (1000) users      (984)     2642 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/utils.py
--rw-r--r--   0 klnt      (1000) users      (984)     3009 2024-04-11 13:11:39.000000 arrnounced-0.9.1/arrnounced/web_handler.py
--rw-r--r--   0 klnt      (1000) users      (984)     5621 2024-04-11 17:07:40.000000 arrnounced-0.9.1/arrnounced/webui.py
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.316747 arrnounced-0.9.1/arrnounced.egg-info/
--rw-r--r--   0 klnt      (1000) users      (984)     4199 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/PKG-INFO
--rw-r--r--   0 klnt      (1000) users      (984)     2011 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/SOURCES.txt
--rw-r--r--   0 klnt      (1000) users      (984)        1 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/dependency_links.txt
--rw-r--r--   0 klnt      (1000) users      (984)       51 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/entry_points.txt
--rw-r--r--   0 klnt      (1000) users      (984)      200 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/requires.txt
--rw-r--r--   0 klnt      (1000) users      (984)       11 2024-04-11 18:44:00.000000 arrnounced-0.9.1/arrnounced.egg-info/top_level.txt
--rw-r--r--   0 klnt      (1000) users      (984)     1410 2024-04-11 18:42:57.000000 arrnounced-0.9.1/pyproject.toml
--rw-r--r--   0 klnt      (1000) users      (984)       38 2024-04-11 18:44:00.316747 arrnounced-0.9.1/setup.cfg
-drwxr-xr-x   0 klnt      (1000) users      (984)        0 2024-04-11 18:44:00.316747 arrnounced-0.9.1/tests/
--rw-r--r--   0 klnt      (1000) users      (984)    21011 2022-01-09 10:50:51.000000 arrnounced-0.9.1/tests/test_announce_parser.py
--rw-r--r--   0 klnt      (1000) users      (984)    28235 2022-01-09 10:50:51.000000 arrnounced-0.9.1/tests/test_announcement.py
--rw-r--r--   0 klnt      (1000) users      (984)    14986 2022-02-05 21:34:00.000000 arrnounced-0.9.1/tests/test_config.py
+-rw-r--r--   0        0        0     3371 2022-02-13 14:14:40.477951 arrnounced-0.9.1a0/README.md
+-rw-r--r--   0        0        0      167 2022-01-09 10:50:51.308989 arrnounced-0.9.1a0/arrnounced/__init__.py
+-rw-r--r--   0        0        0     5562 2022-01-09 10:50:51.308989 arrnounced-0.9.1a0/arrnounced/announce_parser.py
+-rw-r--r--   0        0        0     8871 2022-02-05 21:34:00.201835 arrnounced-0.9.1a0/arrnounced/announcement.py
+-rw-r--r--   0        0        0     4828 2022-01-09 10:50:51.308989 arrnounced-0.9.1a0/arrnounced/backend.py
+-rwxr-xr-x   0        0        0     2646 2022-01-09 10:50:51.312989 arrnounced-0.9.1a0/arrnounced/cli.py
+-rw-r--r--   0        0        0    10396 2022-03-13 15:21:40.239257 arrnounced-0.9.1a0/arrnounced/config.py
+-rw-r--r--   0        0        0     4249 2022-02-07 19:44:54.264092 arrnounced-0.9.1a0/arrnounced/db.py
+-rw-r--r--   0        0        0     1080 2022-02-07 19:59:08.227354 arrnounced-0.9.1a0/arrnounced/eventloop_utils.py
+-rw-r--r--   0        0        0     7080 2022-04-03 12:18:47.057159 arrnounced-0.9.1a0/arrnounced/irc.py
+-rw-r--r--   0        0        0     2832 2022-01-09 10:50:51.312989 arrnounced-0.9.1a0/arrnounced/irc_modes.py
+-rw-r--r--   0        0        0     1172 2022-01-09 10:50:51.312989 arrnounced-0.9.1a0/arrnounced/log.py
+-rw-r--r--   0        0        0     2879 2022-02-13 12:35:41.596683 arrnounced-0.9.1a0/arrnounced/manager.py
+-rw-r--r--   0        0        0     2709 2022-02-05 21:34:00.205834 arrnounced-0.9.1a0/arrnounced/message_handler.py
+-rw-r--r--   0        0        0     1434 2022-01-09 10:50:51.312989 arrnounced-0.9.1a0/arrnounced/session_provider.py
+-rw-r--r--   0        0        0   131226 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0    20127 2022-01-09 10:50:51.316989 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2022-01-09 10:50:51.316989 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2022-01-09 10:50:51.316989 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2022-01-09 10:50:51.316989 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0    37045 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0      357 2022-01-16 15:11:23.616469 arrnounced-0.9.1a0/arrnounced/templates/assets/css/index.css
+-rw-r--r--   0        0        0      349 2022-02-05 21:34:00.205834 arrnounced-0.9.1a0/arrnounced/templates/assets/css/status.css
+-rw-r--r--   0        0        0     1740 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/css/styles.min.css
+-rw-r--r--   0        0        0     7518 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/css/toastr.css
+-rw-r--r--   0        0        0     6740 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/css/toastr.min.css
+-rw-r--r--   0        0        0     2243 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/css/user.css
+-rw-r--r--   0        0        0      704 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/js/common.js
+-rw-r--r--   0        0        0     4437 2022-01-09 10:50:51.316989 arrnounced-0.9.1a0/arrnounced/templates/assets/js/index.js
+-rw-r--r--   0        0        0    97162 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/js/jquery.min.js
+-rw-r--r--   0        0        0     6543 2022-01-09 10:50:51.320989 arrnounced-0.9.1a0/arrnounced/templates/assets/js/jquery.twbsPagination.min.js
+-rw-r--r--   0        0        0       13 2022-01-09 10:50:51.320989 arrnounced-0.9.1a0/arrnounced/templates/assets/js/logs.js
+-rw-r--r--   0        0        0      857 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/js/script.min.js
+-rw-r--r--   0        0        0     1845 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/js/settings.js
+-rw-r--r--   0        0        0     5536 2022-02-07 19:46:14.777003 arrnounced-0.9.1a0/arrnounced/templates/assets/js/toastr.js
+-rw-r--r--   0        0        0     4815 2022-02-06 11:34:59.773769 arrnounced-0.9.1a0/arrnounced/templates/index.html
+-rw-r--r--   0        0        0     1800 2022-02-05 22:15:29.166480 arrnounced-0.9.1a0/arrnounced/templates/login.html
+-rw-r--r--   0        0        0     2550 2022-02-05 22:15:03.291471 arrnounced-0.9.1a0/arrnounced/templates/logs.html
+-rw-r--r--   0        0        0     7029 2022-02-05 22:15:18.022907 arrnounced-0.9.1a0/arrnounced/templates/status.html
+-rw-r--r--   0        0        0     8260 2022-03-13 15:23:28.999174 arrnounced-0.9.1a0/arrnounced/tracker.py
+-rw-r--r--   0        0        0     6801 2022-01-09 10:50:51.320989 arrnounced-0.9.1a0/arrnounced/tracker_xml_config.py
+-rw-r--r--   0        0        0     2642 2022-01-09 10:50:51.320989 arrnounced-0.9.1a0/arrnounced/utils.py
+-rw-r--r--   0        0        0     3009 2022-02-27 18:56:34.788698 arrnounced-0.9.1a0/arrnounced/web_handler.py
+-rw-r--r--   0        0        0     5581 2022-02-27 18:56:31.212835 arrnounced-0.9.1a0/arrnounced/webui.py
+-rw-r--r--   0        0        0      726 2022-04-03 12:26:08.914165 arrnounced-0.9.1a0/pyproject.toml
+-rw-r--r--   0        0        0     4799 2022-04-03 12:27:25.849958 arrnounced-0.9.1a0/setup.py
+-rw-r--r--   0        0        0     4223 2022-04-03 12:27:25.850766 arrnounced-0.9.1a0/PKG-INFO
```

### Comparing `arrnounced-0.9.1/PKG-INFO` & `arrnounced-0.9.1a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: arrnounced
-Version: 0.9.1
+Version: 0.9.1a0
 Summary: Notify Sonarr/Radarr/Lidarr of tracker IRC announcements
-Author-email: WeAnnounce <weannounce@protonmail.com>
-Project-URL: homepage, https://github.com/weannounce/arrnounced
-Requires-Python: <3.10,>=3.7
+Home-page: https://github.com/weannounce/arrnounced
+Author: WeAnnounce
+Author-email: weannounce@protonmail.com
+Requires-Python: >=3.7,<3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Flask (==1.1.1)
+Requires-Dist: Flask-Login (==0.4.1)
+Requires-Dist: Flask-SocketIO (>=4.3.2,<5.0.0)
+Requires-Dist: aiohttp (==3.8.1)
+Requires-Dist: defusedxml (==0.6.0)
+Requires-Dist: importlib-metadata (>=1.0,<2.0); python_version < "3.8"
+Requires-Dist: pony (==0.7.14)
+Requires-Dist: pydle (==0.9.4)
+Requires-Dist: tomlkit (==0.7.0)
 Description-Content-Type: text/markdown
-Requires-Dist: Flask-Login~=0.6.3
-Requires-Dist: Flask-SocketIO~=5.3.6
-Requires-Dist: Flask~=3.0.3
-Requires-Dist: aiohttp~=3.9.3
-Requires-Dist: defusedxml~=0.7.1
-Requires-Dist: pony~=0.7.17
-Requires-Dist: pydle~=0.9.4
-Requires-Dist: tomlkit~=0.12.4
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: bumpver==2023.1129; extra == "dev"
-Requires-Dist: coverage~=5.0; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 
 # Arrnounced
 Notify Sonarr/Radarr/Lidarr of tracker IRC announcements.
 
 Built on the work of
 [sonarrAnnounced](https://github.com/l3uddz/sonarrAnnounced) with tracker
 configuration from
@@ -53,15 +52,15 @@
 
 _Release v0.7 updated the configuration format. See the [release
 notes](https://github.com/weannounce/arrnounced/releases/tag/v0.7) for more
 information._
 
 ## Configuration
 The default configuration path is `~/.arrnounced/settings.toml`.
-[example.toml](https://github.com/weannounce/arrnounced/blob/master/example.toml)
+[example.cfg](https://github.com/weannounce/arrnounced/blob/master/example.cfg)
 is the acting configuration documentation.
 
 The default XML tracker configuration path is `~/.arrnounced/autodl-trackers/trackers`
 
 ## Installation
 
 ```bash
@@ -108,7 +107,8 @@
 The database design was updated in [v0.3](https://github.com/weannounce/arrnounced/releases/tag/v0.3)
 ([ef931ee](https://github.com/weannounce/arrnounced/commit/ef931eef27348f82254d601f96d094a7b9f147bb)).
 If you used Arrnounced prior to this or used its predecessor you have two options.
 * Convert your old database using [convert_db.py](https://github.com/weannounce/arrnounced/blob/master/convert_db.py)
 * Move the old database file for safe keeping and let Arrnounced create a new file.
 
 The default path to the database is `~/.arrnounced/brain.db`
+
```

### Comparing `arrnounced-0.9.1/README.md` & `arrnounced-0.9.1a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 _Release v0.7 updated the configuration format. See the [release
 notes](https://github.com/weannounce/arrnounced/releases/tag/v0.7) for more
 information._
 
 ## Configuration
 The default configuration path is `~/.arrnounced/settings.toml`.
-[example.toml](https://github.com/weannounce/arrnounced/blob/master/example.toml)
+[example.cfg](https://github.com/weannounce/arrnounced/blob/master/example.cfg)
 is the acting configuration documentation.
 
 The default XML tracker configuration path is `~/.arrnounced/autodl-trackers/trackers`
 
 ## Installation
 
 ```bash
```

### Comparing `arrnounced-0.9.1/arrnounced/announce_parser.py` & `arrnounced-0.9.1a0/arrnounced/announce_parser.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/announcement.py` & `arrnounced-0.9.1a0/arrnounced/announcement.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/backend.py` & `arrnounced-0.9.1a0/arrnounced/backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 import logging
 import re
 from asyncio import Lock
-from functools import reduce
-from operator import and_
 
 from arrnounced.eventloop_utils import eventloop_util
 from arrnounced.session_provider import SessionProvider
 
 
 logger = logging.getLogger("BACKEND")
 
 
 def _extract_approval(json_response, backend_name):
     try:
-        approvals = (
-            e["approved"]
-            for e in (
-                json_response if isinstance(json_response, list) else [json_response]
-            )
-        )
-        # Not sure why the response is a list when the push is a single item.
-        # Reducing all the values with "and" seems reasonable
-        return reduce(and_, approvals)
+        return json_response["approved"]
     except TypeError:
         logger.warning("No valid JSON reply from %s", backend_name, exc_info=True)
     except KeyError:
         logger.warning("No approval info in reply from %s", backend_name, exc_info=True)
     return False
 
 
@@ -69,26 +59,34 @@
             headers={"X-Api-Key": self.apikey},
         )
         result = json_response is not None
         logger.debug("%s access: %s", self.name, "granted" if result else "failed")
         return result
 
 
-class V3Api(Backend):
-    push_path_v3 = "/api/v3/release/push"
-    diskspace_path_v3 = "/api/v3/diskspace"
-    push_path_legacy = "/api/release/push"
-    diskspace_path_legacy = "/api/diskspace"
-
+class UseIndexer(Backend):
     def _create_json(self, announcement):
         params = super()._create_json(announcement)
         params["indexer"] = "Irc" + announcement.indexer
 
         return params
 
+
+# TODO: Use v3 API
+class Sonarr(UseIndexer):
+    push_path = "/api/release/push"
+    diskspace_path = "/api/diskspace"
+
+
+class Radarr(UseIndexer):
+    push_path_v3 = "/api/v3/release/push"
+    diskspace_path_v3 = "/api/v3/diskspace"
+    push_path_legacy = "/api/release/push"
+    diskspace_path_legacy = "/api/diskspace"
+
     def __init__(self, user_backend):
         self._set_v3()
         super().__init__(user_backend)
 
     def _set_v3(self):
         self.push_path = self.push_path_v3
         self.diskspace_path = self.diskspace_path_v3
@@ -107,20 +105,14 @@
             return True
 
         # Neither worked, setting v3 as default
         self._set_v3()
         return False
 
 
-class Sonarr(V3Api): ...
-
-
-class Radarr(V3Api): ...
-
-
 class Lidarr(Backend):
     push_path = "/api/v1/release/push"
     diskspace_path = "/api/v1/diskspace"
 
 
 backend_mapping = {
     "sonarr": Sonarr,
```

### Comparing `arrnounced-0.9.1/arrnounced/cli.py` & `arrnounced-0.9.1a0/arrnounced/cli.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/config.py` & `arrnounced-0.9.1a0/arrnounced/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
 
 def _init_trackers(toml_cfg):
     valid_types = True
     for tracker_type in toml_cfg["trackers"]:
         # Init default values
         default_tracker_values = [
+            ("irc_server", ""),
             ("irc_tls", False),
             ("irc_tls_verify", False),
             ("torrent_https", False),
             ("announce_delay", 0),
             ("category", {}),
             ("settings", {}),
         ]
```

### Comparing `arrnounced-0.9.1/arrnounced/db.py` & `arrnounced-0.9.1a0/arrnounced/db.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/eventloop_utils.py` & `arrnounced-0.9.1a0/arrnounced/eventloop_utils.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/irc.py` & `arrnounced-0.9.1a0/arrnounced/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 
         clients.append(client)
         try:
             pool.connect(
                 client,
                 hostname=tracker.config.irc_server,
                 port=tracker.config.irc_port,
+                password=tracker.config.irc_password,
                 tls=tracker.config.irc_tls,
                 tls_verify=tracker.config.irc_tls_verify,
             )
         except Exception:
             logger.exception("Error while connecting to: %s", tracker.config.irc_server)
 
     try:
```

### Comparing `arrnounced-0.9.1/arrnounced/irc_modes.py` & `arrnounced-0.9.1a0/arrnounced/irc_modes.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/log.py` & `arrnounced-0.9.1a0/arrnounced/log.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/manager.py` & `arrnounced-0.9.1a0/arrnounced/manager.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/message_handler.py` & `arrnounced-0.9.1a0/arrnounced/message_handler.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/session_provider.py` & `arrnounced-0.9.1a0/arrnounced/session_provider.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/css/bootstrap.min.css` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.eot` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.svg` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/bootstrap/js/bootstrap.min.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/css/styles.min.css` & `arrnounced-0.9.1a0/arrnounced/templates/assets/css/styles.min.css`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/css/toastr.css` & `arrnounced-0.9.1a0/arrnounced/templates/assets/css/toastr.css`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/css/toastr.min.css` & `arrnounced-0.9.1a0/arrnounced/templates/assets/css/toastr.min.css`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/css/user.css` & `arrnounced-0.9.1a0/arrnounced/templates/assets/css/user.css`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/common.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/common.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/index.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/index.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/jquery.min.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/jquery.twbsPagination.min.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/jquery.twbsPagination.min.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/script.min.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/script.min.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/settings.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/settings.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/assets/js/toastr.js` & `arrnounced-0.9.1a0/arrnounced/templates/assets/js/toastr.js`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/index.html` & `arrnounced-0.9.1a0/arrnounced/templates/index.html`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/login.html` & `arrnounced-0.9.1a0/arrnounced/templates/login.html`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/logs.html` & `arrnounced-0.9.1a0/arrnounced/templates/logs.html`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/templates/status.html` & `arrnounced-0.9.1a0/arrnounced/templates/status.html`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         </div>
       </div>
     </div>
     <script src="assets/js/jquery.min.js"></script>
     <script src="assets/bootstrap/js/bootstrap.min.js"></script>
     <script src="assets/js/common.js"></script>
     <script src="assets/js/status.js"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.7.5/socket.io.min.js"
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/2.4.0/socket.io.js"
       crossorigin="anonymous"></script>
 <script type="text/javascript" charset="utf-8">
   var socket = io();
   function add_indexer_row(tbody, indexer_status) {
       var newRow = tbody.insertRow();
       newRow.setAttribute("id", "indexer_" + indexer_status["indexer_type"])
       var keys = ["name", "connected", "channels", "latest_announcement", "latest_snatch"]
```

### Comparing `arrnounced-0.9.1/arrnounced/tracker.py` & `arrnounced-0.9.1a0/arrnounced/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,18 @@
         return self._user_tracker["irc_nickname"]
 
     @property
     def irc_server(self):
         return str(self._user_tracker["irc_server"])
 
     @property
+    def irc_password(self):
+        return str(self._user_tracker["irc_password"])
+
+    @property
     def irc_tls(self):
         return self._user_tracker["irc_tls"]
 
     @property
     def irc_tls_verify(self):
         return self._user_tracker["irc_tls_verify"]
```

### Comparing `arrnounced-0.9.1/arrnounced/tracker_xml_config.py` & `arrnounced-0.9.1a0/arrnounced/tracker_xml_config.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/utils.py` & `arrnounced-0.9.1a0/arrnounced/utils.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/web_handler.py` & `arrnounced-0.9.1a0/arrnounced/web_handler.py`

 * *Files identical despite different names*

### Comparing `arrnounced-0.9.1/arrnounced/webui.py` & `arrnounced-0.9.1a0/arrnounced/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     try:
         socketio.run(
             app,
             host=user_config.webui_host,
             port=user_config.webui_port,
             debug=False,
             use_reloader=False,
-            allow_unsafe_werkzeug=True,
         )
     except OSError as e:
         logger.error("Error starting webserver: %s", e)
     logger.info("Flask thread finished")
 
 
 def update(tracker_status_dict):
```

### Comparing `arrnounced-0.9.1/arrnounced.egg-info/PKG-INFO` & `arrnounced-0.9.1a0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,51 @@
-Metadata-Version: 2.1
-Name: arrnounced
-Version: 0.9.1
-Summary: Notify Sonarr/Radarr/Lidarr of tracker IRC announcements
-Author-email: WeAnnounce <weannounce@protonmail.com>
-Project-URL: homepage, https://github.com/weannounce/arrnounced
-Requires-Python: <3.10,>=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: Flask-Login~=0.6.3
-Requires-Dist: Flask-SocketIO~=5.3.6
-Requires-Dist: Flask~=3.0.3
-Requires-Dist: aiohttp~=3.9.3
-Requires-Dist: defusedxml~=0.7.1
-Requires-Dist: pony~=0.7.17
-Requires-Dist: pydle~=0.9.4
-Requires-Dist: tomlkit~=0.12.4
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: bumpver==2023.1129; extra == "dev"
-Requires-Dist: coverage~=5.0; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-
-# Arrnounced
-Notify Sonarr/Radarr/Lidarr of tracker IRC announcements.
-
-Built on the work of
-[sonarrAnnounced](https://github.com/l3uddz/sonarrAnnounced) with tracker
-configuration from
-[autodl-trackers](https://github.com/autodl-community/autodl-trackers) (used by
-[autodl-irssi](https://github.com/autodl-community/autodl-irssi))
-
-## Features
-* All trackers from
-[autodl-trackers](https://github.com/autodl-community/autodl-trackers/tree/master/trackers)
-are supported.
-* Web UI to list announcements and accepted notifications
-    * Ability to search among the announcements remains to be implemented though
-* Notify based on announcement category
-* Configurable delay between IRC announcement and notification
-
-Only a few of the supported trackers are tested at the moment. Please report any issues you find.
-
-## Screenshots
-
-### Main page
-![Index Page](https://raw.githubusercontent.com/weannounce/arrnounced/img/doc/index.PNG)
-### Status page
-![Status Page](https://raw.githubusercontent.com/weannounce/arrnounced/img/doc/status.gif)
-
-# Setup
-
-_Release v0.7 updated the configuration format. See the [release
-notes](https://github.com/weannounce/arrnounced/releases/tag/v0.7) for more
-information._
-
-## Configuration
-The default configuration path is `~/.arrnounced/settings.toml`.
-[example.toml](https://github.com/weannounce/arrnounced/blob/master/example.toml)
-is the acting configuration documentation.
-
-The default XML tracker configuration path is `~/.arrnounced/autodl-trackers/trackers`
-
-## Installation
-
-```bash
-# Optional virtual environment
-$ python -m venv path/to/venv
-$ source path/to/venv/bin/activate
-
-# Install
-$ pip install arrnounced
-
-# Run
-$ arrnounced
-```
-
-Configuration files path as well as log and database location may be changed with command line arguments.
-
-
-### Docker
-[Arrnounced on dockerhub](https://hub.docker.com/r/weannounce/arrnounced)
-
-* You must provide `settings.toml` in `/config`. This is also where logs and the database will be stored.
-* To access the web UI using bridged network the webui host in settings.toml must be `0.0.0.0`.
-* As Arrnounced runs as a non-root user by default it is recommended to specify your own user to handle write access to `/config`.
-
-```bash
-# Default example
-docker run -v /path/to/settings:/config \
-           --user 1000 \
-           -p 3467:3467 weannounce/arrnounced:latest
-```
-
-The docker image comes with a snapshot of XML tracker configurations located under `/trackers`. If you prefer your own version you can mount over it.
-
-```bash
-# Example with custom XML tracker configs and verbose logging
-docker run -v /path/to/settings:/config \
-           -v /path/to/autodl-trackers/trackers:/trackers \
-           -e VERBOSE=Y \
-           --user 1000 \
-           -p 3467:3467 weannounce/arrnounced:latest
-```
-
-## Database design update
-The database design was updated in [v0.3](https://github.com/weannounce/arrnounced/releases/tag/v0.3)
-([ef931ee](https://github.com/weannounce/arrnounced/commit/ef931eef27348f82254d601f96d094a7b9f147bb)).
-If you used Arrnounced prior to this or used its predecessor you have two options.
-* Convert your old database using [convert_db.py](https://github.com/weannounce/arrnounced/blob/master/convert_db.py)
-* Move the old database file for safe keeping and let Arrnounced create a new file.
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-The default path to the database is `~/.arrnounced/brain.db`
+packages = \
+['arrnounced']
+
+package_data = \
+{'': ['*'],
+ 'arrnounced': ['templates/*',
+                'templates/assets/bootstrap/css/*',
+                'templates/assets/bootstrap/fonts/*',
+                'templates/assets/bootstrap/js/*',
+                'templates/assets/css/*',
+                'templates/assets/js/*']}
+
+install_requires = \
+['Flask-Login==0.4.1',
+ 'Flask-SocketIO>=4.3.2,<5.0.0',
+ 'Flask==1.1.1',
+ 'aiohttp==3.8.1',
+ 'defusedxml==0.6.0',
+ 'pony==0.7.14',
+ 'pydle==0.9.4',
+ 'tomlkit==0.7.0']
+
+extras_require = \
+{':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
+
+entry_points = \
+{'console_scripts': ['arrnounced = arrnounced.cli:main']}
+
+setup_kwargs = {
+    'name': 'arrnounced',
+    'version': '0.9.1a0',
+    'description': 'Notify Sonarr/Radarr/Lidarr of tracker IRC announcements',
+    'long_description': '# Arrnounced\nNotify Sonarr/Radarr/Lidarr of tracker IRC announcements.\n\nBuilt on the work of\n[sonarrAnnounced](https://github.com/l3uddz/sonarrAnnounced) with tracker\nconfiguration from\n[autodl-trackers](https://github.com/autodl-community/autodl-trackers) (used by\n[autodl-irssi](https://github.com/autodl-community/autodl-irssi))\n\n## Features\n* All trackers from\n[autodl-trackers](https://github.com/autodl-community/autodl-trackers/tree/master/trackers)\nare supported.\n* Web UI to list announcements and accepted notifications\n    * Ability to search among the announcements remains to be implemented though\n* Notify based on announcement category\n* Configurable delay between IRC announcement and notification\n\nOnly a few of the supported trackers are tested at the moment. Please report any issues you find.\n\n## Screenshots\n\n### Main page\n![Index Page](https://raw.githubusercontent.com/weannounce/arrnounced/img/doc/index.PNG)\n### Status page\n![Status Page](https://raw.githubusercontent.com/weannounce/arrnounced/img/doc/status.gif)\n\n# Setup\n\n_Release v0.7 updated the configuration format. See the [release\nnotes](https://github.com/weannounce/arrnounced/releases/tag/v0.7) for more\ninformation._\n\n## Configuration\nThe default configuration path is `~/.arrnounced/settings.toml`.\n[example.cfg](https://github.com/weannounce/arrnounced/blob/master/example.cfg)\nis the acting configuration documentation.\n\nThe default XML tracker configuration path is `~/.arrnounced/autodl-trackers/trackers`\n\n## Installation\n\n```bash\n# Optional virtual environment\n$ python -m venv path/to/venv\n$ source path/to/venv/bin/activate\n\n# Install\n$ pip install arrnounced\n\n# Run\n$ arrnounced\n```\n\nConfiguration files path as well as log and database location may be changed with command line arguments.\n\n\n### Docker\n[Arrnounced on dockerhub](https://hub.docker.com/r/weannounce/arrnounced)\n\n* You must provide `settings.toml` in `/config`. This is also where logs and the database will be stored.\n* To access the web UI using bridged network the webui host in settings.toml must be `0.0.0.0`.\n* As Arrnounced runs as a non-root user by default it is recommended to specify your own user to handle write access to `/config`.\n\n```bash\n# Default example\ndocker run -v /path/to/settings:/config \\\n           --user 1000 \\\n           -p 3467:3467 weannounce/arrnounced:latest\n```\n\nThe docker image comes with a snapshot of XML tracker configurations located under `/trackers`. If you prefer your own version you can mount over it.\n\n```bash\n# Example with custom XML tracker configs and verbose logging\ndocker run -v /path/to/settings:/config \\\n           -v /path/to/autodl-trackers/trackers:/trackers \\\n           -e VERBOSE=Y \\\n           --user 1000 \\\n           -p 3467:3467 weannounce/arrnounced:latest\n```\n\n## Database design update\nThe database design was updated in [v0.3](https://github.com/weannounce/arrnounced/releases/tag/v0.3)\n([ef931ee](https://github.com/weannounce/arrnounced/commit/ef931eef27348f82254d601f96d094a7b9f147bb)).\nIf you used Arrnounced prior to this or used its predecessor you have two options.\n* Convert your old database using [convert_db.py](https://github.com/weannounce/arrnounced/blob/master/convert_db.py)\n* Move the old database file for safe keeping and let Arrnounced create a new file.\n\nThe default path to the database is `~/.arrnounced/brain.db`\n',
+    'author': 'WeAnnounce',
+    'author_email': 'weannounce@protonmail.com',
+    'maintainer': None,
+    'maintainer_email': None,
+    'url': 'https://github.com/weannounce/arrnounced',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'extras_require': extras_require,
+    'entry_points': entry_points,
+    'python_requires': '>=3.7,<3.10',
+}
+
+
+setup(**setup_kwargs)
```

