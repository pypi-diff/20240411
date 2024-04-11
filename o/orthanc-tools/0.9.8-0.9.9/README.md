# Comparing `tmp/orthanc_tools-0.9.8.tar.gz` & `tmp/orthanc_tools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_tools-0.9.8.tar", last modified: Thu Oct  5 11:56:16 2023, max compression
+gzip compressed data, was "orthanc_tools-0.9.9.tar", last modified: Mon Nov  6 08:28:43 2023, max compression
```

## Comparing `orthanc_tools-0.9.8.tar` & `orthanc_tools-0.9.9.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.807905 orthanc_tools-0.9.8/orthanc_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/orthanc_tools/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/helpers/old_files_deleter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/helpers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/helpers/time_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_message_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_report_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_cloner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17647 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_folder_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19250 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/orthanc_test_db_populator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16767 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/orthanc_tools/pacs_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/orthanc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2023-10-05 11:56:16.000000 orthanc_tools-0.9.8/orthanc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-10-05 11:56:16.000000 orthanc_tools-0.9.8/orthanc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 11:56:16.000000 orthanc_tools-0.9.8/orthanc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-05 11:56:16.000000 orthanc_tools-0.9.8/orthanc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-05 11:56:16.000000 orthanc_tools-0.9.8/orthanc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-05 11:56:16.815905 orthanc_tools-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 11:56:16.811905 orthanc_tools-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23838 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/tests/test_3_orthancs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-10-05 11:53:40.000000 orthanc_tools-0.9.8/tests/test_old_files_deleter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.933244 orthanc_tools-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2023-11-06 08:28:43.933244 orthanc_tools-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.929244 orthanc_tools-0.9.9/orthanc_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.929244 orthanc_tools-0.9.9/orthanc_tools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/helpers/old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/helpers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/helpers/time_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.933244 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_message_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_report_series_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_worklist_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_cloner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17647 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_folder_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19250 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/orthanc_test_db_populator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16767 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/orthanc_tools/pacs_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.929244 orthanc_tools-0.9.9/orthanc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2023-11-06 08:28:43.000000 orthanc_tools-0.9.9/orthanc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-11-06 08:28:43.000000 orthanc_tools-0.9.9/orthanc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 08:28:43.000000 orthanc_tools-0.9.9/orthanc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-06 08:28:43.000000 orthanc_tools-0.9.9/orthanc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-06 08:28:43.000000 orthanc_tools-0.9.9/orthanc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-06 08:28:43.933244 orthanc_tools-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 08:28:43.933244 orthanc_tools-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23847 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/tests/test_3_orthancs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/tests/test_old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2023-11-06 08:25:30.000000 orthanc_tools-0.9.9/tests/test_orthanc_replicator.py
```

### Comparing `orthanc_tools-0.9.8/LICENSE.txt` & `orthanc_tools-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/PKG-INFO` & `orthanc_tools-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc_tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
@@ -17,19 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
-Requires-Dist: orthanc-api-client>=0.13.7
+Requires-Dist: orthanc-api-client>=0.14.2
 Requires-Dist: pydicom>=2.3.1
 Requires-Dist: hl7==0.4.2
 Requires-Dist: six
 Requires-Dist: schedule==1.2.0
+Requires-Dist: pika
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `orthanc_tools-0.9.8/README.md` & `orthanc_tools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/__init__.py` & `orthanc_tools-0.9.9/orthanc_tools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .orthanc_folder_importer import *
 from .orthanc_forwarder import *
 from .orthanc_monitor import OrthancMonitor
 from .orthanc_test_db_populator import OrthancTestDbPopulator
 from .pacs_migrator import PacsMigrator
 from .orthanc_comparator import OrthancComparator
 from .orthanc_cleaner import OrthancCleaner
+from .orthanc_replicator import OrthancReplicator
 
 from .hl7Lib import *
 from .helpers import *
 
 # Set default logging handler to avoid "No handler found" warnings.
 import logging
 from logging import NullHandler
```

### Comparing `orthanc_tools-0.9.8/orthanc_tools/helpers/old_files_deleter.py` & `orthanc_tools-0.9.9/orthanc_tools/helpers/old_files_deleter.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/helpers/scheduler.py` & `orthanc_tools-0.9.9/orthanc_tools/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/helpers/time_out.py` & `orthanc_tools-0.9.9/orthanc_tools/helpers/time_out.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/helpers/timer.py` & `orthanc_tools-0.9.9/orthanc_tools/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/__init__.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_client.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_error.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_error.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_message_parser.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_message_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_message_validator.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_message_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import typing
-import socketserver, subprocess, sys, re, socket
-from threading import Thread
-import hl7
+import re
 
-
-class Hl7MessageValidator():
+class Hl7MessageValidator:
     """
     This class validates the structure of HL7 message (it actually only checks the start/end chars and line splits)
     and returns a string with the real message.
     """
 
     def __init__(self, encoding: str = 'iso-8859-1', sb: bytes = b'\x0b', eb: bytes = b'\x1c', cr: bytes = b'\r'):
         self.encoding = encoding
