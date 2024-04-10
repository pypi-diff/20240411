# Comparing `tmp/cadcutils-1.5.1.3.tar.gz` & `tmp/cadcutils-1.5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadcutils-1.5.1.3.tar", last modified: Fri Apr  5 21:00:41 2024, max compression
+gzip compressed data, was "cadcutils-1.5.1.4.tar", last modified: Wed Apr 10 23:45:24 2024, max compression
```

## Comparing `cadcutils-1.5.1.3.tar` & `cadcutils-1.5.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.003358 cadcutils-1.5.1.3/cadcutils/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.003358 cadcutils-1.5.1.3/cadcutils/net/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9055 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/group_xml/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/group_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_user_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/user_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/group_xml/user_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29291 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/groups_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/netutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.007358 cadcutils-1.5.1.3/cadcutils/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_groups_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_int_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_netutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    64620 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/tests/test_wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55249 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/ws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12263 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/net/wscapabilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8457 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/old_get_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/cadcutils/util/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/cadcutils/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/cadcutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 21:00:40.000000 cadcutils-1.5.1.3/cadcutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-05 21:00:41.011358 cadcutils-1.5.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-05 21:00:37.000000 cadcutils-1.5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.574341 cadcutils-1.5.1.4/cadcutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.574341 cadcutils-1.5.1.4/cadcutils/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14480 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9055 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.574341 cadcutils-1.5.1.4/cadcutils/net/group_xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/group_property_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/group_property_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/group_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/group_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/groups_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/groups_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_group_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_groups_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_user_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/user_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/group_xml/user_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29291 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/netutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/cadcutils/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_groups_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_int_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_netutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64620 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/tests/test_wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55249 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/ws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12263 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/net/wscapabilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8457 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/old_get_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/cadcutils/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/cadcutils/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 23:45:23.000000 cadcutils-1.5.1.4/cadcutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:45:24.578341 cadcutils-1.5.1.4/cadcutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 23:45:24.000000 cadcutils-1.5.1.4/cadcutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-10 23:45:24.582341 cadcutils-1.5.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-10 23:45:20.000000 cadcutils-1.5.1.4/setup.py
```

### Comparing `cadcutils-1.5.1.3/LICENSE` & `cadcutils-1.5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/PKG-INFO` & `cadcutils-1.5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.1.3
+Version: 1.5.1.4
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.1.3/README.rst` & `cadcutils-1.5.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/exceptions.py` & `cadcutils-1.5.1.4/cadcutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/__init__.py` & `cadcutils-1.5.1.4/cadcutils/net/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/auth.py` & `cadcutils-1.5.1.4/cadcutils/net/auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group.py` & `cadcutils-1.5.1.4/cadcutils/net/group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/__init__.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_reader.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/group_property_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_property_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/group_property_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_reader.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/group_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/group_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/group_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_reader.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/groups_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/groups_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/groups_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_group_property_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_group_reader_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_group_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_groups_reader_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_groups_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/tests/test_user_reader_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/tests/test_user_reader_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/user_reader.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/user_reader.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/group_xml/user_writer.py` & `cadcutils-1.5.1.4/cadcutils/net/group_xml/user_writer.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/groups_client.py` & `cadcutils-1.5.1.4/cadcutils/net/groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/netutils.py` & `cadcutils-1.5.1.4/cadcutils/net/netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_auth.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_group.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_groups_client.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_groups_client.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_int_groups.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_int_groups.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_netutils.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_netutils.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_ws.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/tests/test_wscapabilities.py` & `cadcutils-1.5.1.4/cadcutils/net/tests/test_wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/ws.py` & `cadcutils-1.5.1.4/cadcutils/net/ws.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/net/wscapabilities.py` & `cadcutils-1.5.1.4/cadcutils/net/wscapabilities.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/old_get_cert.py` & `cadcutils-1.5.1.4/cadcutils/old_get_cert.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/util/__init__.py` & `cadcutils-1.5.1.4/cadcutils/util/__init__.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/util/config.py` & `cadcutils-1.5.1.4/cadcutils/util/config.py`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/cadcutils/util/utils.py` & `cadcutils-1.5.1.4/cadcutils/util/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,13 +599,19 @@
                 continue
         strict_versions.sort()
     except Exception as e:
         logger.debug(
             'Unexpected exception in PyPI version checking: {}'.format(str(e)))
         pass
     if strict_versions and current_version < strict_versions[-1]:
+        current_warn_formatting = warnings.formatwarning
+        warnings.formatwarning = lambda message, *ignore: 'WARNING: {}\n'.format(message)
         warnings.warn('Current version {}. A newer version, {}, '
-                      'is available on PyPI'.format(version, strict_versions[-1]),
+                      'is available on PyPI'.format(version,
+                                                    strict_versions[-1]),
                       category=VersionWarning)
+        sys.stdout.flush()
+        sys.stderr.flush()
+        warnings.formatwarning = current_warn_formatting
 
 
 check_version.checked = []  # packages already checked
```

### Comparing `cadcutils-1.5.1.3/cadcutils.egg-info/PKG-INFO` & `cadcutils-1.5.1.4/cadcutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadcutils
-Version: 1.5.1.3
+Version: 1.5.1.4
 Summary: Generic CADC Python libary of utilities
 Home-page: http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 Author: Canadian Astronomy Data Centre
 Author-email: cadc@nrc-cnrc.gc.ca
 License: AGPLv3
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `cadcutils-1.5.1.3/cadcutils.egg-info/SOURCES.txt` & `cadcutils-1.5.1.4/cadcutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cadcutils-1.5.1.3/setup.cfg` & `cadcutils-1.5.1.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 long_description = Library of utilities. It includes generic utilities for logging and command line parsing, networking utilities, etc.
 author = Canadian Astronomy Data Centre
 author_email = cadc@nrc-cnrc.gc.ca
 license = AGPLv3
 url = http://www.cadc-ccda.hia-iha.nrc-cnrc.gc.ca
 edit_on_github = False
 github_project = opencadc/cadctools
-version = 1.5.1.3
+version = 1.5.1.4
 
 [options]
 install_requires = 
 	setuptools>=36.0
 	requests>=2.8
 	lxml>=3.7.0
 	html2text
```

### Comparing `cadcutils-1.5.1.3/setup.py` & `cadcutils-1.5.1.4/setup.py`

 * *Files identical despite different names*

