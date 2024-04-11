# Comparing `tmp/pgworkload-0.1.8.tar.gz` & `tmp/pgworkload-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgworkload-0.1.8.tar", max compression
+gzip compressed data, was "pgworkload-0.1.9.tar", max compression
```

## Comparing `pgworkload-0.1.8.tar` & `pgworkload-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.8/LICENSE
--rw-r--r--   0        0        0    10356 2024-04-09 18:26:42.210700 pgworkload-0.1.8/README.md
--rw-r--r--   0        0        0      510 2024-04-09 13:52:42.542259 pgworkload-0.1.8/pgworkload/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-08 20:27:05.487329 pgworkload-0.1.8/pgworkload/cli/dep.py
--rw-r--r--   0        0        0     6857 2024-04-09 15:08:48.393900 pgworkload-0.1.8/pgworkload/cli/main.py
--rw-r--r--   0        0        0     3863 2024-04-07 22:29:46.279410 pgworkload-0.1.8/pgworkload/cli/util.py
--rw-r--r--   0        0        0    10746 2024-04-07 22:27:57.469736 pgworkload-0.1.8/pgworkload/models/init.py
--rw-r--r--   0        0        0    10814 2024-04-09 16:23:08.486672 pgworkload-0.1.8/pgworkload/models/run.py
--rw-r--r--   0        0        0     7614 2024-04-08 20:36:44.283029 pgworkload-0.1.8/pgworkload/models/util.py
--rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.8/pgworkload/utils/builtin_workloads.py
--rw-r--r--   0        0        0    19696 2024-04-09 15:58:45.107198 pgworkload-0.1.8/pgworkload/utils/common.py
--rw-r--r--   0        0        0    21875 2024-04-08 20:36:56.464511 pgworkload-0.1.8/pgworkload/utils/simplefaker.py
--rw-r--r--   0        0        0      867 2024-04-09 18:28:44.359293 pgworkload-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    11514 1970-01-01 00:00:00.000000 pgworkload-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-01-28 22:12:07.442794 pgworkload-0.1.9/LICENSE
+-rw-r--r--   0        0        0    10596 2024-04-10 13:47:03.627929 pgworkload-0.1.9/README.md
+-rw-r--r--   0        0        0      510 2024-04-09 13:52:42.542259 pgworkload-0.1.9/pgworkload/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-08 20:27:05.487329 pgworkload-0.1.9/pgworkload/cli/dep.py
+-rw-r--r--   0        0        0     6858 2024-04-10 20:35:15.242271 pgworkload-0.1.9/pgworkload/cli/main.py
+-rw-r--r--   0        0        0     3863 2024-04-07 22:29:46.279410 pgworkload-0.1.9/pgworkload/cli/util.py
+-rw-r--r--   0        0        0    10746 2024-04-07 22:27:57.469736 pgworkload-0.1.9/pgworkload/models/init.py
+-rw-r--r--   0        0        0    10814 2024-04-09 16:23:08.486672 pgworkload-0.1.9/pgworkload/models/run.py
+-rw-r--r--   0        0        0     7614 2024-04-08 20:36:44.283029 pgworkload-0.1.9/pgworkload/models/util.py
+-rw-r--r--   0        0        0     2208 2023-08-09 14:49:46.761340 pgworkload-0.1.9/pgworkload/utils/builtin_workloads.py
+-rw-r--r--   0        0        0    20352 2024-04-10 20:35:15.396197 pgworkload-0.1.9/pgworkload/utils/common.py
+-rw-r--r--   0        0        0    23226 2024-04-10 20:35:15.434634 pgworkload-0.1.9/pgworkload/utils/simplefaker.py
+-rw-r--r--   0        0        0      867 2024-04-10 20:35:39.523038 pgworkload-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11754 1970-01-01 00:00:00.000000 pgworkload-0.1.9/PKG-INFO
```

### Comparing `pgworkload-0.1.8/LICENSE` & `pgworkload-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/README.md` & `pgworkload-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -176,37 +176,40 @@
 `pgworkload` will spread the load across the processes, so that each process has an even amount of threads.
 
 Example: if we set `--procs 4` and `--concurrency 10`, pgworkload will create as follows:
 
 - Process-1: MainThread + 2 extra threads. Total = 3
 - Process-2: MainThread + 2 extra threads. Total = 3
 - Process-3: MainThread + 1 extra thread.  Total = 2
-- Process-3: MainThread + 1 extra thread.  Total = 2
+- Process-4: MainThread + 1 extra thread.  Total = 2
 
 Total workloads = 10
 
 This allows you to fine tune the count of Python processes and threads to fit your system.
 
 ## Generating CSV files
 
