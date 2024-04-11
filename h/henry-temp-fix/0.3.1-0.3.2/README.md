# Comparing `tmp/henry-temp-fix-0.3.1.tar.gz` & `tmp/henry-temp-fix-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henry-temp-fix-0.3.1.tar", last modified: Tue Apr  9 19:59:33 2024, max compression
+gzip compressed data, was "henry-temp-fix-0.3.2.tar", last modified: Wed Apr 10 18:30:24 2024, max compression
```

## Comparing `henry-temp-fix-0.3.1.tar` & `henry-temp-fix-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.309137 henry-temp-fix-0.3.1/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     1106 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/LICENSE.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-09 19:59:33.308313 henry-temp-fix-0.3.1/PKG-INFO
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    13971 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/README.md
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.286415 henry-temp-fix-0.3.1/henry/
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.287480 henry-temp-fix-0.3.1/henry/.support_files/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     2239 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/.support_files/help.rtf
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/__init__.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       22 2024-04-09 19:57:44.000000 henry-temp-fix-0.3.1/henry/__version__.py
--rwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)     7242 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/cli.py
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.291114 henry-temp-fix-0.3.1/henry/commands/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/commands/__init__.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     4330 2024-04-09 16:22:47.000000 henry-temp-fix-0.3.1/henry/commands/analyze.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     6516 2024-04-03 19:38:21.000000 henry-temp-fix-0.3.1/henry/commands/pulse.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     2163 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/commands/vacuum.py
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.295092 henry-temp-fix-0.3.1/henry/modules/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/modules/__init__.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/modules/exceptions.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    16523 2024-04-09 19:38:37.000000 henry-temp-fix-0.3.1/henry/modules/fetcher.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)      758 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/henry/modules/spinner.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)      740 2024-04-09 19:31:19.000000 henry-temp-fix-0.3.1/henry/test.py
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.307245 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/PKG-INFO
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)      645 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/SOURCES.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)        1 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/dependency_links.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/entry_points.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       24 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/requires.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       35 2024-04-09 19:59:33.000000 henry-temp-fix-0.3.1/henry_temp_fix.egg-info/top_level.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)       38 2024-04-09 19:59:33.309289 henry-temp-fix-0.3.1/setup.cfg
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)      887 2024-04-04 17:22:49.000000 henry-temp-fix-0.3.1/setup.py
-drwxr-xr-x   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-09 19:59:33.305866 henry-temp-fix-0.3.1/tests/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     4252 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/tests/test_analyze.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)      739 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/tests/test_cli.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    10927 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/tests/test_fetcher.py
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)     4877 2024-04-03 18:32:29.000000 henry-temp-fix-0.3.1/tests/test_vacuum.py
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.492239 henry-temp-fix-0.3.2/
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     1106 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/LICENSE.txt
+-rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-10 18:30:24.492239 henry-temp-fix-0.3.2/PKG-INFO
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)    13971 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/README.md
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.488239 henry-temp-fix-0.3.2/henry/
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.488239 henry-temp-fix-0.3.2/henry/.support_files/
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     2239 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/.support_files/help.rtf
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/__init__.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       22 2024-04-10 16:56:58.000000 henry-temp-fix-0.3.2/henry/__version__.py
+-rwxr-x---   0 rbobrowski (924420) primarygroup (89939)     7242 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/cli.py
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.488239 henry-temp-fix-0.3.2/henry/commands/
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/commands/__init__.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4330 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/commands/analyze.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     6830 2024-04-10 16:56:17.000000 henry-temp-fix-0.3.2/henry/commands/pulse.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     2163 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/commands/vacuum.py
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.488239 henry-temp-fix-0.3.2/henry/modules/
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/modules/__init__.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/modules/exceptions.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)    16523 2024-04-10 16:56:17.000000 henry-temp-fix-0.3.2/henry/modules/fetcher.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)      758 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/henry/modules/spinner.py
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.492239 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/
+-rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/PKG-INFO
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)      631 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/SOURCES.txt
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)        1 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/dependency_links.txt
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/entry_points.txt
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       24 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/requires.txt
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       35 2024-04-10 18:30:24.000000 henry-temp-fix-0.3.2/henry_temp_fix.egg-info/top_level.txt
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)       38 2024-04-10 18:30:24.492239 henry-temp-fix-0.3.2/setup.cfg
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)      887 2024-04-10 18:29:44.000000 henry-temp-fix-0.3.2/setup.py
+drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 18:30:24.492239 henry-temp-fix-0.3.2/tests/
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4252 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/tests/test_analyze.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)      739 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/tests/test_cli.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)    10927 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/tests/test_fetcher.py
+-rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4877 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.2/tests/test_vacuum.py
```

### Comparing `henry-temp-fix-0.3.1/LICENSE.txt` & `henry-temp-fix-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/PKG-INFO` & `henry-temp-fix-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henry-temp-fix
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Looker Cleanup Tool (Temp Fix Version)
 Home-page: https://pypi.python.org/pypi/henry
 Author: Ryan Bobrowski
 Author-email: rbobrowski@google.com
 License: MIT
 Keywords: Looker Cleanup,Looker Henry,Henry
 Requires-Python: >=3.7.0
