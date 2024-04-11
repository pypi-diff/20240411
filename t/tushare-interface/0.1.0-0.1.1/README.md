# Comparing `tmp/tushare-interface-0.1.0.tar.gz` & `tmp/tushare_interface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tushare-interface-0.1.0.tar", last modified: Thu Apr 11 10:43:36 2024, max compression
+gzip compressed data, was "tushare_interface-0.1.1.tar", last modified: Thu Apr 11 13:58:14 2024, max compression
```

## Comparing `tushare-interface-0.1.0.tar` & `tushare_interface-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 10:43:36.658603 tushare-interface-0.1.0/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)    11357 2024-04-11 04:15:48.000000 tushare-interface-0.1.0/LICENSE
--rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1807 2024-04-11 10:43:36.658603 tushare-interface-0.1.0/PKG-INFO
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     1131 2024-04-11 04:15:48.000000 tushare-interface-0.1.0/README.md
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       38 2024-04-11 10:43:36.658603 tushare-interface-0.1.0/setup.cfg
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     1049 2024-04-11 10:42:38.000000 tushare-interface-0.1.0/setup.py
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 10:43:36.650603 tushare-interface-0.1.0/test/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     5200 2024-04-11 09:53:20.000000 tushare-interface-0.1.0/test/test_tushare_interface.py
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 10:43:36.654603 tushare-interface-0.1.0/tushare_interface/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 09:49:11.000000 tushare-interface-0.1.0/tushare_interface/__init__.py
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     6202 2024-04-11 09:49:11.000000 tushare-interface-0.1.0/tushare_interface/tushare_interface.py
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 10:43:36.654603 tushare-interface-0.1.0/tushare_interface.egg-info/
--rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1807 2024-04-11 10:43:36.000000 tushare-interface-0.1.0/tushare_interface.egg-info/PKG-INFO
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      330 2024-04-11 10:43:36.000000 tushare-interface-0.1.0/tushare_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)        1 2024-04-11 10:43:36.000000 tushare-interface-0.1.0/tushare_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       29 2024-04-11 10:43:36.000000 tushare-interface-0.1.0/tushare_interface.egg-info/requires.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       18 2024-04-11 10:43:36.000000 tushare-interface-0.1.0/tushare_interface.egg-info/top_level.txt
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)    11357 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/LICENSE
+-rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/PKG-INFO
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     1131 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/README.md
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      787 2024-04-11 13:57:06.000000 tushare_interface-0.1.1/pyproject.toml
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       38 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/setup.cfg
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.877601 tushare_interface-0.1.1/src/
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.881601 tushare_interface-0.1.1/src/tushare_interface/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       62 2024-04-11 11:21:25.000000 tushare_interface-0.1.1/src/tushare_interface/__init__.py
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     6202 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/src/tushare_interface/tushare_interface.py
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/src/tushare_interface.egg-info/
+-rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      365 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)        1 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       29 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/requires.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       18 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/top_level.txt
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.881601 tushare_interface-0.1.1/tests/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     5473 2024-04-11 11:28:29.000000 tushare_interface-0.1.1/tests/test_tushare_interface.py
```

### Comparing `tushare-interface-0.1.0/LICENSE` & `tushare_interface-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tushare-interface-0.1.0/PKG-INFO` & `tushare_interface-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: tushare-interface
-Version: 0.1.0
+Name: tushare_interface
+Version: 0.1.1
 Summary: An interface encapsulated based on Tushare, which implements rate limiting and retry mechanisms.
-Home-page: https://github.com/polaritec/tushare-interface
-Author: polaritec
-Author-email: yuan.xin@polaritec.com
+Author-email: polaritec <yuan.xin@polaritec.com>
+Project-URL: Homepage, https://github.com/polaritec/tushare-interface
+Keywords: tushare,stock
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tushare-interface-0.1.0/README.md` & `tushare_interface-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tushare-interface-0.1.0/test/test_tushare_interface.py` & `tushare_interface-0.1.1/tests/test_tushare_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import unittest
 import datetime
 import os
 import time
+import sys
+from pathlib import Path
 
-from tushare_interface.tushare_interface import interfaceTuShare as pro
+# 获取当前文件的绝对路径
+current_path = Path(__file__).resolve().parent
+# 构造src目录的绝对路径
+src_path = current_path.parent / "src"
+
+# 将src目录添加到sys.path中
+sys.path.append(str(src_path))
+
+from tushare_interface.tushare_interface import interfaceTuShare as pro  # noqa: E402
 
 
 class MyTest(unittest.TestCase):
     def setUp(self):
         # 测试前的设置工作
         pass
```

### Comparing `tushare-interface-0.1.0/tushare_interface/tushare_interface.py` & `tushare_interface-0.1.1/src/tushare_interface/tushare_interface.py`

 * *Files identical despite different names*

### Comparing `tushare-interface-0.1.0/tushare_interface.egg-info/PKG-INFO` & `tushare_interface-0.1.1/src/tushare_interface.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: tushare-interface
-Version: 0.1.0
+Name: tushare_interface
+Version: 0.1.1
 Summary: An interface encapsulated based on Tushare, which implements rate limiting and retry mechanisms.
-Home-page: https://github.com/polaritec/tushare-interface
-Author: polaritec
-Author-email: yuan.xin@polaritec.com
+Author-email: polaritec <yuan.xin@polaritec.com>
+Project-URL: Homepage, https://github.com/polaritec/tushare-interface
+Keywords: tushare,stock
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