-- You can seed a database quickly by letting pgworkload generate pseudo-random data and import it.
+- You can seed a database quickly by letting `pgworkload` generate pseudo-random data and import it.
 - `pgworkload` takes the DDL as an input and creates an intermediate YAML file, with the definition of what data you want to create (a string, a number, a date, a bool..) based on the column data type.
 - You then refine the YAML file to suit your needs, for example, the size of the string, a range for a date, the precision for a decimal, a choice among a discrete list of values..
 - You can also specify what is the percentage of NULL for any column, or how many elements in an ARRAY type.
 - You then specify the total row count, how many rows per file, and in what order, if any, to sort by.
 - Then `pgworkload` will generate the data into CSV or TSV files, compress them if so requested.
+- You can then optionally merge-sort the files using command `merge`.
 
-Write up: <https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4>
+Write up blog: [Generate multiple large sorted csv files with pseudo-random data](https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4)
 
-Find out more on the `yaml` and `csv` commands by running
+Find out more on the `yaml`, `csv` and `merge` commands by running
 
 ```bash
 pgworkload util --help
 ```
 
+Consult file `workloads/bank.yaml` for a list of all available generators and options.
+
 ## Built-in Workloads
 
 `pgworkload` has the following workload already built-in and can be called without the need to pass a class file
 
 ### Querybench
 
 Querybench runs a list of SQL Statements sequentially and iteratively.
```

### Comparing `pgworkload-0.1.8/pgworkload/cli/dep.py` & `pgworkload-0.1.9/pgworkload/cli/dep.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/cli/main.py` & `pgworkload-0.1.9/pgworkload/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         duration=duration,
         conn_duration=conn_duration,
         args=args,
         log_level=log_level.upper(),
     )
 
 