```

### Comparing `henry-temp-fix-0.3.1/README.md` & `henry-temp-fix-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry/.support_files/help.rtf` & `henry-temp-fix-0.3.2/henry/.support_files/help.rtf`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry/cli.py` & `henry-temp-fix-0.3.2/henry/cli.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry/commands/analyze.py` & `henry-temp-fix-0.3.2/henry/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry/commands/pulse.py` & `henry-temp-fix-0.3.2/henry/commands/pulse.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,24 +36,28 @@
         if not db_connections:
             raise exceptions.NotFoundError("No connections found.")
 
         formatted_results = []
         for connection in db_connections:
             assert connection.dialect
             assert isinstance(connection.name, str)
-            resp = self.sdk.test_connection(
-                connection.name,
-                models.DelimSequence(connection.dialect.connection_tests),
-            )
-            results = list(filter(lambda r: r.status == "error", resp))
-            errors = [f"- {fill(cast(str, e.message), width=100)}" for e in results]
+            try:
+                resp = self.sdk.test_connection(
+                    connection.name,
+                    models.DelimSequence(connection.dialect.connection_tests),
+                )
+                results = list(filter(lambda r: r.status == "error", resp))
+                errors = [f"- {fill(cast(str, e.message), width=100)}" for e in results]
+            except SDKError:
+                results = []
+                errors = ["API JSONDecode Error"]
             resp = self.sdk.run_inline_query(
                 "json",
                 models.WriteQuery(
-                    model="i__looker",
+                    model="system__activity",
                     view="history",
                     fields=["history.query_run_count"],
                     filters={"history.connection_name": connection.name},
                     limit="1",
                 ),
             )
             query_run_count = json.loads(resp)[0]["history.query_run_count"]
@@ -72,15 +76,15 @@
         """Prints a list of dashboards with slow running queries in the past
         7 days"""
         print(
             "\bTest 2/6: Checking for dashboards with queries slower than "
             "30 seconds in the last 7 days"
         )
         request = models.WriteQuery(
-            model="i__looker",
+            model="system__activity",
             view="history",
             fields=["dashboard.title, query.count"],
             filters={
                 "history.created_date": "7 days",
                 "history.real_dash_id": "-NULL",
                 "history.runtime": ">30",
                 "history.status": "complete",
@@ -95,15 +99,15 @@
     @spinner.Spinner()
     def check_dashboard_errors(self):
         """Prints a list of erroring dashboard queries."""
         print(
             "\bTest 3/6: Checking for dashboards with erroring queries in the last 7 days"  # noqa: B950
         )
         request = models.WriteQuery(
-            model="i__looker",
+            model="system__activity",
             view="history",
             fields=["dashboard.title", "history.query_run_count"],
             filters={
                 "dashboard.title": "-NULL",
                 "history.created_date": "7 days",
                 "history.dashboard_session": "-NULL",
                 "history.status": "error",
@@ -116,15 +120,15 @@
         self._tabularize_and_print(erroring_dashboards)
 
     @spinner.Spinner()
     def check_explore_performance(self):
         """Prints a list of the slowest running explores."""
         print("\bTest 4/6: Checking for the slowest explores in the past 7 days")
         request = models.WriteQuery(
-            model="i__looker",
+            model="system__activity",
             view="history",
             fields=["query.model", "query.view", "history.average_runtime"],
             filters={
                 "history.created_date": "7 days",
                 "query.model": "-NULL, -system^_^_activity",
             },
             sorts=["history.average_runtime desc"],
@@ -144,15 +148,15 @@
         self._tabularize_and_print(slowest_explores)
 
     @spinner.Spinner()
     def check_schedule_failures(self):
         """Prints a list of schedules that have failed in the past 7 days."""
         print("\bTest 5/6: Checking for failing schedules")
         request = models.WriteQuery(
-            model="i__looker",
+            model="system__activity",
             view="scheduled_plan",
             fields=["scheduled_job.name", "scheduled_job.count"],
             filters={
                 "scheduled_job.created_date": "7 days",
                 "scheduled_job.status": "failure",
             },
             sorts=["scheduled_job.count desc"],
@@ -162,10 +166,13 @@
         failed_schedules = json.loads(result)
         self._tabularize_and_print(failed_schedules)
 
     @spinner.Spinner()
     def check_legacy_features(self):
         """Prints a list of enabled legacy features."""
         print("\bTest 6/6: Checking for enabled legacy features")
-        lf = list(filter(lambda f: f.enabled, self.sdk.all_legacy_features()))
-        legacy_features = [{"Feature": cast(str, f.name)} for f in lf]
+        try:
+            lf = list(filter(lambda f: f.enabled, self.sdk.all_legacy_features()))
+            legacy_features = [{"Feature": cast(str, f.name)} for f in lf]
+        except SDKError:
+            legacy_features = [["Unable to pull legacy features due to SDK error"]]
         self._tabularize_and_print(legacy_features)
```

