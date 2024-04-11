# Comparing `tmp/lazy_main-0.1.2.tar.gz` & `tmp/lazy_main-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_main-0.1.2.tar", max compression
+gzip compressed data, was "lazy_main-0.1.3.tar", max compression
```

## Comparing `lazy_main-0.1.2.tar` & `lazy_main-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      789 2024-03-27 01:42:39.964025 lazy_main-0.1.2/README.md
--rw-r--r--   0        0        0       32 2024-03-21 06:24:25.541134 lazy_main-0.1.2/lazy_main/__init__.py
--rw-r--r--   0        0        0     2053 2024-03-27 01:41:06.184883 lazy_main-0.1.2/lazy_main/lazy_main.py
--rw-r--r--   0        0        0      277 2024-03-27 01:38:11.134642 lazy_main-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 lazy_main-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      789 2024-03-27 01:42:39.964025 lazy_main-0.1.3/README.md
+-rw-r--r--   0        0        0       32 2024-03-21 06:24:25.541134 lazy_main-0.1.3/lazy_main/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-11 06:26:22.699016 lazy_main-0.1.3/lazy_main/lazy_main.py
+-rw-r--r--   0        0        0      277 2024-04-11 06:26:43.010839 lazy_main-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 lazy_main-0.1.3/PKG-INFO
```

### Comparing `lazy_main-0.1.2/README.md` & `lazy_main-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lazy_main-0.1.2/lazy_main/lazy_main.py` & `lazy_main-0.1.3/lazy_main/lazy_main.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,33 +6,43 @@
 
 class LazyMain:
     def __init__(
         self,
         main: Callable[..., bool],
         error_handler: Callable[[Exception], None] = None,  # type: ignore
         print_logs: bool = True,
-        sleep_min=3,
-        sleep_max=5,
-        loop_count=-1,
+        sleep_min: int = 3,
+        sleep_max: int = 5,
+        loop_count: int = -1,
+        run_once: bool = None,  # type: ignore
+        run_forever: bool = None,  # type: ignore
     ):
         """
         main: The function that will be called every loop.
         error_handler: If the `main` function throws an error, this will be called.
         print_logs: If it should print logs.
         sleep_min: Minimum sleep time, in seconds.
         sleep_max: Maximum sleep time, in seconds.
-        loop_count: How many times this will loop. If -1, it will infinitely loop.
+        loop_count: How many times this will loop. If `-1` or less, it will infinitely loop.
+        run_once: If `true`, the `main` function will only run once, otherwise it will run forever.
+        run_forever: If `true`, the `main` function will run forever, otherwise it will only run once.
         """
         self.main = main
         self.error_handler = error_handler
         self.print_logs = print_logs
         self.sleep_min = sleep_min
         self.sleep_max = sleep_max
         self.loop_count = loop_count
 
+        if run_once != None:
+            self.loop_count = 1 if run_once else -1
+
+        elif run_forever != None:
+            self.loop_count = -1 if run_forever else 1
+
     def __get_sleep_time(self):
         return random() * self.sleep_min + self.sleep_max - self.sleep_min
 
     def run(self, *args, **kwargs):
         """
         Starts the loop.
         """
```

### Comparing `lazy_main-0.1.2/PKG-INFO` & `lazy_main-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-main
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Mister Nyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

