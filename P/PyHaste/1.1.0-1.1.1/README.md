# Comparing `tmp/pyhaste-1.1.0.tar.gz` & `tmp/pyhaste-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhaste-1.1.0.tar", max compression
+gzip compressed data, was "pyhaste-1.1.1.tar", max compression
```

## Comparing `pyhaste-1.1.0.tar` & `pyhaste-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1506 2024-04-11 14:35:32.580277 pyhaste-1.1.0/LICENSE.md
--rw-r--r--   0        0        0    10741 2024-04-11 14:35:32.580277 pyhaste-1.1.0/README.md
--rw-r--r--   0        0        0      235 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/__init__.py
--rw-r--r--   0        0        0     2903 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/analyzer.py
--rw-r--r--   0        0        0      343 2024-04-11 14:35:32.580277 pyhaste-1.1.0/pyhaste/test_analyzer.py
--rw-r--r--   0        0        0      878 2024-04-11 14:36:01.556232 pyhaste-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 pyhaste-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-04-11 15:25:12.020279 pyhaste-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0    11561 2024-04-11 15:25:12.020279 pyhaste-1.1.1/README.md
+-rw-r--r--   0        0        0      235 2024-04-11 15:25:12.020279 pyhaste-1.1.1/pyhaste/__init__.py
+-rw-r--r--   0        0        0     3231 2024-04-11 15:25:12.020279 pyhaste-1.1.1/pyhaste/analyzer.py
+-rw-r--r--   0        0        0      337 2024-04-11 15:25:12.020279 pyhaste-1.1.1/pyhaste/test_analyzer.py
+-rw-r--r--   0        0        0      878 2024-04-11 15:25:40.100074 pyhaste-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12293 1970-01-01 00:00:00.000000 pyhaste-1.1.1/PKG-INFO
```

### Comparing `pyhaste-1.1.0/LICENSE.md` & `pyhaste-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhaste-1.1.0/README.md` & `pyhaste-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,27 +56,27 @@
 
 time.sleep(0.01)
 report()
 
 ```
 
 ```
-───────────────── PyHaste report ─────────────────
+───────────────────── PyHaste report ─────────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
-┃ Name               ┃    Time ┃  Tot % ┃  Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
-│ task               │ 0.700 s │ 98.58% │        │
-│ task ›process_item │ 0.600 s │ 84.49% │ 85.70% │
-│ task ›prepare_task │ 0.100 s │ 14.09% │ 14.29% │
-│ Unmeasured         │ 0.010 s │  1.42% │        │
-│ task ›find_items   │ 0.000 s │  0.00% │  0.00% │
-├────────────────────┼─────────┼────────┼────────┤
-│ Total              │ 0.710 s │   100% │        │
-└────────────────────┴─────────┴────────┴────────┘
+┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━┓
+┃ Name               ┃    Time ┃  Tot % ┃  Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━┩
+│ task               │ 0.700 s │ 98.58% │        │     1 │
+│ task ›process_item │ 0.600 s │ 84.49% │ 85.71% │     3 │
+│ task ›prepare_task │ 0.100 s │ 14.08% │ 14.29% │     1 │
+│ Unmeasured         │ 0.010 s │  1.42% │        │       │
+│ task ›find_items   │ 0.000 s │  0.00% │  0.00% │     1 │
+├────────────────────┼─────────┼────────┼────────┼───────┤
+│ Total              │ 0.710 s │   100% │        │       │
+└────────────────────┴─────────┴────────┴────────┴───────┘
 ```
 
 In case you need more complex analysis, you might benefit from `pyhaste.Analyzer` and creating your own instances, e.g. for measuring time spent on separate tasks in a longer running job:
 
 ```python
 import time
 from random import uniform
@@ -94,61 +94,61 @@
     with analyzer.measure("save"):
       time.sleep(uniform(0.05, 0.075) * item)
   time.sleep(uniform(0.01, 0.025) * item)
   analyzer.report()
 ```
 
 ```
