# Comparing `tmp/pih-0.36.1.tar.gz` & `tmp/pih-0.36.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.1.tar", last modified: Wed Apr 10 09:23:31 2024, max compression
+gzip compressed data, was "pih-0.36.2.tar", last modified: Wed Apr 10 10:22:39 2024, max compression
```

## Comparing `pih-0.36.1.tar` & `pih-0.36.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.833505 pih-0.36.1/
--rw-rw-rw-   0        0        0      249 2024-04-10 09:23:31.801938 pih-0.36.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:29.431079 pih-0.36.1/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.1/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:30.057101 pih-0.36.1/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.1/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.1/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.1/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.1/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.409246 pih-0.36.1/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-10 09:22:43.000000 pih-0.36.1/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.1/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.1/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.1/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.1/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.1/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.1/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.1/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.1/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.1/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.1/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.1/pih/consts/password.py
--rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36.1/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36.1/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.1/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.1/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.1/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.1/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.1/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.1/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.1/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.1/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.1/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547912 2024-04-10 06:39:42.000000 pih-0.36.1/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.583170 pih-0.36.1/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.1/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.1/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.1/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.1/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.708192 pih-0.36.1/pih/tools/
--rw-rw-rw-   0        0        0    51419 2024-04-10 09:08:04.000000 pih-0.36.1/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.1/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.1/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:23:31.755064 pih-0.36.1/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-10 09:23:28.000000 pih-0.36.1/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:23:31.849141 pih-0.36.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.835213 pih-0.36.2/
+-rw-rw-rw-   0        0        0      249 2024-04-10 10:22:39.788345 pih-0.36.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:37.013144 pih-0.36.2/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.2/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:37.381862 pih-0.36.2/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.2/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.2/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.2/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.2/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.265255 pih-0.36.2/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-10 10:21:26.000000 pih-0.36.2/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.2/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.2/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.2/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.2/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.2/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.2/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.2/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.2/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.2/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.2/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.2/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36.2/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36.2/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.2/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.2/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.2/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.2/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.2/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.2/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.2/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.2/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.2/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547814 2024-04-10 10:20:59.000000 pih-0.36.2/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.531925 pih-0.36.2/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.2/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.2/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.2/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.2/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.678990 pih-0.36.2/pih/tools/
+-rw-rw-rw-   0        0        0    51419 2024-04-10 09:08:04.000000 pih-0.36.2/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.2/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.2/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.741479 pih-0.36.2/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 10:22:36.000000 pih-0.36.2/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 10:22:39.835213 pih-0.36.2/setup.cfg
```

### Comparing `pih-0.36.1/pih/collections/__init__.py` & `pih-0.36.2/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/collections/service.py` & `pih-0.36.2/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/console_api.py` & `pih-0.36.2/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/console_api_wrapper.py` & `pih-0.36.2/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/__init__.py` & `pih-0.36.2/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.1"
+VERSION: str = "0.36.2"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36.1/pih/consts/ad.py` & `pih-0.36.2/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/addresses.py` & `pih-0.36.2/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/date_time.py` & `pih-0.36.2/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/errors.py` & `pih-0.36.2/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/events.py` & `pih-0.36.2/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/hosts.py` & `pih-0.36.2/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/names.py` & `pih-0.36.2/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/password.py` & `pih-0.36.2/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/paths.py` & `pih-0.36.2/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/polibase.py` & `pih-0.36.2/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/service.py` & `pih-0.36.2/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/service_commands.py` & `pih-0.36.2/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/service_roles.py` & `pih-0.36.2/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/consts/settings.py` & `pih-0.36.2/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/pih.py` & `pih-0.36.2/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -9079,15 +9079,15 @@
                 )
                 start_date = DateTimeTool.begin_date(start_date or now)
                 end_date = DateTimeTool.end_date(end_date or now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
                     return DataTool.check_not_none(
                         entity,
-                        lambda: entity.TimeVal.split(DATE_TIME.CONST.SPLITTER)[
+                        lambda: entity.TimeVal.split(DATE_TIME.SPLITTER)[
                             not date
                         ],
                     )
 
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
                 result_data = defaultdict(
@@ -9168,17 +9168,14 @@
                                 TimeTrackingResultByDate(
                                     date,
                                     get_date_or_time(time_tracking_enter_entity, False),
                                     get_date_or_time(time_tracking_exit_entity, False),
                                     duration,
                                 )
                             )
-                #
-                #
-                # print(has_lunch_break)
                 for division in result:
                     for person in division.list:
                         index: int = 0
                         length: int = len(person.list)
                         for _ in range(length):
                             item: TimeTrackingResultByDate = person.list[index]
                             if item.duration == 0:
@@ -9188,20 +9185,20 @@
                                         index + 1
                                     ]
                                     if nn(item.exit_time):
                                         if nn(item_next.enter_time):
                                             duration = int(
                                                 datetime.fromisoformat(
                                                     item.date
-                                                    + DATE_TIME.CONST.SPLITTER
+                                                    + DATE_TIME.SPLITTER
                                                     + item.exit_time
                                                 ).timestamp()
                                                 - datetime.fromisoformat(
                                                     item_next.date
-                                                    + DATE_TIME.CONST.SPLITTER
+                                                    + DATE_TIME.SPLITTER
                                                     + item_next.enter_time
                                                 ).timestamp()
                                             )
                                             # print(full_name, full_name in has_lunch_break)
                                             # duration -= 60*60 if (full_name in has_lunch_break) else 0
                                             item.duration = duration
                                             person.duration += duration
```

### Comparing `pih-0.36.1/pih/rpc/__init__.py` & `pih-0.36.2/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.2/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.2/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/tools/__init__.py` & `pih-0.36.2/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/tools/service.py` & `pih-0.36.2/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih/widgets.py` & `pih-0.36.2/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.1/pih.egg-info/SOURCES.txt` & `pih-0.36.2/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

