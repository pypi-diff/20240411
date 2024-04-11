# Comparing `tmp/pyhaste-1.0.1.tar.gz` & `tmp/pyhaste-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhaste-1.0.1.tar", max compression
+gzip compressed data, was "pyhaste-1.1.0.tar", max compression
```

## Comparing `pyhaste-1.0.1.tar` & `pyhaste-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1506 2024-04-10 17:24:17.748694 pyhaste-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     7977 2024-04-10 17:24:17.748694 pyhaste-1.0.1/README.md
--rw-r--r--   0        0        0      177 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/__init__.py
--rw-r--r--   0        0        0     2175 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/analyzer.py
--rw-r--r--   0        0        0      343 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/test_analyzer.py
--rw-r--r--   0        0        0      878 2024-04-10 17:24:43.629260 pyhaste-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8709 1970-01-01 00:00:00.000000 pyhaste-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-04-11 14:35:32.580277 pyhaste-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0    10741 2024-04-11 14:35:32.580277 pyhaste-1.1.0/README.md
+-rw-r--r--   0        0        0      235 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/__init__.py
+-rw-r--r--   0        0        0     2903 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/analyzer.py
+-rw-r--r--   0        0        0      343 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/test_analyzer.py
+-rw-r--r--   0        0        0      878 2024-04-11 14:36:01.556232 pyhaste-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 pyhaste-1.1.0/PKG-INFO
```

### Comparing `pyhaste-1.0.1/LICENSE.md` & `pyhaste-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhaste-1.0.1/README.md` & `pyhaste-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: PyHaste
+Version: 1.1.0
+Summary: Python code speed analyzer
+Home-page: https://github.com/cocreators-ee/pyhaste/
+License: BSD-3-Clause
+Keywords: performance,measuring,benchmark,benchmarking,analyzer
+Author: Janne Enberg
+Author-email: janne.enberg@lietu.net
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Project-URL: Documentation, https://github.com/cocreators-ee/pyhaste/
+Project-URL: Repository, https://github.com/cocreators-ee/pyhaste/
+Description-Content-Type: text/markdown
+
 # PyHaste
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/cocreators-ee/pyhaste/publish.yaml)](https://github.com/cocreators-ee/pyhaste/actions/workflows/publish.yaml)
 [![Code style: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/cocreators-ee/pyhaste/blob/master/.pre-commit-config.yaml)
 [![PyPI](https://img.shields.io/pypi/v/pyhaste)](https://pypi.org/project/pyhaste/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhaste)](https://pypi.org/project/pyhaste/)
@@ -26,56 +45,57 @@
 ## Usage
 
 To measure your code, `pyhaste` exports a `measure` context manager, give it a name as an argument. Once you want a report call `report` from `pyhaste`.
 
 ```python
 import time
 
-from pyhaste import measure, report
+from pyhaste import measure, report, measure_wrap
 
 
+@measure_wrap("prepare_task")
 def prepare_task():
   time.sleep(0.1)
 
 
+@measure_wrap("find_items")
 def find_items():
-  with measure("find_items"):
-    return [1, 2, 3]
+  return [1, 2, 3]
 
 
+@measure_wrap("process_item")
 def process_item(item):
-  with measure("process_item"):
-    time.sleep(item * 0.1)
+  time.sleep(item * 0.1)
 
 
 with measure("task"):
-  with measure("prepare"):
-    prepare_task()
+  prepare_task()
 
   for item in find_items():
     process_item(item)
 
 time.sleep(0.01)
 report()
+
 ```
 
 ```
 ───────────────── PyHaste report ─────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┓
-┃ Name                 ┃    Time ┃      % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━┩
-│ task                 │ 0.700 s │ 98.58% │
-│ task -> process_item │ 0.600 s │ 84.49% │
-│ task -> prepare      │ 0.100 s │ 14.09% │
-│ Unmeasured           │ 0.010 s │  1.42% │
-│ task -> find_items   │ 0.000 s │  0.00% │
-├──────────────────────┼─────────┼────────┤
-│ Total                │ 0.710 s │   100% │
-└──────────────────────┴─────────┴────────┘
+┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
+┃ Name               ┃    Time ┃  Tot % ┃  Rel % ┃
+┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
+│ task               │ 0.700 s │ 98.58% │        │
+│ task ›process_item │ 0.600 s │ 84.49% │ 85.70% │
+│ task ›prepare_task │ 0.100 s │ 14.09% │ 14.29% │
+│ Unmeasured         │ 0.010 s │  1.42% │        │
+│ task ›find_items   │ 0.000 s │  0.00% │  0.00% │
+├────────────────────┼─────────┼────────┼────────┤
+│ Total              │ 0.710 s │   100% │        │
+└────────────────────┴─────────┴────────┴────────┘
 ```
 
 In case you need more complex analysis, you might benefit from `pyhaste.Analyzer` and creating your own instances, e.g. for measuring time spent on separate tasks in a longer running job:
 
 ```python
 import time
 from random import uniform
@@ -83,63 +103,71 @@
 
 for item in [1, 2, 3]:
   analyzer = Analyzer()
   with analyzer.measure(f"process_item({item})"):
     with analyzer.measure("db.find"):
       time.sleep(uniform(0.04, 0.06) * item)
     with analyzer.measure("calculate"):
-      time.sleep(uniform(0.1, 0.15) * item)
+      with analyzer.measure("guestimate"):
+        with analyzer.measure("do_math"):
+          time.sleep(uniform(0.1, 0.15) * item)
     with analyzer.measure("save"):
       time.sleep(uniform(0.05, 0.075) * item)
   time.sleep(uniform(0.01, 0.025) * item)
   analyzer.report()
 ```
 
 ```
-─────────────────── PyHaste report ────────────────────
+──────────────────────────────── PyHaste report ────────────────────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┓
-┃ Name                         ┃    Time ┃      % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━┩
-│ process_item(1)              │ 0.217 s │ 91.81% │
-│ process_item(1) -> calculate │ 0.108 s │ 45.87% │
-│ process_item(1) -> save      │ 0.054 s │ 22.97% │
-│ process_item(1) -> db.find   │ 0.054 s │ 22.95% │
-│ Unmeasured                   │ 0.019 s │  8.19% │
-├──────────────────────────────┼─────────┼────────┤
-│ Total                        │ 0.236 s │   100% │
-└──────────────────────────────┴─────────┴────────┘
-
-─────────────────── PyHaste report ────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┓
-┃ Name                         ┃    Time ┃      % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━┩
-│ process_item(2)              │ 0.465 s │ 92.61% │
-│ process_item(2) -> calculate │ 0.214 s │ 42.68% │
-│ process_item(2) -> save      │ 0.139 s │ 27.77% │
-│ process_item(2) -> db.find   │ 0.111 s │ 22.15% │
-│ Unmeasured                   │ 0.037 s │  7.39% │
-├──────────────────────────────┼─────────┼────────┤
-│ Total                        │ 0.502 s │   100% │
-└──────────────────────────────┴─────────┴────────┘
-
-─────────────────── PyHaste report ────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┓
-┃ Name                         ┃    Time ┃      % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━┩
-│ process_item(3)              │ 0.759 s │ 93.85% │
-│ process_item(3) -> calculate │ 0.424 s │ 52.34% │
-│ process_item(3) -> save      │ 0.178 s │ 21.99% │
-│ process_item(3) -> db.find   │ 0.158 s │ 19.51% │
-│ Unmeasured                   │ 0.050 s │  6.15% │
-├──────────────────────────────┼─────────┼────────┤
-│ Total                        │ 0.809 s │   100% │
-└──────────────────────────────┴─────────┴────────┘
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
+│ process_item(1)                                 │ 0.235 s │ 95.78% │         │
+│ process_item(1) ›calculate                      │ 0.121 s │ 49.36% │  51.53% │
+│ process_item(1) ›calculate ›guestimate          │ 0.121 s │ 49.36% │ 100.00% │
+│ process_item(1) ›calculate ›guestimate ›do_math │ 0.121 s │ 49.35% │  99.99% │
+│ process_item(1) ›save                           │ 0.071 s │ 29.19% │  30.48% │
+│ process_item(1) ›db.find                        │ 0.042 s │ 17.22% │  17.98% │
+│ Unmeasured                                      │ 0.010 s │  4.22% │         │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
+│ Total                                           │ 0.245 s │   100% │         │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
+
+──────────────────────────────── PyHaste report ────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
+│ process_item(2)                                 │ 0.505 s │ 95.09% │         │
+│ process_item(2) ›calculate                      │ 0.284 s │ 53.37% │  56.13% │
+│ process_item(2) ›calculate ›guestimate          │ 0.284 s │ 53.37% │ 100.00% │
+│ process_item(2) ›calculate ›guestimate ›do_math │ 0.284 s │ 53.37% │ 100.00% │
+│ process_item(2) ›save                           │ 0.130 s │ 24.45% │  25.71% │
+│ process_item(2) ›db.find                        │ 0.092 s │ 17.26% │  18.16% │
+│ Unmeasured                                      │ 0.026 s │  4.91% │         │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
+│ Total                                           │ 0.531 s │   100% │         │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
+
+──────────────────────────────── PyHaste report ────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
+│ process_item(3)                                 │ 0.671 s │ 95.36% │         │
+│ process_item(3) ›calculate                      │ 0.330 s │ 46.87% │  49.15% │
+│ process_item(3) ›calculate ›guestimate          │ 0.330 s │ 46.87% │ 100.00% │
+│ process_item(3) ›calculate ›guestimate ›do_math │ 0.330 s │ 46.87% │ 100.00% │
+│ process_item(3) ›save                           │ 0.196 s │ 27.87% │  29.22% │
+│ process_item(3) ›db.find                        │ 0.145 s │ 20.62% │  21.62% │
+│ Unmeasured                                      │ 0.033 s │  4.64% │         │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
+│ Total                                           │ 0.704 s │   100% │         │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
 ```
 
 ## Development
 
 Issues and PRs are welcome!
 
 Please open an issue first to discuss the idea before sending a PR so that you know if it would be wanted or needs
@@ -164,7 +192,8 @@
 # Financial support
 
 This project has been made possible thanks to [Cocreators](https://cocreators.ee) and [Lietu](https://lietu.net). You
 can help us continue our open source work by supporting us
 on [Buy me a coffee](https://www.buymeacoffee.com/cocreators).
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/cocreators)
+
```

### Comparing `pyhaste-1.0.1/pyhaste/analyzer.py` & `pyhaste-1.1.0/pyhaste/analyzer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from contextlib import contextmanager
+from functools import wraps
 from time import perf_counter
 from typing import Iterable, Tuple
 
 from rich.console import Console
 from rich.table import Table
 
 Item = Tuple[str, float]
 console = Console()
+SEP = " -> "
 
 
 def format_elapsed(elapsed: float) -> str:
     if elapsed < 5:
         decimals = 3
     elif elapsed < 25:
         decimals = 2
@@ -38,42 +40,65 @@
     @contextmanager
     def measure(self, name):
         start = perf_counter()
         if not self.start_time:
             self.start_time = start
 
         self.nested.append(name)
-        counter_name = " [blue]->[/blue] ".join(self.nested)
+        counter_name = SEP.join(self.nested)
         yield
         self.nested.pop()
 
         elapsed = perf_counter() - start
         self.counters[counter_name] = elapsed + self.counters.get(counter_name, 0.0)
         if not self.nested:
             self.total += elapsed
 
+    def measure_wrap(self, name):
+        def decorator(f):
+            @wraps(f)
+            def wrapper(*args, **kwargs):
+                with self.measure(name):
+                    return f(*args, **kwargs)
+
+            return wrapper
+
+        return decorator
+
+    def get_parent_pct(self, name, elapsed):
+        parts = name.split(SEP)
+        if len(parts) == 1:
+            return ""
+
+        parent_name = SEP.join(parts[:-1])
+        parent_total = self.counters[parent_name]
+
+        pct = (elapsed / parent_total) * 100
+        return f"{pct:.2f}%"
+
     def report(self):
         total_elapsed = perf_counter() - self.start_time
         self.counters["Unmeasured"] = total_elapsed - self.total
         self.total += self.counters["Unmeasured"]
 
         tbl = Table()
         tbl.add_column("Name", style="bright_green")
         tbl.add_column("Time", style="bright_magenta", justify="right", no_wrap=True)
-        tbl.add_column("%", style="bright_blue", justify="right", no_wrap=True)
+        tbl.add_column("Tot %", style="bright_blue", justify="right", no_wrap=True)
+        tbl.add_column("Rel %", style="bright_yellow", justify="right", no_wrap=True)
 
-        items = self.counters.items()
-        items = sort_items(items)
-        for name, elapsed in items:
+        for name, elapsed in sort_items(self.counters.items()):
             pct = (elapsed / self.total) * 100
             tbl.add_row(
-                name,
+                " [blue]›[/blue]".join(name.split(SEP)),
                 format_elapsed(elapsed),
                 f"{pct:.2f}%",
+                self.get_parent_pct(name, elapsed),
             )
+
         tbl.add_section()
-        tbl.add_row("Total", format_elapsed(self.total), "100%")
+        tbl.add_row("Total", format_elapsed(self.total), "100%", "")
 
         console.print("")
         console.rule("[bold red]PyHaste report", style="green")
         console.print("")
         console.print(tbl)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyhaste-1.0.1/pyproject.toml` & `pyhaste-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyHaste"
-version = "1.0.1"
+version = "1.1.0"
 description = "Python code speed analyzer"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/pyhaste/"
 repository = "https://github.com/cocreators-ee/pyhaste/"
 documentation = "https://github.com/cocreators-ee/pyhaste/"
```