-──────────────────────────────── PyHaste report ────────────────────────────────
+──────────────────────────────────── PyHaste report ────────────────────────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(1)                                 │ 0.235 s │ 95.78% │         │
-│ process_item(1) ›calculate                      │ 0.121 s │ 49.36% │  51.53% │
-│ process_item(1) ›calculate ›guestimate          │ 0.121 s │ 49.36% │ 100.00% │
-│ process_item(1) ›calculate ›guestimate ›do_math │ 0.121 s │ 49.35% │  99.99% │
-│ process_item(1) ›save                           │ 0.071 s │ 29.19% │  30.48% │
-│ process_item(1) ›db.find                        │ 0.042 s │ 17.22% │  17.98% │
-│ Unmeasured                                      │ 0.010 s │  4.22% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.245 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
-
-──────────────────────────────── PyHaste report ────────────────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(2)                                 │ 0.505 s │ 95.09% │         │
-│ process_item(2) ›calculate                      │ 0.284 s │ 53.37% │  56.13% │
-│ process_item(2) ›calculate ›guestimate          │ 0.284 s │ 53.37% │ 100.00% │
-│ process_item(2) ›calculate ›guestimate ›do_math │ 0.284 s │ 53.37% │ 100.00% │
-│ process_item(2) ›save                           │ 0.130 s │ 24.45% │  25.71% │
-│ process_item(2) ›db.find                        │ 0.092 s │ 17.26% │  18.16% │
-│ Unmeasured                                      │ 0.026 s │  4.91% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.531 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
-
-──────────────────────────────── PyHaste report ────────────────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(3)                                 │ 0.671 s │ 95.36% │         │
-│ process_item(3) ›calculate                      │ 0.330 s │ 46.87% │  49.15% │
-│ process_item(3) ›calculate ›guestimate          │ 0.330 s │ 46.87% │ 100.00% │
-│ process_item(3) ›calculate ›guestimate ›do_math │ 0.330 s │ 46.87% │ 100.00% │
-│ process_item(3) ›save                           │ 0.196 s │ 27.87% │  29.22% │
-│ process_item(3) ›db.find                        │ 0.145 s │ 20.62% │  21.62% │
-│ Unmeasured                                      │ 0.033 s │  4.64% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.704 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(1)                                 │ 0.219 s │ 93.61% │         │     1 │
+│ process_item(1) ›calculate                      │ 0.121 s │ 51.69% │  55.22% │     1 │
+│ process_item(1) ›calculate ›guestimate          │ 0.121 s │ 51.69% │ 100.00% │     1 │
+│ process_item(1) ›calculate ›guestimate ›do_math │ 0.121 s │ 51.69% │  99.99% │     1 │
+│ process_item(1) ›save                           │ 0.055 s │ 23.66% │  25.28% │     1 │
+│ process_item(1) ›db.find                        │ 0.043 s │ 18.24% │  19.49% │     1 │
+│ Unmeasured                                      │ 0.015 s │  6.39% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.234 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
+
+──────────────────────────────────── PyHaste report ────────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(2)                                 │ 0.474 s │ 92.57% │         │     1 │
+│ process_item(2) ›calculate                      │ 0.211 s │ 41.26% │  44.57% │     1 │
+│ process_item(2) ›calculate ›guestimate          │ 0.211 s │ 41.26% │ 100.00% │     1 │
+│ process_item(2) ›calculate ›guestimate ›do_math │ 0.211 s │ 41.26% │  99.99% │     1 │
+│ process_item(2) ›save                           │ 0.146 s │ 28.44% │  30.72% │     1 │
+│ process_item(2) ›db.find                        │ 0.117 s │ 22.86% │  24.70% │     1 │
+│ Unmeasured                                      │ 0.038 s │  7.43% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.512 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
+
+──────────────────────────────────── PyHaste report ────────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(3)                                 │ 0.719 s │ 91.02% │         │     1 │
+│ process_item(3) ›calculate                      │ 0.374 s │ 47.32% │  51.99% │     1 │
+│ process_item(3) ›calculate ›guestimate          │ 0.374 s │ 47.32% │ 100.00% │     1 │
+│ process_item(3) ›calculate ›guestimate ›do_math │ 0.374 s │ 47.32% │  99.99% │     1 │
+│ process_item(3) ›save                           │ 0.190 s │ 23.99% │  26.36% │     1 │
+│ process_item(3) ›db.find                        │ 0.156 s │ 19.70% │  21.64% │     1 │
+│ Unmeasured                                      │ 0.071 s │  8.98% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.790 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
 ```
 
 ## Development
 
 Issues and PRs are welcome!
 
 Please open an issue first to discuss the idea before sending a PR so that you know if it would be wanted or needs
```

