# Comparing `tmp/decorator_validation-3.0.2.tar.gz` & `tmp/decorator_validation-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_validation-3.0.2.tar", max compression
+gzip compressed data, was "decorator_validation-3.0.3.tar", max compression
```

## Comparing `decorator_validation-3.0.2.tar` & `decorator_validation-3.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      119 2023-08-07 18:01:40.419170 decorator_validation-3.0.2/decorator_validation/__init__.py
--rw-r--r--   0        0        0    10270 2023-10-22 18:24:33.121185 decorator_validation-3.0.2/decorator_validation/decorators.py
--rw-r--r--   0        0        0     1507 2023-08-10 17:41:45.823410 decorator_validation-3.0.2/decorator_validation/std_validators.py
--rw-r--r--   0        0        0      228 2023-08-07 18:01:40.420171 decorator_validation-3.0.2/decorator_validation/types.py
--rw-r--r--   0        0        0     1086 2023-08-05 06:26:33.296117 decorator_validation-3.0.2/LICENSE
--rw-r--r--   0        0        0      668 2023-10-22 18:25:31.666494 decorator_validation-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     4407 2023-10-22 18:22:49.441493 decorator_validation-3.0.2/README.md
--rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 decorator_validation-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-08-07 18:01:40.419170 decorator_validation-3.0.3/decorator_validation/__init__.py
+-rw-r--r--   0        0        0    10270 2023-10-22 18:24:33.121185 decorator_validation-3.0.3/decorator_validation/decorators.py
+-rw-r--r--   0        0        0     1582 2024-04-11 09:49:39.671030 decorator_validation-3.0.3/decorator_validation/std_validators.py
+-rw-r--r--   0        0        0      228 2023-08-07 18:01:40.420171 decorator_validation-3.0.3/decorator_validation/types.py
+-rw-r--r--   0        0        0     1086 2023-08-05 06:26:33.296117 decorator_validation-3.0.3/LICENSE
+-rw-r--r--   0        0        0      668 2024-04-11 09:45:33.420173 decorator_validation-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4407 2023-10-22 18:22:49.441493 decorator_validation-3.0.3/README.md
+-rw-r--r--   0        0        0     4769 1970-01-01 00:00:00.000000 decorator_validation-3.0.3/PKG-INFO
```

### Comparing `decorator_validation-3.0.2/decorator_validation/decorators.py` & `decorator_validation-3.0.3/decorator_validation/decorators.py`

 * *Files identical despite different names*

### Comparing `decorator_validation-3.0.2/decorator_validation/std_validators.py` & `decorator_validation-3.0.3/decorator_validation/std_validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Union, Tuple, Iterable, Sequence
 from pathlib import Path
 
 
 def is_file(file: Union[str, Path]) -> bool:
     """check if file is a file"""
-    return Path(file).resolve().is_file()
+    if not Path(file).resolve().is_file():
+        raise TypeError(f"File {file} does not exist!")
+    return True
 
 
 def is_iterable_of(type_: Union[type, Tuple[type]]):
     def check_fn(arg: Iterable):
         if not isinstance(arg, Iterable):
             raise TypeError("Argument has to be an iterable!")
         for a in arg:
```

### Comparing `decorator_validation-3.0.2/LICENSE` & `decorator_validation-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator_validation-3.0.2/pyproject.toml` & `decorator_validation-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decorator_validation"
-version = "3.0.2"
+version = "3.0.3"
 description = "Fast Argument validation for functions using decorators"
 authors = ["FailedRobot <sry@nomail.com>"]
 homepage = "https://github.com/ahartlba/decorator_validation"
 readme = "README.md"
 packages = [{include = "decorator_validation"}]
 
 [tool.poetry.dependencies]
```

### Comparing `decorator_validation-3.0.2/README.md` & `decorator_validation-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `decorator_validation-3.0.2/PKG-INFO` & `decorator_validation-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-validation
-Version: 3.0.2
+Version: 3.0.3
 Summary: Fast Argument validation for functions using decorators
 Home-page: https://github.com/ahartlba/decorator_validation
 Author: FailedRobot
 Author-email: sry@nomail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

