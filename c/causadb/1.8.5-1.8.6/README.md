# Comparing `tmp/causadb-1.8.5.tar.gz` & `tmp/causadb-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.8.5.tar", max compression
+gzip compressed data, was "causadb-1.8.6.tar", max compression
```

## Comparing `causadb-1.8.5.tar` & `causadb-1.8.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      642 2024-04-08 14:43:25.874668 causadb-1.8.5/README.md
--rw-r--r--   0        0        0      115 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-08 14:43:56.814809 causadb-1.8.5/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/causadb.py
--rw-r--r--   0        0        0     2109 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/cli/account.py
--rw-r--r--   0        0        0     3153 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/cli/main.py
--rw-r--r--   0        0        0     7104 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-08 14:43:25.874668 causadb-1.8.5/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-08 14:43:25.878668 causadb-1.8.5/causadb/examples/heating.py
--rw-r--r--   0        0        0    15743 2024-04-08 14:43:25.878668 causadb-1.8.5/causadb/model.py
--rw-r--r--   0        0        0     2555 2024-04-08 14:43:25.878668 causadb-1.8.5/causadb/plotting.py
--rw-r--r--   0        0        0      215 2024-04-08 14:43:25.878668 causadb-1.8.5/causadb/utils.py
--rw-r--r--   0        0        0      797 2024-04-08 14:43:56.066806 causadb-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-10 19:34:03.400593 causadb-1.8.6/README.md
+-rw-r--r--   0        0        0      115 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-10 19:34:31.796477 causadb-1.8.6/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/causadb.py
+-rw-r--r--   0        0        0     2109 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/cli/account.py
+-rw-r--r--   0        0        0     3153 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/cli/main.py
+-rw-r--r--   0        0        0     7104 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15743 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-10 19:34:03.400593 causadb-1.8.6/causadb/utils.py
+-rw-r--r--   0        0        0      797 2024-04-10 19:34:30.812481 causadb-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.6/PKG-INFO
```

### Comparing `causadb-1.8.5/README.md` & `causadb-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/causadb.py` & `causadb-1.8.6/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/cli/account.py` & `causadb-1.8.6/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/cli/data.py` & `causadb-1.8.6/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/cli/main.py` & `causadb-1.8.6/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/cli/models.py` & `causadb-1.8.6/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/cli/utils.py` & `causadb-1.8.6/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/data.py` & `causadb-1.8.6/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/examples/heating.py` & `causadb-1.8.6/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/model.py` & `causadb-1.8.6/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/causadb/plotting.py` & `causadb-1.8.6/causadb/plotting.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.5/pyproject.toml` & `causadb-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.8.5"
+version = "1.8.6"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.8.5/PKG-INFO` & `causadb-1.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.8.5
+Version: 1.8.6
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