### Comparing `pyhaste-1.1.0/pyhaste/analyzer.py` & `pyhaste-1.1.1/pyhaste/analyzer.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,39 +23,42 @@
 
 
 def sort_items(items: Iterable[Item]):
     return sorted(items, key=lambda item: item[1], reverse=True)
 
 
 class Analyzer:
-    counters: dict[str, float]
-    total: float
+    counters: dict[str, int]
+    timers: dict[str, float]
+    total_time: float
     nested: list[str]
 
     def __init__(self):
         self.counters = {}
-        self.total = 0.0
+        self.timers = {}
+        self.total_time = 0.0
         self.start_time = None
         self.nested = []
 
     @contextmanager
     def measure(self, name):
         start = perf_counter()
         if not self.start_time:
             self.start_time = start
 
         self.nested.append(name)
-        counter_name = SEP.join(self.nested)
+        key = SEP.join(self.nested)
         yield
         self.nested.pop()
 
         elapsed = perf_counter() - start
-        self.counters[counter_name] = elapsed + self.counters.get(counter_name, 0.0)
+        self.counters[key] = 1 + self.counters.get(key, 0.0)
+        self.timers[key] = elapsed + self.timers.get(key, 0.0)
         if not self.nested:
-            self.total += elapsed
+            self.total_time += elapsed
 
     def measure_wrap(self, name):
         def decorator(f):
             @wraps(f)
             def wrapper(*args, **kwargs):
                 with self.measure(name):
                     return f(*args, **kwargs)
@@ -66,39 +69,44 @@
 
     def get_parent_pct(self, name, elapsed):
         parts = name.split(SEP)
         if len(parts) == 1:
             return ""
 
         parent_name = SEP.join(parts[:-1])
-        parent_total = self.counters[parent_name]
+        parent_total = self.timers[parent_name]
 
         pct = (elapsed / parent_total) * 100
         return f"{pct:.2f}%"
 
     def report(self):
         total_elapsed = perf_counter() - self.start_time
-        self.counters["Unmeasured"] = total_elapsed - self.total
-        self.total += self.counters["Unmeasured"]
+        self.timers["Unmeasured"] = total_elapsed - self.total_time
+        self.total_time += self.timers["Unmeasured"]
 
         tbl = Table()
         tbl.add_column("Name", style="bright_green")
         tbl.add_column("Time", style="bright_magenta", justify="right", no_wrap=True)
         tbl.add_column("Tot %", style="bright_blue", justify="right", no_wrap=True)
         tbl.add_column("Rel %", style="bright_yellow", justify="right", no_wrap=True)
+        tbl.add_column("Calls", style="cyan", justify="right", no_wrap=True)
 
-        for name, elapsed in sort_items(self.counters.items()):
-            pct = (elapsed / self.total) * 100
+        for name, elapsed in sort_items(self.timers.items()):
+            pct = (elapsed / self.total_time) * 100
+            count = ""
+            if name in self.counters:
+                count = f"{self.counters[name]:,.0f}"
             tbl.add_row(
                 " [blue]›[/blue]".join(name.split(SEP)),
                 format_elapsed(elapsed),
                 f"{pct:.2f}%",
                 self.get_parent_pct(name, elapsed),
+                count,
             )
 
         tbl.add_section()
-        tbl.add_row("Total", format_elapsed(self.total), "100%", "")
+        tbl.add_row("Total", format_elapsed(self.total_time), "100%", "", "")
 
         console.print("")
         console.rule("[bold red]PyHaste report", style="green")
         console.print("")
         console.print(tbl)
