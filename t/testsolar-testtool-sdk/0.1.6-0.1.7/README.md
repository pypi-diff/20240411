# Comparing `tmp/testsolar-testtool-sdk-0.1.6.tar.gz` & `tmp/testsolar-testtool-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.1.6.tar", last modified: Wed Apr 10 10:00:29 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.1.7.tar", last modified: Wed Apr 10 12:23:35 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.1.6.tar` & `testsolar-testtool-sdk-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.447548 testsolar-testtool-sdk-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 10:00:29.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 10:00:29.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:00:29.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 10:00:29.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 10:00:29.000000 testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:00:29.451548 testsolar-testtool-sdk-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-10 10:00:05.000000 testsolar-testtool-sdk-0.1.6/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.104102 testsolar-testtool-sdk-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 12:23:35.104102 testsolar-testtool-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:23:35.104102 testsolar-testtool-sdk-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.100103 testsolar-testtool-sdk-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.100103 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.100103 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.104102 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 12:23:35.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 12:23:35.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:23:35.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 12:23:35.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 12:23:35.000000 testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:23:35.100103 testsolar-testtool-sdk-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-10 12:23:11.000000 testsolar-testtool-sdk-0.1.7/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1.6/LICENSE` & `testsolar-testtool-sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk/reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
     def report_load_result(self, load_result: LoadResult) -> None:
         with portalocker.Lock(self.lock_file, timeout=60):
             self._send_json(dataclasses.asdict(load_result))
 
-    def report_run_case_result(self, run_case_result: TestResult) -> None:
+    def report_case_result(self, case_result: TestResult) -> None:
         with portalocker.Lock(self.lock_file, timeout=60):
-            self._send_json(dataclasses.asdict(run_case_result))
+            self._send_json(dataclasses.asdict(case_result))
 
     def close(self) -> None:
         if self.pipe_io:
             self.pipe_io.close()
 
     def _send_json(self, result: dict) -> None:
         data = json.dumps(result, cls=DateTimeEncoder).encode('utf-8')
```

### Comparing `testsolar-testtool-sdk-0.1.6/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.1.7/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.6/tests/test_report.py` & `testsolar-testtool-sdk-0.1.7/tests/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         assert loaded == load_result
 
 
 def send_test_result(reporter: Reporter):
     test_results = []
     run_case_result = generate_test_result(0)
     test_results.append(run_case_result)
-    reporter.report_run_case_result(run_case_result)
+    reporter.report_case_result(run_case_result)
 
 
 def test_datetime_formatted():
     run_case_result = generate_test_result(0)
     data = json.dumps(dataclasses.asdict(run_case_result), cls=DateTimeEncoder)
     tr = json.loads(data)
     assert tr['StartTime'].endswith("Z")
```

