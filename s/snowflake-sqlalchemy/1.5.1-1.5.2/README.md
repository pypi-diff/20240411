# Comparing `tmp/snowflake-sqlalchemy-1.5.1.tar.gz` & `tmp/snowflake_sqlalchemy-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-sqlalchemy-1.5.1.tar", last modified: Thu Nov  2 19:53:19 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `snowflake-sqlalchemy-1.5.1.tar` & `snowflake_sqlalchemy-1.5.2.tar`

### file list

```diff
@@ -1,29 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 19:53:19.981799 snowflake-sqlalchemy-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2023-11-02 19:53:19.981799 snowflake-sqlalchemy-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18170 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-11-02 19:53:19.981799 snowflake-sqlalchemy-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 19:53:19.973800 snowflake-sqlalchemy-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 19:53:19.973800 snowflake-sqlalchemy-1.5.1/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 19:53:19.977800 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    37609 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21443 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/custom_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/provision.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/snowdialect.py
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-02 19:53:05.000000 snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 19:53:19.977800 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-02 19:53:19.000000 snowflake-sqlalchemy-1.5.1/src/snowflake_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.gitmodules
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/DESCRIPTION.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/license_header.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/setup.cfg
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tox.ini
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/build.sh
+-rwxr-xr-x   0        0        0      962 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/build_docker.sh
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/set_base_image.sh
+-rwxr-xr-x   0        0        0     1011 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test.sh
+-rwxr-xr-x   0        0        0     1637 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test_docker.sh
+-rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/test_linux.sh
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/docker/sqlalchemy_build/Dockerfile
+-rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/ci/docker/sqlalchemy_build/scripts/entrypoint.sh
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/_constants.py
+-rw-r--r--   0        0        0    38942 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/base.py
+-rw-r--r--   0        0        0    21461 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_commands.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_types.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/provision.py
+-rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0    32313 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/snowdialect.py
+-rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/util.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/version.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_310.reqs
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_37.reqs
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_38.reqs
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tested_requirements/requirements_39.reqs
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/README.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_compiler.py
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_copy.py
+-rw-r--r--   0        0        0    68382 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_core.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_create.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_custom_types.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_geography.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_geometry.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_multivalues_insert.py
+-rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_orm.py
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_pandas.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_qmark.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_quote.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_semi_structured_datatypes.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_sequence.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_timestamp.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_core.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_cte.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_types.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/test_unit_url.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/util.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/data/users.txt
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/README.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/conftest.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/tests/sqlalchemy_test_suite/test_suite.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/.gitignore
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/LICENSE.txt
+-rw-r--r--   0        0        0    18170 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/README.md
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 snowflake_sqlalchemy-1.5.2/PKG-INFO
```

### Comparing `snowflake-sqlalchemy-1.5.1/DESCRIPTION.md` & `snowflake_sqlalchemy-1.5.2/DESCRIPTION.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 <https://docs.snowflake.net/>
 
 Source code is also available at:
 <https://github.com/snowflakedb/snowflake-sqlalchemy>
 
 # Release Notes
 
+- v1.5.2(April 11, 2024)
+
+  - Bump min SQLAlchemy to 1.4.19 for outer lateral join
+  - Add support for sequence ordering in tests
+
 - v1.5.1(November 03, 2023)
 
   - Fixed a compatibility issue with Snowflake Behavioral Change 1057 on outer lateral join, for more details check https://docs.snowflake.com/en/release-notes/bcr-bundles/2023_04/bcr-1057.
   - Fixed credentials with `externalbrowser` authentication not caching due to incorrect parsing of boolean query parameters.
     - This fixes other boolean parameter passing to driver as well.
 
 - v1.5.0(Aug 23, 2023)
