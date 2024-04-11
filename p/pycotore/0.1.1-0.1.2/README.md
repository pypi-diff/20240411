# Comparing `tmp/pycotore-0.1.1.tar.gz` & `tmp/pycotore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.1.1.tar", max compression
+gzip compressed data, was "pycotore-0.1.2.tar", max compression
```

## Comparing `pycotore-0.1.1.tar` & `pycotore-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.1/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.1/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.1/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.1/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.1/pycotore/logger.py
--rw-r--r--   0        0        0     5079 2024-04-11 06:34:59.472616 pycotore-0.1.1/pycotore/progress.py
--rw-r--r--   0        0        0      597 2024-04-11 06:39:34.676105 pycotore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.2/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.2/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.2/pycotore/constants.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.2/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.2/pycotore/logger.py
+-rw-r--r--   0        0        0     5196 2024-04-11 09:37:50.889172 pycotore-0.1.2/pycotore/progress.py
+-rw-r--r--   0        0        0      597 2024-04-11 08:46:30.043071 pycotore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.2/PKG-INFO
```

### Comparing `pycotore-0.1.1/LICENSE` & `pycotore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.1/pycotore/logger.py` & `pycotore-0.1.2/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.1/pycotore/progress.py` & `pycotore-0.1.2/pycotore/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,32 +44,30 @@
         self.run_time = "|RUN: 00:00:00"
         self.show_runtime: bool = show_runtime
 
     def flush_line(self) -> None:
         sys.stdout.write("\n")
         sys.stdout.flush()
 
-    def __clear_line(self, line) -> None:
-        sys.stdout.write("\033[K")
-        sys.stdout.flush()
-
     def __update_terminal_size(self) -> None:
         self.terminal_size = os.get_terminal_size().columns
         self.__update_bar_length()
 
     def __update_run_time(self) -> None:
         now = datetime.now()
         run_time = now - self.time_start
         self.run_time = f"|RUN: {run_time.seconds // 3600:0>2}:{run_time.seconds // 60:0>2}:{run_time.seconds % 60:0>2}"
 
     def __calculate_estimate(self) -> None:
         now = datetime.now()
         run_time = now - self.time_start
-        left = self.total * run_time / self.progress - run_time
-        self.estimate = f"|ETA: {left.seconds // 3600:0>2}:{left.seconds // 60:0>2}:{left.seconds % 60:0>2}"
+        run_data_left = self.total - self.progress
+        run_avg_speed = int(self.progress // run_time.total_seconds())
+        run_estimate = int(run_data_left // run_avg_speed)
+        self.estimate = f"|ETA: {run_estimate // 3600:0>2}:{run_estimate // 60:0>2}:{run_estimate % 60:0>2}"
 
     def __update_percent_done(self) -> None:
         percents = round(self.progress * 100 / self.total, 2)
         self.percents = f"{percents:0>6.2f}%"
 
     def __update_bar_length(self) -> None:
         """
@@ -156,7 +154,11 @@
         Set progress bar total value
         """
         try:
             if float(total):
                 self.total = total
         except ValueError:
             _logger.warning("Unable to set total")
+
+    def __clear_line(self, line) -> None:
+        sys.stdout.write("\033[K")
+        sys.stdout.flush()
```

### Comparing `pycotore-0.1.1/pyproject.toml` & `pycotore-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Generic classes for reuse"
-version = "0.1.1"
+version = "0.1.2"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.1.1/PKG-INFO` & `pycotore-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

