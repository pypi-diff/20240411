# Comparing `tmp/pycotore-0.1.0.tar.gz` & `tmp/pycotore-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.1.0.tar", max compression
+gzip compressed data, was "pycotore-0.1.1.tar", max compression
```

## Comparing `pycotore-0.1.0.tar` & `pycotore-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.0/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.0/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.0/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.0/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.0/pycotore/logger.py
--rw-r--r--   0        0        0     5004 2024-04-10 17:31:42.465918 pycotore-0.1.0/pycotore/progress.py
--rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.1/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.1/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.1/pycotore/constants.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.1/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.1/pycotore/logger.py
+-rw-r--r--   0        0        0     5079 2024-04-11 06:34:59.472616 pycotore-0.1.1/pycotore/progress.py
+-rw-r--r--   0        0        0      597 2024-04-11 06:39:34.676105 pycotore-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.1/PKG-INFO
```

### Comparing `pycotore-0.1.0/LICENSE` & `pycotore-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.0/pycotore/logger.py` & `pycotore-0.1.1/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.1.0/pycotore/progress.py` & `pycotore-0.1.1/pycotore/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 
 class ProgressBar():
     """
     Progress bar class
     """
 
+    show_suffix: bool = True
+    show_preffix: bool = True
+    show_bar: bool = True
+
     def __init__(
                 self,
                 base_marker: str = ".",
                 done_marke: str = "#",
                 current_marker: str = ">",
                 show_percents: bool = True,
                 show_estimate: bool = True,
@@ -40,17 +44,21 @@
         self.run_time = "|RUN: 00:00:00"
         self.show_runtime: bool = show_runtime
 
     def flush_line(self) -> None:
         sys.stdout.write("\n")
         sys.stdout.flush()
 
-    def __str__(self):
-        bar = f"prefix: {self.preffix}\nsufix: {self.suffix}\nbar size: {self.bar_length}\ncurrent terminal: {self.terminal_size}\nbar size: {self.bar_size}\nMarker: {self.done_marker}\ntotal: {self.total}\nprogress: {self.progress}"
-        return bar
+    def __clear_line(self, line) -> None:
+        sys.stdout.write("\033[K")
+        sys.stdout.flush()
+
+    def __update_terminal_size(self) -> None:
+        self.terminal_size = os.get_terminal_size().columns
+        self.__update_bar_length()
 
     def __update_run_time(self) -> None:
         now = datetime.now()
         run_time = now - self.time_start
         self.run_time = f"|RUN: {run_time.seconds // 3600:0>2}:{run_time.seconds // 60:0>2}:{run_time.seconds % 60:0>2}"
 
     def __calculate_estimate(self) -> None:
@@ -64,55 +72,55 @@
         self.percents = f"{percents:0>6.2f}%"
 
     def __update_bar_length(self) -> None:
         """
         Updating progress bar total size
         """
         self.bar_length = len(self.preffix) + len(self.suffix)
-        self.__update_bar_size()
-
-    def __update_bar_size(self) -> None:
         self.bar_size = self.terminal_size - self.bar_length - 3
         if self.show_percents:
             self.bar_size -= len(self.percents)
         if self.show_estimate:
             self.bar_size -= len(self.estimate)
         if self.show_runtime:
             self.bar_size -= len(self.run_time)
 
     def __format_bar(self) -> str:
-        bar = ["\r"]
+        bar = []
         finished = int(self.bar_size * self.progress / self.total)
         finished_mark = self.done_marker * finished
         in_progress_mark = self.in_progress_marker * (self.bar_size - finished - 1)
         if self.bar_size <= finished:
             self.current_marker = ""
         if self.preffix:
             bar.append(f"{self.preffix} ")
-        bar.append(f"[{finished_mark}{self.current_marker}{in_progress_mark}]")
+        if self.show_bar:
+            bar.append(f"[{finished_mark}{self.current_marker}{in_progress_mark}]")
         if self.show_percents:
             bar.append(self.percents)
         if self.show_estimate:
             bar.append(self.estimate)
         if self.show_runtime:
             bar.append(self.run_time)
-        if self.suffix:
+        if self.show_suffix:
             bar.append(f"|{self.suffix}")
+        bar.append("\r")
         return "".join(bar)
 
     def draw(self) -> None:
         """
         Draw a progress bar
         """
         if self.show_percents:
             self.__update_percent_done()
         if self.show_estimate:
             self.__calculate_estimate()
         if self.show_runtime:
             self.__update_run_time()
+        self.__update_terminal_size()
         bar = self.__format_bar()
         sys.stdout.write(bar)
         sys.stdout.flush()
 
     def set_prefix(self, preffix: str) -> None:
         """
         Change bar prefix
```

### Comparing `pycotore-0.1.0/pyproject.toml` & `pycotore-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycotore"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Generic classes for reuse"
-version = "0.0.0a0"
+version = "0.1.1"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pycotore"
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `pycotore-0.1.0/PKG-INFO` & `pycotore-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