```

### Comparing `snowflake-sqlalchemy-1.5.1/LICENSE.txt` & `snowflake_sqlalchemy-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-sqlalchemy-1.5.1/README.md` & `snowflake_sqlalchemy-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/__init__.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/base.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 """
 
 
 # handle Snowflake BCR bcr-1057
 @CompileState.plugin_for("default", "select")
 class SnowflakeSelectState(SelectState):
     def _setup_joins(self, args, raw_columns):
-        for (right, onclause, left, flags) in args:
+        for right, onclause, left, flags in args:
             isouter = flags["isouter"]
             full = flags["full"]
 
             if left is None:
                 (
                     left,
                     replace_from_obj_index,
@@ -575,17 +575,19 @@
         options = (
             (
                 " "
                 + " ".join(
                     [
                         "{} = {}".format(
                             n,
-                            v._compiler_dispatch(self, **kw)
-                            if getattr(v, "compiler_dispatch", False)
-                            else str(v),
+                            (
+                                v._compiler_dispatch(self, **kw)
+                                if getattr(v, "compiler_dispatch", False)
+                                else str(v)
+                            ),
                         )
                         for n, v in options_list
                     ]
                 )
             )
             if copy_into.copy_options
             else ""
@@ -600,28 +602,32 @@
         options_list = list(formatter.options.items())
         if kw.get("deterministic", False):
             options_list.sort(key=operator.itemgetter(0))
         if "format_name" in formatter.options:
             return f"FILE_FORMAT=(format_name = {formatter.options['format_name']})"
         return "FILE_FORMAT=(TYPE={}{})".format(
             formatter.file_format,
-            " "
-            + " ".join(
-                [
-                    "{}={}".format(
-                        name,
-                        value._compiler_dispatch(self, **kw)
-                        if hasattr(value, "_compiler_dispatch")
-                        else formatter.value_repr(name, value),
-                    )
-                    for name, value in options_list
-                ]
-            )
-            if formatter.options
-            else "",
+            (
+                " "
+                + " ".join(
+                    [
+                        "{}={}".format(
+                            name,
+                            (
+                                value._compiler_dispatch(self, **kw)
+                                if hasattr(value, "_compiler_dispatch")
+                                else formatter.value_repr(name, value)
+                            ),
+                        )
+                        for name, value in options_list
+                    ]
+                )
+                if formatter.options
+                else ""
+            ),
         )
 
     def visit_aws_bucket(self, aws_bucket, **kw):
         credentials_list = list(aws_bucket.credentials_used.items())
         if kw.get("deterministic", False):
             credentials_list.sort(key=operator.itemgetter(0))
         credentials = "CREDENTIALS=({})".format(
@@ -963,14 +969,37 @@
         text = " IDENTITY"
         if identity.start is not None or identity.increment is not None:
             start = 1 if identity.start is None else identity.start
             increment = 1 if identity.increment is None else identity.increment
             text += f"({start},{increment})"
         return text
 
+    def get_identity_options(self, identity_options):
+        text = []
+        if identity_options.increment is not None:
+            text.append(f"INCREMENT BY {identity_options.increment:d}")
+        if identity_options.start is not None:
+            text.append(f"START WITH {identity_options.start:d}")
+        if identity_options.minvalue is not None:
+            text.append(f"MINVALUE {identity_options.minvalue:d}")
+        if identity_options.maxvalue is not None:
+            text.append(f"MAXVALUE {identity_options.maxvalue:d}")
+        if identity_options.nominvalue is not None:
+            text.append("NO MINVALUE")
+        if identity_options.nomaxvalue is not None:
+            text.append("NO MAXVALUE")
+        if identity_options.cache is not None:
+            text.append(f"CACHE {identity_options.cache:d}")
+        if identity_options.cycle is not None:
+            text.append("CYCLE" if identity_options.cycle else "NO CYCLE")
+        if identity_options.order is not None:
+            text.append("ORDER" if identity_options.order else "NOORDER")
+
+        return " ".join(text)
+
 
 class SnowflakeTypeCompiler(compiler.GenericTypeCompiler):
     def visit_BYTEINT(self, type_, **kw):
         return "BYTEINT"
 
     def visit_CHARACTER(self, type_, **kw):
         return "CHARACTER"
```

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/custom_commands.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,16 @@
             self.options["FIELD_DELIMITER"] = hex(deli_type)
         else:
             self.options["FIELD_DELIMITER"] = deli_type
         return self
 
     def file_extension(self, ext):
         """String that specifies the extension for files unloaded to a stage. Accepts any extension. The user is
-        responsible for specifying a valid file extension that can be read by the desired software or service."""
+        responsible for specifying a valid file extension that can be read by the desired software or service.
+        """
         if not isinstance(ext, (NoneType, string_types)):
             raise TypeError("File extension should be a string")
         self.options["FILE_EXTENSION"] = ext
         return self
 
     def date_format(self, dt_frmt):
         """String that defines the format of date values in the unloaded data files."""