```

### Comparing `pyhaste-1.1.0/pyproject.toml` & `pyhaste-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyHaste"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python code speed analyzer"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/pyhaste/"
 repository = "https://github.com/cocreators-ee/pyhaste/"
 documentation = "https://github.com/cocreators-ee/pyhaste/"
```

### Comparing `pyhaste-1.1.0/PKG-INFO` & `pyhaste-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHaste
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python code speed analyzer
 Home-page: https://github.com/cocreators-ee/pyhaste/
 License: BSD-3-Clause
 Keywords: performance,measuring,benchmark,benchmarking,analyzer
 Author: Janne Enberg
 Author-email: janne.enberg@lietu.net
 Requires-Python: >=3.11,<4.0
@@ -75,27 +75,27 @@
 
 time.sleep(0.01)
 report()
 
 ```
 
 ```
-───────────────── PyHaste report ─────────────────
+───────────────────── PyHaste report ─────────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
-┃ Name               ┃    Time ┃  Tot % ┃  Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━┩
-│ task               │ 0.700 s │ 98.58% │        │
-│ task ›process_item │ 0.600 s │ 84.49% │ 85.70% │
-│ task ›prepare_task │ 0.100 s │ 14.09% │ 14.29% │
-│ Unmeasured         │ 0.010 s │  1.42% │        │
-│ task ›find_items   │ 0.000 s │  0.00% │  0.00% │
-├────────────────────┼─────────┼────────┼────────┤
-│ Total              │ 0.710 s │   100% │        │
-└────────────────────┴─────────┴────────┴────────┘
+┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━┳━━━━━━━┓
+┃ Name               ┃    Time ┃  Tot % ┃  Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━╇━━━━━━━┩
+│ task               │ 0.700 s │ 98.58% │        │     1 │
+│ task ›process_item │ 0.600 s │ 84.49% │ 85.71% │     3 │
+│ task ›prepare_task │ 0.100 s │ 14.08% │ 14.29% │     1 │
+│ Unmeasured         │ 0.010 s │  1.42% │        │       │
+│ task ›find_items   │ 0.000 s │  0.00% │  0.00% │     1 │
+├────────────────────┼─────────┼────────┼────────┼───────┤
+│ Total              │ 0.710 s │   100% │        │       │
+└────────────────────┴─────────┴────────┴────────┴───────┘
 ```
 
 In case you need more complex analysis, you might benefit from `pyhaste.Analyzer` and creating your own instances, e.g. for measuring time spent on separate tasks in a longer running job:
 
 ```python
 import time
 from random import uniform
@@ -113,61 +113,61 @@
     with analyzer.measure("save"):
       time.sleep(uniform(0.05, 0.075) * item)
   time.sleep(uniform(0.01, 0.025) * item)
   analyzer.report()
 ```
 
 ```
