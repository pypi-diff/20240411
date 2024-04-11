# Comparing `tmp/pandas_datatypes-0.1.2.tar.gz` & `tmp/pandas_datatypes-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_datatypes-0.1.2.tar", last modified: Wed Apr 10 23:55:57 2024, max compression
+gzip compressed data, was "pandas_datatypes-1.1.2.tar", last modified: Thu Apr 11 20:57:52 2024, max compression
```

## Comparing `pandas_datatypes-0.1.2.tar` & `pandas_datatypes-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:55:57.917276 pandas_datatypes-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 23:55:57.917276 pandas_datatypes-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 23:55:54.000000 pandas_datatypes-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:55:57.917276 pandas_datatypes-0.1.2/pandas_datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 23:55:54.000000 pandas_datatypes-0.1.2/pandas_datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-10 23:55:54.000000 pandas_datatypes-0.1.2/pandas_datatypes/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:55:57.917276 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-10 23:55:57.000000 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 23:55:57.000000 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:55:57.000000 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 23:55:57.000000 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 23:55:57.000000 pandas_datatypes-0.1.2/pandas_datatypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:55:57.917276 pandas_datatypes-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 23:55:54.000000 pandas_datatypes-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:57:52.477042 pandas_datatypes-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 20:57:52.477042 pandas_datatypes-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-11 20:57:47.000000 pandas_datatypes-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:57:52.477042 pandas_datatypes-1.1.2/pandas_datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 20:57:47.000000 pandas_datatypes-1.1.2/pandas_datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-11 20:57:47.000000 pandas_datatypes-1.1.2/pandas_datatypes/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:57:52.477042 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 20:57:52.000000 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 20:57:52.000000 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:57:52.000000 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:57:52.000000 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 20:57:52.000000 pandas_datatypes-1.1.2/pandas_datatypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:57:52.477042 pandas_datatypes-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-11 20:57:47.000000 pandas_datatypes-1.1.2/setup.py
```

### Comparing `pandas_datatypes-0.1.2/PKG-INFO` & `pandas_datatypes-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas_datatypes
-Version: 0.1.2
+Version: 1.1.2
 Summary: A library for getting correct datatype from pandas DataFrame
 Author: Brajesh
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 
 # pandas_datatypes
```

### Comparing `pandas_datatypes-0.1.2/README.md` & `pandas_datatypes-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pandas_datatypes-0.1.2/pandas_datatypes/data_types.py` & `pandas_datatypes-1.1.2/pandas_datatypes/data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     def fill_zeros(col):
         if pd.api.types.is_numeric_dtype(col) and not pd.api.types.is_bool_dtype(col):
             if fill_numeric_zeros and col.any():
                 col.fillna(0, inplace=True)
                 if (col % 1 == 0).all():
                     return col.astype(int)
         return col
-
-    temp_df = df.apply(fill_zeros)
+    temp_df = df.copy()
+    temp_df = temp_df.apply(fill_zeros)
 
     for column in df.columns:
         if not pd.api.types.is_any_real_numeric_dtype(temp_df[column]):
             try:
                 temp_df[column] = pd.to_datetime(temp_df[column])
             except:
                 pass
```

### Comparing `pandas_datatypes-0.1.2/pandas_datatypes.egg-info/PKG-INFO` & `pandas_datatypes-1.1.2/pandas_datatypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas_datatypes
-Version: 0.1.2
+Version: 1.1.2
 Summary: A library for getting correct datatype from pandas DataFrame
 Author: Brajesh
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 
 # pandas_datatypes
```

