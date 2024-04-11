# Comparing `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020.tar.gz` & `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020.tar", last modified: Thu Apr 11 11:59:03 2024, max compression
+gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572.tar", last modified: Thu Apr 11 12:07:16 2024, max compression
```

## Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020.tar` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 11:57:47.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 11:57:47.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-11 11:57:47.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-11 11:58:41.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-11 11:57:47.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 11:59:03.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 12:05:58.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 12:05:58.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-11 12:05:58.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:07:15.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:07:15.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-11 12:06:53.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-11 12:05:58.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-11 12:07:15.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-11 12:07:15.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-11 12:07:15.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 12:07:16.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/PKG-INFO` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_uiframework_win_demo
-Version: 1.3.0.dev8646259020
+Version: 1.3.0.dev8646358572
 Summary: th2_grpc_act_uiframework_win_demo
 Home-page: https://github.com/th2-net/th2-grpc-act-uiframework-win-demo
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: ## th2-grpc-act-ui-framework-demo (1.3.0)
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/setup.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-uiframework-win-demo
-Version: 1.3.0.dev8646259020
+Version: 1.3.0.dev8646358572
 Summary: th2_grpc_act_uiframework_win_demo
 Home-page: https://github.com/th2-net/th2-grpc-act-uiframework-win-demo
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: ## th2-grpc-act-ui-framework-demo (1.3.0)
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646259020/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8646358572/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