### Comparing `henry-temp-fix-0.3.1/henry/commands/vacuum.py` & `henry-temp-fix-0.3.2/henry/commands/vacuum.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry/modules/fetcher.py` & `henry-temp-fix-0.3.2/henry/modules/fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,22 +120,22 @@
         return ml
 
     def get_used_models(self) -> Dict[str, int]:
         """Returns a dictionary with model names as keys and query count as values."""
         resp = self.sdk.run_inline_query(
             "json",
             models.WriteQuery(
-                model="i__looker",
+                model="system__activity",
                 view="history",
                 fields=["history.query_run_count", "query.model"],
                 filters={
                     "history.created_date": self.timeframe,
                     "query.model": "-system^_^_activity, -i^_^_looker",
                     "history.query_run_count": ">0",
-                    "user.dev_mode": "No",
+                    "user.dev_branch_name": "NULL",
                 },
                 limit="5000",
             ),
         )
         _results: MutableSequence[Dict[str, int]] = json.loads(resp)
         results = {
             str(row["query.model"]): int(row["history.query_run_count"])
@@ -173,15 +173,15 @@
     ) -> Dict[str, int]:
         """Returns a dictionary with used explore names as keys and query count as
         values.
         """
         resp = self.sdk.run_inline_query(
             "json",
             models.WriteQuery(
-                model="i__looker",
+                model="system__activity",
                 view="history",
                 fields=["query.view", "history.query_run_count"],
                 filters={
                     "history.created_date": self.timeframe,
                     "query.model": model.replace("_", "^_") if model else "",
                     "history.query_run_count": ">0",
                     "query.view": explore,
@@ -221,21 +221,21 @@
         """Returns a list of model.view scoped explore fields as well as the
         number of times they were used in the specified timeframe as value.
         Should always be called with either model, or model and explore
         """
         resp = self.sdk.run_inline_query(
             "json",
             models.WriteQuery(
-                model="i__looker",
+                model="system__activity",
                 view="history",
                 fields=[
                     "query.model",
                     "query.view",
                     "query.formatted_fields",
-                    "query.formatted_filters",
+                    "query.filters",
                     "history.query_run_count",
                 ],
                 filters={
                     "history.created_date": self.timeframe,
                     "query.model": model.replace("_", "^_"),
                     "query.view": explore.replace("_", "^_") if explore else "",
                     "query.formatted_fields": "-NULL",
@@ -257,17 +257,17 @@
                 else:
                     used_fields[f] = row["history.query_run_count"]
                 recorded.append(f)
 
             # A field used as a filter in a query is not listed in
             # query.formatted_fields BUT if the field is used as both a filter
             # and a dimension/measure, it's listed in both query.formatted_fields
-            # and query.formatted_filters. The recorded variable keeps track of
+            # and query.filters. The recorded variable keeps track of
             # this, so that no double counting occurs.
-            filters = row["query.formatted_filters"]
+            filters = row["query.filters"]
             if filters:
                 parsed_filters = re.findall(r"(\w+\.\w+)+", filters)
                 for f in parsed_filters:
                     if f in recorded:
                         continue
                     elif used_fields.get(f):
                         used_fields[f] += row["history.query_run_count"]
```

### Comparing `henry-temp-fix-0.3.1/henry/modules/spinner.py` & `henry-temp-fix-0.3.2/henry/modules/spinner.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/henry_temp_fix.egg-info/PKG-INFO` & `henry-temp-fix-0.3.2/henry_temp_fix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henry-temp-fix
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Looker Cleanup Tool (Temp Fix Version)
 Home-page: https://pypi.python.org/pypi/henry
 Author: Ryan Bobrowski
 Author-email: rbobrowski@google.com
 License: MIT
 Keywords: Looker Cleanup,Looker Henry,Henry
 Requires-Python: >=3.7.0
```

### Comparing `henry-temp-fix-0.3.1/henry_temp_fix.egg-info/SOURCES.txt` & `henry-temp-fix-0.3.2/henry_temp_fix.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 README.md
 setup.py
 henry/__init__.py
 henry/__version__.py
 henry/cli.py
-henry/test.py
 henry/.support_files/help.rtf
 henry/commands/__init__.py
 henry/commands/analyze.py
 henry/commands/pulse.py
 henry/commands/vacuum.py
 henry/modules/__init__.py
 henry/modules/exceptions.py
```

### Comparing `henry-temp-fix-0.3.1/setup.py` & `henry-temp-fix-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/tests/test_analyze.py` & `henry-temp-fix-0.3.2/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/tests/test_cli.py` & `henry-temp-fix-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/tests/test_fetcher.py` & `henry-temp-fix-0.3.2/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.1/tests/test_vacuum.py` & `henry-temp-fix-0.3.2/tests/test_vacuum.py`

 * *Files identical despite different names*

