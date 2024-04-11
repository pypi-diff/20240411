# Comparing `tmp/fidelius-1.0.0.tar.gz` & `tmp/fidelius-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fidelius-1.0.0.tar", last modified: Thu Apr 11 17:16:10 2024, max compression
+gzip compressed data, was "fidelius-1.0.0b1.tar", last modified: Thu Apr 11 15:52:23 2024, max compression
```

## Comparing `fidelius-1.0.0.tar` & `fidelius-1.0.0b1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.674915 fidelius-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 17:16:01.000000 fidelius-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-04-11 17:16:10.674915 fidelius-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-04-11 17:16:01.000000 fidelius-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.666915 fidelius-1.0.0/fidelius/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.670915 fidelius-1.0.0/fidelius/fideliusapi/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/fideliusapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.670915 fidelius-1.0.0/fidelius/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.670915 fidelius-1.0.0/fidelius/gateway/mock/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/mock/_inmemcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/mock/_mockadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/mock/_mockrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/mock/_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.670915 fidelius-1.0.0/fidelius/gateway/paramstore/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/paramstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/paramstore/_paramstoreadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/paramstore/_paramstorerepo.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/gateway/paramstore/_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.674915 fidelius-1.0.0/fidelius/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/_appprops.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 17:16:01.000000 fidelius-1.0.0/fidelius/structs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:10.674915 fidelius-1.0.0/fidelius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-04-11 17:16:10.000000 fidelius-1.0.0/fidelius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 17:16:10.000000 fidelius-1.0.0/fidelius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:16:10.000000 fidelius-1.0.0/fidelius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 17:16:10.000000 fidelius-1.0.0/fidelius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 17:16:10.000000 fidelius-1.0.0/fidelius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-11 17:16:01.000000 fidelius-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:16:10.674915 fidelius-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 17:16:01.000000 fidelius-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/fideliusapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/fideliusapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_inmemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_mockadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_mockrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/mock/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.413746 fidelius-1.0.0b1/fidelius/gateway/paramstore/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstoreadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstorerepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/gateway/paramstore/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/fidelius/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_appprops.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/fidelius/structs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/fidelius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 15:52:23.000000 fidelius-1.0.0b1/fidelius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:52:23.417746 fidelius-1.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 15:52:13.000000 fidelius-1.0.0b1/setup.py
```

### Comparing `fidelius-1.0.0/LICENSE` & `fidelius-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/PKG-INFO` & `fidelius-1.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 1.0.0
+Version: 1.0.0b1
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fidelius-1.0.0/README.md` & `fidelius-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/__init__.py` & `fidelius-1.0.0b1/fidelius/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/_abstract.py` & `fidelius-1.0.0b1/fidelius/gateway/_abstract.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/interface.py` & `fidelius-1.0.0b1/fidelius/gateway/interface.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/mock/_mockadmin.py` & `fidelius-1.0.0b1/fidelius/gateway/mock/_mockadmin.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/mock/_mockrepo.py` & `fidelius-1.0.0b1/fidelius/gateway/mock/_mockrepo.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/paramstore/_paramstoreadmin.py` & `fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstoreadmin.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/gateway/paramstore/_paramstorerepo.py` & `fidelius-1.0.0b1/fidelius/gateway/paramstore/_paramstorerepo.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/structs/_appprops.py` & `fidelius-1.0.0b1/fidelius/structs/_appprops.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius/structs/_tags.py` & `fidelius-1.0.0b1/fidelius/structs/_tags.py`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/fidelius.egg-info/PKG-INFO` & `fidelius-1.0.0b1/fidelius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidelius
-Version: 1.0.0
+Version: 1.0.0b1
 Summary: The Fidelius Charm! (keeping things secret)
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Kristin Fjola Tomasdottir <kristinf@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2022-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fidelius-1.0.0/fidelius.egg-info/SOURCES.txt` & `fidelius-1.0.0b1/fidelius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fidelius-1.0.0/pyproject.toml` & `fidelius-1.0.0b1/pyproject.toml`

 * *Files identical despite different names*