@@ -382,15 +383,16 @@
         if comp_type not in _available_options:
             raise TypeError(f"Compression type should be one of : {_available_options}")
         self.options["COMPRESSION"] = comp_type
         return self
 
     def file_extension(self, ext):
         """String that specifies the extension for files unloaded to a stage. Accepts any extension. The user is
-        responsible for specifying a valid file extension that can be read by the desired software or service."""
+        responsible for specifying a valid file extension that can be read by the desired software or service.
+        """
         if not isinstance(ext, (NoneType, string_types)):
             raise TypeError("File extension should be a string")
         self.options["FILE_EXTENSION"] = ext
         return self
 
 
 class PARQUETFormatter(CopyFormatter):
```

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/custom_types.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/custom_types.py`

 * *Files identical despite different names*

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/requirements.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/snowdialect.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/snowdialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,19 +591,21 @@
                     "name": column_name,
                     "type": type_instance,
                     "nullable": is_nullable == "YES",
                     "default": column_default,
                     "autoincrement": is_identity == "YES",
                     "comment": comment,
                     "primary_key": (
-                        column_name
-                        in schema_primary_keys[table_name]["constrained_columns"]
-                    )
-                    if current_table_pks
-                    else False,
+                        (
+                            column_name
+                            in schema_primary_keys[table_name]["constrained_columns"]
+                        )
+                        if current_table_pks
+                        else False
+                    ),
                 }
             )
             if is_identity == "YES":
                 ans[table_name][-1]["identity"] = {
                     "start": identity_start,
                     "increment": identity_increment,
                 }
@@ -684,19 +686,21 @@
                     "name": column_name,
                     "type": type_instance,
                     "nullable": is_nullable == "YES",
                     "default": column_default,
                     "autoincrement": is_identity == "YES",
                     "comment": comment if comment != "" else None,
                     "primary_key": (
-                        column_name
-                        in schema_primary_keys[table_name]["constrained_columns"]
-                    )
-                    if current_table_pks
-                    else False,
+                        (
+                            column_name
+                            in schema_primary_keys[table_name]["constrained_columns"]
+                        )
+                        if current_table_pks
+                        else False
+                    ),
                 }
             )
 
         # If we didn't find any columns for the table, the table doesn't exist.
         if len(ans) == 0:
             raise sa_exc.NoSuchTableError()
         return ans
@@ -872,26 +876,30 @@
         """
         result = self._get_table_comment(connection, table_name, schema)
         if result is None:
             # the "table" being reflected is actually a view
             result = self._get_view_comment(connection, table_name, schema)
 
         return {
-            "text": result._mapping["comment"]
-            if result and result._mapping["comment"]
-            else None
+            "text": (
+                result._mapping["comment"]
+                if result and result._mapping["comment"]
+                else None
+            )
         }
 
     def connect(self, *cargs, **cparams):
         return (
             super().connect(
                 *cargs,
-                **_update_connection_application_name(**cparams)
-                if _ENABLE_SQLALCHEMY_AS_APPLICATION_NAME
-                else cparams,
+                **(
+                    _update_connection_application_name(**cparams)
+                    if _ENABLE_SQLALCHEMY_AS_APPLICATION_NAME
+                    else cparams
+                ),
             )
             if _ENABLE_SQLALCHEMY_AS_APPLICATION_NAME
             else super().connect(*cargs, **cparams)
         )
 
 
 @sa_vnt.listens_for(Table, "before_create")
```

### Comparing `snowflake-sqlalchemy-1.5.1/src/snowflake/sqlalchemy/util.py` & `snowflake_sqlalchemy-1.5.2/src/snowflake/sqlalchemy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,22 @@
             left_selectable = left_info.selectable
 
             if sql_util.clause_is_present(on_selectable, left_selectable):
                 adapt_from = on_selectable
             else:
                 adapt_from = left_selectable
 
-            (pj, sj, source, dest, secondary, target_adapter,) = prop._create_joins(
+            (
+                pj,
+                sj,
+                source,
+                dest,
+                secondary,
+                target_adapter,
+            ) = prop._create_joins(
                 source_selectable=adapt_from,
                 dest_selectable=adapt_to,
                 source_polymorphic=True,
                 of_type_entity=right_info,
                 alias_secondary=True,
                 extra_criteria=_extra_criteria,
             )
```

