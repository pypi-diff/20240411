# Comparing `tmp/pandas_pyarrow-0.1.5.tar.gz` & `tmp/pandas_pyarrow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_pyarrow-0.1.5.tar", max compression
+gzip compressed data, was "pandas_pyarrow-0.1.6.tar", max compression
```

## Comparing `pandas_pyarrow-0.1.5.tar` & `pandas_pyarrow-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/LICENSE
--rw-r--r--   0        0        0     6620 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/README.md
--rw-r--r--   0        0        0      150 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/__init__.py
--rw-r--r--   0        0        0      833 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/__init__.py
--rw-r--r--   0        0        0      552 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/datetime_mapper.py
--rw-r--r--   0        0        0      133 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/db_types.py
--rw-r--r--   0        0        0      561 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/dtype_mapper.py
--rw-r--r--   0        0        0      810 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/numeric_mapper.py
--rw-r--r--   0        0        0     2034 2024-03-19 17:15:26.235576 pandas_pyarrow-0.1.5/pandas_pyarrow/pda_converter.py
--rw-r--r--   0        0        0     2582 2024-03-19 17:15:54.803938 pandas_pyarrow-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8287 1970-01-01 00:00:00.000000 pandas_pyarrow-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6620 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/README.md
+-rw-r--r--   0        0        0      230 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/pandas_pyarrow/__init__.py
+-rw-r--r--   0        0        0      833 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/datetime_mapper.py
+-rw-r--r--   0        0        0      133 2024-04-11 19:41:02.860644 pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/db_types.py
+-rw-r--r--   0        0        0      561 2024-04-11 19:41:02.864644 pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/dtype_mapper.py
+-rw-r--r--   0        0        0      810 2024-04-11 19:41:02.864644 pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/numeric_mapper.py
+-rw-r--r--   0        0        0     2034 2024-04-11 19:41:02.864644 pandas_pyarrow-0.1.6/pandas_pyarrow/pda_converter.py
+-rw-r--r--   0        0        0     2582 2024-04-11 19:41:31.048720 pandas_pyarrow-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8287 1970-01-01 00:00:00.000000 pandas_pyarrow-0.1.6/PKG-INFO
```

### Comparing `pandas_pyarrow-0.1.5/LICENSE` & `pandas_pyarrow-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/README.md` & `pandas_pyarrow-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/__init__.py` & `pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/datetime_mapper.py` & `pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/datetime_mapper.py`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/dtype_mapper.py` & `pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/dtype_mapper.py`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pandas_pyarrow/mappers/numeric_mapper.py` & `pandas_pyarrow-0.1.6/pandas_pyarrow/mappers/numeric_mapper.py`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pandas_pyarrow/pda_converter.py` & `pandas_pyarrow-0.1.6/pandas_pyarrow/pda_converter.py`

 * *Files identical despite different names*

### Comparing `pandas_pyarrow-0.1.5/pyproject.toml` & `pandas_pyarrow-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-pyarrow"
-version = "v0.1.5"
+version = "v0.1.6"
 description = "A library for switching pandas backend to pyarrow"
 authors = ["DanielAvdar <66269169+DanielAvdar@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DanielAvdar/pandas-pyarrow"
 repository = "https://github.com/DanielAvdar/pandas-pyarrow"
 documentation = "https://github.com/DanielAvdar/pandas-pyarrow"
```

### Comparing `pandas_pyarrow-0.1.5/PKG-INFO` & `pandas_pyarrow-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-pyarrow
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for switching pandas backend to pyarrow
 Home-page: https://github.com/DanielAvdar/pandas-pyarrow
 License: MIT
 Keywords: python,pandas,pyarrow,arrow,dataframe,bigquery,pandas-pyarrow,pandas-arrow
 Author: DanielAvdar
 Author-email: 66269169+DanielAvdar@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
```

