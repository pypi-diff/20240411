# Comparing `tmp/dropbase-0.3.0.tar.gz` & `tmp/dropbase-0.3.1.tar.gz`

## Comparing `dropbase-0.3.0.tar` & `dropbase-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/constants.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/connect.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/database.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/sources.py
--rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/databases/mysql.py
--rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/databases/postgres.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/databases/snowflake.py
--rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/database/databases/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/helpers/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/helpers/dataframe.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/category.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/common.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/button_column.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/mysql_column.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/pg_column.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/py_column.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/snowflake_column.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/sqlite_column.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/table/tables.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/__init__.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/boolean.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/button.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/input.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/select.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/text.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/models/widget/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/columns.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/database.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/display_rules.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/edit_cell.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/files.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/function.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/page.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/query.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/run_python.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/table.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/schemas/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/worker/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/worker/run_python_file.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 dropbase-0.3.0/src/dropbase/worker/run_python_string.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dropbase-0.3.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dropbase-0.3.0/LICENSE
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dropbase-0.3.0/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 dropbase-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dropbase-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/constants.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/connect.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/database.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/sources.py
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/databases/mysql.py
+-rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/databases/postgres.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/databases/snowflake.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/database/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/helpers/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/helpers/dataframe.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/category.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/common.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/__init__.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/button_column.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/mysql_column.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/pg_column.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/py_column.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/snowflake_column.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/sqlite_column.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/table/tables.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/__init__.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/boolean.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/button.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/input.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/select.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/text.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/models/widget/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/columns.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/database.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/display_rules.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/edit_cell.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/files.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/function.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/page.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/query.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/run_python.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/table.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/schemas/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/worker/__init__.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/worker/run_python_file.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 dropbase-0.3.1/src/dropbase/worker/run_python_string.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dropbase-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dropbase-0.3.1/LICENSE
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dropbase-0.3.1/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 dropbase-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dropbase-0.3.1/PKG-INFO
```

### Comparing `dropbase-0.3.0/src/dropbase/database/connect.py` & `dropbase-0.3.1/src/dropbase/database/connect.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/database.py` & `dropbase-0.3.1/src/dropbase/database/database.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/sources.py` & `dropbase-0.3.1/src/dropbase/database/sources.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/databases/mysql.py` & `dropbase-0.3.1/src/dropbase/database/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/databases/postgres.py` & `dropbase-0.3.1/src/dropbase/database/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/databases/snowflake.py` & `dropbase-0.3.1/src/dropbase/database/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/database/databases/sqlite.py` & `dropbase-0.3.1/src/dropbase/database/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/helpers/dataframe.py` & `dropbase-0.3.1/src/dropbase/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/common.py` & `dropbase-0.3.1/src/dropbase/models/common.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/button_column.py` & `dropbase-0.3.1/src/dropbase/models/table/button_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/mysql_column.py` & `dropbase-0.3.1/src/dropbase/models/table/mysql_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/pg_column.py` & `dropbase-0.3.1/src/dropbase/models/table/pg_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/snowflake_column.py` & `dropbase-0.3.1/src/dropbase/models/table/snowflake_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/sqlite_column.py` & `dropbase-0.3.1/src/dropbase/models/table/sqlite_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/table/tables.py` & `dropbase-0.3.1/src/dropbase/models/table/tables.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/boolean.py` & `dropbase-0.3.1/src/dropbase/models/widget/boolean.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/button.py` & `dropbase-0.3.1/src/dropbase/models/widget/button.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/input.py` & `dropbase-0.3.1/src/dropbase/models/widget/input.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/select.py` & `dropbase-0.3.1/src/dropbase/models/widget/select.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/text.py` & `dropbase-0.3.1/src/dropbase/models/widget/text.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/models/widget/widgets.py` & `dropbase-0.3.1/src/dropbase/models/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/schemas/database.py` & `dropbase-0.3.1/src/dropbase/schemas/database.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/schemas/files.py` & `dropbase-0.3.1/src/dropbase/schemas/files.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/schemas/page.py` & `dropbase-0.3.1/src/dropbase/schemas/page.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/schemas/run_python.py` & `dropbase-0.3.1/src/dropbase/schemas/run_python.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/schemas/table.py` & `dropbase-0.3.1/src/dropbase/schemas/table.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/src/dropbase/worker/run_python_file.py` & `dropbase-0.3.1/src/dropbase/worker/run_python_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 import json
 import os
 import traceback
 
 from dotenv import load_dotenv
 
 from dropbase.helpers.dataframe import convert_df_to_resp_obj
+from server.controllers.display_rules import run_display_rule
 
 load_dotenv()
 
 
 def get_function_by_name(app_name: str, page_name: str, function_name: str):
     file_module = f"workspace.{app_name}.{page_name}.scripts.{function_name}"
     scripts = importlib.import_module(file_module)
     function = getattr(scripts, function_name)
     return function
 
 
-def get_state(app_name: str, page_name: str, class_dict: dict, class_name: str = "State"):
+def get_state(
+    app_name: str, page_name: str, class_dict: dict, class_name: str = "State"
+):
     page_module = f"workspace.{app_name}.{page_name}"
     page = importlib.import_module(page_module)
     ClassName = getattr(page, class_name)
     return ClassName(**class_dict)
 
 
 # run data fetcher code
@@ -31,21 +34,24 @@
     function_name = get_function_by_name(app_name, page_name, file.get("name"))
     # call function
     df = function_name(**args)
     return convert_df_to_resp_obj(df, "python")
 
 
 # for ui functions
-def run_python_ui(app_name: str, page_name: str, file: dict, state: dict, context: dict):
+def run_python_ui(
+    app_name: str, page_name: str, file: dict, state: dict, context: dict
+):
     state = get_state(app_name, page_name, state, "State")
     context = get_state(app_name, page_name, context, "Context")
     args = {"state": state, "context": context}
     function_name = get_function_by_name(app_name, page_name, file.get("name"))
     # call function
     context = function_name(**args)
+    context = run_display_rule(app_name, page_name, state, context)
     return context.dict()
 
 
 def run(r, response):
     try:
         # get evn variables
         app_name = os.getenv("app_name")
```

### Comparing `dropbase-0.3.0/src/dropbase/worker/run_python_string.py` & `dropbase-0.3.1/src/dropbase/worker/run_python_string.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/LICENSE` & `dropbase-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.0/pyproject.toml` & `dropbase-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dropbase"
-version = "0.3.0"
+version = "0.3.1"
 authors = [{ name = "Dropbase", email = "support@dropbase.io" }]
 description = "Dropbase"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
   "sqlalchemy==1.4.46",
   "pymysql==1.1.0",
```

### Comparing `dropbase-0.3.0/PKG-INFO` & `dropbase-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dropbase
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dropbase
 Project-URL: Homepage, https://github.com/dropbase/dropbase_package
 Project-URL: Bug Tracker, https://github.com/dropbase/dropbase_package/issues
 Author-email: Dropbase <support@dropbase.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

