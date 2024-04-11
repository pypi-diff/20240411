# Comparing `tmp/davify-1.1.0.tar.gz` & `tmp/davify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davify-1.1.0.tar", max compression
+gzip compressed data, was "davify-1.1.1.tar", max compression
```

## Comparing `davify-1.1.0.tar` & `davify-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35122 2021-02-19 06:41:32.248090 davify-1.1.0/LICENSE
--rw-r--r--   0        0        0     2748 2024-04-11 05:32:53.538977 davify-1.1.0/README.md
--rw-r--r--   0        0        0      896 2024-04-11 06:31:01.806561 davify-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-19 06:41:32.248090 davify-1.1.0/src/davify/__init__.py
--rwxr-xr-x   0        0        0     9355 2024-04-11 06:35:33.101893 davify-1.1.0/src/davify/cli.py
--rw-r--r--   0        0        0      838 2024-04-11 05:32:53.542978 davify-1.1.0/src/davify/config.py
--rw-r--r--   0        0        0     1885 2024-04-11 06:32:39.654287 davify-1.1.0/src/davify/housekeeping.py
--rw-r--r--   0        0        0     1671 2024-04-11 06:22:48.338681 davify-1.1.0/src/davify/keyring.py
--rw-r--r--   0        0        0     2953 2024-04-11 06:21:17.358621 davify-1.1.0/src/davify/transform.py
--rw-r--r--   0        0        0      552 2024-04-11 05:51:39.133037 davify-1.1.0/src/davify/upload.py
--rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 davify-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35122 2021-02-19 06:41:32.248090 davify-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2748 2024-04-11 05:32:53.538977 davify-1.1.1/README.md
+-rw-r--r--   0        0        0      919 2024-04-11 06:40:25.269411 davify-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-19 06:41:32.248090 davify-1.1.1/src/davify/__init__.py
+-rwxr-xr-x   0        0        0     9355 2024-04-11 06:35:33.101893 davify-1.1.1/src/davify/cli.py
+-rw-r--r--   0        0        0      838 2024-04-11 05:32:53.542978 davify-1.1.1/src/davify/config.py
+-rw-r--r--   0        0        0     1885 2024-04-11 06:32:39.654287 davify-1.1.1/src/davify/housekeeping.py
+-rw-r--r--   0        0        0     1671 2024-04-11 06:22:48.338681 davify-1.1.1/src/davify/keyring.py
+-rw-r--r--   0        0        0     2953 2024-04-11 06:21:17.358621 davify-1.1.1/src/davify/transform.py
+-rw-r--r--   0        0        0      552 2024-04-11 05:51:39.133037 davify-1.1.1/src/davify/upload.py
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 davify-1.1.1/PKG-INFO
```

### Comparing `davify-1.1.0/LICENSE` & `davify-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/README.md` & `davify-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/pyproject.toml` & `davify-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "davify"
-version = "1.1.0"
+version = "1.1.1"
 description = "Davify uploads files to webdav servers and provides a download link for accessing them."
 keywords = ["webdav"]
 authors = ["Albert Weichselbraun <albert@weichselbraun.net>"]
 license = "GPL3"
 homepage = "https://github.com/AlbertWeichselbraun/davify"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8 || ^3.9 || ^3.10 || ^3.11 || ^3.12"
 secretstorage = "^3.3.3"
 pyperclip = "^1.8.2"
+requests = "^2.31.0"
+
 
 
 [tool.poetry.scripts]
 davify = "davify.cli:cli"
 clean-davify-directory = "davify.housekeeping:cli"
 
 [tool.poetry.extras]
@@ -28,8 +30,8 @@
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311", "py312"]
 extend-exclude = '\.html$|\.txt$'
 include = '''
   ^/src/|^/tests/
-'''
+'''
```

### Comparing `davify-1.1.0/src/davify/cli.py` & `davify-1.1.1/src/davify/cli.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/src/davify/config.py` & `davify-1.1.1/src/davify/config.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/src/davify/housekeeping.py` & `davify-1.1.1/src/davify/housekeeping.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/src/davify/keyring.py` & `davify-1.1.1/src/davify/keyring.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/src/davify/transform.py` & `davify-1.1.1/src/davify/transform.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/src/davify/upload.py` & `davify-1.1.1/src/davify/upload.py`

 * *Files identical despite different names*

### Comparing `davify-1.1.0/PKG-INFO` & `davify-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: davify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Davify uploads files to webdav servers and provides a download link for accessing them.
 Home-page: https://github.com/AlbertWeichselbraun/davify
 License: GPL3
 Keywords: webdav
 Author: Albert Weichselbraun
 Author-email: albert@weichselbraun.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: secretstorage (>=3.3.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 ## davify 
 Uploads files to a WebDAV server for retrieval via https.
 
 ## The problem davify solves
```

