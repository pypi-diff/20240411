# Comparing `tmp/pih-event-0.11.tar.gz` & `tmp/pih-event-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-event-0.11.tar", last modified: Wed Mar 13 14:08:06 2024, max compression
+gzip compressed data, was "pih-event-0.12.tar", last modified: Wed Apr 10 01:40:45 2024, max compression
```

## Comparing `pih-event-0.11.tar` & `pih-event-0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:08:07.052575 pih-event-0.11/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:08:06.630718 pih-event-0.11/EventService/
--rw-rw-rw-   0        0        0       26 2024-02-15 08:19:09.000000 pih-event-0.11/EventService/__init__.py
--rw-rw-rw-   0        0        0      147 2024-02-15 07:53:14.000000 pih-event-0.11/EventService/__main__.py
--rw-rw-rw-   0        0        0     5816 2024-03-08 08:58:19.000000 pih-event-0.11/EventService/api.py
--rw-rw-rw-   0        0        0      573 2024-03-13 14:07:35.000000 pih-event-0.11/EventService/const.py
--rw-rw-rw-   0        0        0     1986 2024-03-13 14:07:46.000000 pih-event-0.11/EventService/service.py
--rw-rw-rw-   0        0        0      305 2024-03-13 14:08:07.021320 pih-event-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 14:08:06.990075 pih-event-0.11/pih_event.egg-info/
--rw-rw-rw-   0        0        0      305 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-13 14:08:06.000000 pih-event-0.11/pih_event.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 14:08:07.068213 pih-event-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:40:45.664478 pih-event-0.12/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:40:45.217645 pih-event-0.12/EventService/
+-rw-rw-rw-   0        0        0       26 2024-02-15 08:19:09.000000 pih-event-0.12/EventService/__init__.py
+-rw-rw-rw-   0        0        0      147 2024-02-15 07:53:14.000000 pih-event-0.12/EventService/__main__.py
+-rw-rw-rw-   0        0        0     5816 2024-03-08 08:58:19.000000 pih-event-0.12/EventService/api.py
+-rw-rw-rw-   0        0        0      573 2024-04-10 00:00:18.000000 pih-event-0.12/EventService/const.py
+-rw-rw-rw-   0        0        0     1986 2024-03-13 14:07:46.000000 pih-event-0.12/EventService/service.py
+-rw-rw-rw-   0        0        0      305 2024-04-10 01:40:45.633227 pih-event-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:40:45.598511 pih-event-0.12/pih_event.egg-info/
+-rw-rw-rw-   0        0        0      305 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 01:40:44.000000 pih-event-0.12/pih_event.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:40:45.664478 pih-event-0.12/setup.cfg
```

### Comparing `pih-event-0.11/EventService/api.py` & `pih-event-0.12/EventService/api.py`

 * *Files identical despite different names*

### Comparing `pih-event-0.11/EventService/const.py` & `pih-event-0.12/EventService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Event"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.11"
+VERSION: str = "0.12"
 
 CONFIG_FOLDER_NAME: str = "telegram_send_config"
 
 PACKAGES: tuple[str, ...] = ("telegram-send",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-event-0.11/EventService/service.py` & `pih-event-0.12/EventService/service.py`

 * *Files identical despite different names*