-──────────────────────────────── PyHaste report ────────────────────────────────
+──────────────────────────────────── PyHaste report ────────────────────────────────────
 
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(1)                                 │ 0.235 s │ 95.78% │         │
-│ process_item(1) ›calculate                      │ 0.121 s │ 49.36% │  51.53% │
-│ process_item(1) ›calculate ›guestimate          │ 0.121 s │ 49.36% │ 100.00% │
-│ process_item(1) ›calculate ›guestimate ›do_math │ 0.121 s │ 49.35% │  99.99% │
-│ process_item(1) ›save                           │ 0.071 s │ 29.19% │  30.48% │
-│ process_item(1) ›db.find                        │ 0.042 s │ 17.22% │  17.98% │
-│ Unmeasured                                      │ 0.010 s │  4.22% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.245 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
-
-──────────────────────────────── PyHaste report ────────────────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(2)                                 │ 0.505 s │ 95.09% │         │
-│ process_item(2) ›calculate                      │ 0.284 s │ 53.37% │  56.13% │
-│ process_item(2) ›calculate ›guestimate          │ 0.284 s │ 53.37% │ 100.00% │
-│ process_item(2) ›calculate ›guestimate ›do_math │ 0.284 s │ 53.37% │ 100.00% │
-│ process_item(2) ›save                           │ 0.130 s │ 24.45% │  25.71% │
-│ process_item(2) ›db.find                        │ 0.092 s │ 17.26% │  18.16% │
-│ Unmeasured                                      │ 0.026 s │  4.91% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.531 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
-
-──────────────────────────────── PyHaste report ────────────────────────────────
-
-┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┓
-┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃
-┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━┩
-│ process_item(3)                                 │ 0.671 s │ 95.36% │         │
-│ process_item(3) ›calculate                      │ 0.330 s │ 46.87% │  49.15% │
-│ process_item(3) ›calculate ›guestimate          │ 0.330 s │ 46.87% │ 100.00% │
-│ process_item(3) ›calculate ›guestimate ›do_math │ 0.330 s │ 46.87% │ 100.00% │
-│ process_item(3) ›save                           │ 0.196 s │ 27.87% │  29.22% │
-│ process_item(3) ›db.find                        │ 0.145 s │ 20.62% │  21.62% │
-│ Unmeasured                                      │ 0.033 s │  4.64% │         │
-├─────────────────────────────────────────────────┼─────────┼────────┼─────────┤
-│ Total                                           │ 0.704 s │   100% │         │
-└─────────────────────────────────────────────────┴─────────┴────────┴─────────┘
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(1)                                 │ 0.219 s │ 93.61% │         │     1 │
+│ process_item(1) ›calculate                      │ 0.121 s │ 51.69% │  55.22% │     1 │
+│ process_item(1) ›calculate ›guestimate          │ 0.121 s │ 51.69% │ 100.00% │     1 │
+│ process_item(1) ›calculate ›guestimate ›do_math │ 0.121 s │ 51.69% │  99.99% │     1 │
+│ process_item(1) ›save                           │ 0.055 s │ 23.66% │  25.28% │     1 │
+│ process_item(1) ›db.find                        │ 0.043 s │ 18.24% │  19.49% │     1 │
+│ Unmeasured                                      │ 0.015 s │  6.39% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.234 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
+
+──────────────────────────────────── PyHaste report ────────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(2)                                 │ 0.474 s │ 92.57% │         │     1 │
+│ process_item(2) ›calculate                      │ 0.211 s │ 41.26% │  44.57% │     1 │
+│ process_item(2) ›calculate ›guestimate          │ 0.211 s │ 41.26% │ 100.00% │     1 │
+│ process_item(2) ›calculate ›guestimate ›do_math │ 0.211 s │ 41.26% │  99.99% │     1 │
+│ process_item(2) ›save                           │ 0.146 s │ 28.44% │  30.72% │     1 │
+│ process_item(2) ›db.find                        │ 0.117 s │ 22.86% │  24.70% │     1 │
+│ Unmeasured                                      │ 0.038 s │  7.43% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.512 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
+
+──────────────────────────────────── PyHaste report ────────────────────────────────────
+
+┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━┳━━━━━━━┓
+┃ Name                                            ┃    Time ┃  Tot % ┃   Rel % ┃ Calls ┃
+┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━╇━━━━━━━┩
+│ process_item(3)                                 │ 0.719 s │ 91.02% │         │     1 │
+│ process_item(3) ›calculate                      │ 0.374 s │ 47.32% │  51.99% │     1 │
+│ process_item(3) ›calculate ›guestimate          │ 0.374 s │ 47.32% │ 100.00% │     1 │
+│ process_item(3) ›calculate ›guestimate ›do_math │ 0.374 s │ 47.32% │  99.99% │     1 │
+│ process_item(3) ›save                           │ 0.190 s │ 23.99% │  26.36% │     1 │
+│ process_item(3) ›db.find                        │ 0.156 s │ 19.70% │  21.64% │     1 │
+│ Unmeasured                                      │ 0.071 s │  8.98% │         │       │
+├─────────────────────────────────────────────────┼─────────┼────────┼─────────┼───────┤
+│ Total                                           │ 0.790 s │   100% │         │       │
+└─────────────────────────────────────────────────┴─────────┴────────┴─────────┴───────┘
 ```
 
 ## Development
 
 Issues and PRs are welcome!
 
 Please open an issue first to discuss the idea before sending a PR so that you know if it would be wanted or needs
```

