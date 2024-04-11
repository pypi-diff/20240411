# Comparing `tmp/pycotore-0.0.4.tar.gz` & `tmp/pycotore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotore-0.0.4.tar", max compression
+gzip compressed data, was "pycotore-0.1.0.tar", max compression
```

## Comparing `pycotore-0.0.4.tar` & `pycotore-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.0.4/LICENSE
--rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.0.4/pycotore/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.0.4/pycotore/constants.py
--rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.0.4/pycotore/exceptions.py
--rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.0.4/pycotore/logger.py
--rw-r--r--   0        0        0     4429 2024-04-10 14:42:29.019304 pycotore-0.0.4/pycotore/progress.py
--rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 17:39:36.901662 pycotore-0.1.0/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-03 18:34:41.156694 pycotore-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:34:41.132509 pycotore-0.1.0/pycotore/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 17:00:15.277697 pycotore-0.1.0/pycotore/constants.py
+-rw-r--r--   0        0        0       86 2024-04-09 16:57:44.180967 pycotore-0.1.0/pycotore/exceptions.py
+-rw-r--r--   0        0        0     1988 2024-04-09 18:10:49.086870 pycotore-0.1.0/pycotore/logger.py
+-rw-r--r--   0        0        0     5004 2024-04-10 17:31:42.465918 pycotore-0.1.0/pycotore/progress.py
+-rw-r--r--   0        0        0      599 2024-04-10 07:47:48.046176 pycotore-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 pycotore-0.1.0/PKG-INFO
```

### Comparing `pycotore-0.0.4/LICENSE` & `pycotore-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.4/pycotore/logger.py` & `pycotore-0.1.0/pycotore/logger.py`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.4/pycotore/progress.py` & `pycotore-0.1.0/pycotore/progress.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,64 +14,74 @@
 
     def __init__(
                 self,
                 base_marker: str = ".",
                 done_marke: str = "#",
                 current_marker: str = ">",
                 show_percents: bool = True,
-                show_estimate: bool = True
+                show_estimate: bool = True,
+                show_runtime: bool = True
             ):
         self.preffix: str = ""
         self.suffix: str = ""
         self.bar_length: int = 0
         self.bar_size: int = 0
         self.terminal_size: int = os.get_terminal_size().columns
         self.progress: float = 0.00
         self.total: float = 100.00
         self.done_marker: str = done_marke
         self.in_progress_marker: str = base_marker
         self.current_marker: str = current_marker
-        self.percents: float = "|000.00%"
+        self.percents: float = "000.00%"
         self.show_percents: bool = show_percents
         self.show_numbers: bool = False
         self.time_start = datetime.now()
         self.show_estimate: bool = show_estimate
         self.estimate = "|ETA: 00:00:00"
+        self.run_time = "|RUN: 00:00:00"
+        self.show_runtime: bool = show_runtime
 
     def flush_line(self) -> None:
         sys.stdout.write("\n")
         sys.stdout.flush()
 
     def __str__(self):
         bar = f"prefix: {self.preffix}\nsufix: {self.suffix}\nbar size: {self.bar_length}\ncurrent terminal: {self.terminal_size}\nbar size: {self.bar_size}\nMarker: {self.done_marker}\ntotal: {self.total}\nprogress: {self.progress}"
         return bar
 
+    def __update_run_time(self) -> None:
+        now = datetime.now()
+        run_time = now - self.time_start
+        self.run_time = f"|RUN: {run_time.seconds // 3600:0>2}:{run_time.seconds // 60:0>2}:{run_time.seconds % 60:0>2}"
+
     def __calculate_estimate(self) -> None:
         now = datetime.now()
         run_time = now - self.time_start
         left = self.total * run_time / self.progress - run_time
         self.estimate = f"|ETA: {left.seconds // 3600:0>2}:{left.seconds // 60:0>2}:{left.seconds % 60:0>2}"
 
     def __update_percent_done(self) -> None:
         percents = round(self.progress * 100 / self.total, 2)
-        self.percents = f"|{percents:0>6.2f}%"
+        self.percents = f"{percents:0>6.2f}%"
 
     def __update_bar_length(self) -> None:
         """
         Updating progress bar total size
         """
         self.bar_length = len(self.preffix) + len(self.suffix)
         self.__update_bar_size()
 
     def __update_bar_size(self) -> None:
         self.bar_size = self.terminal_size - self.bar_length - 3
         if self.show_percents:
             self.bar_size -= len(self.percents)
         if self.show_estimate:
             self.bar_size -= len(self.estimate)
+        if self.show_runtime:
+            self.bar_size -= len(self.run_time)
 
     def __format_bar(self) -> str:
         bar = ["\r"]
         finished = int(self.bar_size * self.progress / self.total)
         finished_mark = self.done_marker * finished
         in_progress_mark = self.in_progress_marker * (self.bar_size - finished - 1)
         if self.bar_size <= finished:
@@ -79,26 +89,30 @@
         if self.preffix:
             bar.append(f"{self.preffix} ")
         bar.append(f"[{finished_mark}{self.current_marker}{in_progress_mark}]")
         if self.show_percents:
             bar.append(self.percents)
         if self.show_estimate:
             bar.append(self.estimate)
+        if self.show_runtime:
+            bar.append(self.run_time)
         if self.suffix:
             bar.append(f"|{self.suffix}")
         return "".join(bar)
 
     def draw(self) -> None:
         """
         Draw a progress bar
         """
         if self.show_percents:
             self.__update_percent_done()
         if self.show_estimate:
             self.__calculate_estimate()
+        if self.show_runtime:
+            self.__update_run_time()
         bar = self.__format_bar()
         sys.stdout.write(bar)
         sys.stdout.flush()
 
     def set_prefix(self, preffix: str) -> None:
         """
         Change bar prefix
```

### Comparing `pycotore-0.0.4/pyproject.toml` & `pycotore-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycotore-0.0.4/PKG-INFO` & `pycotore-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycotore
-Version: 0.0.4
+Version: 0.1.0
 Summary: Generic classes for reuse
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