```

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_report_parser.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_report_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_report_series_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_server.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_server.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py` & `orthanc_tools-0.9.9/orthanc_tools/hl7Lib/hl7_worklist_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_cleaner.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_cleaner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_cloner.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_cloner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_comparator.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_comparator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_folder_importer.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_folder_importer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_forwarder.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_forwarder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_monitor.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_monitor.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/orthanc_test_db_populator.py` & `orthanc_tools-0.9.9/orthanc_tools/orthanc_test_db_populator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools/pacs_migrator.py` & `orthanc_tools-0.9.9/orthanc_tools/pacs_migrator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.9.8/orthanc_tools.egg-info/PKG-INFO` & `orthanc_tools-0.9.9/orthanc_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
@@ -17,19 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
-Requires-Dist: orthanc-api-client>=0.13.7
+Requires-Dist: orthanc-api-client>=0.14.2
 Requires-Dist: pydicom>=2.3.1
 Requires-Dist: hl7==0.4.2
 Requires-Dist: six
 Requires-Dist: schedule==1.2.0
+Requires-Dist: pika
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `orthanc_tools-0.9.8/orthanc_tools.egg-info/SOURCES.txt` & `orthanc_tools-0.9.9/orthanc_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 orthanc_tools/__init__.py
 orthanc_tools/orthanc_cleaner.py
 orthanc_tools/orthanc_cloner.py
 orthanc_tools/orthanc_comparator.py
 orthanc_tools/orthanc_folder_importer.py
 orthanc_tools/orthanc_forwarder.py
 orthanc_tools/orthanc_monitor.py
+orthanc_tools/orthanc_replicator.py
 orthanc_tools/orthanc_test_db_populator.py
 orthanc_tools/pacs_migrator.py
 orthanc_tools.egg-info/PKG-INFO
 orthanc_tools.egg-info/SOURCES.txt
 orthanc_tools.egg-info/dependency_links.txt
 orthanc_tools.egg-info/requires.txt
 orthanc_tools.egg-info/top_level.txt
@@ -34,8 +35,9 @@
 orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
 orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
 orthanc_tools/hl7Lib/hl7_report_parser.py
 orthanc_tools/hl7Lib/hl7_report_series_builder.py
 orthanc_tools/hl7Lib/hl7_server.py
 orthanc_tools/hl7Lib/hl7_worklist_parser.py
 tests/test_3_orthancs.py
-tests/test_old_files_deleter.py
+tests/test_old_files_deleter.py
+tests/test_orthanc_replicator.py
```

### Comparing `orthanc_tools-0.9.8/release-notes.md` & `orthanc_tools-0.9.9/release-notes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v 0.9.9
+=======
+- added `OrthancReplicator`
+
 v 0.9.8
 =======
 - `OrthancForwarder`: added 2 callbacks `on_instances_set_forwarded` and `on_instances_set_forward_error`
 
 v 0.9.7
 =======
 - `PacsMigrator`: fixed arg bug (exit_on_error)
```

### Comparing `orthanc_tools-0.9.8/setup.py` & `orthanc_tools-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.9.8',  # Required
+    version='0.9.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc Tools',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -126,19 +126,20 @@
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
         'requests',
-        'orthanc-api-client>=0.13.7',
+        'orthanc-api-client>=0.14.2',
         'pydicom>=2.3.1',
         'hl7==0.4.2',
         'six',
-        'schedule==1.2.0'
+        'schedule==1.2.0',
+        'pika'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
```

### Comparing `orthanc_tools-0.9.8/tests/test_3_orthancs.py` & `orthanc_tools-0.9.9/tests/test_3_orthancs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 forwarder_count_failed = 0
 forwarder_count_success = 0
 
 class Test3Orthancs(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
-        subprocess.run(["docker-compose", "down", "-v"], cwd=here/"docker-setup")
-        subprocess.run(["docker-compose", "up", "-d"], cwd=here/"docker-setup")
+        subprocess.run(["docker", "compose", "down", "-v"], cwd=here/"docker-setup")
+        subprocess.run(["docker", "compose", "up", "-d"], cwd=here/"docker-setup")
 
         cls.oa = OrthancApiClient('http://localhost:10042', user='test', pwd='test')
         cls.oa.wait_started()
         cls.ob = OrthancApiClient('http://localhost:10043', user='test', pwd='test')
         cls.ob.wait_started()
         cls.oc = OrthancApiClient('http://localhost:10044', user='test', pwd='test')
         cls.oc.wait_started()
 
     @classmethod
     def tearDownClass(cls):
-        subprocess.run(["docker-compose", "down", "-v"], cwd=here/"docker-setup")
+        subprocess.run(["docker", "compose", "down", "-v"], cwd=here/"docker-setup")
 
     def test_cloner_default(self):
         self.oa.delete_all_content()
         self.ob.delete_all_content()
 
         self.oa.upload_file(here / "stimuli/CT_small.dcm")
```

### Comparing `orthanc_tools-0.9.8/tests/test_old_files_deleter.py` & `orthanc_tools-0.9.9/tests/test_old_files_deleter.py`

 * *Files identical despite different names*

