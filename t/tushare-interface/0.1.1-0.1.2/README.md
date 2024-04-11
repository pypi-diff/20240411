# Comparing `tmp/tushare_interface-0.1.1.tar.gz` & `tmp/tushare_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tushare_interface-0.1.1.tar", last modified: Thu Apr 11 13:58:14 2024, max compression
+gzip compressed data, was "tushare_interface-0.1.2.tar", last modified: Thu Apr 11 15:08:29 2024, max compression
```

## Comparing `tushare_interface-0.1.1.tar` & `tushare_interface-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)    11357 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/LICENSE
--rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/PKG-INFO
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     1131 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/README.md
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      787 2024-04-11 13:57:06.000000 tushare_interface-0.1.1/pyproject.toml
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       38 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/setup.cfg
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.877601 tushare_interface-0.1.1/src/
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.881601 tushare_interface-0.1.1/src/tushare_interface/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       62 2024-04-11 11:21:25.000000 tushare_interface-0.1.1/src/tushare_interface/__init__.py
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     6202 2024-04-11 11:16:32.000000 tushare_interface-0.1.1/src/tushare_interface/tushare_interface.py
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.885602 tushare_interface-0.1.1/src/tushare_interface.egg-info/
--rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/PKG-INFO
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      365 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)        1 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       29 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/requires.txt
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       18 2024-04-11 13:58:14.000000 tushare_interface-0.1.1/src/tushare_interface.egg-info/top_level.txt
-drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 13:58:14.881601 tushare_interface-0.1.1/tests/
--rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     5473 2024-04-11 11:28:29.000000 tushare_interface-0.1.1/tests/test_tushare_interface.py
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 15:08:29.532071 tushare_interface-0.1.2/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)    11357 2024-04-11 11:16:32.000000 tushare_interface-0.1.2/LICENSE
+-rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 15:08:29.532071 tushare_interface-0.1.2/PKG-INFO
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     1131 2024-04-11 11:16:32.000000 tushare_interface-0.1.2/README.md
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      787 2024-04-11 15:05:27.000000 tushare_interface-0.1.2/pyproject.toml
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       38 2024-04-11 15:08:29.532071 tushare_interface-0.1.2/setup.cfg
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 15:08:29.520071 tushare_interface-0.1.2/src/
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 15:08:29.528071 tushare_interface-0.1.2/src/tushare_interface/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       62 2024-04-11 11:21:25.000000 tushare_interface-0.1.2/src/tushare_interface/__init__.py
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     6202 2024-04-11 11:16:32.000000 tushare_interface-0.1.2/src/tushare_interface/tushare_interface.py
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 15:08:29.532071 tushare_interface-0.1.2/src/tushare_interface.egg-info/
+-rw-r--r--   0 ecs-user  (1000) ecs-user  (1000)     1837 2024-04-11 15:08:29.000000 tushare_interface-0.1.2/src/tushare_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)      365 2024-04-11 15:08:29.000000 tushare_interface-0.1.2/src/tushare_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)        1 2024-04-11 15:08:29.000000 tushare_interface-0.1.2/src/tushare_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       29 2024-04-11 15:08:29.000000 tushare_interface-0.1.2/src/tushare_interface.egg-info/requires.txt
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)       18 2024-04-11 15:08:29.000000 tushare_interface-0.1.2/src/tushare_interface.egg-info/top_level.txt
+drwxrwxr-x   0 ecs-user  (1000) ecs-user  (1000)        0 2024-04-11 15:08:29.532071 tushare_interface-0.1.2/tests/
+-rw-rw-r--   0 ecs-user  (1000) ecs-user  (1000)     5766 2024-04-11 14:53:28.000000 tushare_interface-0.1.2/tests/test_tushare_interface.py
```

### Comparing `tushare_interface-0.1.1/LICENSE` & `tushare_interface-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tushare_interface-0.1.1/PKG-INFO` & `tushare_interface-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tushare_interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: An interface encapsulated based on Tushare, which implements rate limiting and retry mechanisms.
 Author-email: polaritec <yuan.xin@polaritec.com>
 Project-URL: Homepage, https://github.com/polaritec/tushare-interface
 Keywords: tushare,stock
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `tushare_interface-0.1.1/README.md` & `tushare_interface-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tushare_interface-0.1.1/pyproject.toml` & `tushare_interface-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tushare_interface"
 keywords = ["tushare", "stock"]
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="polaritec", email="yuan.xin@polaritec.com" },
 ]
 description = "An interface encapsulated based on Tushare, which implements rate limiting and retry mechanisms."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `tushare_interface-0.1.1/src/tushare_interface/tushare_interface.py` & `tushare_interface-0.1.2/src/tushare_interface/tushare_interface.py`

 * *Files identical despite different names*

### Comparing `tushare_interface-0.1.1/src/tushare_interface.egg-info/PKG-INFO` & `tushare_interface-0.1.2/src/tushare_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tushare_interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: An interface encapsulated based on Tushare, which implements rate limiting and retry mechanisms.
 Author-email: polaritec <yuan.xin@polaritec.com>
 Project-URL: Homepage, https://github.com/polaritec/tushare-interface
 Keywords: tushare,stock
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `tushare_interface-0.1.1/tests/test_tushare_interface.py` & `tushare_interface-0.1.2/tests/test_tushare_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,22 @@
         # 测试前的设置工作
         pass
 
     def tearDown(self):
         # 测试后的清理工作
         pass
 
-    def test_queryOnce(self):
+    def test_00_env(self):
+        timesPerMinutusEnv = os.environ.get("TUSHARE_API_PER_MINUTUS")
+        self.assertEqual(
+            pro._InterfaceTuShare__intervalMicroSecond,
+            (60 * 1000) / int(timesPerMinutusEnv),
+        )
+
+    def test_01_queryOnce(self):
         token = os.environ.get("TUSHARE_TOKEN")
         pro.setToken(token)
 
         start_date = "20240101"
         end_date = (datetime.date.today() + datetime.timedelta(days=28)).strftime(
             "%Y%m%d"
         )
@@ -39,23 +46,23 @@
             start_date=start_date,
             end_date=end_date,
             fields="ts_code,sub_code,name,ipo_date",
             is_open="1",
         )
         self.assertIsNotNone(df)  # 使用断言方法验证预期结果
 
-    def test_setToken_1(self):
+    def test_02_setToken_1(self):
         with self.assertRaises(TypeError):
             pro.setToken(1)
 
-    def test_setToken_2(self):
+    def test_03_setToken_2(self):
         with self.assertRaises(ValueError):
             pro.setToken("1")
 
-    def test_setToken_3(self):
+    def test_04_setToken_3(self):
         pro.setToken("12345678901234567890123456789012345678901234567890123456")
         pro.setTimesPerMinutus(5)
         pro.setRetry(0, 2)
         start_date = "20240101"
         end_date = (datetime.date.today() + datetime.timedelta(days=28)).strftime(
             "%Y%m%d"
         )
@@ -65,15 +72,15 @@
             start_date=start_date,
             end_date=end_date,
             fields="ts_code,sub_code,name,ipo_date",
             is_open="1",
         )
         self.assertIsNone(df)
 
-    def test_setToken_4(self):
+    def test_05_setToken_4(self):
         token = os.environ.get("TUSHARE_TOKEN")
         pro.setToken(token)
         pro.setTimesPerMinutus(5)
         pro.setRetry(0, 2)
 
         start_date = "20240101"
         end_date = (datetime.date.today() + datetime.timedelta(days=28)).strftime(
@@ -85,55 +92,55 @@
             start_date=start_date,
             end_date=end_date,
             fields="ts_code,sub_code,name,ipo_date",
             is_open="1",
         )
         self.assertIsNotNone(df)  # 使用断言方法验证预期结果
 
-    def test_setTimesPerMinutus_1(self):
+    def test_06_setTimesPerMinutus_1(self):
         with self.assertRaises(TypeError):
             pro.setTimesPerMinutus("1")
 
-    def test_setTimesPerMinutus_2(self):
+    def test_07_setTimesPerMinutus_2(self):
         with self.assertRaises(ValueError):
             pro.setTimesPerMinutus(0)
 
-    def test_setTimesPerMinutus_3(self):
+    def test_08_setTimesPerMinutus_3(self):
         pro.setTimesPerMinutus(5)
         self.assertEqual(pro._InterfaceTuShare__intervalMicroSecond, 12 * 1000)
 
-    def test_setRetry_1(self):
+    def test_09_setRetry_1(self):
         with self.assertRaises(TypeError):
             pro.setRetry(1)
 
-    def test_setRetry_2(self):
+    def test_10_setRetry_2(self):
         with self.assertRaises(TypeError):
             pro.setRetry("1", 1)
 
-    def test_setRetry_3(self):
+    def test_11_setRetry_3(self):
         with self.assertRaises(ValueError):
             pro.setRetry(-1, 1)
 
-    def test_setRetry_4(self):
+    def test_12_setRetry_4(self):
         with self.assertRaises(TypeError):
             pro.setRetry(0, "1")
 
-    def test_setRetry_5(self):
+    def test_13_setRetry_5(self):
         with self.assertRaises(ValueError):
             pro.setRetry(-1, 0)
 
-    def test_setRetry_6(self):
+    def test_14_setRetry_6(self):
         pro.setRetry(0, 1)
         self.assertEqual(pro._InterfaceTuShare__retrys, 0)
 
-    def test_setRetry_7(self):
+    def test_15_setRetry_7(self):
         pro.setRetry(0, 1)
         self.assertEqual(pro._InterfaceTuShare__secondsWaitRetry, 1)
 
-    def test_setRetry_setTimesPerMinutus_1(self):
+    def test_16_setRetry_setTimesPerMinutus_1(self):
         token = os.environ.get("TUSHARE_TOKEN")
         pro.setToken(token)
         pro.setTimesPerMinutus(5)
         pro.setRetry(1, 1)
 
         start_date = "20240101"
         end_date = (datetime.date.today() + datetime.timedelta(days=28)).strftime(
@@ -150,15 +157,15 @@
                 is_open="1",
             )
 
         endSeconds = time.perf_counter_ns() / (1000 * 1000 * 1000)
         duration = endSeconds - startSeconds
         self.assertGreaterEqual(duration, 60)
 
-    def test_setRetry_setTimesPerMinutus_2(self):
+    def test_17_setRetry_setTimesPerMinutus_2(self):
         pro.setTimesPerMinutus(5)
         pro.setRetry(10, 2)
         pro.setToken("12345678901234567890123456789012345678901234567890123456")
 
         start_date = "20240101"
         end_date = (datetime.date.today() + datetime.timedelta(days=28)).strftime(
             "%Y%m%d"
```