-#@app.command(help="Init the workload.", epilog=EPILOG, no_args_is_help=True)
+# @app.command(help="Init the workload.", epilog=EPILOG, no_args_is_help=True)
 def init(
     workload_path: Optional[Path] = Param.WorkloadPath,
     procs: int = Param.Procs,
     dburl: str = Param.DBUrl,
     drop: bool = typer.Option(False, "--drop", help="Drop the database if it exists."),
     csv_max_rows: int = Param.CSVMaxRows,
     skip_schema: bool = typer.Option(
```

### Comparing `pgworkload-0.1.8/pgworkload/cli/util.py` & `pgworkload-0.1.9/pgworkload/cli/util.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/models/init.py` & `pgworkload-0.1.9/pgworkload/models/init.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/models/run.py` & `pgworkload-0.1.9/pgworkload/models/run.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/models/util.py` & `pgworkload-0.1.9/pgworkload/models/util.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/utils/builtin_workloads.py` & `pgworkload-0.1.9/pgworkload/utils/builtin_workloads.py`

 * *Files identical despite different names*

### Comparing `pgworkload-0.1.8/pgworkload/utils/common.py` & `pgworkload-0.1.9/pgworkload/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -340,17 +340,17 @@
             arg = col_type_and_args[1:]
 
         if datatype.lower() in ["bool", "boolean"]:
             return {
                 "type": "bool",
                 "args": {
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in [
             "int",
             "integer",
@@ -363,17 +363,17 @@
         ]:
             return {
                 "type": "integer",
                 "args": {
                     "min": 0,
                     "max": 1000000,
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["string", "char", "character", "varchar", "text"]:
             _min = 10
             _max = 30
@@ -383,17 +383,17 @@
 
             return {
                 "type": "string",
                 "args": {
                     "min": _min,
                     "max": _max,
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in [
             "decimal",
             "float",
@@ -419,116 +419,137 @@
 
             return {
                 "type": "float",
                 "args": {
                     "max": _max,
                     "round": _round,
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["time", "timetz"]:
             return {
                 "type": "time",
                 "args": {
                     "start": "07:30:00",
                     "end": "15:30:00",
                     "micros": False,
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["json", "jsonb"]:
             return {
                 "type": "jsonb",
                 "args": {
                     "min": 10,
                     "max": 50,
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                 },
             }
 
         elif datatype.lower() == "date":
             return {
                 "type": "date",
                 "args": {
                     "start": "2022-01-01",
                     "end": "2022-12-31",
                     "format": "%Y-%m-%d",
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() in ["timestamp", "timestamptz"]:
             return {
                 "type": "timestamp",
                 "args": {
                     "start": "2022-01-01",
                     "end": "2022-12-31",
                     "format": "%Y-%m-%d %H:%M:%S.%f",
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         elif datatype.lower() == "uuid":
             return {
                 "type": "UUIDv4",
                 "args": {
                     "seed": random.random(),
-                    "null_pct": 0.0
-                    if is_not_null
-                    else round(random.randint(20, 80) / 100, 2),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
+                    "array": DEFAULT_ARRAY_COUNT if is_array else 0,
+                },
+            }
+
+        elif datatype.lower() in ["bit", "varbit"]:
+            _size = 1
+            if arg and arg[0].isdigit():
+                _size = int(arg[0])
+
+            return {
+                "type": "bit",
+                "args": {
+                    "size": _size,
+                    "seed": random.random(),
+                    "null_pct": (
+                        0.0 if is_not_null else round(random.randint(20, 80) / 100, 2)
+                    ),
                     "array": DEFAULT_ARRAY_COUNT if is_array else 0,
                 },
             }
 
         else:
             raise ValueError(f"Data type not implemented: '{datatype}'")
 
     def get_table_name_and_table_list(
         create_table_stmt: str, sort_by: list, count: int = 1000000
     ):
+        # find CREATE TABLE opening parenthesis
         p1 = create_table_stmt.find("(")
-        p2 = create_table_stmt.rfind(")")
+
+        # find CREATE TABLE closing parenthesis
+        within_brackets = 1
+        for i, c in enumerate(create_table_stmt[p1:]):
+            if c == "(":
+                within_brackets += 1
+            elif c == ")":
+                within_brackets -= 1
+            if within_brackets == 0:
+                break
+
+        # extract column definitions (within parentheses part)
+        # eg: id uuid primary key, s string(30)
+        col_def_raw = create_table_stmt[p1 + 1 : p1 + i].strip()
 
         # find table name (before parenthesis part)
         for i in create_table_stmt[:p1].split():
             if i.lower() not in RESERVED_WORDS:
                 table_name = i.replace(".", "__")
                 break
 
-        # extract column definitions (within parentheses part)
-        # eg:
-        #   id uuid primary key
-        #   s string(30)
-        col_def_raw = create_table_stmt[p1 + 1 : p2]
-
-        # remove slices delimited by parenthesis
-        # eg: from id 'sting(30)' to 'id string'
-        # this is important as within parenthesis we might find commas
-        # and we need to split on commas later
         within_brackets = 0
         col_def = ""
         for i in col_def_raw:
             if i == "(":
                 within_brackets += 1
                 col_def += " "
                 continue
@@ -575,34 +596,30 @@
             list: the list of CREATE TABLE stmts
         """
 
         # separate input into a 'create table' stmts list
         stmts = " ".join(x.lower() for x in ddl.split())
 
         # strip whitespace and remove empty items
-        stmts: list = [x.strip() for x in stmts.split(";") if x != ""]
+        stmts = [x.strip() for x in stmts.split(";") if x != ""]
 
         # keep only string that start with 'create' and
         # have word 'table' between beginning and the first open parenthesis
         create_table_stmts = []
-        for i in stmts:
-            p1 = i.find("(")
-            if i.startswith("create"):
-                if "table" in i[:p1].lower():
-                    i = i[: i.find("with")]
-                    create_table_stmts.append(i)
-
+        for stmt in stmts:
+            if stmt.startswith("create") and "table" in stmt[: stmt.find("(")].lower():
+                create_table_stmts.append(stmt)
         return create_table_stmts
 
     stmts = get_create_table_stmts(ddl)
 
     d = {}
-    for x in stmts:
+    for stmt in stmts:
         table_name, table_list = get_table_name_and_table_list(
-            x, count=1000, sort_by=[]
+            stmt, count=1000, sort_by=[]
         )
         d[table_name] = table_list
 
     return yaml.dump(d, default_flow_style=False, sort_keys=False)
 
 
 def get_threads_per_proc(procs: int, threads: int):
```

### Comparing `pgworkload-0.1.8/pgworkload/utils/simplefaker.py` & `pgworkload-0.1.9/pgworkload/utils/simplefaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,43 @@
                         f"{x}"
                         for x in [
                             self.rng.randint(self.min_num, self.max_num)
                             for _ in range(self.array)
                         ]
                     )
 
+    class Bit(Abc):
+        """Iterator that yields random bits"""
+
+        def __init__(self, size: int, seed: float, null_pct: float, array: int):
+            super().__init__(seed, null_pct, array)
+            self.size: int = 1 if size is None else size
+
+        def __next__(self):
+            if self.null_pct and self.rng.random() < self.null_pct:
+                return ""
+            else:
+                if not self.array:
+                    return "".join(
+                        [str(int(self.rng.random() > 0.5)) for _ in range(self.size)]
+                    )
+                else:
+                    return "ARRAY[%s]" % ",".join(
+                        f"B'{x}'"
+                        for x in [
+                            "".join(
+                                [
+                                    str(int(self.rng.random() > 0.5))
+                                    for _ in range(self.size)
+                                ]
+                            )
+                            for _ in range(self.array)
+                        ]
+                    )
+
     class Bool(Integer):
         """Iterator that yields a random boolean (0, 1)"""
 
         def __init__(self, seed: float, null_pct: float, array: int):
             super().__init__(
                 min_num=0, max_num=1, null_pct=null_pct, seed=seed, array=array
             )
@@ -492,14 +521,17 @@
         population = args.get("population")
         weights = args.get("weights")
         cum_weights = args.get("cum_weights")
 
         # constant
         value = args.get("value")
 
+        # bit
+        size = args.get("size")
+
         # all types
         seed = args.get("seed", self.rng.random())
 
         # create a list of pseudo random seeds
         r = random.Random(seed)
         seeds = [r.random() for _ in range(exec_threads)]
 
@@ -548,14 +580,20 @@
                 for seed in seeds
             ]
         elif type == "constant":
             return [SimpleFaker.Constant(value, seed, null_pct) for seed in seeds]
         elif type == "sequence":
             div = int(count / exec_threads)
             return [SimpleFaker.Sequence(div * x + start) for x in range(exec_threads)]
+        elif type == "bit":
+            div = int(count / exec_threads)
+            return [
+                SimpleFaker.Bit(size, seed, null_pct, array)
+                for x in range(exec_threads)
+            ]
         else:
             raise ValueError(
                 f"SimpleFaker type not implemented or recognized: '{type}'"
             )
 
     def worker(
         self,
```

### Comparing `pgworkload-0.1.8/pyproject.toml` & `pgworkload-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgworkload"
-version = "0.1.8"
+version = "0.1.9"
 description = "Workload framework for the PostgreSQL protocol"
 authors = ["Fabio Ghirardello"]
 license = "GPLv3+"
 readme = "README.md"
 homepage = "https://github.com/fabiog1901/pgworkload"
 repository = "https://github.com/fabiog1901/pgworkload"
 classifiers = [
```

### Comparing `pgworkload-0.1.8/PKG-INFO` & `pgworkload-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgworkload
-Version: 0.1.8
+Version: 0.1.9
 Summary: Workload framework for the PostgreSQL protocol
 Home-page: https://github.com/fabiog1901/pgworkload
 License: GPLv3+
 Author: Fabio Ghirardello
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
@@ -204,37 +204,40 @@
 `pgworkload` will spread the load across the processes, so that each process has an even amount of threads.
 
 Example: if we set `--procs 4` and `--concurrency 10`, pgworkload will create as follows:
 
 - Process-1: MainThread + 2 extra threads. Total = 3
 - Process-2: MainThread + 2 extra threads. Total = 3
 - Process-3: MainThread + 1 extra thread.  Total = 2
-- Process-3: MainThread + 1 extra thread.  Total = 2
+- Process-4: MainThread + 1 extra thread.  Total = 2
 
 Total workloads = 10
 
 This allows you to fine tune the count of Python processes and threads to fit your system.
 
 ## Generating CSV files
 
-- You can seed a database quickly by letting pgworkload generate pseudo-random data and import it.
+- You can seed a database quickly by letting `pgworkload` generate pseudo-random data and import it.
 - `pgworkload` takes the DDL as an input and creates an intermediate YAML file, with the definition of what data you want to create (a string, a number, a date, a bool..) based on the column data type.
 - You then refine the YAML file to suit your needs, for example, the size of the string, a range for a date, the precision for a decimal, a choice among a discrete list of values..
 - You can also specify what is the percentage of NULL for any column, or how many elements in an ARRAY type.
 - You then specify the total row count, how many rows per file, and in what order, if any, to sort by.
 - Then `pgworkload` will generate the data into CSV or TSV files, compress them if so requested.
+- You can then optionally merge-sort the files using command `merge`.
 
-Write up: <https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4>
+Write up blog: [Generate multiple large sorted csv files with pseudo-random data](https://dev.to/cockroachlabs/generate-multiple-large-sorted-csv-files-with-pseudo-random-data-1jo4)
 
-Find out more on the `yaml` and `csv` commands by running
+Find out more on the `yaml`, `csv` and `merge` commands by running
 
 ```bash
 pgworkload util --help
 ```
 
+Consult file `workloads/bank.yaml` for a list of all available generators and options.
+
 ## Built-in Workloads
 
 `pgworkload` has the following workload already built-in and can be called without the need to pass a class file
 
 ### Querybench
 
 Querybench runs a list of SQL Statements sequentially and iteratively.
```

