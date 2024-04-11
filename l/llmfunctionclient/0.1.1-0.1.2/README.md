# Comparing `tmp/llmfunctionclient-0.1.1.tar.gz` & `tmp/llmfunctionclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfunctionclient-0.1.1.tar", max compression
+gzip compressed data, was "llmfunctionclient-0.1.2.tar", max compression
```

## Comparing `llmfunctionclient-0.1.1.tar` & `llmfunctionclient-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4328 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/README.md
--rw-r--r--   0        0        0       19 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/llmfunctionclient/__init__.py
--rw-r--r--   0        0        0     3936 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/llmfunctionclient/main.py
--rw-r--r--   0        0        0      321 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-10 23:40:47.422759 llmfunctionclient-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     4328 2024-04-10 23:40:47.422759 llmfunctionclient-0.1.2/README.md
+-rw-r--r--   0        0        0       19 2024-04-10 23:40:47.422759 llmfunctionclient-0.1.2/llmfunctionclient/__init__.py
+-rw-r--r--   0        0        0     6832 2024-04-10 23:40:47.422759 llmfunctionclient-0.1.2/llmfunctionclient/main.py
+-rw-r--r--   0        0        0      321 2024-04-10 23:40:47.422759 llmfunctionclient-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.2/PKG-INFO
```

### Comparing `llmfunctionclient-0.1.1/LICENSE.md` & `llmfunctionclient-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmfunctionclient-0.1.1/README.md` & `llmfunctionclient-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llmfunctionclient-0.1.1/PKG-INFO` & `llmfunctionclient-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfunctionclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: James Mills
 Author-email: jimmyemills@gmail.com
 Requires-Python: >=3.4,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

