# Comparing `tmp/gimmetool-0.1.8.tar.gz` & `tmp/gimmetool-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimmetool-0.1.8.tar", max compression
+gzip compressed data, was "gimmetool-0.1.9.tar", max compression
```

## Comparing `gimmetool-0.1.8.tar` & `gimmetool-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.8/README.md
--rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.8/gimmetool/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.8/gimmetool/gimme.py
--rwxr-xr-x   0        0        0      616 2024-04-09 22:33:40.953646 gimmetool-0.1.8/gimmetool/gimme.sh
--rwxr-xr-x   0        0        0    24798 2024-04-09 22:50:17.217717 gimmetool-0.1.8/gimmetool/gimmetool.py
--rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.8/gimmetool/setup.py
--rwxr-xr-x   0        0        0      428 2024-04-09 22:50:17.221085 gimmetool-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 gimmetool-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.9/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.9/gimmetool/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.9/gimmetool/gimme.py
+-rwxr-xr-x   0        0        0      616 2024-04-09 22:33:40.953646 gimmetool-0.1.9/gimmetool/gimme.sh
+-rwxr-xr-x   0        0        0    24798 2024-04-09 22:50:17.217717 gimmetool-0.1.9/gimmetool/gimmetool.py
+-rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.9/gimmetool/setup.py
+-rwxr-xr-x   0        0        0      428 2024-04-09 22:51:16.252336 gimmetool-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 gimmetool-0.1.9/PKG-INFO
```

### Comparing `gimmetool-0.1.8/README.md` & `gimmetool-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.8/gimmetool/gimme.sh` & `gimmetool-0.1.9/gimmetool/gimme.sh`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.8/gimmetool/gimmetool.py` & `gimmetool-0.1.9/gimmetool/gimmetool.py`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.8/gimmetool/setup.py` & `gimmetool-0.1.9/gimmetool/setup.py`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.8/PKG-INFO` & `gimmetool-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimmetool
-Version: 0.1.8
+Version: 0.1.9
 Summary: The multi-repo manager
 Author: Jeff
 Author-email: jhilton@qualtrics.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

