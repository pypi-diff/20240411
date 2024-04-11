# Comparing `tmp/geventhttpclient-2.1.0.tar.gz` & `tmp/geventhttpclient-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.1.0.tar", last modified: Thu Apr 11 05:46:06 2024, max compression
+gzip compressed data, was "geventhttpclient-2.1.1.tar", last modified: Thu Apr 11 06:49:11 2024, max compression
```

## Comparing `geventhttpclient-2.1.0.tar` & `geventhttpclient-2.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/ext/Python_compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/ext/_parser.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/LICENSE-MIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/include/
--rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/include/llhttp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/api.c
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/http.c
--rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/llhttp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.081257 geventhttpclient-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/src/geventhttpclient/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/connectionpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/src/geventhttpclient/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/oncert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/server.key
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_http_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_network_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_no_module_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/ext/Python_compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/ext/_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/LICENSE-MIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/llhttp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/src/geventhttpclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/connectionpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/src/geventhttpclient/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/oncert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_http_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_network_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_no_module_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/top_level.txt
```

### Comparing `geventhttpclient-2.1.0/LICENSE.txt` & `geventhttpclient-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/PKG-INFO` & `geventhttpclient-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.1.0
+Version: 2.1.1
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: Based on llhttp, copyright Fedor Indutny, 2018.
         
         Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
         licensed under the same terms.
```

### Comparing `geventhttpclient-2.1.0/README.md` & `geventhttpclient-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/ext/_parser.c` & `geventhttpclient-2.1.1/ext/_parser.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/llhttp/LICENSE-MIT` & `geventhttpclient-2.1.1/llhttp/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/llhttp/include/llhttp.h` & `geventhttpclient-2.1.1/llhttp/include/llhttp.h`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/llhttp/src/api.c` & `geventhttpclient-2.1.1/llhttp/src/api.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/llhttp/src/http.c` & `geventhttpclient-2.1.1/llhttp/src/http.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/llhttp/src/llhttp.c` & `geventhttpclient-2.1.1/llhttp/src/llhttp.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/pyproject.toml` & `geventhttpclient-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "geventhttpclient"
-version = "2.1.0" # dont forget to update version __init__.py as well
+version = "2.1.1" # dont forget to update version __init__.py as well
 description = "HTTP client library for gevent"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = ["http", "gevent", "client"]
 authors = [{name = "Antonin Amand", email = "antonin.amand@gmail.com"}]
 classifiers = [
```

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/client.py` & `geventhttpclient-2.1.1/src/geventhttpclient/client.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/connectionpool.py` & `geventhttpclient-2.1.1/src/geventhttpclient/connectionpool.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/header.py` & `geventhttpclient-2.1.1/src/geventhttpclient/header.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/httplib.py` & `geventhttpclient-2.1.1/src/geventhttpclient/httplib.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/response.py` & `geventhttpclient-2.1.1/src/geventhttpclient/response.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/oncert.pem` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/oncert.pem`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/server.crt` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/server.crt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/server.key` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/server.key`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_client.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import gevent.server
 import pytest
 from gevent.ssl import SSLError
 
 from geventhttpclient import HTTPClient, __version__
 
 LISTENER = "127.0.0.1", 54323
-HTTPBIN_HOST = "httpbin.org"  # this might be exchanged with a self-hosted version
+HTTPBIN_HOST = "httpbingo.org"  # this might be exchanged with a self-hosted version
 
 
 @contextmanager
 def server(handler):
     server = gevent.server.StreamServer(LISTENER, handle=handler)
     server.start()
     try:
@@ -291,29 +291,42 @@
 
 FIREFOX_USER_AGENT = (
     "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:124.0) Gecko/20100101 Firefox/124.0"
 )
 FIREFOX_HEADERS = {"User-Agent": FIREFOX_USER_AGENT}
 
 
+def check_user_agent_header(ua_header, ua_header_ref):
+    """
+    unlike original httpbin, httpbingo.org sends back a list of header
+    strings instead of a simple string. So we need to be a bit flexible
+    with the answer.
+    """
+    if isinstance(ua_header, list):
+        assert len(ua_header) == 1
+        assert ua_header[0] == ua_header_ref
+        return
+    assert ua_header == ua_header_ref
+
+
 @pytest.mark.network
 def test_client_with_default_headers():
     httpbin = httpbin_client(headers=FIREFOX_HEADERS)
     response = httpbin.get("/headers")
     assert response.status_code == 200
     sent_headers = json.loads(response.read().decode())["headers"]
-    assert sent_headers["User-Agent"] == FIREFOX_USER_AGENT
+    check_user_agent_header(sent_headers["User-Agent"], FIREFOX_USER_AGENT)
 
 
 @pytest.mark.network
 def test_request_with_headers(httpbin):
     response = httpbin.get("/headers", headers=FIREFOX_HEADERS)
     assert response.status_code == 200
     sent_headers = json.loads(response.read().decode())["headers"]
-    assert sent_headers["User-Agent"] == FIREFOX_USER_AGENT
+    check_user_agent_header(sent_headers["User-Agent"], FIREFOX_USER_AGENT)
 
 
 @pytest.mark.network
 def test_response_context_manager(httpbin):
     r = None
     with httpbin.get("/") as response:
         assert response.status_code == 200
```

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_headers.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_httplib.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_httplib.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_keep_alive.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_network_failures.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_network_failures.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_no_module_ssl.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_no_module_ssl.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_parser.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_ssl.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_url.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_useragent.py` & `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_useragent.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/url.py` & `geventhttpclient-2.1.1/src/geventhttpclient/url.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient/useragent.py` & `geventhttpclient-2.1.1/src/geventhttpclient/useragent.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient.egg-info/PKG-INFO` & `geventhttpclient-2.1.1/src/geventhttpclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.1.0
+Version: 2.1.1
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: Based on llhttp, copyright Fedor Indutny, 2018.
         
         Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
         licensed under the same terms.
```

### Comparing `geventhttpclient-2.1.0/src/geventhttpclient.egg-info/SOURCES.txt` & `geventhttpclient-2.1.1/src/geventhttpclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

