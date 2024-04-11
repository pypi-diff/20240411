# Comparing `tmp/py_ballisticcalc.exts-2.0.0b5.tar.gz` & `tmp/py_ballisticcalc.exts-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc.exts-2.0.0b5.tar", last modified: Sat Apr  6 18:54:55 2024, max compression
+gzip compressed data, was "py_ballisticcalc.exts-2.0.1.tar", last modified: Thu Apr 11 16:15:00 2024, max compression
```

## Comparing `py_ballisticcalc.exts-2.0.0b5.tar` & `py_ballisticcalc.exts-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:55.828181 py_ballisticcalc.exts-2.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-06 18:54:44.000000 py_ballisticcalc.exts-2.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-06 18:54:55.828181 py_ballisticcalc.exts-2.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-06 18:54:44.000000 py_ballisticcalc.exts-2.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:55.828181 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-06 18:54:55.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 18:54:55.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:54:55.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 18:54:55.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:54:55.828181 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc_exts/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-06 18:54:44.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc_exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   816102 2024-04-06 18:54:55.000000 py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc_exts/trajectory_calc.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-06 18:54:44.000000 py_ballisticcalc.exts-2.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:54:55.828181 py_ballisticcalc.exts-2.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-06 18:54:44.000000 py_ballisticcalc.exts-2.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:15:00.035876 py_ballisticcalc.exts-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 16:14:46.000000 py_ballisticcalc.exts-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-04-11 16:15:00.035876 py_ballisticcalc.exts-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-11 16:14:46.000000 py_ballisticcalc.exts-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:15:00.031876 py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-04-11 16:15:00.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 16:15:00.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:15:00.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 16:15:00.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:15:00.031876 py_ballisticcalc.exts-2.0.1/py_ballisticcalc_exts/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 16:14:46.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc_exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   816102 2024-04-11 16:14:59.000000 py_ballisticcalc.exts-2.0.1/py_ballisticcalc_exts/trajectory_calc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-11 16:14:46.000000 py_ballisticcalc.exts-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:15:00.035876 py_ballisticcalc.exts-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-11 16:14:46.000000 py_ballisticcalc.exts-2.0.1/setup.py
```

### Comparing `py_ballisticcalc.exts-2.0.0b5/LICENSE` & `py_ballisticcalc.exts-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b5/PKG-INFO` & `py_ballisticcalc.exts-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b5
+Version: 2.0.1
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b5/README.md` & `py_ballisticcalc.exts-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc.exts.egg-info/PKG-INFO` & `py_ballisticcalc.exts-2.0.1/py_ballisticcalc.exts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b5
+Version: 2.0.1
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py_ballisticcalc.exts-2.0.0b5/py_ballisticcalc_exts/trajectory_calc.c` & `py_ballisticcalc.exts-2.0.1/py_ballisticcalc_exts/trajectory_calc.c`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b5/pyproject.toml` & `py_ballisticcalc.exts-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel", 'cython']
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc.exts"
-version = "2.0.0b5"
+version = "2.0.1"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
```

### Comparing `py_ballisticcalc.exts-2.0.0b5/setup.py` & `py_ballisticcalc.exts-2.0.1/setup.py`

 * *Files identical despite different names*

