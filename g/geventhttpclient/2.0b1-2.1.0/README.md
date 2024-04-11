# Comparing `tmp/geventhttpclient-2.0b1.tar.gz` & `tmp/geventhttpclient-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.0b1.tar", last modified: Fri Jul  1 18:12:03 2022, max compression
+gzip compressed data, was "geventhttpclient-2.1.0.tar", last modified: Thu Apr 11 05:46:06 2024, max compression
```

## Comparing `geventhttpclient-2.0b1.tar` & `geventhttpclient-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.329784 geventhttpclient-2.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-07-01 18:12:03.329784 geventhttpclient-2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/README.mdown
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.325785 geventhttpclient-2.0b1/ext/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/Python_compat.h
--rw-r--r--   0 runner    (1001) docker     (121)    12764 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/_parser.c
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/api.c
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/http.c
--rw-r--r--   0 runner    (1001) docker     (121)   444714 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/llhttp.c
--rw-r--r--   0 runner    (1001) docker     (121)    15786 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/ext/llhttp.h
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-01 18:12:03.329784 geventhttpclient-2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.325785 geventhttpclient-2.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.325785 geventhttpclient-2.0b1/src/geventhttpclient/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10813 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/connectionpool.py
--rw-r--r--   0 runner    (1001) docker     (121)     7846 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/httplib.py
--rw-r--r--   0 runner    (1001) docker     (121)     9045 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.329784 geventhttpclient-2.0b1/src/geventhttpclient/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/oncert.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/server.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/server.key
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_network_failures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_no_module_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7825 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     6946 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (121)     6984 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/url.py
--rw-r--r--   0 runner    (1001) docker     (121)    21663 2022-07-01 18:12:00.000000 geventhttpclient-2.0b1/src/geventhttpclient/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 18:12:03.325785 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-07-01 18:12:03.000000 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-01 18:12:03.000000 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 18:12:03.000000 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-01 18:12:03.000000 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-01 18:12:03.000000 geventhttpclient-2.0b1/src/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/ext/Python_compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/ext/_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/LICENSE-MIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-11 05:45:56.000000 geventhttpclient-2.1.0/llhttp/src/llhttp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.081257 geventhttpclient-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.085257 geventhttpclient-2.1.0/src/geventhttpclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/connectionpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/src/geventhttpclient/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/oncert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_http_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_network_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_no_module_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-11 05:45:55.000000 geventhttpclient-2.1.0/src/geventhttpclient/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:46:06.089257 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 05:46:06.000000 geventhttpclient-2.1.0/src/geventhttpclient.egg-info/top_level.txt
```

### Comparing `geventhttpclient-2.0b1/LICENSE.txt` & `geventhttpclient-2.1.0/llhttp/LICENSE-MIT`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-http_parser.c is based on src/http/ngx_http_parse.c from NGINX copyright
-Igor Sysoev.
+This software is licensed under the MIT License.
 
-Additional changes to http_parser.c are licensed under the same terms as NGINX and
-copyright Joyent, Inc. and other Node contributors. All rights reserved.
+Copyright Fedor Indutny, 2018.
 
-Python extension by Antonin Amand <antonin.amand@gmail.com> licensed under
-the same terms.
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to permit
+persons to whom the Software is furnished to do so, subject to the
+following conditions:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `geventhttpclient-2.0b1/README.mdown` & `geventhttpclient-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-# geventhttpclient
+[![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
+[![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
-[![Build Status](https://travis-ci.org/gwik/geventhttpclient.svg?branch=master)](https://travis-ci.org/gwik/geventhttpclient)
+# geventhttpclient
 
 A high performance, concurrent HTTP client library for python using 
 [gevent](http://gevent.org).
 
 `gevent.httplib` support was removed in [gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6
 ), **geventhttpclient** now provides that missing functionality.
 
@@ -16,18 +19,15 @@
 designed for efficiently pulling from REST APIs and streaming APIs
 like Twitter's.
 
 Safe SSL support is provided by default. **geventhttpclient** depends on
 the certifi CA Bundle. This is the same CA Bundle which ships with the
 Requests codebase, and is derived from Mozilla Firefox's canonical set.
 
-As of version 1.5, only Python 3.6+ is fully supported (with prebuilt wheels), 
-but Python 2.7 and 3.5 *should* work too.
-
-Use of SSL/TLS with python 2.7.9 is not recommended and may be broken.
+As of version 2.1, only Python 3.9+ is fully supported (with prebuilt wheels).
 
 A simple example:
 
 ```python
 #!/usr/bin/python
 
 from geventhttpclient import HTTPClient
@@ -109,18 +109,18 @@
 def print_friend_username(http, friend_id):
     friend_url = URL('/' + str(friend_id))
     friend_url['access_token'] = TOKEN
     # the greenlet will block until a connection is available
     response = http.get(friend_url.request_uri)
     assert response.status_code == 200
     friend = json.load(response)
-    if friend.has_key('username'):
-        print '%s: %s' % (friend['username'], friend['name'])
+    if 'username' in friend:
+        print('%s: %s' % (friend['username'], friend['name']))
     else:
-        print '%s has no username.' % friend['name']
+        print('%s has no username.' % friend['name'])
 
 # allow to run 20 greenlet at a time, this is more than concurrency
 # of the http client but isn't a problem since the client has its own
 # connection pool.
 pool = gevent.pool.Pool(20)
 for item in data:
     friend_id = item['id']
@@ -155,13 +155,19 @@
     while data:
         f.write(data)
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
-The benchmark does 1000 get requests against a local nginx server with
-a concurrency of 10. See *benchmarks* folder.
-
-- httplib2 with geventhttpclient monkey patch (*benchmarks/httplib2_patched.py*): **~2500 req/s**
-- geventhttpclient.HTTPClient (*benchmarks/httpclient.py*): **~4000 req/s**
+The benchmark does 10000 get requests against a local nginx server in the default 
+configuration with a concurrency of 10. See `benchmarks` folder. The requests per
+second for a couple of popular clients is given in the table below.
+
+| HTTP Client          | RPS    |
+|----------------------|--------|
+| GeventHTTPClient     | 7181.2 |
+| Urllib3              | 2847.5 |
+| Httpx                | 1682.9 |
+| Requests             | 1186.4 |
 
+*Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
```

### Comparing `geventhttpclient-2.0b1/ext/_parser.c` & `geventhttpclient-2.1.0/ext/_parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include "Python_compat.h"
-#include "llhttp.h"
+#include <llhttp.h>
 #include <stdio.h>
 
 static PyObject * PyExc_HTTPParseError;
 
 enum py_parser_should_keep_alive {
     KA_INCOMPLETE,
     KA_FALSE,
```

### Comparing `geventhttpclient-2.0b1/ext/api.c` & `geventhttpclient-2.1.0/llhttp/src/api.c`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,22 @@
   if (enabled) {
     parser->lenient_flags |= LENIENT_KEEP_ALIVE;
   } else {
     parser->lenient_flags &= ~LENIENT_KEEP_ALIVE;
   }
 }
 
+void llhttp_set_lenient_transfer_encoding(llhttp_t* parser, int enabled) {
+  if (enabled) {
+    parser->lenient_flags |= LENIENT_TRANSFER_ENCODING;
+  } else {
+    parser->lenient_flags &= ~LENIENT_TRANSFER_ENCODING;
+  }
+}
+
 /* Callbacks */
 
 
 int llhttp__on_message_begin(llhttp_t* s, const char* p, const char* endp) {
   int err;
   CALLBACK_MAYBE(s, on_message_begin);
   return err;
```

### Comparing `geventhttpclient-2.0b1/ext/http.c` & `geventhttpclient-2.1.0/llhttp/src/http.c`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
   if (parser->flags & F_SKIPBODY) {
     return 0;
   } else if (parser->flags & F_CHUNKED) {
     /* chunked encoding - ignore Content-Length header, prepare for a chunk */
     return 2;
   } else if (parser->flags & F_TRANSFER_ENCODING) {
     if (parser->type == HTTP_REQUEST &&
-        (parser->lenient_flags & LENIENT_CHUNKED_LENGTH) == 0) {
+        (parser->lenient_flags & LENIENT_CHUNKED_LENGTH) == 0 &&
+        (parser->lenient_flags & LENIENT_TRANSFER_ENCODING) == 0) {
       /* RFC 7230 3.3.3 */
 
       /* If a Transfer-Encoding header field
        * is present in a request and the chunked transfer coding is not
        * the final encoding, the message body length cannot be determined
        * reliably; the server MUST respond with the 400 (Bad Request)
        * status code and then close the connection.
```

### Comparing `geventhttpclient-2.0b1/ext/llhttp.c` & `geventhttpclient-2.1.0/llhttp/src/llhttp.c`

 * *Files 2% similar despite different names*

```diff
@@ -355,29 +355,32 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value,
   s_n_llhttp__internal__n_header_value_discard_lws,
   s_n_llhttp__internal__n_header_value_discard_ws_almost_done,
   s_n_llhttp__internal__n_header_value_lws,
   s_n_llhttp__internal__n_header_value_almost_done,
   s_n_llhttp__internal__n_header_value_lenient,
+  s_n_llhttp__internal__n_error_25,
   s_n_llhttp__internal__n_header_value_otherwise,
   s_n_llhttp__internal__n_header_value_connection_token,
   s_n_llhttp__internal__n_header_value_connection_ws,
   s_n_llhttp__internal__n_header_value_connection_1,
   s_n_llhttp__internal__n_header_value_connection_2,
   s_n_llhttp__internal__n_header_value_connection_3,
   s_n_llhttp__internal__n_header_value_connection,
-  s_n_llhttp__internal__n_error_25,
-  s_n_llhttp__internal__n_error_26,
+  s_n_llhttp__internal__n_error_27,
+  s_n_llhttp__internal__n_error_28,
   s_n_llhttp__internal__n_header_value_content_length_ws,
   s_n_llhttp__internal__n_header_value_content_length,
-  s_n_llhttp__internal__n_header_value_te_chunked_last,
+  s_n_llhttp__internal__n_error_30,
+  s_n_llhttp__internal__n_error_29,
   s_n_llhttp__internal__n_header_value_te_token_ows,
   s_n_llhttp__internal__n_header_value,
   s_n_llhttp__internal__n_header_value_te_token,
+  s_n_llhttp__internal__n_header_value_te_chunked_last,
   s_n_llhttp__internal__n_header_value_te_chunked,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1,
   s_n_llhttp__internal__n_header_value_discard_ws,
   s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete,
   s_n_llhttp__internal__n_header_field_general_otherwise,
   s_n_llhttp__internal__n_header_field_general,
   s_n_llhttp__internal__n_header_field_colon,
@@ -806,39 +809,39 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 8;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_2(
+int llhttp__internal__c_update_header_state_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 6;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_4(
+int llhttp__internal__c_update_header_state_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 0;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_5(
+int llhttp__internal__c_update_header_state_6(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 5;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_6(
+int llhttp__internal__c_update_header_state_7(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 7;
   return 0;
 }
 
@@ -879,14 +882,28 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 32;
   return 0;
 }
 
+int llhttp__internal__c_test_flags_3(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->flags & 8) == 8;
+}
+
+int llhttp__internal__c_test_lenient_flags_7(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 8) == 8;
+}
+
 int llhttp__internal__c_or_flags_16(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 512;
   return 0;
 }
@@ -895,23 +912,23 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags &= -9;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_7(
+int llhttp__internal__c_update_header_state_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 8;
   return 0;
 }
 
-int llhttp__internal__c_or_flags_17(
+int llhttp__internal__c_or_flags_18(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 16;
   return 0;
 }
 
@@ -936,14 +953,35 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->http_minor = match;
   return 0;
 }
 
+int llhttp__internal__c_test_lenient_flags_9(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 16) == 16;
+}
+
+int llhttp__internal__c_load_http_major(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->http_major;
+}
+
+int llhttp__internal__c_load_http_minor(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->http_minor;
+}
+
 int llhttp__internal__c_update_status_code(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->status_code = 0;
   return 0;
 }
@@ -1615,19 +1653,19 @@
     s_n_llhttp__internal__n_header_value_discard_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_lws;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_load_header_state;
         }
       }
       /* UNREACHABLE */;
       abort();
@@ -1639,34 +1677,34 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_21;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lws:
     s_n_llhttp__internal__n_header_value_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lws;
       }
       switch (*p) {
         case 9: {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         case ' ': {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_almost_done:
     s_n_llhttp__internal__n_header_value_almost_done: {
@@ -1675,54 +1713,61 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_22;
+          goto s_n_llhttp__internal__n_error_24;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lenient:
     s_n_llhttp__internal__n_header_value_lenient: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lenient;
       }
       switch (*p) {
         case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3;
         }
         case 13: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4;
         }
         default: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lenient;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_25:
+    s_n_llhttp__internal__n_error_25: {
+      state->error = 0xa;
+      state->reason = "Invalid header value char";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_header_value_otherwise:
     s_n_llhttp__internal__n_header_value_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_otherwise;
       }
       switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
-        }
         case 13: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_token:
     s_n_llhttp__internal__n_header_value_connection_token: {
@@ -1777,18 +1822,18 @@
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_connection_ws;
         }
         case ',': {
           p++;
-          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_5;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_1:
     s_n_llhttp__internal__n_header_value_connection_1: {
@@ -1798,15 +1843,15 @@
         return s_n_llhttp__internal__n_header_value_connection_1;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob3, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_2;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_1;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1822,15 +1867,15 @@
         return s_n_llhttp__internal__n_header_value_connection_2;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob4, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_2;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1846,15 +1891,15 @@
         return s_n_llhttp__internal__n_header_value_connection_3;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob5, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_3;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -1891,26 +1936,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_25:
-    s_n_llhttp__internal__n_error_25: {
+    case s_n_llhttp__internal__n_error_27:
+    s_n_llhttp__internal__n_error_27: {
       state->error = 0xb;
       state->reason = "Content-Length overflow";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_26:
-    s_n_llhttp__internal__n_error_26: {
+    case s_n_llhttp__internal__n_error_28:
+    s_n_llhttp__internal__n_error_28: {
       state->error = 0xb;
       state->reason = "Invalid character in Content-Length";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -1928,15 +1973,15 @@
           goto s_n_llhttp__internal__n_invoke_or_flags_15;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
         default: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_6;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_content_length:
     s_n_llhttp__internal__n_header_value_content_length: {
@@ -1997,34 +2042,31 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_header_value_te_chunked_last:
-    s_n_llhttp__internal__n_header_value_te_chunked_last: {
-      if (p == endp) {
-        return s_n_llhttp__internal__n_header_value_te_chunked_last;
-      }
-      switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
-        }
-        case 13: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
-        }
-        case ' ': {
-          p++;
-          goto s_n_llhttp__internal__n_header_value_te_chunked_last;
-        }
-        default: {
-          goto s_n_llhttp__internal__n_header_value_te_chunked;
-        }
-      }
+    case s_n_llhttp__internal__n_error_30:
+    s_n_llhttp__internal__n_error_30: {
+      state->error = 0xf;
+      state->reason = "Invalid `Transfer-Encoding` header value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_29:
+    s_n_llhttp__internal__n_error_29: {
+      state->error = 0xf;
+      state->reason = "Invalid `Transfer-Encoding` header value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_token_ows:
     s_n_llhttp__internal__n_header_value_te_token_ows: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_te_token_ows;
@@ -2133,16 +2175,42 @@
           goto s_n_llhttp__internal__n_header_value_te_token;
         }
         case 2: {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_token_ows;
         }
         default: {
+          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_header_value_te_chunked_last:
+    s_n_llhttp__internal__n_header_value_te_chunked_last: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_header_value_te_chunked_last;
+      }
+      switch (*p) {
+        case 10: {
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        }
+        case 13: {
           goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_header_value_te_chunked_last;
+        }
+        case ',': {
+          goto s_n_llhttp__internal__n_invoke_load_type_1;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_header_value_te_token;
+        }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_chunked:
     s_n_llhttp__internal__n_header_value_te_chunked: {
       llparse_match_t match_seq;
@@ -2186,15 +2254,15 @@
       switch (*p) {
         case 9: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_lws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
         }
         case ' ': {
           p++;
@@ -2222,15 +2290,15 @@
         return s_n_llhttp__internal__n_header_field_general_otherwise;
       }
       switch (*p) {
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_2;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_27;
+          goto s_n_llhttp__internal__n_error_31;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general:
     s_n_llhttp__internal__n_header_field_general: {
@@ -2312,15 +2380,15 @@
         case ' ': {
           goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
         }
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_3:
     s_n_llhttp__internal__n_header_field_3: {
@@ -2337,15 +2405,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_4:
     s_n_llhttp__internal__n_header_field_4: {
@@ -2362,15 +2430,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_2:
     s_n_llhttp__internal__n_header_field_2: {
@@ -2383,15 +2451,15 @@
           goto s_n_llhttp__internal__n_header_field_3;
         }
         case 't': {
           p++;
           goto s_n_llhttp__internal__n_header_field_4;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_1:
     s_n_llhttp__internal__n_header_field_1: {
@@ -2407,15 +2475,15 @@
           p++;
           goto s_n_llhttp__internal__n_header_field_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_5:
     s_n_llhttp__internal__n_header_field_5: {
@@ -2432,15 +2500,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_5;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_6:
     s_n_llhttp__internal__n_header_field_6: {
@@ -2457,15 +2525,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_7:
     s_n_llhttp__internal__n_header_field_7: {
@@ -2482,15 +2550,15 @@
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_7;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field:
     s_n_llhttp__internal__n_header_field: {
@@ -2511,15 +2579,15 @@
           goto s_n_llhttp__internal__n_header_field_6;
         }
         case 'u': {
           p++;
           goto s_n_llhttp__internal__n_header_field_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_field:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_field: {
@@ -2602,15 +2670,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_url_to_http_09;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_28;
+          goto s_n_llhttp__internal__n_error_32;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_skip_lf_to_http09:
     s_n_llhttp__internal__n_url_skip_lf_to_http09: {
@@ -2627,15 +2695,15 @@
           goto s_n_llhttp__internal__n_error_1;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_url_skip_lf_to_http09_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_28;
+          goto s_n_llhttp__internal__n_error_32;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_pri_upgrade:
     s_n_llhttp__internal__n_req_pri_upgrade: {
@@ -2645,21 +2713,21 @@
         return s_n_llhttp__internal__n_req_pri_upgrade;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob15, 10);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_error_31;
+          goto s_n_llhttp__internal__n_error_37;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_pri_upgrade;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_32;
+          goto s_n_llhttp__internal__n_error_38;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete_1:
     s_n_llhttp__internal__n_req_http_complete_1: {
@@ -2668,15 +2736,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_field_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_30;
+          goto s_n_llhttp__internal__n_error_36;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete:
     s_n_llhttp__internal__n_req_http_complete: {
@@ -2689,15 +2757,15 @@
           goto s_n_llhttp__internal__n_header_field_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_req_http_complete_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_30;
+          goto s_n_llhttp__internal__n_error_36;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_minor:
     s_n_llhttp__internal__n_req_http_minor: {
@@ -2752,15 +2820,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_33;
+          goto s_n_llhttp__internal__n_error_41;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_dot:
     s_n_llhttp__internal__n_req_http_dot: {
@@ -2769,15 +2837,15 @@
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_req_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_34;
+          goto s_n_llhttp__internal__n_error_42;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_major:
     s_n_llhttp__internal__n_req_http_major: {
@@ -2832,15 +2900,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_35;
+          goto s_n_llhttp__internal__n_error_43;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_1:
     s_n_llhttp__internal__n_req_http_start_1: {
@@ -2856,15 +2924,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_38;
+          goto s_n_llhttp__internal__n_error_46;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_2:
     s_n_llhttp__internal__n_req_http_start_2: {
@@ -2880,15 +2948,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_38;
+          goto s_n_llhttp__internal__n_error_46;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_3:
     s_n_llhttp__internal__n_req_http_start_3: {
@@ -2904,15 +2972,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_38;
+          goto s_n_llhttp__internal__n_error_46;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start:
     s_n_llhttp__internal__n_req_http_start: {
@@ -2933,15 +3001,15 @@
           goto s_n_llhttp__internal__n_req_http_start_2;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_req_http_start_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_38;
+          goto s_n_llhttp__internal__n_error_46;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_to_http:
     s_n_llhttp__internal__n_url_to_http: {
@@ -3024,15 +3092,15 @@
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_8;
         }
         case 5: {
           p++;
           goto s_n_llhttp__internal__n_url_fragment;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_47;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_query_3:
     s_n_llhttp__internal__n_span_end_stub_query_3: {
@@ -3085,15 +3153,15 @@
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 6: {
           goto s_n_llhttp__internal__n_span_end_stub_query_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_40;
+          goto s_n_llhttp__internal__n_error_48;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_query_or_fragment:
     s_n_llhttp__internal__n_url_query_or_fragment: {
@@ -3123,15 +3191,15 @@
           goto s_n_llhttp__internal__n_url_fragment;
         }
         case '?': {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_41;
+          goto s_n_llhttp__internal__n_error_49;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_path:
     s_n_llhttp__internal__n_url_path: {
@@ -3248,18 +3316,18 @@
         }
         case 7: {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 8: {
           p++;
-          goto s_n_llhttp__internal__n_error_42;
+          goto s_n_llhttp__internal__n_error_50;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_43;
+          goto s_n_llhttp__internal__n_error_51;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_server:
     s_n_llhttp__internal__n_url_server: {
@@ -3310,15 +3378,15 @@
           goto s_n_llhttp__internal__n_url_query;
         }
         case 8: {
           p++;
           goto s_n_llhttp__internal__n_url_server_with_at;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_44;
+          goto s_n_llhttp__internal__n_error_52;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim_1:
     s_n_llhttp__internal__n_url_schema_delim_1: {
@@ -3327,15 +3395,15 @@
       }
       switch (*p) {
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_server;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_54;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim:
     s_n_llhttp__internal__n_url_schema_delim: {
@@ -3345,34 +3413,34 @@
       switch (*p) {
         case 9: {
           p++;
           goto s_n_llhttp__internal__n_error_1;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_53;
         }
         case 12: {
           p++;
           goto s_n_llhttp__internal__n_error_1;
         }
         case 13: {
           p++;
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_53;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_53;
         }
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_schema_delim_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_54;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_schema:
     s_n_llhttp__internal__n_span_end_stub_schema: {
@@ -3410,25 +3478,25 @@
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
           goto s_n_llhttp__internal__n_error_1;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_53;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_end_stub_schema;
         }
         case 4: {
           p++;
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_47;
+          goto s_n_llhttp__internal__n_error_55;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_start:
     s_n_llhttp__internal__n_url_start: {
@@ -3456,24 +3524,24 @@
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
           goto s_n_llhttp__internal__n_error_1;
         }
         case 2: {
           p++;
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_53;
         }
         case 3: {
           goto s_n_llhttp__internal__n_span_start_stub_path_2;
         }
         case 4: {
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_48;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_url_1:
     s_n_llhttp__internal__n_span_start_llhttp__on_url_1: {
@@ -3563,15 +3631,15 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_req_spaces_before_url;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_49;
+          goto s_n_llhttp__internal__n_error_57;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_2:
     s_n_llhttp__internal__n_start_req_2: {
@@ -3581,15 +3649,15 @@
       switch (*p) {
         case 'L': {
           p++;
           match = 19;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_3:
     s_n_llhttp__internal__n_start_req_3: {
@@ -3606,15 +3674,15 @@
           match = 36;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_1:
     s_n_llhttp__internal__n_start_req_1: {
@@ -3627,15 +3695,15 @@
           goto s_n_llhttp__internal__n_start_req_2;
         }
         case 'N': {
           p++;
           goto s_n_llhttp__internal__n_start_req_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_4:
     s_n_llhttp__internal__n_start_req_4: {
@@ -3652,15 +3720,15 @@
           match = 16;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_6:
     s_n_llhttp__internal__n_start_req_6: {
@@ -3677,15 +3745,15 @@
           match = 22;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_8:
     s_n_llhttp__internal__n_start_req_8: {
@@ -3702,15 +3770,15 @@
           match = 5;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_8;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_9:
     s_n_llhttp__internal__n_start_req_9: {
@@ -3720,15 +3788,15 @@
       switch (*p) {
         case 'Y': {
           p++;
           match = 8;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_7:
     s_n_llhttp__internal__n_start_req_7: {
@@ -3741,15 +3809,15 @@
           goto s_n_llhttp__internal__n_start_req_8;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_9;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_5:
     s_n_llhttp__internal__n_start_req_5: {
@@ -3762,15 +3830,15 @@
           goto s_n_llhttp__internal__n_start_req_6;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_12:
     s_n_llhttp__internal__n_start_req_12: {
@@ -3787,15 +3855,15 @@
           match = 0;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_12;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_13:
     s_n_llhttp__internal__n_start_req_13: {
@@ -3812,15 +3880,15 @@
           match = 35;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_13;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_11:
     s_n_llhttp__internal__n_start_req_11: {
@@ -3833,15 +3901,15 @@
           goto s_n_llhttp__internal__n_start_req_12;
         }
         case 'S': {
           p++;
           goto s_n_llhttp__internal__n_start_req_13;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_10:
     s_n_llhttp__internal__n_start_req_10: {
@@ -3850,15 +3918,15 @@
       }
       switch (*p) {
         case 'E': {
           p++;
           goto s_n_llhttp__internal__n_start_req_11;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_14:
     s_n_llhttp__internal__n_start_req_14: {
@@ -3875,15 +3943,15 @@
           match = 45;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_14;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_17:
     s_n_llhttp__internal__n_start_req_17: {
@@ -3900,15 +3968,15 @@
           match = 41;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_17;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_16:
     s_n_llhttp__internal__n_start_req_16: {
@@ -3942,15 +4010,15 @@
           p++;
           goto s_n_llhttp__internal__n_start_req_16;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_15;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_18:
     s_n_llhttp__internal__n_start_req_18: {
@@ -3967,15 +4035,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_18;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_20:
     s_n_llhttp__internal__n_start_req_20: {
@@ -3992,15 +4060,15 @@
           match = 31;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_20;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_21:
     s_n_llhttp__internal__n_start_req_21: {
@@ -4017,15 +4085,15 @@
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_21;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_19:
     s_n_llhttp__internal__n_start_req_19: {
@@ -4038,15 +4106,15 @@
           goto s_n_llhttp__internal__n_start_req_20;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_21;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_23:
     s_n_llhttp__internal__n_start_req_23: {
@@ -4063,15 +4131,15 @@
           match = 24;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_23;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_24:
     s_n_llhttp__internal__n_start_req_24: {
@@ -4088,15 +4156,15 @@
           match = 23;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_24;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_26:
     s_n_llhttp__internal__n_start_req_26: {
@@ -4113,15 +4181,15 @@
           match = 21;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_26;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_28:
     s_n_llhttp__internal__n_start_req_28: {
@@ -4138,15 +4206,15 @@
           match = 30;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_28;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_29:
     s_n_llhttp__internal__n_start_req_29: {
@@ -4156,15 +4224,15 @@
       switch (*p) {
         case 'L': {
           p++;
           match = 10;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_27:
     s_n_llhttp__internal__n_start_req_27: {
@@ -4177,15 +4245,15 @@
           goto s_n_llhttp__internal__n_start_req_28;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_29;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_25:
     s_n_llhttp__internal__n_start_req_25: {
@@ -4198,15 +4266,15 @@
           goto s_n_llhttp__internal__n_start_req_26;
         }
         case 'C': {
           p++;
           goto s_n_llhttp__internal__n_start_req_27;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_30:
     s_n_llhttp__internal__n_start_req_30: {
@@ -4223,15 +4291,15 @@
           match = 11;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_30;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_22:
     s_n_llhttp__internal__n_start_req_22: {
@@ -4252,15 +4320,15 @@
           goto s_n_llhttp__internal__n_start_req_25;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_30;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_31:
     s_n_llhttp__internal__n_start_req_31: {
@@ -4277,15 +4345,15 @@
           match = 25;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_31;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_32:
     s_n_llhttp__internal__n_start_req_32: {
@@ -4302,15 +4370,15 @@
           match = 6;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_32;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_35:
     s_n_llhttp__internal__n_start_req_35: {
@@ -4327,15 +4395,15 @@
           match = 28;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_35;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_36:
     s_n_llhttp__internal__n_start_req_36: {
@@ -4352,15 +4420,15 @@
           match = 39;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_36;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_34:
     s_n_llhttp__internal__n_start_req_34: {
@@ -4373,15 +4441,15 @@
           goto s_n_llhttp__internal__n_start_req_35;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_36;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_37:
     s_n_llhttp__internal__n_start_req_37: {
@@ -4398,15 +4466,15 @@
           match = 38;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_37;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_38:
     s_n_llhttp__internal__n_start_req_38: {
@@ -4423,15 +4491,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_38;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_42:
     s_n_llhttp__internal__n_start_req_42: {
@@ -4448,15 +4516,15 @@
           match = 12;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_42;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_43:
     s_n_llhttp__internal__n_start_req_43: {
@@ -4473,15 +4541,15 @@
           match = 13;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_43;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_41:
     s_n_llhttp__internal__n_start_req_41: {
@@ -4494,15 +4562,15 @@
           goto s_n_llhttp__internal__n_start_req_42;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_43;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_40:
     s_n_llhttp__internal__n_start_req_40: {
@@ -4511,15 +4579,15 @@
       }
       switch (*p) {
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_41;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_39:
     s_n_llhttp__internal__n_start_req_39: {
@@ -4533,15 +4601,15 @@
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_40;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_45:
     s_n_llhttp__internal__n_start_req_45: {
@@ -4558,15 +4626,15 @@
           match = 29;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_45;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_44:
     s_n_llhttp__internal__n_start_req_44: {
@@ -4580,15 +4648,15 @@
         }
         case 'T': {
           p++;
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_33:
     s_n_llhttp__internal__n_start_req_33: {
@@ -4613,15 +4681,15 @@
           goto s_n_llhttp__internal__n_start_req_39;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_44;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_48:
     s_n_llhttp__internal__n_start_req_48: {
@@ -4638,15 +4706,15 @@
           match = 17;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_48;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_49:
     s_n_llhttp__internal__n_start_req_49: {
@@ -4663,15 +4731,15 @@
           match = 44;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_49;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_50:
     s_n_llhttp__internal__n_start_req_50: {
@@ -4688,15 +4756,15 @@
           match = 43;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_50;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_51:
     s_n_llhttp__internal__n_start_req_51: {
@@ -4713,15 +4781,15 @@
           match = 20;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_51;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_47:
     s_n_llhttp__internal__n_start_req_47: {
@@ -4742,15 +4810,15 @@
           goto s_n_llhttp__internal__n_start_req_50;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_51;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_46:
     s_n_llhttp__internal__n_start_req_46: {
@@ -4759,15 +4827,15 @@
       }
       switch (*p) {
         case 'E': {
           p++;
           goto s_n_llhttp__internal__n_start_req_47;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_54:
     s_n_llhttp__internal__n_start_req_54: {
@@ -4784,15 +4852,15 @@
           match = 14;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_54;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_56:
     s_n_llhttp__internal__n_start_req_56: {
@@ -4802,15 +4870,15 @@
       switch (*p) {
         case 'P': {
           p++;
           match = 37;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_57:
     s_n_llhttp__internal__n_start_req_57: {
@@ -4827,15 +4895,15 @@
           match = 42;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_57;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_55:
     s_n_llhttp__internal__n_start_req_55: {
@@ -4848,15 +4916,15 @@
           goto s_n_llhttp__internal__n_start_req_56;
         }
         case '_': {
           p++;
           goto s_n_llhttp__internal__n_start_req_57;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_53:
     s_n_llhttp__internal__n_start_req_53: {
@@ -4869,15 +4937,15 @@
           goto s_n_llhttp__internal__n_start_req_54;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_start_req_55;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_58:
     s_n_llhttp__internal__n_start_req_58: {
@@ -4894,15 +4962,15 @@
           match = 33;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_58;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_59:
     s_n_llhttp__internal__n_start_req_59: {
@@ -4919,15 +4987,15 @@
           match = 26;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_59;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_52:
     s_n_llhttp__internal__n_start_req_52: {
@@ -4944,15 +5012,15 @@
           goto s_n_llhttp__internal__n_start_req_58;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_59;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_61:
     s_n_llhttp__internal__n_start_req_61: {
@@ -4969,15 +5037,15 @@
           match = 40;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_61;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_62:
     s_n_llhttp__internal__n_start_req_62: {
@@ -4994,15 +5062,15 @@
           match = 7;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_62;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_60:
     s_n_llhttp__internal__n_start_req_60: {
@@ -5015,15 +5083,15 @@
           goto s_n_llhttp__internal__n_start_req_61;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_start_req_62;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_65:
     s_n_llhttp__internal__n_start_req_65: {
@@ -5040,15 +5108,15 @@
           match = 18;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_65;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_67:
     s_n_llhttp__internal__n_start_req_67: {
@@ -5065,15 +5133,15 @@
           match = 32;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_67;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_68:
     s_n_llhttp__internal__n_start_req_68: {
@@ -5090,15 +5158,15 @@
           match = 15;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_68;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_66:
     s_n_llhttp__internal__n_start_req_66: {
@@ -5111,15 +5179,15 @@
           goto s_n_llhttp__internal__n_start_req_67;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_68;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_69:
     s_n_llhttp__internal__n_start_req_69: {
@@ -5136,15 +5204,15 @@
           match = 27;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_69;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_64:
     s_n_llhttp__internal__n_start_req_64: {
@@ -5161,15 +5229,15 @@
           goto s_n_llhttp__internal__n_start_req_66;
         }
         case 'S': {
           p++;
           goto s_n_llhttp__internal__n_start_req_69;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_63:
     s_n_llhttp__internal__n_start_req_63: {
@@ -5178,15 +5246,15 @@
       }
       switch (*p) {
         case 'N': {
           p++;
           goto s_n_llhttp__internal__n_start_req_64;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req:
     s_n_llhttp__internal__n_start_req: {
@@ -5255,15 +5323,15 @@
           goto s_n_llhttp__internal__n_start_req_60;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_63;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_58;
+          goto s_n_llhttp__internal__n_error_70;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_status_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_status_complete: {
@@ -5281,15 +5349,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_invoke_llhttp__on_status_complete;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_status:
     s_n_llhttp__internal__n_res_status: {
@@ -5356,15 +5424,15 @@
           goto s_n_llhttp__internal__n_res_status_start;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_res_status_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_62;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_status_code:
     s_n_llhttp__internal__n_res_status_code: {
@@ -5436,15 +5504,15 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_invoke_update_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_53;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_minor:
     s_n_llhttp__internal__n_res_http_minor: {
@@ -5499,15 +5567,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_54;
+          goto s_n_llhttp__internal__n_error_66;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_dot:
     s_n_llhttp__internal__n_res_http_dot: {
@@ -5516,15 +5584,15 @@
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_res_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_55;
+          goto s_n_llhttp__internal__n_error_67;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_major:
     s_n_llhttp__internal__n_res_http_major: {
@@ -5579,15 +5647,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_56;
+          goto s_n_llhttp__internal__n_error_68;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_res:
     s_n_llhttp__internal__n_start_res: {
@@ -5603,15 +5671,15 @@
           p++;
           goto s_n_llhttp__internal__n_res_http_major;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_res;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_59;
+          goto s_n_llhttp__internal__n_error_71;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_2:
     s_n_llhttp__internal__n_req_or_res_method_2: {
@@ -5628,15 +5696,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_57;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_3:
     s_n_llhttp__internal__n_req_or_res_method_3: {
@@ -5652,15 +5720,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_update_type_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_57;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_1:
     s_n_llhttp__internal__n_req_or_res_method_1: {
@@ -5673,15 +5741,15 @@
           goto s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_57;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method:
     s_n_llhttp__internal__n_req_or_res_method: {
@@ -5690,15 +5758,15 @@
       }
       switch (*p) {
         case 'H': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_57;
+          goto s_n_llhttp__internal__n_error_69;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_or_res:
     s_n_llhttp__internal__n_start_req_or_res: {
@@ -5759,15 +5827,15 @@
     state->reason = "Invalid characters in url (strict mode)";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_45: {
+  s_n_llhttp__internal__n_error_53: {
     state->error = 0x7;
     state->reason = "Invalid characters in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6236,15 +6304,34 @@
         goto s_n_llhttp__internal__n_header_field_colon_discard_ws;
       default:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_20: {
+  s_n_llhttp__internal__n_error_21: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_ws;
+      default:
+        goto s_n_llhttp__internal__n_error_21;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_22: {
     state->error = 0xb;
     state->reason = "Empty Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6321,71 +6408,118 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 2:
-        goto s_n_llhttp__internal__n_error_20;
+        goto s_n_llhttp__internal__n_error_22;
       default:
         goto s_n_llhttp__internal__n_invoke_load_header_state_1;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_21: {
+  s_n_llhttp__internal__n_error_20: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_20;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_23: {
     state->error = 0x2;
     state->reason = "Expected LF after CR";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_23;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_header_state_1: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+    switch (llhttp__internal__c_load_header_state(state, p, endp)) {
+      case 8:
+        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_2: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_7: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_8: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_9: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_10: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+  s_n_llhttp__internal__n_invoke_load_header_state_4: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_7;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_8;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_9;
@@ -6393,15 +6527,15 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_10;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_22: {
+  s_n_llhttp__internal__n_error_24: {
     state->error = 0x3;
     state->reason = "Missing expected LF after header value";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6411,41 +6545,41 @@
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) p;
+      state->error_pos = (const char*) (p + 1);
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_almost_done;
       return s_error;
     }
+    p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) (p + 1);
+      state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_almost_done;
       return s_error;
     }
-    p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
@@ -6455,74 +6589,82 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_23: {
-    state->error = 0xa;
-    state->reason = "Invalid header value char";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_25;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_25;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
     switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_lenient;
       default:
-        goto s_n_llhttp__internal__n_error_23;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+  s_n_llhttp__internal__n_invoke_update_header_state_4: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_11: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_12: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_13: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_14: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_4: {
+  s_n_llhttp__internal__n_invoke_load_header_state_5: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_11;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_12;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_13;
@@ -6530,167 +6672,261 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_14;
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_4: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_5: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_token;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_2: {
-    switch (llhttp__internal__c_update_header_state_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+    switch (llhttp__internal__c_update_header_state_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_5: {
-    switch (llhttp__internal__c_update_header_state_5(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_6: {
+    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_6: {
-    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_7: {
+    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_25;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_27;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_25;
+    goto s_n_llhttp__internal__n_error_27;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length_1: {
     switch (llhttp__internal__c_mul_add_content_length_1(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
       default:
         goto s_n_llhttp__internal__n_header_value_content_length;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_15: {
     switch (llhttp__internal__c_or_flags_15(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_6: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_26;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_28;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_26;
+    goto s_n_llhttp__internal__n_error_28;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_24: {
+  s_n_llhttp__internal__n_error_26: {
     state->error = 0x4;
     state->reason = "Duplicate Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_2: {
     switch (llhttp__internal__c_test_flags_2(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_header_value_content_length;
       default:
-        goto s_n_llhttp__internal__n_error_24;
+        goto s_n_llhttp__internal__n_error_26;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_7: {
-    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_30;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_30;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_8: {
+    switch (llhttp__internal__c_update_header_state_8(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_8: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_29;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_29;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
+    switch (llhttp__internal__c_test_lenient_flags_7(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7;
+      default:
+        goto s_n_llhttp__internal__n_header_value_te_chunked;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_type_1: {
+    switch (llhttp__internal__c_load_type(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
+      default:
+        goto s_n_llhttp__internal__n_header_value_te_chunked;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_9: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_and_flags: {
     switch (llhttp__internal__c_and_flags(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_invoke_or_flags_17: {
+    switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_invoke_and_flags;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_8: {
+    switch (llhttp__internal__c_test_lenient_flags_7(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_type_2: {
+    switch (llhttp__internal__c_load_type(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_8;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_or_flags_16: {
     switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_and_flags;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_or_flags_17: {
-    switch (llhttp__internal__c_or_flags_17(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_flags_3: {
+    switch (llhttp__internal__c_test_flags_3(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_type_2;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_16;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_or_flags_18: {
+    switch (llhttp__internal__c_or_flags_18(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_9;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state_2: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_connection;
       case 2:
         goto s_n_llhttp__internal__n_invoke_test_flags_2;
       case 3:
-        goto s_n_llhttp__internal__n_invoke_or_flags_16;
+        goto s_n_llhttp__internal__n_invoke_test_flags_3;
       case 4:
-        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+        goto s_n_llhttp__internal__n_invoke_or_flags_18;
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1: {
@@ -6725,41 +6961,41 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_27: {
+  s_n_llhttp__internal__n_error_31: {
     state->error = 0xa;
     state->reason = "Invalid header token";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_9: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_10: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_header_state: {
     switch (llhttp__internal__c_store_header_state(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_header_field_colon;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_10: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_11: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete: {
@@ -6799,15 +7035,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_28: {
+  s_n_llhttp__internal__n_error_32: {
     state->error = 0x7;
     state->reason = "Expected CRLF";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6825,33 +7061,33 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_lf_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_lf_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_31: {
+  s_n_llhttp__internal__n_error_37: {
     state->error = 0x17;
     state->reason = "Pause on PRI/Upgrade";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_32: {
+  s_n_llhttp__internal__n_error_38: {
     state->error = 0x9;
     state->reason = "Expected HTTP/2 Connection Preface";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_30: {
+  s_n_llhttp__internal__n_error_36: {
     state->error = 0x9;
     state->reason = "Expected CRLF after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6862,32 +7098,124 @@
         goto s_n_llhttp__internal__n_req_pri_upgrade;
       default:
         goto s_n_llhttp__internal__n_req_http_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_35: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_35;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_39: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_1: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_39;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_40: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_2: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_40;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_34: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_major: {
+    switch (llhttp__internal__c_load_http_major(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_1;
+      case 2:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_2;
+      default:
+        goto s_n_llhttp__internal__n_error_34;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_9: {
+    switch (llhttp__internal__c_test_lenient_flags_9(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_invoke_load_http_major;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_http_minor: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_9;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_33: {
+  s_n_llhttp__internal__n_error_41: {
     state->error = 0x9;
     state->reason = "Invalid minor version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_34: {
+  s_n_llhttp__internal__n_error_42: {
     state->error = 0x9;
     state->reason = "Expected dot";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6896,24 +7224,24 @@
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_35: {
+  s_n_llhttp__internal__n_error_43: {
     state->error = 0x9;
     state->reason = "Invalid major version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_29: {
+  s_n_llhttp__internal__n_error_33: {
     state->error = 0x8;
     state->reason = "Invalid method for HTTP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -6987,48 +7315,48 @@
       case 32:
         goto s_n_llhttp__internal__n_req_http_major;
       case 33:
         goto s_n_llhttp__internal__n_req_http_major;
       case 34:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_29;
+        goto s_n_llhttp__internal__n_error_33;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_38: {
+  s_n_llhttp__internal__n_error_46: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_36: {
+  s_n_llhttp__internal__n_error_44: {
     state->error = 0x8;
     state->reason = "Expected SOURCE method for ICE/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_2: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 33:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_36;
+        goto s_n_llhttp__internal__n_error_44;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_37: {
+  s_n_llhttp__internal__n_error_45: {
     state->error = 0x8;
     state->reason = "Invalid method for RTSP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7060,15 +7388,15 @@
       case 43:
         goto s_n_llhttp__internal__n_req_http_major;
       case 44:
         goto s_n_llhttp__internal__n_req_http_major;
       case 45:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_37;
+        goto s_n_llhttp__internal__n_error_45;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete_1: {
     switch (llhttp__on_url_complete(state, p, endp)) {
       default:
@@ -7141,15 +7469,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_39: {
+  s_n_llhttp__internal__n_error_47: {
     state->error = 0x7;
     state->reason = "Invalid char in url fragment start";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7201,24 +7529,24 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_40: {
+  s_n_llhttp__internal__n_error_48: {
     state->error = 0x7;
     state->reason = "Invalid char in url query";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_41: {
+  s_n_llhttp__internal__n_error_49: {
     state->error = 0x7;
     state->reason = "Invalid char in url path";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7321,60 +7649,60 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_42: {
+  s_n_llhttp__internal__n_error_50: {
     state->error = 0x7;
     state->reason = "Double @ in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_43: {
+  s_n_llhttp__internal__n_error_51: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_44: {
+  s_n_llhttp__internal__n_error_52: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_46: {
+  s_n_llhttp__internal__n_error_54: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_47: {
+  s_n_llhttp__internal__n_error_55: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_48: {
+  s_n_llhttp__internal__n_error_56: {
     state->error = 0x7;
     state->reason = "Unexpected start char in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7385,15 +7713,15 @@
         goto s_n_llhttp__internal__n_url_entry_normal;
       default:
         goto s_n_llhttp__internal__n_url_entry_connect;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_49: {
+  s_n_llhttp__internal__n_error_57: {
     state->error = 0x6;
     state->reason = "Expected space after method";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7402,43 +7730,43 @@
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_first_space_before_url;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_58: {
+  s_n_llhttp__internal__n_error_70: {
     state->error = 0x6;
     state->reason = "Invalid method encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_50: {
+  s_n_llhttp__internal__n_error_60: {
     state->error = 0xd;
     state->reason = "Response overflow";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_status_code: {
     switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_error_50;
+        goto s_n_llhttp__internal__n_error_60;
       default:
         goto s_n_llhttp__internal__n_res_status_code;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_51: {
+  s_n_llhttp__internal__n_error_61: {
     state->error = 0x2;
     state->reason = "Expected LF after CR";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7475,15 +7803,15 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_res_line_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_52: {
+  s_n_llhttp__internal__n_error_62: {
     state->error = 0xd;
     state->reason = "Invalid response status";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7492,41 +7820,133 @@
     switch (llhttp__internal__c_update_status_code(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_res_status_code;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_53: {
+  s_n_llhttp__internal__n_error_63: {
     state->error = 0x9;
     state->reason = "Expected space after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_59: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_59;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_64: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_res_http_end;
+      case 1:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_64;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_65: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_65;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_58: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_major_1: {
+    switch (llhttp__internal__c_load_http_major(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_3;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_4;
+      case 2:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_5;
+      default:
+        goto s_n_llhttp__internal__n_error_58;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_10: {
+    switch (llhttp__internal__c_test_lenient_flags_9(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_invoke_load_http_major_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_http_minor_1: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_10;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_54: {
+  s_n_llhttp__internal__n_error_66: {
     state->error = 0x9;
     state->reason = "Invalid minor version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_55: {
+  s_n_llhttp__internal__n_error_67: {
     state->error = 0x9;
     state->reason = "Expected dot";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7535,24 +7955,24 @@
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_res_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_56: {
+  s_n_llhttp__internal__n_error_68: {
     state->error = 0x9;
     state->reason = "Invalid major version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_59: {
+  s_n_llhttp__internal__n_error_71: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -7569,15 +7989,15 @@
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_invoke_update_type;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_57: {
+  s_n_llhttp__internal__n_error_69: {
     state->error = 0x8;
     state->reason = "Invalid word encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -8036,29 +8456,32 @@
   s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value,
   s_n_llhttp__internal__n_header_value_discard_lws,
   s_n_llhttp__internal__n_header_value_discard_ws_almost_done,
   s_n_llhttp__internal__n_header_value_lws,
   s_n_llhttp__internal__n_header_value_almost_done,
   s_n_llhttp__internal__n_header_value_lenient,
+  s_n_llhttp__internal__n_error_20,
   s_n_llhttp__internal__n_header_value_otherwise,
   s_n_llhttp__internal__n_header_value_connection_token,
   s_n_llhttp__internal__n_header_value_connection_ws,
   s_n_llhttp__internal__n_header_value_connection_1,
   s_n_llhttp__internal__n_header_value_connection_2,
   s_n_llhttp__internal__n_header_value_connection_3,
   s_n_llhttp__internal__n_header_value_connection,
-  s_n_llhttp__internal__n_error_19,
-  s_n_llhttp__internal__n_error_20,
+  s_n_llhttp__internal__n_error_22,
+  s_n_llhttp__internal__n_error_23,
   s_n_llhttp__internal__n_header_value_content_length_ws,
   s_n_llhttp__internal__n_header_value_content_length,
-  s_n_llhttp__internal__n_header_value_te_chunked_last,
+  s_n_llhttp__internal__n_error_25,
+  s_n_llhttp__internal__n_error_24,
   s_n_llhttp__internal__n_header_value_te_token_ows,
   s_n_llhttp__internal__n_header_value,
   s_n_llhttp__internal__n_header_value_te_token,
+  s_n_llhttp__internal__n_header_value_te_chunked_last,
   s_n_llhttp__internal__n_header_value_te_chunked,
   s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1,
   s_n_llhttp__internal__n_header_value_discard_ws,
   s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete,
   s_n_llhttp__internal__n_header_field_general_otherwise,
   s_n_llhttp__internal__n_header_field_general,
   s_n_llhttp__internal__n_header_field_colon,
@@ -8482,39 +8905,39 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 8;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_2(
+int llhttp__internal__c_update_header_state_3(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 6;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_4(
+int llhttp__internal__c_update_header_state_1(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 0;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_5(
+int llhttp__internal__c_update_header_state_6(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 5;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_6(
+int llhttp__internal__c_update_header_state_7(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 7;
   return 0;
 }
 
@@ -8555,14 +8978,28 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 32;
   return 0;
 }
 
+int llhttp__internal__c_test_flags_3(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->flags & 8) == 8;
+}
+
+int llhttp__internal__c_test_lenient_flags_7(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 8) == 8;
+}
+
 int llhttp__internal__c_or_flags_16(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 512;
   return 0;
 }
@@ -8571,23 +9008,23 @@
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags &= -9;
   return 0;
 }
 
-int llhttp__internal__c_update_header_state_7(
+int llhttp__internal__c_update_header_state_8(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->header_state = 8;
   return 0;
 }
 
-int llhttp__internal__c_or_flags_17(
+int llhttp__internal__c_or_flags_18(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->flags |= 16;
   return 0;
 }
 
@@ -8612,14 +9049,35 @@
     const unsigned char* p,
     const unsigned char* endp,
     int match) {
   state->http_minor = match;
   return 0;
 }
 
+int llhttp__internal__c_test_lenient_flags_9(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return (state->lenient_flags & 16) == 16;
+}
+
+int llhttp__internal__c_load_http_major(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->http_major;
+}
+
+int llhttp__internal__c_load_http_minor(
+    llhttp__internal_t* state,
+    const unsigned char* p,
+    const unsigned char* endp) {
+  return state->http_minor;
+}
+
 int llhttp__internal__c_update_status_code(
     llhttp__internal_t* state,
     const unsigned char* p,
     const unsigned char* endp) {
   state->status_code = 0;
   return 0;
 }
@@ -9261,51 +9719,58 @@
     s_n_llhttp__internal__n_header_value_discard_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_lws;
       }
       switch (*p) {
         case 9: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_ws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_4;
         }
         default: {
           goto s_n_llhttp__internal__n_invoke_load_header_state;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_discard_ws_almost_done:
     s_n_llhttp__internal__n_header_value_discard_ws_almost_done: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
       }
-      p++;
-      goto s_n_llhttp__internal__n_header_value_discard_lws;
+      switch (*p) {
+        case 10: {
+          p++;
+          goto s_n_llhttp__internal__n_header_value_discard_lws;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_5;
+        }
+      }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lws:
     s_n_llhttp__internal__n_header_value_lws: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lws;
       }
       switch (*p) {
         case 9: {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         case ' ': {
-          goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_load_header_state_3;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_almost_done:
     s_n_llhttp__internal__n_header_value_almost_done: {
@@ -9314,54 +9779,61 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lws;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_16;
+          goto s_n_llhttp__internal__n_error_19;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_lenient:
     s_n_llhttp__internal__n_header_value_lenient: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_lenient;
       }
       switch (*p) {
         case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3;
         }
         case 13: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4;
         }
         default: {
           p++;
           goto s_n_llhttp__internal__n_header_value_lenient;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
+    case s_n_llhttp__internal__n_error_20:
+    s_n_llhttp__internal__n_error_20: {
+      state->error = 0xa;
+      state->reason = "Invalid header value char";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
     case s_n_llhttp__internal__n_header_value_otherwise:
     s_n_llhttp__internal__n_header_value_otherwise: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_otherwise;
       }
       switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
-        }
         case 13: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_6;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_token:
     s_n_llhttp__internal__n_header_value_connection_token: {
@@ -9416,18 +9888,18 @@
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_connection_ws;
         }
         case ',': {
           p++;
-          goto s_n_llhttp__internal__n_invoke_load_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_load_header_state_5;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_4;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_connection_1:
     s_n_llhttp__internal__n_header_value_connection_1: {
@@ -9437,15 +9909,15 @@
         return s_n_llhttp__internal__n_header_value_connection_1;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob3, 4);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_2;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_1;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9461,15 +9933,15 @@
         return s_n_llhttp__internal__n_header_value_connection_2;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob4, 9);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_5;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_2;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9485,15 +9957,15 @@
         return s_n_llhttp__internal__n_header_value_connection_3;
       }
       match_seq = llparse__match_sequence_to_lower(state, p, endp, llparse_blob5, 6);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_invoke_update_header_state_6;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_value_connection_3;
         }
         case kMatchMismatch: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
@@ -9530,26 +10002,26 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_connection_token;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_19:
-    s_n_llhttp__internal__n_error_19: {
+    case s_n_llhttp__internal__n_error_22:
+    s_n_llhttp__internal__n_error_22: {
       state->error = 0xb;
       state->reason = "Content-Length overflow";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_error_20:
-    s_n_llhttp__internal__n_error_20: {
+    case s_n_llhttp__internal__n_error_23:
+    s_n_llhttp__internal__n_error_23: {
       state->error = 0xb;
       state->reason = "Invalid character in Content-Length";
       state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_error;
       return s_error;
       /* UNREACHABLE */;
       abort();
@@ -9567,15 +10039,15 @@
           goto s_n_llhttp__internal__n_invoke_or_flags_15;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
         default: {
-          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
+          goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_6;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_content_length:
     s_n_llhttp__internal__n_header_value_content_length: {
@@ -9636,34 +10108,31 @@
         default: {
           goto s_n_llhttp__internal__n_header_value_content_length_ws;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
-    case s_n_llhttp__internal__n_header_value_te_chunked_last:
-    s_n_llhttp__internal__n_header_value_te_chunked_last: {
-      if (p == endp) {
-        return s_n_llhttp__internal__n_header_value_te_chunked_last;
-      }
-      switch (*p) {
-        case 10: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
-        }
-        case 13: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_7;
-        }
-        case ' ': {
-          p++;
-          goto s_n_llhttp__internal__n_header_value_te_chunked_last;
-        }
-        default: {
-          goto s_n_llhttp__internal__n_header_value_te_chunked;
-        }
-      }
+    case s_n_llhttp__internal__n_error_25:
+    s_n_llhttp__internal__n_error_25: {
+      state->error = 0xf;
+      state->reason = "Invalid `Transfer-Encoding` header value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_error_24:
+    s_n_llhttp__internal__n_error_24: {
+      state->error = 0xf;
+      state->reason = "Invalid `Transfer-Encoding` header value";
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_error;
+      return s_error;
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_token_ows:
     s_n_llhttp__internal__n_header_value_te_token_ows: {
       if (p == endp) {
         return s_n_llhttp__internal__n_header_value_te_token_ows;
@@ -9772,16 +10241,42 @@
           goto s_n_llhttp__internal__n_header_value_te_token;
         }
         case 2: {
           p++;
           goto s_n_llhttp__internal__n_header_value_te_token_ows;
         }
         default: {
+          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+        }
+      }
+      /* UNREACHABLE */;
+      abort();
+    }
+    case s_n_llhttp__internal__n_header_value_te_chunked_last:
+    s_n_llhttp__internal__n_header_value_te_chunked_last: {
+      if (p == endp) {
+        return s_n_llhttp__internal__n_header_value_te_chunked_last;
+      }
+      switch (*p) {
+        case 10: {
+          goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        }
+        case 13: {
           goto s_n_llhttp__internal__n_invoke_update_header_state_8;
         }
+        case ' ': {
+          p++;
+          goto s_n_llhttp__internal__n_header_value_te_chunked_last;
+        }
+        case ',': {
+          goto s_n_llhttp__internal__n_invoke_load_type_1;
+        }
+        default: {
+          goto s_n_llhttp__internal__n_header_value_te_token;
+        }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_value_te_chunked:
     s_n_llhttp__internal__n_header_value_te_chunked: {
       llparse_match_t match_seq;
@@ -9825,15 +10320,15 @@
       switch (*p) {
         case 9: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws;
         }
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_header_value_discard_lws;
+          goto s_n_llhttp__internal__n_invoke_test_lenient_flags_3;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_header_value_discard_ws_almost_done;
         }
         case ' ': {
           p++;
@@ -9861,15 +10356,15 @@
         return s_n_llhttp__internal__n_header_field_general_otherwise;
       }
       switch (*p) {
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_2;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_21;
+          goto s_n_llhttp__internal__n_error_26;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_general:
     s_n_llhttp__internal__n_header_field_general: {
@@ -9951,15 +10446,15 @@
         case ' ': {
           goto s_n_llhttp__internal__n_invoke_test_lenient_flags_2;
         }
         case ':': {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_9;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_3:
     s_n_llhttp__internal__n_header_field_3: {
@@ -9976,15 +10471,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_4:
     s_n_llhttp__internal__n_header_field_4: {
@@ -10001,15 +10496,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_2:
     s_n_llhttp__internal__n_header_field_2: {
@@ -10022,15 +10517,15 @@
           goto s_n_llhttp__internal__n_header_field_3;
         }
         case 't': {
           p++;
           goto s_n_llhttp__internal__n_header_field_4;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_1:
     s_n_llhttp__internal__n_header_field_1: {
@@ -10046,15 +10541,15 @@
           p++;
           goto s_n_llhttp__internal__n_header_field_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_5:
     s_n_llhttp__internal__n_header_field_5: {
@@ -10071,15 +10566,15 @@
           match = 1;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_5;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_6:
     s_n_llhttp__internal__n_header_field_6: {
@@ -10096,15 +10591,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field_7:
     s_n_llhttp__internal__n_header_field_7: {
@@ -10121,15 +10616,15 @@
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_header_state;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_header_field_7;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_header_field:
     s_n_llhttp__internal__n_header_field: {
@@ -10150,15 +10645,15 @@
           goto s_n_llhttp__internal__n_header_field_6;
         }
         case 'u': {
           p++;
           goto s_n_llhttp__internal__n_header_field_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_invoke_update_header_state_10;
+          goto s_n_llhttp__internal__n_invoke_update_header_state_11;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_header_field:
     s_n_llhttp__internal__n_span_start_llhttp__on_header_field: {
@@ -10215,15 +10710,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_update_http_major;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_url_skip_lf_to_http09;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_22;
+          goto s_n_llhttp__internal__n_error_27;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_pri_upgrade:
     s_n_llhttp__internal__n_req_pri_upgrade: {
@@ -10233,21 +10728,21 @@
         return s_n_llhttp__internal__n_req_pri_upgrade;
       }
       match_seq = llparse__match_sequence_id(state, p, endp, llparse_blob16, 10);
       p = match_seq.current;
       switch (match_seq.status) {
         case kMatchComplete: {
           p++;
-          goto s_n_llhttp__internal__n_error_25;
+          goto s_n_llhttp__internal__n_error_32;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_pri_upgrade;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_26;
+          goto s_n_llhttp__internal__n_error_33;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete_1:
     s_n_llhttp__internal__n_req_http_complete_1: {
@@ -10256,15 +10751,15 @@
       }
       switch (*p) {
         case 10: {
           p++;
           goto s_n_llhttp__internal__n_header_field_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_24;
+          goto s_n_llhttp__internal__n_error_31;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_complete:
     s_n_llhttp__internal__n_req_http_complete: {
@@ -10277,15 +10772,15 @@
           goto s_n_llhttp__internal__n_header_field_start;
         }
         case 13: {
           p++;
           goto s_n_llhttp__internal__n_req_http_complete_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_24;
+          goto s_n_llhttp__internal__n_error_31;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_minor:
     s_n_llhttp__internal__n_req_http_minor: {
@@ -10340,15 +10835,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_27;
+          goto s_n_llhttp__internal__n_error_36;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_dot:
     s_n_llhttp__internal__n_req_http_dot: {
@@ -10357,15 +10852,15 @@
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_req_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_28;
+          goto s_n_llhttp__internal__n_error_37;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_major:
     s_n_llhttp__internal__n_req_http_major: {
@@ -10420,15 +10915,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_29;
+          goto s_n_llhttp__internal__n_error_38;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_1:
     s_n_llhttp__internal__n_req_http_start_1: {
@@ -10444,15 +10939,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_1;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_32;
+          goto s_n_llhttp__internal__n_error_41;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_2:
     s_n_llhttp__internal__n_req_http_start_2: {
@@ -10468,15 +10963,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_2;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_32;
+          goto s_n_llhttp__internal__n_error_41;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start_3:
     s_n_llhttp__internal__n_req_http_start_3: {
@@ -10492,15 +10987,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_load_method_3;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_http_start_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_32;
+          goto s_n_llhttp__internal__n_error_41;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_http_start:
     s_n_llhttp__internal__n_req_http_start: {
@@ -10521,15 +11016,15 @@
           goto s_n_llhttp__internal__n_req_http_start_2;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_req_http_start_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_32;
+          goto s_n_llhttp__internal__n_error_41;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_skip_to_http:
     s_n_llhttp__internal__n_url_skip_to_http: {
@@ -10575,15 +11070,15 @@
         case 3: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_7;
         }
         case 4: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_8;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_33;
+          goto s_n_llhttp__internal__n_error_42;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_query_3:
     s_n_llhttp__internal__n_span_end_stub_query_3: {
@@ -10632,15 +11127,15 @@
         case 4: {
           goto s_n_llhttp__internal__n_span_end_llhttp__on_url_11;
         }
         case 5: {
           goto s_n_llhttp__internal__n_span_end_stub_query_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_34;
+          goto s_n_llhttp__internal__n_error_43;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_query_or_fragment:
     s_n_llhttp__internal__n_url_query_or_fragment: {
@@ -10662,15 +11157,15 @@
           goto s_n_llhttp__internal__n_url_fragment;
         }
         case '?': {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_35;
+          goto s_n_llhttp__internal__n_error_44;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_path:
     s_n_llhttp__internal__n_url_path: {
@@ -10803,18 +11298,18 @@
         }
         case 6: {
           p++;
           goto s_n_llhttp__internal__n_url_query;
         }
         case 7: {
           p++;
-          goto s_n_llhttp__internal__n_error_36;
+          goto s_n_llhttp__internal__n_error_45;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_37;
+          goto s_n_llhttp__internal__n_error_46;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_server:
     s_n_llhttp__internal__n_url_server: {
@@ -10861,15 +11356,15 @@
           goto s_n_llhttp__internal__n_url_query;
         }
         case 7: {
           p++;
           goto s_n_llhttp__internal__n_url_server_with_at;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_38;
+          goto s_n_llhttp__internal__n_error_47;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim_1:
     s_n_llhttp__internal__n_url_schema_delim_1: {
@@ -10878,44 +11373,44 @@
       }
       switch (*p) {
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_server;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_40;
+          goto s_n_llhttp__internal__n_error_49;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_schema_delim:
     s_n_llhttp__internal__n_url_schema_delim: {
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema_delim;
       }
       switch (*p) {
         case 10: {
           p++;
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_48;
         }
         case 13: {
           p++;
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_48;
         }
         case ' ': {
           p++;
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_48;
         }
         case '/': {
           p++;
           goto s_n_llhttp__internal__n_url_schema_delim_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_40;
+          goto s_n_llhttp__internal__n_error_49;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_end_stub_schema:
     s_n_llhttp__internal__n_span_end_stub_schema: {
@@ -10949,25 +11444,25 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_schema;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_48;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_end_stub_schema;
         }
         case 3: {
           p++;
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_41;
+          goto s_n_llhttp__internal__n_error_50;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_url_start:
     s_n_llhttp__internal__n_url_start: {
@@ -10991,24 +11486,24 @@
       };
       if (p == endp) {
         return s_n_llhttp__internal__n_url_start;
       }
       switch (lookup_table[(uint8_t) *p]) {
         case 1: {
           p++;
-          goto s_n_llhttp__internal__n_error_39;
+          goto s_n_llhttp__internal__n_error_48;
         }
         case 2: {
           goto s_n_llhttp__internal__n_span_start_stub_path_2;
         }
         case 3: {
           goto s_n_llhttp__internal__n_url_schema;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_42;
+          goto s_n_llhttp__internal__n_error_51;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_span_start_llhttp__on_url_1:
     s_n_llhttp__internal__n_span_start_llhttp__on_url_1: {
@@ -11056,15 +11551,15 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_req_spaces_before_url;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_43;
+          goto s_n_llhttp__internal__n_error_52;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_2:
     s_n_llhttp__internal__n_start_req_2: {
@@ -11074,15 +11569,15 @@
       switch (*p) {
         case 'L': {
           p++;
           match = 19;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_3:
     s_n_llhttp__internal__n_start_req_3: {
@@ -11099,15 +11594,15 @@
           match = 36;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_1:
     s_n_llhttp__internal__n_start_req_1: {
@@ -11120,15 +11615,15 @@
           goto s_n_llhttp__internal__n_start_req_2;
         }
         case 'N': {
           p++;
           goto s_n_llhttp__internal__n_start_req_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_4:
     s_n_llhttp__internal__n_start_req_4: {
@@ -11145,15 +11640,15 @@
           match = 16;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_4;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_6:
     s_n_llhttp__internal__n_start_req_6: {
@@ -11170,15 +11665,15 @@
           match = 22;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_6;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_8:
     s_n_llhttp__internal__n_start_req_8: {
@@ -11195,15 +11690,15 @@
           match = 5;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_8;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_9:
     s_n_llhttp__internal__n_start_req_9: {
@@ -11213,15 +11708,15 @@
       switch (*p) {
         case 'Y': {
           p++;
           match = 8;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_7:
     s_n_llhttp__internal__n_start_req_7: {
@@ -11234,15 +11729,15 @@
           goto s_n_llhttp__internal__n_start_req_8;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_9;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_5:
     s_n_llhttp__internal__n_start_req_5: {
@@ -11255,15 +11750,15 @@
           goto s_n_llhttp__internal__n_start_req_6;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_7;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_12:
     s_n_llhttp__internal__n_start_req_12: {
@@ -11280,15 +11775,15 @@
           match = 0;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_12;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_13:
     s_n_llhttp__internal__n_start_req_13: {
@@ -11305,15 +11800,15 @@
           match = 35;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_13;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_11:
     s_n_llhttp__internal__n_start_req_11: {
@@ -11326,15 +11821,15 @@
           goto s_n_llhttp__internal__n_start_req_12;
         }
         case 'S': {
           p++;
           goto s_n_llhttp__internal__n_start_req_13;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_10:
     s_n_llhttp__internal__n_start_req_10: {
@@ -11343,15 +11838,15 @@
       }
       switch (*p) {
         case 'E': {
           p++;
           goto s_n_llhttp__internal__n_start_req_11;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_14:
     s_n_llhttp__internal__n_start_req_14: {
@@ -11368,15 +11863,15 @@
           match = 45;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_14;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_17:
     s_n_llhttp__internal__n_start_req_17: {
@@ -11393,15 +11888,15 @@
           match = 41;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_17;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_16:
     s_n_llhttp__internal__n_start_req_16: {
@@ -11435,15 +11930,15 @@
           p++;
           goto s_n_llhttp__internal__n_start_req_16;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_15;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_18:
     s_n_llhttp__internal__n_start_req_18: {
@@ -11460,15 +11955,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_18;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_20:
     s_n_llhttp__internal__n_start_req_20: {
@@ -11485,15 +11980,15 @@
           match = 31;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_20;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_21:
     s_n_llhttp__internal__n_start_req_21: {
@@ -11510,15 +12005,15 @@
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_21;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_19:
     s_n_llhttp__internal__n_start_req_19: {
@@ -11531,15 +12026,15 @@
           goto s_n_llhttp__internal__n_start_req_20;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_21;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_23:
     s_n_llhttp__internal__n_start_req_23: {
@@ -11556,15 +12051,15 @@
           match = 24;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_23;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_24:
     s_n_llhttp__internal__n_start_req_24: {
@@ -11581,15 +12076,15 @@
           match = 23;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_24;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_26:
     s_n_llhttp__internal__n_start_req_26: {
@@ -11606,15 +12101,15 @@
           match = 21;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_26;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_28:
     s_n_llhttp__internal__n_start_req_28: {
@@ -11631,15 +12126,15 @@
           match = 30;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_28;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_29:
     s_n_llhttp__internal__n_start_req_29: {
@@ -11649,15 +12144,15 @@
       switch (*p) {
         case 'L': {
           p++;
           match = 10;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_27:
     s_n_llhttp__internal__n_start_req_27: {
@@ -11670,15 +12165,15 @@
           goto s_n_llhttp__internal__n_start_req_28;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_29;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_25:
     s_n_llhttp__internal__n_start_req_25: {
@@ -11691,15 +12186,15 @@
           goto s_n_llhttp__internal__n_start_req_26;
         }
         case 'C': {
           p++;
           goto s_n_llhttp__internal__n_start_req_27;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_30:
     s_n_llhttp__internal__n_start_req_30: {
@@ -11716,15 +12211,15 @@
           match = 11;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_30;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_22:
     s_n_llhttp__internal__n_start_req_22: {
@@ -11745,15 +12240,15 @@
           goto s_n_llhttp__internal__n_start_req_25;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_30;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_31:
     s_n_llhttp__internal__n_start_req_31: {
@@ -11770,15 +12265,15 @@
           match = 25;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_31;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_32:
     s_n_llhttp__internal__n_start_req_32: {
@@ -11795,15 +12290,15 @@
           match = 6;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_32;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_35:
     s_n_llhttp__internal__n_start_req_35: {
@@ -11820,15 +12315,15 @@
           match = 28;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_35;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_36:
     s_n_llhttp__internal__n_start_req_36: {
@@ -11845,15 +12340,15 @@
           match = 39;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_36;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_34:
     s_n_llhttp__internal__n_start_req_34: {
@@ -11866,15 +12361,15 @@
           goto s_n_llhttp__internal__n_start_req_35;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_36;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_37:
     s_n_llhttp__internal__n_start_req_37: {
@@ -11891,15 +12386,15 @@
           match = 38;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_37;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_38:
     s_n_llhttp__internal__n_start_req_38: {
@@ -11916,15 +12411,15 @@
           match = 3;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_38;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_42:
     s_n_llhttp__internal__n_start_req_42: {
@@ -11941,15 +12436,15 @@
           match = 12;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_42;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_43:
     s_n_llhttp__internal__n_start_req_43: {
@@ -11966,15 +12461,15 @@
           match = 13;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_43;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_41:
     s_n_llhttp__internal__n_start_req_41: {
@@ -11987,15 +12482,15 @@
           goto s_n_llhttp__internal__n_start_req_42;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_43;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_40:
     s_n_llhttp__internal__n_start_req_40: {
@@ -12004,15 +12499,15 @@
       }
       switch (*p) {
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_41;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_39:
     s_n_llhttp__internal__n_start_req_39: {
@@ -12026,15 +12521,15 @@
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_40;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_45:
     s_n_llhttp__internal__n_start_req_45: {
@@ -12051,15 +12546,15 @@
           match = 29;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_45;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_44:
     s_n_llhttp__internal__n_start_req_44: {
@@ -12073,15 +12568,15 @@
         }
         case 'T': {
           p++;
           match = 4;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_33:
     s_n_llhttp__internal__n_start_req_33: {
@@ -12106,15 +12601,15 @@
           goto s_n_llhttp__internal__n_start_req_39;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_44;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_48:
     s_n_llhttp__internal__n_start_req_48: {
@@ -12131,15 +12626,15 @@
           match = 17;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_48;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_49:
     s_n_llhttp__internal__n_start_req_49: {
@@ -12156,15 +12651,15 @@
           match = 44;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_49;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_50:
     s_n_llhttp__internal__n_start_req_50: {
@@ -12181,15 +12676,15 @@
           match = 43;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_50;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_51:
     s_n_llhttp__internal__n_start_req_51: {
@@ -12206,15 +12701,15 @@
           match = 20;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_51;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_47:
     s_n_llhttp__internal__n_start_req_47: {
@@ -12235,15 +12730,15 @@
           goto s_n_llhttp__internal__n_start_req_50;
         }
         case 'P': {
           p++;
           goto s_n_llhttp__internal__n_start_req_51;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_46:
     s_n_llhttp__internal__n_start_req_46: {
@@ -12252,15 +12747,15 @@
       }
       switch (*p) {
         case 'E': {
           p++;
           goto s_n_llhttp__internal__n_start_req_47;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_54:
     s_n_llhttp__internal__n_start_req_54: {
@@ -12277,15 +12772,15 @@
           match = 14;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_54;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_56:
     s_n_llhttp__internal__n_start_req_56: {
@@ -12295,15 +12790,15 @@
       switch (*p) {
         case 'P': {
           p++;
           match = 37;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_57:
     s_n_llhttp__internal__n_start_req_57: {
@@ -12320,15 +12815,15 @@
           match = 42;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_57;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_55:
     s_n_llhttp__internal__n_start_req_55: {
@@ -12341,15 +12836,15 @@
           goto s_n_llhttp__internal__n_start_req_56;
         }
         case '_': {
           p++;
           goto s_n_llhttp__internal__n_start_req_57;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_53:
     s_n_llhttp__internal__n_start_req_53: {
@@ -12362,15 +12857,15 @@
           goto s_n_llhttp__internal__n_start_req_54;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_start_req_55;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_58:
     s_n_llhttp__internal__n_start_req_58: {
@@ -12387,15 +12882,15 @@
           match = 33;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_58;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_59:
     s_n_llhttp__internal__n_start_req_59: {
@@ -12412,15 +12907,15 @@
           match = 26;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_59;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_52:
     s_n_llhttp__internal__n_start_req_52: {
@@ -12437,15 +12932,15 @@
           goto s_n_llhttp__internal__n_start_req_58;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_59;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_61:
     s_n_llhttp__internal__n_start_req_61: {
@@ -12462,15 +12957,15 @@
           match = 40;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_61;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_62:
     s_n_llhttp__internal__n_start_req_62: {
@@ -12487,15 +12982,15 @@
           match = 7;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_62;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_60:
     s_n_llhttp__internal__n_start_req_60: {
@@ -12508,15 +13003,15 @@
           goto s_n_llhttp__internal__n_start_req_61;
         }
         case 'R': {
           p++;
           goto s_n_llhttp__internal__n_start_req_62;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_65:
     s_n_llhttp__internal__n_start_req_65: {
@@ -12533,15 +13028,15 @@
           match = 18;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_65;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_67:
     s_n_llhttp__internal__n_start_req_67: {
@@ -12558,15 +13053,15 @@
           match = 32;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_67;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_68:
     s_n_llhttp__internal__n_start_req_68: {
@@ -12583,15 +13078,15 @@
           match = 15;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_68;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_66:
     s_n_llhttp__internal__n_start_req_66: {
@@ -12604,15 +13099,15 @@
           goto s_n_llhttp__internal__n_start_req_67;
         }
         case 'O': {
           p++;
           goto s_n_llhttp__internal__n_start_req_68;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_69:
     s_n_llhttp__internal__n_start_req_69: {
@@ -12629,15 +13124,15 @@
           match = 27;
           goto s_n_llhttp__internal__n_invoke_store_method_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_req_69;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_64:
     s_n_llhttp__internal__n_start_req_64: {
@@ -12654,15 +13149,15 @@
           goto s_n_llhttp__internal__n_start_req_66;
         }
         case 'S': {
           p++;
           goto s_n_llhttp__internal__n_start_req_69;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_63:
     s_n_llhttp__internal__n_start_req_63: {
@@ -12671,15 +13166,15 @@
       }
       switch (*p) {
         case 'N': {
           p++;
           goto s_n_llhttp__internal__n_start_req_64;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req:
     s_n_llhttp__internal__n_start_req: {
@@ -12748,15 +13243,15 @@
           goto s_n_llhttp__internal__n_start_req_60;
         }
         case 'U': {
           p++;
           goto s_n_llhttp__internal__n_start_req_63;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_51;
+          goto s_n_llhttp__internal__n_error_64;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_invoke_llhttp__on_status_complete:
     s_n_llhttp__internal__n_invoke_llhttp__on_status_complete: {
@@ -12842,15 +13337,15 @@
           goto s_n_llhttp__internal__n_res_status_start;
         }
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_res_status_start;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_45;
+          goto s_n_llhttp__internal__n_error_56;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_status_code:
     s_n_llhttp__internal__n_res_status_code: {
@@ -12922,15 +13417,15 @@
       }
       switch (*p) {
         case ' ': {
           p++;
           goto s_n_llhttp__internal__n_invoke_update_status_code;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_46;
+          goto s_n_llhttp__internal__n_error_57;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_minor:
     s_n_llhttp__internal__n_res_http_minor: {
@@ -12985,15 +13480,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_minor_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_47;
+          goto s_n_llhttp__internal__n_error_60;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_dot:
     s_n_llhttp__internal__n_res_http_dot: {
@@ -13002,15 +13497,15 @@
       }
       switch (*p) {
         case '.': {
           p++;
           goto s_n_llhttp__internal__n_res_http_minor;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_48;
+          goto s_n_llhttp__internal__n_error_61;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_res_http_major:
     s_n_llhttp__internal__n_res_http_major: {
@@ -13065,15 +13560,15 @@
         }
         case '9': {
           p++;
           match = 9;
           goto s_n_llhttp__internal__n_invoke_store_http_major_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_49;
+          goto s_n_llhttp__internal__n_error_62;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_res:
     s_n_llhttp__internal__n_start_res: {
@@ -13089,15 +13584,15 @@
           p++;
           goto s_n_llhttp__internal__n_res_http_major;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_start_res;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_52;
+          goto s_n_llhttp__internal__n_error_65;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_2:
     s_n_llhttp__internal__n_req_or_res_method_2: {
@@ -13114,15 +13609,15 @@
           match = 2;
           goto s_n_llhttp__internal__n_invoke_store_method;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_3:
     s_n_llhttp__internal__n_req_or_res_method_3: {
@@ -13138,15 +13633,15 @@
           p++;
           goto s_n_llhttp__internal__n_invoke_update_type_1;
         }
         case kMatchPause: {
           return s_n_llhttp__internal__n_req_or_res_method_3;
         }
         case kMatchMismatch: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method_1:
     s_n_llhttp__internal__n_req_or_res_method_1: {
@@ -13159,15 +13654,15 @@
           goto s_n_llhttp__internal__n_req_or_res_method_2;
         }
         case 'T': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_3;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_req_or_res_method:
     s_n_llhttp__internal__n_req_or_res_method: {
@@ -13176,15 +13671,15 @@
       }
       switch (*p) {
         case 'H': {
           p++;
           goto s_n_llhttp__internal__n_req_or_res_method_1;
         }
         default: {
-          goto s_n_llhttp__internal__n_error_50;
+          goto s_n_llhttp__internal__n_error_63;
         }
       }
       /* UNREACHABLE */;
       abort();
     }
     case s_n_llhttp__internal__n_start_req_or_res:
     s_n_llhttp__internal__n_start_req_or_res: {
@@ -13236,15 +13731,15 @@
       /* UNREACHABLE */;
       abort();
     }
     default:
       /* UNREACHABLE */
       abort();
   }
-  s_n_llhttp__internal__n_error_39: {
+  s_n_llhttp__internal__n_error_48: {
     state->error = 0x7;
     state->reason = "Invalid characters in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13677,15 +14172,34 @@
         goto s_n_llhttp__internal__n_header_field_colon_discard_ws;
       default:
         goto s_n_llhttp__internal__n_span_end_llhttp__on_header_field;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_15: {
+  s_n_llhttp__internal__n_error_16: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_4: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_ws;
+      default:
+        goto s_n_llhttp__internal__n_error_16;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_17: {
     state->error = 0xb;
     state->reason = "Empty Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13762,62 +14276,118 @@
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 2:
-        goto s_n_llhttp__internal__n_error_15;
+        goto s_n_llhttp__internal__n_error_17;
       default:
         goto s_n_llhttp__internal__n_invoke_load_header_state_1;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_15: {
+    state->error = 0xa;
+    state->reason = "Invalid header value char";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_15;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_18: {
+    state->error = 0x2;
+    state->reason = "Expected LF after CR";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_5: {
+    switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_header_value_discard_lws;
+      default:
+        goto s_n_llhttp__internal__n_error_18;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_update_header_state_1: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+    switch (llhttp__internal__c_load_header_state(state, p, endp)) {
+      case 8:
+        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+      default:
+        goto s_n_llhttp__internal__n_span_start_llhttp__on_header_value_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_2: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_7: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_8: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_9: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_1;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_2;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_10: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_3: {
+  s_n_llhttp__internal__n_invoke_load_header_state_4: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_7;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_8;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_9;
@@ -13825,15 +14395,15 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_10;
       default:
         goto s_n_llhttp__internal__n_invoke_llhttp__on_header_value_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_16: {
+  s_n_llhttp__internal__n_error_19: {
     state->error = 0x3;
     state->reason = "Missing expected LF after header value";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -13843,41 +14413,41 @@
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) p;
+      state->error_pos = (const char*) (p + 1);
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_almost_done;
       return s_error;
     }
+    p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
-      state->error_pos = (const char*) (p + 1);
+      state->error_pos = (const char*) p;
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_header_value_almost_done;
       return s_error;
     }
-    p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_3: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
@@ -13887,74 +14457,82 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_header_value_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_17: {
-    state->error = 0xa;
-    state->reason = "Invalid header value char";
-    state->error_pos = (const char*) p;
-    state->_current = (void*) (intptr_t) s_error;
-    return s_error;
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) p;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_20;
+      return s_error;
+    }
+    goto s_n_llhttp__internal__n_error_20;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_test_lenient_flags_3: {
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_6: {
     switch (llhttp__internal__c_test_lenient_flags_2(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_lenient;
       default:
-        goto s_n_llhttp__internal__n_error_17;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_2;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+  s_n_llhttp__internal__n_invoke_update_header_state_4: {
     switch (llhttp__internal__c_update_header_state(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_11: {
     switch (llhttp__internal__c_or_flags_3(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_12: {
     switch (llhttp__internal__c_or_flags_4(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_13: {
     switch (llhttp__internal__c_or_flags_5(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_3;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_4;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_14: {
     switch (llhttp__internal__c_or_flags_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_load_header_state_4: {
+  s_n_llhttp__internal__n_invoke_load_header_state_5: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 5:
         goto s_n_llhttp__internal__n_invoke_or_flags_11;
       case 6:
         goto s_n_llhttp__internal__n_invoke_or_flags_12;
       case 7:
         goto s_n_llhttp__internal__n_invoke_or_flags_13;
@@ -13962,167 +14540,261 @@
         goto s_n_llhttp__internal__n_invoke_or_flags_14;
       default:
         goto s_n_llhttp__internal__n_header_value_connection;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_4: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_5: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_token;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_2: {
-    switch (llhttp__internal__c_update_header_state_2(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_3: {
+    switch (llhttp__internal__c_update_header_state_3(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_5: {
-    switch (llhttp__internal__c_update_header_state_5(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_6: {
+    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_6: {
-    switch (llhttp__internal__c_update_header_state_6(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_7: {
+    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_connection_ws;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_19;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_22;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_19;
+    goto s_n_llhttp__internal__n_error_22;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_content_length_1: {
     switch (llhttp__internal__c_mul_add_content_length_1(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_4;
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5;
       default:
         goto s_n_llhttp__internal__n_header_value_content_length;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_or_flags_15: {
     switch (llhttp__internal__c_or_flags_15(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_5: {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_6: {
     const unsigned char* start;
     int err;
     
     start = state->_span_pos0;
     state->_span_pos0 = NULL;
     err = llhttp__on_header_value(state, start, p);
     if (err != 0) {
       state->error = err;
       state->error_pos = (const char*) p;
-      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_20;
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_23;
       return s_error;
     }
-    goto s_n_llhttp__internal__n_error_20;
+    goto s_n_llhttp__internal__n_error_23;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_18: {
+  s_n_llhttp__internal__n_error_21: {
     state->error = 0x4;
     state->reason = "Duplicate Content-Length";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_test_flags_2: {
     switch (llhttp__internal__c_test_flags_2(state, p, endp)) {
       case 0:
         goto s_n_llhttp__internal__n_header_value_content_length;
       default:
-        goto s_n_llhttp__internal__n_error_18;
+        goto s_n_llhttp__internal__n_error_21;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_7: {
-    switch (llhttp__internal__c_update_header_state_7(state, p, endp)) {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_25;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_25;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_8: {
+    switch (llhttp__internal__c_update_header_state_8(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_otherwise;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_8: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7: {
+    const unsigned char* start;
+    int err;
+    
+    start = state->_span_pos0;
+    state->_span_pos0 = NULL;
+    err = llhttp__on_header_value(state, start, p);
+    if (err != 0) {
+      state->error = err;
+      state->error_pos = (const char*) (p + 1);
+      state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_error_24;
+      return s_error;
+    }
+    p++;
+    goto s_n_llhttp__internal__n_error_24;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_7: {
+    switch (llhttp__internal__c_test_lenient_flags_7(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_7;
+      default:
+        goto s_n_llhttp__internal__n_header_value_te_chunked;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_type_1: {
+    switch (llhttp__internal__c_load_type(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_7;
+      default:
+        goto s_n_llhttp__internal__n_header_value_te_chunked;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_update_header_state_9: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_and_flags: {
     switch (llhttp__internal__c_and_flags(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_value_te_chunked;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_invoke_or_flags_17: {
+    switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
+      default:
+        goto s_n_llhttp__internal__n_invoke_and_flags;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_8: {
+    switch (llhttp__internal__c_test_lenient_flags_7(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_span_end_llhttp__on_header_value_8;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_type_2: {
+    switch (llhttp__internal__c_load_type(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_8;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_or_flags_16: {
     switch (llhttp__internal__c_or_flags_16(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_invoke_and_flags;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_or_flags_17: {
-    switch (llhttp__internal__c_or_flags_17(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_test_flags_3: {
+    switch (llhttp__internal__c_test_flags_3(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_type_2;
+      default:
+        goto s_n_llhttp__internal__n_invoke_or_flags_16;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_or_flags_18: {
+    switch (llhttp__internal__c_or_flags_18(state, p, endp)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_update_header_state_8;
+        goto s_n_llhttp__internal__n_invoke_update_header_state_9;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_header_state_2: {
     switch (llhttp__internal__c_load_header_state(state, p, endp)) {
       case 1:
         goto s_n_llhttp__internal__n_header_value_connection;
       case 2:
         goto s_n_llhttp__internal__n_invoke_test_flags_2;
       case 3:
-        goto s_n_llhttp__internal__n_invoke_or_flags_16;
+        goto s_n_llhttp__internal__n_invoke_test_flags_3;
       case 4:
-        goto s_n_llhttp__internal__n_invoke_or_flags_17;
+        goto s_n_llhttp__internal__n_invoke_or_flags_18;
       default:
         goto s_n_llhttp__internal__n_header_value;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_header_field_1: {
@@ -14157,41 +14829,41 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_invoke_llhttp__on_header_field_complete;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_21: {
+  s_n_llhttp__internal__n_error_26: {
     state->error = 0xa;
     state->reason = "Invalid header token";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_9: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_10: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_store_header_state: {
     switch (llhttp__internal__c_store_header_state(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_header_field_colon;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_invoke_update_header_state_10: {
-    switch (llhttp__internal__c_update_header_state_4(state, p, endp)) {
+  s_n_llhttp__internal__n_invoke_update_header_state_11: {
+    switch (llhttp__internal__c_update_header_state_1(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_header_field_general;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete: {
@@ -14231,15 +14903,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_22: {
+  s_n_llhttp__internal__n_error_27: {
     state->error = 0x7;
     state->reason = "Expected CRLF";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14257,33 +14929,33 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_lf_to_http09;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_lf_to_http09;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_25: {
+  s_n_llhttp__internal__n_error_32: {
     state->error = 0x17;
     state->reason = "Pause on PRI/Upgrade";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_26: {
+  s_n_llhttp__internal__n_error_33: {
     state->error = 0x9;
     state->reason = "Expected HTTP/2 Connection Preface";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_24: {
+  s_n_llhttp__internal__n_error_31: {
     state->error = 0x9;
     state->reason = "Expected CRLF after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14294,32 +14966,124 @@
         goto s_n_llhttp__internal__n_req_pri_upgrade;
       default:
         goto s_n_llhttp__internal__n_req_http_complete;
     }
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_30: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_30;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_34: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_1: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_34;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_35: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_2: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_error_35;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_29: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_major: {
+    switch (llhttp__internal__c_load_http_major(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_1;
+      case 2:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_2;
+      default:
+        goto s_n_llhttp__internal__n_error_29;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_9: {
+    switch (llhttp__internal__c_test_lenient_flags_9(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_method_1;
+      default:
+        goto s_n_llhttp__internal__n_invoke_load_http_major;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_http_minor: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_invoke_load_method_1;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_9;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_27: {
+  s_n_llhttp__internal__n_error_36: {
     state->error = 0x9;
     state->reason = "Invalid minor version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_28: {
+  s_n_llhttp__internal__n_error_37: {
     state->error = 0x9;
     state->reason = "Expected dot";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14328,24 +15092,24 @@
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_29: {
+  s_n_llhttp__internal__n_error_38: {
     state->error = 0x9;
     state->reason = "Invalid major version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_23: {
+  s_n_llhttp__internal__n_error_28: {
     state->error = 0x8;
     state->reason = "Invalid method for HTTP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14419,48 +15183,48 @@
       case 32:
         goto s_n_llhttp__internal__n_req_http_major;
       case 33:
         goto s_n_llhttp__internal__n_req_http_major;
       case 34:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_23;
+        goto s_n_llhttp__internal__n_error_28;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_32: {
+  s_n_llhttp__internal__n_error_41: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_30: {
+  s_n_llhttp__internal__n_error_39: {
     state->error = 0x8;
     state->reason = "Expected SOURCE method for ICE/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_load_method_2: {
     switch (llhttp__internal__c_load_method(state, p, endp)) {
       case 33:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_30;
+        goto s_n_llhttp__internal__n_error_39;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_31: {
+  s_n_llhttp__internal__n_error_40: {
     state->error = 0x8;
     state->reason = "Invalid method for RTSP/x.x request";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14492,15 +15256,15 @@
       case 43:
         goto s_n_llhttp__internal__n_req_http_major;
       case 44:
         goto s_n_llhttp__internal__n_req_http_major;
       case 45:
         goto s_n_llhttp__internal__n_req_http_major;
       default:
-        goto s_n_llhttp__internal__n_error_31;
+        goto s_n_llhttp__internal__n_error_40;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_llhttp__on_url_complete_1: {
     switch (llhttp__on_url_complete(state, p, endp)) {
       default:
@@ -14573,15 +15337,15 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_33: {
+  s_n_llhttp__internal__n_error_42: {
     state->error = 0x7;
     state->reason = "Invalid char in url fragment start";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14633,24 +15397,24 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_34: {
+  s_n_llhttp__internal__n_error_43: {
     state->error = 0x7;
     state->reason = "Invalid char in url query";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_35: {
+  s_n_llhttp__internal__n_error_44: {
     state->error = 0x7;
     state->reason = "Invalid char in url path";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14753,60 +15517,60 @@
       state->_current = (void*) (intptr_t) s_n_llhttp__internal__n_url_skip_to_http;
       return s_error;
     }
     goto s_n_llhttp__internal__n_url_skip_to_http;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_36: {
+  s_n_llhttp__internal__n_error_45: {
     state->error = 0x7;
     state->reason = "Double @ in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_37: {
+  s_n_llhttp__internal__n_error_46: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_38: {
+  s_n_llhttp__internal__n_error_47: {
     state->error = 0x7;
     state->reason = "Unexpected char in url server";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_40: {
+  s_n_llhttp__internal__n_error_49: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_41: {
+  s_n_llhttp__internal__n_error_50: {
     state->error = 0x7;
     state->reason = "Unexpected char in url schema";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_42: {
+  s_n_llhttp__internal__n_error_51: {
     state->error = 0x7;
     state->reason = "Unexpected start char in url";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14817,15 +15581,15 @@
         goto s_n_llhttp__internal__n_span_start_llhttp__on_url_1;
       default:
         goto s_n_llhttp__internal__n_span_start_llhttp__on_url;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_43: {
+  s_n_llhttp__internal__n_error_52: {
     state->error = 0x6;
     state->reason = "Expected space after method";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14834,36 +15598,36 @@
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_req_first_space_before_url;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_51: {
+  s_n_llhttp__internal__n_error_64: {
     state->error = 0x6;
     state->reason = "Invalid method encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_44: {
+  s_n_llhttp__internal__n_error_55: {
     state->error = 0xd;
     state->reason = "Response overflow";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_invoke_mul_add_status_code: {
     switch (llhttp__internal__c_mul_add_status_code(state, p, endp, match)) {
       case 1:
-        goto s_n_llhttp__internal__n_error_44;
+        goto s_n_llhttp__internal__n_error_55;
       default:
         goto s_n_llhttp__internal__n_res_status_code;
     }
     /* UNREACHABLE */;
     abort();
   }
   s_n_llhttp__internal__n_span_end_llhttp__on_status: {
@@ -14898,15 +15662,15 @@
       return s_error;
     }
     p++;
     goto s_n_llhttp__internal__n_res_line_almost_done;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_45: {
+  s_n_llhttp__internal__n_error_56: {
     state->error = 0xd;
     state->reason = "Invalid response status";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14915,41 +15679,133 @@
     switch (llhttp__internal__c_update_status_code(state, p, endp)) {
       default:
         goto s_n_llhttp__internal__n_res_status_code;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_46: {
+  s_n_llhttp__internal__n_error_57: {
     state->error = 0x9;
     state->reason = "Expected space after version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
+  s_n_llhttp__internal__n_error_54: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_3: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 9:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_54;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_58: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_4: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_res_http_end;
+      case 1:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_58;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_59: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_minor_5: {
+    switch (llhttp__internal__c_load_http_minor(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_error_59;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_error_53: {
+    state->error = 0x9;
+    state->reason = "Invalid HTTP version";
+    state->error_pos = (const char*) p;
+    state->_current = (void*) (intptr_t) s_error;
+    return s_error;
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_load_http_major_1: {
+    switch (llhttp__internal__c_load_http_major(state, p, endp)) {
+      case 0:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_3;
+      case 1:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_4;
+      case 2:
+        goto s_n_llhttp__internal__n_invoke_load_http_minor_5;
+      default:
+        goto s_n_llhttp__internal__n_error_53;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
+  s_n_llhttp__internal__n_invoke_test_lenient_flags_10: {
+    switch (llhttp__internal__c_test_lenient_flags_9(state, p, endp)) {
+      case 1:
+        goto s_n_llhttp__internal__n_res_http_end;
+      default:
+        goto s_n_llhttp__internal__n_invoke_load_http_major_1;
+    }
+    /* UNREACHABLE */;
+    abort();
+  }
   s_n_llhttp__internal__n_invoke_store_http_minor_1: {
     switch (llhttp__internal__c_store_http_minor(state, p, endp, match)) {
       default:
-        goto s_n_llhttp__internal__n_res_http_end;
+        goto s_n_llhttp__internal__n_invoke_test_lenient_flags_10;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_47: {
+  s_n_llhttp__internal__n_error_60: {
     state->error = 0x9;
     state->reason = "Invalid minor version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_48: {
+  s_n_llhttp__internal__n_error_61: {
     state->error = 0x9;
     state->reason = "Expected dot";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14958,24 +15814,24 @@
     switch (llhttp__internal__c_store_http_major(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_res_http_dot;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_49: {
+  s_n_llhttp__internal__n_error_62: {
     state->error = 0x9;
     state->reason = "Invalid major version";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_52: {
+  s_n_llhttp__internal__n_error_65: {
     state->error = 0x8;
     state->reason = "Expected HTTP/";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
@@ -14992,15 +15848,15 @@
     switch (llhttp__internal__c_store_method(state, p, endp, match)) {
       default:
         goto s_n_llhttp__internal__n_invoke_update_type;
     }
     /* UNREACHABLE */;
     abort();
   }
-  s_n_llhttp__internal__n_error_50: {
+  s_n_llhttp__internal__n_error_63: {
     state->error = 0x8;
     state->reason = "Invalid word encountered";
     state->error_pos = (const char*) p;
     state->_current = (void*) (intptr_t) s_error;
     return s_error;
     /* UNREACHABLE */;
     abort();
```

### Comparing `geventhttpclient-2.0b1/ext/llhttp.h` & `geventhttpclient-2.1.0/llhttp/include/llhttp.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #ifndef INCLUDE_LLHTTP_H_
 #define INCLUDE_LLHTTP_H_
 
 #define LLHTTP_VERSION_MAJOR 6
 #define LLHTTP_VERSION_MINOR 0
-#define LLHTTP_VERSION_PATCH 6
+#define LLHTTP_VERSION_PATCH 11
 
 #ifndef LLHTTP_STRICT_MODE
 # define LLHTTP_STRICT_MODE 0
 #endif
 
 #ifndef INCLUDE_LLHTTP_ITSELF_H_
 #define INCLUDE_LLHTTP_ITSELF_H_
@@ -55,14 +55,15 @@
 extern "C" {
 #endif
 
 enum llhttp_errno {
   HPE_OK = 0,
   HPE_INTERNAL = 1,
   HPE_STRICT = 2,
+  HPE_CR_EXPECTED = 25,
   HPE_LF_EXPECTED = 3,
   HPE_UNEXPECTED_CONTENT_LENGTH = 4,
   HPE_CLOSED_CONNECTION = 5,
   HPE_INVALID_METHOD = 6,
   HPE_INVALID_URL = 7,
   HPE_INVALID_CONSTANT = 8,
   HPE_INVALID_VERSION = 9,
@@ -96,15 +97,17 @@
   F_TRANSFER_ENCODING = 0x200
 };
 typedef enum llhttp_flags llhttp_flags_t;
 
 enum llhttp_lenient_flags {
   LENIENT_HEADERS = 0x1,
   LENIENT_CHUNKED_LENGTH = 0x2,
-  LENIENT_KEEP_ALIVE = 0x4
+  LENIENT_KEEP_ALIVE = 0x4,
+  LENIENT_TRANSFER_ENCODING = 0x8,
+  LENIENT_VERSION = 0x10
 };
 typedef enum llhttp_lenient_flags llhttp_lenient_flags_t;
 
 enum llhttp_type {
   HTTP_BOTH = 0,
   HTTP_REQUEST = 1,
   HTTP_RESPONSE = 2
@@ -168,14 +171,15 @@
 };
 typedef enum llhttp_method llhttp_method_t;
 
 #define HTTP_ERRNO_MAP(XX) \
   XX(0, OK, OK) \
   XX(1, INTERNAL, INTERNAL) \
   XX(2, STRICT, STRICT) \
+  XX(25, CR_EXPECTED, CR_EXPECTED) \
   XX(3, LF_EXPECTED, LF_EXPECTED) \
   XX(4, UNEXPECTED_CONTENT_LENGTH, UNEXPECTED_CONTENT_LENGTH) \
   XX(5, CLOSED_CONNECTION, CLOSED_CONNECTION) \
   XX(6, INVALID_METHOD, INVALID_METHOD) \
   XX(7, INVALID_URL, INVALID_URL) \
   XX(8, INVALID_CONSTANT, INVALID_CONSTANT) \
   XX(9, INVALID_VERSION, INVALID_VERSION) \
@@ -370,16 +374,14 @@
  * the `parser` here. In practice, `settings` has to be either a static
  * variable or be allocated with `malloc`, `new`, etc.
  */
 LLHTTP_EXPORT
 void llhttp_init(llhttp_t* parser, llhttp_type_t type,
                  const llhttp_settings_t* settings);
 
-#if defined(__wasm__)
-
 LLHTTP_EXPORT
 llhttp_t* llhttp_alloc(llhttp_type_t type);
 
 LLHTTP_EXPORT
 void llhttp_free(llhttp_t* parser);
 
 LLHTTP_EXPORT
@@ -396,16 +398,14 @@
 
 LLHTTP_EXPORT
 int llhttp_get_status_code(llhttp_t* parser);
 
 LLHTTP_EXPORT
 uint8_t llhttp_get_upgrade(llhttp_t* parser);
 
-#endif  // defined(__wasm__)
-
 /* Reset an already initialized parser back to the start state, preserving the
  * existing parser type, callback settings, user data, and lenient flags.
  */
 LLHTTP_EXPORT
 void llhttp_reset(llhttp_t* parser);
 
 /* Initialize the settings object */
@@ -552,13 +552,26 @@
  * but might interact badly with outdated and insecure clients. With this flag
  * the extra request/response will be parsed normally.
  *
  * **(USE AT YOUR OWN RISK)**
  */
 void llhttp_set_lenient_keep_alive(llhttp_t* parser, int enabled);
 
+/* Enables/disables lenient handling of `Transfer-Encoding` header.
+ *
+ * Normally `llhttp` would error when a `Transfer-Encoding` has `chunked` value
+ * and another value after it (either in a single header or in multiple
+ * headers whose value are internally joined using `, `).
+ * This is mandated by the spec to reliably determine request body size and thus
+ * avoid request smuggling.
+ * With this flag the extra value will be parsed normally.
+ *
+ * **(USE AT YOUR OWN RISK)**
+ */
+void llhttp_set_lenient_transfer_encoding(llhttp_t* parser, int enabled);
+
 #ifdef __cplusplus
 }  /* extern "C" */
 #endif
 #endif  /* INCLUDE_LLHTTP_API_H_ */
 
 #endif  /* INCLUDE_LLHTTP_H_ */
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/client.py` & `geventhttpclient-2.1.0/src/geventhttpclient/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import errno
 import os
 
 import gevent.socket
-import six
 
 from geventhttpclient import __version__
 from geventhttpclient.connectionpool import ConnectionPool
 from geventhttpclient.header import Headers
-from geventhttpclient.response import HTTPConnectionClosed
-from geventhttpclient.response import HTTPSocketPoolResponse
+from geventhttpclient.response import HTTPConnectionClosed, HTTPSocketPoolResponse
 from geventhttpclient.url import URL
 
 CRLF = "\r\n"
 WHITESPACE = " "
 FIELD_VALUE_SEP = ": "
 HOST_PORT_SEP = ":"
 SLASH = "/"
@@ -44,96 +42,107 @@
     except TypeError:
         try:
             return os.fstat(body.fileno()).st_size
         except (AttributeError, OSError):
             return None
 
 
-class HTTPClient(object):
-    HTTP_11 = 'HTTP/1.1'
-    HTTP_10 = 'HTTP/1.0'
+class HTTPClient:
+    HTTP_11 = "HTTP/1.1"
+    HTTP_10 = "HTTP/1.0"
 
     BLOCK_SIZE = 1024 * 4  # 4KB
 
-    DEFAULT_HEADERS = Headers({
-        'User-Agent': 'python/gevent-http-client-' + __version__
-    })
+    DEFAULT_HEADERS = Headers({"User-Agent": "python/gevent-http-client-" + __version__})
 
     @classmethod
     def from_url(cls, url, **kw):
         if not isinstance(url, URL):
             url = URL(url)
         enable_ssl = url.scheme == PROTO_HTTPS
         if not enable_ssl:
-            kw.pop('ssl_options', None)
+            kw.pop("ssl_options", None)
         return cls(url.host, port=url.port, ssl=enable_ssl, **kw)
 
-    def __init__(self, host, port=None, headers=None,
-                 block_size=BLOCK_SIZE,
-                 connection_timeout=ConnectionPool.DEFAULT_CONNECTION_TIMEOUT,
-                 network_timeout=ConnectionPool.DEFAULT_NETWORK_TIMEOUT,
-                 disable_ipv6=False,
-                 concurrency=1,
-                 ssl=False, ssl_options=None, ssl_context_factory=None,
-                 insecure=False,
-                 proxy_host=None, proxy_port=None, version=HTTP_11,
-                 headers_type=Headers):
+    def __init__(
+        self,
+        host,
+        port=None,
+        headers=None,
+        block_size=BLOCK_SIZE,
+        connection_timeout=ConnectionPool.DEFAULT_CONNECTION_TIMEOUT,
+        network_timeout=ConnectionPool.DEFAULT_NETWORK_TIMEOUT,
+        disable_ipv6=False,
+        concurrency=1,
+        ssl=False,
+        ssl_options=None,
+        ssl_context_factory=None,
+        insecure=False,
+        proxy_host=None,
+        proxy_port=None,
+        version=HTTP_11,
+        headers_type=Headers,
+    ):
         if headers is None:
             headers = {}
         self.host = host
         self.port = port
         connection_host = self.host
         connection_port = self.port
         if proxy_host is not None:
-            assert proxy_port is not None, \
-                'you have to provide proxy_port if you set proxy_host'
+            assert proxy_port is not None, "you have to provide proxy_port if you set proxy_host"
             self.use_proxy = True
             connection_host = proxy_host
             connection_port = proxy_port
         else:
             self.use_proxy = False
         if ssl:
             ssl_options = ssl_options.copy() if ssl_options else {}
         if ssl_options is not None:
             if ssl_context_factory is not None:
-                requested_hostname = headers.get('host', self.host)
-                ssl_options.setdefault('server_hostname', requested_hostname)
+                requested_hostname = headers.get("host", self.host)
+                ssl_options.setdefault("server_hostname", requested_hostname)
             self.ssl = True
             if not self.port:
                 self.port = 443
             if not connection_port:
                 connection_port = self.port
             # Import SSL as late as possible, fail hard with Import Error
             from geventhttpclient.connectionpool import SSLConnectionPool
+
             self._connection_pool = SSLConnectionPool(
-                connection_host, connection_port,
-                self.host, self.port,
+                connection_host,
+                connection_port,
+                self.host,
+                self.port,
                 size=concurrency,
                 ssl_options=ssl_options,
                 ssl_context_factory=ssl_context_factory,
                 insecure=insecure,
                 network_timeout=network_timeout,
                 connection_timeout=connection_timeout,
                 disable_ipv6=disable_ipv6,
-                use_proxy=self.use_proxy
+                use_proxy=self.use_proxy,
             )
         else:
             self.ssl = False
             if not self.port:
                 self.port = 80
             if not connection_port:
                 connection_port = self.port
             self._connection_pool = ConnectionPool(
-                connection_host, connection_port,
-                self.host, self.port,
+                connection_host,
+                connection_port,
+                self.host,
+                self.port,
                 size=concurrency,
                 network_timeout=network_timeout,
                 connection_timeout=connection_timeout,
                 disable_ipv6=disable_ipv6,
-                use_proxy=self.use_proxy
+                use_proxy=self.use_proxy,
             )
         self.version = version
         self.headers_type = headers_type
         self.default_headers = headers_type()
         self.default_headers.update(self.DEFAULT_HEADERS)
         self.default_headers.update(headers)
         self.block_size = block_size
@@ -152,33 +161,36 @@
     # Like urllib2, try to treat the body as a file if we can't determine the
     # file length with `len()`
 
     def _build_request(self, method, request_uri, body="", headers=None):
         """
 
         :param method:
-        :type method: basestring
+        :type method: str or bytes
         :param request_uri:
-        :type request_uri: basestring
+        :type request_uri: str or bytes
         :param body:
-        :type body: basestring or file
+        :type body: str or bytes or file
         :param headers:
         :type headers: dict
         :return:
-        :rtype: basestring
+        :rtype: str or bytes
         """
 
         if headers is None:
             headers = {}
 
         header_fields = self.headers_type()
         header_fields.update(self.default_headers)
         header_fields.update(headers)
         if self.version == self.HTTP_11 and HEADER_HOST not in header_fields:
             host_port = self.host
+            # IPv6 addresses require square brackets in the Host header.
+            if ":" in self.host and self.host[0] != "[" and self.host[-1] != "]":
+                host_port = "[" + host_port + "]"
             if self.port not in (80, 443):
                 host_port += HOST_PORT_SEP + str(self.port)
             header_fields[HEADER_HOST] = host_port
         if body and HEADER_CONTENT_LENGTH not in header_fields:
             body_length = _get_body_length(body)
             if body_length:
                 header_fields[HEADER_CONTENT_LENGTH] = body_length
@@ -189,15 +201,15 @@
             if request_uri.startswith(SLASH):
                 base_url = base_url[:-1]
             request_url = base_url + request_url
         elif not request_url.startswith((SLASH, PROTO_HTTP)):
             request_url = SLASH + request_url
         elif request_url.startswith(PROTO_HTTP):
             if request_url.startswith(self._base_url_string):
-                request_url = request_url[len(self._base_url_string) - 1:]
+                request_url = request_url[len(self._base_url_string) - 1 :]
             else:
                 raise ValueError("Invalid host in URL")
 
         request = method + WHITESPACE + request_url + WHITESPACE + self.version + CRLF
 
         for field, value in header_fields.items():
             request += field + FIELD_VALUE_SEP + str(value) + CRLF
@@ -210,52 +222,49 @@
         :param method:
         :param request_uri:
         :param body: byte or file
         :param headers:
         :return:
         """
 
-        if isinstance(body, six.text_type):
-            body = body.encode('utf-8')
+        if isinstance(body, str):
+            body = body.encode("utf-8")
 
-        request = self._build_request(
-            method.upper(), request_uri, body=body, headers=headers)
+        request = self._build_request(method.upper(), request_uri, body=body, headers=headers)
 
         attempts_left = self._connection_pool.size + 1
 
         while 1:
             sock = self._connection_pool.get_socket()
             try:
                 _request = request.encode()
                 if body:
-                    if isinstance(body, six.binary_type):
+                    if isinstance(body, bytes):
                         sock.sendall(_request + body)
                     else:
                         sock.sendall(_request)
                         # TODO: Support non file-like iterables, e.g. `(u"string1", u"string2")`.
-                        if six.PY3:
-                            sock.sendfile(body)
-                        else:
-                            while True:
-                                chunk = body.read(65536)
-                                if not chunk:
-                                    break
-                                sock.sendall(chunk)
+                        sock.sendfile(body)
                 else:
                     sock.sendall(_request)
             except gevent.socket.error as e:
                 self._connection_pool.release_socket(sock)
                 if (e.errno == errno.ECONNRESET or e.errno == errno.EPIPE) and attempts_left > 0:
                     attempts_left -= 1
                     continue
                 raise e
 
             try:
-                response = HTTPSocketPoolResponse(sock, self._connection_pool,
-                                                  block_size=self.block_size, method=method.upper(), headers_type=self.headers_type)
+                response = HTTPSocketPoolResponse(
+                    sock,
+                    self._connection_pool,
+                    block_size=self.block_size,
+                    method=method.upper(),
+                    headers_type=self.headers_type,
+                )
             except HTTPConnectionClosed as e:
                 # connection is released by the response itself
                 if attempts_left > 0:
                     attempts_left -= 1
                     continue
                 raise e
             else:
@@ -264,35 +273,35 @@
 
     def get(self, request_uri, headers={}):
         return self.request(METHOD_GET, request_uri, headers=headers)
 
     def head(self, request_uri, headers=None):
         return self.request(METHOD_HEAD, request_uri, headers=headers)
 
-    def post(self, request_uri, body=u'', headers=None):
+    def post(self, request_uri, body="", headers=None):
         return self.request(METHOD_POST, request_uri, body=body, headers=headers)
 
-    def put(self, request_uri, body=u'', headers=None):
+    def put(self, request_uri, body="", headers=None):
         return self.request(METHOD_PUT, request_uri, body=body, headers=headers)
 
-    def delete(self, request_uri, body=u'', headers=None):
+    def delete(self, request_uri, body="", headers=None):
         return self.request(METHOD_DELETE, request_uri, body=body, headers=headers)
 
-    def patch(self, request_uri, body=u'', headers=None):
+    def patch(self, request_uri, body="", headers=None):
         return self.request(METHOD_PATCH, request_uri, body=body, headers=headers)
 
-    def trace(self, request_uri, body=u'', headers=None):
+    def trace(self, request_uri, body="", headers=None):
         return self.request(METHOD_TRACE, request_uri, body=body, headers=headers)
 
     def options(self, request_uri, headers=None):
         return self.request(METHOD_OPTIONS, request_uri, headers=headers)
 
 
-class HTTPClientPool(object):
-    """ Factory for maintaining a bunch of clients, one per host:port """
+class HTTPClientPool:
+    """Factory for maintaining a bunch of clients, one per host:port"""
 
     # TODO: Add some housekeeping and cleanup logic
 
     def __init__(self, **kwargs):
         self.clients = dict()
         self.client_args = kwargs
 
@@ -306,7 +315,8 @@
             client = HTTPClient.from_url(url, **self.client_args)
             self.clients[client_key] = client
             return client
 
     def close(self):
         for client in self.clients.values():
             client.close()
+        self.clients.clear()
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/connectionpool.py` & `geventhttpclient-2.1.0/src/geventhttpclient/connectionpool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,57 @@
+import os
+
 import gevent.queue
 import gevent.socket
-import os
-import six
+from gevent import lock
 
 _CA_CERTS = None
 
 try:
     from ssl import get_default_verify_paths
 except ImportError:
     _CA_CERTS = None
 else:
     _certs = get_default_verify_paths()
     _CA_CERTS = _certs.cafile or _certs.capath
 
 if not _CA_CERTS or os.path.isdir(_CA_CERTS):
     import certifi
+
     _CA_CERTS = certifi.where()
 
-try:
-    from ssl import _DEFAULT_CIPHERS
-except ImportError:
-    # ssl._DEFAULT_CIPHERS in python2.7 branch.
-    _DEFAULT_CIPHERS = (
-        'ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:ECDH+HIGH:'
-        'DH+HIGH:ECDH+3DES:DH+3DES:RSA+AESGCM:RSA+AES:RSA+HIGH:RSA+3DES:ECDH+RC4:'
-        'DH+RC4:RSA+RC4:!aNULL:!eNULL:!MD5')
+_DEFAULT_CIPHERS = (
+    "ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:ECDH+HIGH:"
+    "DH+HIGH:ECDH+3DES:DH+3DES:RSA+AESGCM:RSA+AES:RSA+HIGH:RSA+3DES:ECDH+RC4:"
+    "DH+RC4:RSA+RC4:!aNULL:!eNULL:!MD5"
+)
 
-try:
-    from gevent import lock
-except ImportError:
-    # gevent < 1.0b2
-    from gevent import coros as lock
 
 DEFAULT_CONNECTION_TIMEOUT = 5.0
 DEFAULT_NETWORK_TIMEOUT = 5.0
 
 IGNORED = object()
 
 
-class ConnectionPool(object):
+class ConnectionPool:
     DEFAULT_CONNECTION_TIMEOUT = 5.0
     DEFAULT_NETWORK_TIMEOUT = 5.0
 
-    def __init__(self,
-                 connection_host,
-                 connection_port,
-                 request_host,
-                 request_port,
-                 size=5, disable_ipv6=False,
-                 connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
-                 network_timeout=DEFAULT_NETWORK_TIMEOUT,
-                 use_proxy=False):
+    def __init__(
+        self,
+        connection_host,
+        connection_port,
+        request_host,
+        request_port,
+        size=5,
+        disable_ipv6=False,
+        connection_timeout=DEFAULT_CONNECTION_TIMEOUT,
+        network_timeout=DEFAULT_NETWORK_TIMEOUT,
+        use_proxy=False,
+    ):
         self._closed = False
         self._connection_host = connection_host
         self._connection_port = connection_port
         self._request_host = request_host
         self._request_port = request_port
         self._semaphore = lock.BoundedSemaphore(size)
         self._socket_queue = gevent.queue.LifoQueue(size)
@@ -62,22 +59,25 @@
 
         self.connection_timeout = connection_timeout
         self.network_timeout = network_timeout
         self.size = size
         self.disable_ipv6 = disable_ipv6
 
     def _resolve(self):
-        """ resolve (dns) socket informations needed to connect it.
-        """
+        """resolve (dns) socket informations needed to connect it."""
         family = 0
         if self.disable_ipv6:
             family = gevent.socket.AF_INET
-        info = gevent.socket.getaddrinfo(self._connection_host,
-                                         self._connection_port,
-                                         family, 0, gevent.socket.SOL_TCP)
+        info = gevent.socket.getaddrinfo(
+            self._connection_host,
+            self._connection_port,
+            family,
+            0,
+            gevent.socket.SOL_TCP,
+        )
         # family, socktype, proto, canonname, sockaddr = info[0]
         return info
 
     def close(self):
         self._closed = True
         while not self._socket_queue.empty():
             try:
@@ -86,22 +86,21 @@
                     sock.close()
                 except:
                     pass
             except gevent.queue.Empty:
                 pass
 
     def _create_tcp_socket(self, family, socktype, protocol):
-        """ tcp socket factory.
-        """
+        """tcp socket factory."""
         sock = gevent.socket.socket(family, socktype, protocol)
         return sock
 
     def _create_socket(self):
-        """ might be overridden and super for wrapping into a ssl socket
-            or set tcp/socket options
+        """might be overridden and super for wrapping into a ssl socket
+        or set tcp/socket options
         """
         sock_infos = self._resolve()
         first_error = None
         for sock_info in sock_infos:
             try:
                 sock = self._create_tcp_socket(*sock_info[:3])
             except Exception as e:
@@ -111,141 +110,144 @@
 
             try:
                 sock.settimeout(self.connection_timeout)
                 sock = self._connect_socket(sock, sock_info[-1])
                 self.after_connect(sock)
                 sock.settimeout(self.network_timeout)
                 return sock
-            except IOError as e:
+            except OSError as e:
                 sock.close()
                 if not first_error:
                     first_error = e
             except:
                 sock.close()
                 raise
 
         if first_error:
             raise first_error
         else:
-            raise RuntimeError(
-                "Cannot resolve %s:%s" % (self._host, self._port))
+            raise RuntimeError(f"Cannot resolve {self._host}:{self._port}")
 
     def after_connect(self, sock):
         pass
 
     def _connect_socket(self, sock, address):
         sock.connect(address)
         self._setup_proxy(sock)
         return sock
 
     def _setup_proxy(self, sock):
         if self._use_proxy:
             sock.send(
-                six.binary_type(
-                    "CONNECT {self._request_host}:{self._request_port} "
-                    "HTTP/1.1\r\n\r\n".format(self=self),
-                    'utf8'
+                bytes(
+                    f"CONNECT {self._request_host}:{self._request_port} HTTP/1.1\r\n\r\n",
+                    "utf8",
                 )
             )
 
             resp = sock.recv(4096)
             parts = resp.split()
             if not parts or parts[1] != b"200":
-                raise RuntimeError(
-                    "Error response from Proxy server : %s" % resp)
+                raise RuntimeError(f"Error response from Proxy server : {resp}")
 
     def get_socket(self):
-        """ get a socket from the pool. This blocks until one is available.
-        """
+        """get a socket from the pool. This blocks until one is available."""
         self._semaphore.acquire()
         if self._closed:
-            raise RuntimeError('connection pool closed')
+            raise RuntimeError("connection pool closed")
         try:
             return self._socket_queue.get(block=False)
         except gevent.queue.Empty:
             try:
                 return self._create_socket()
             except:
                 self._semaphore.release()
                 raise
 
     def return_socket(self, sock):
-        """ return a socket to the pool.
-        """
+        """return a socket to the pool."""
         if self._closed:
             try:
                 sock.close()
             except:
                 pass
             return
         self._socket_queue.put(sock)
         self._semaphore.release()
 
     def release_socket(self, sock):
-        """ call when the socket is no more usable.
-        """
+        """call when the socket is no more usable."""
         try:
             sock.close()
         except:
             pass
         if not self._closed:
             self._semaphore.release()
 
 
 try:
     import gevent.ssl
-
     try:
-        from gevent.ssl import match_hostname
+        from gevent.ssl import create_default_context
     except ImportError:
-        from backports.ssl_match_hostname import match_hostname
+        create_default_context = None
 except ImportError:
     pass
 else:
+
     class SSLConnectionPool(ConnectionPool):
-        """ SSLConnectionPool creates connections wrapped with SSL/TLS.
+        """SSLConnectionPool creates connections wrapped with SSL/TLS.
 
         :param host: hostname
         :param port: port
         :param ssl_options: accepts any options supported by `ssl.wrap_socket`
         :param ssl_context_factory: use `ssl.create_default_context` by default
             if provided. It must be a callable that returns a SSLContext.
         """
 
         default_options = {
-            'ciphers': _DEFAULT_CIPHERS,
-            'ca_certs': _CA_CERTS,
-            'cert_reqs': gevent.ssl.CERT_REQUIRED
+            "ciphers": _DEFAULT_CIPHERS,
+            "ca_certs": _CA_CERTS,
+            "cert_reqs": gevent.ssl.CERT_REQUIRED,
         }
 
-        ssl_context_factory = getattr(gevent.ssl, "create_default_context",
-                                      None)
+        def __init__(
+            self,
+            connection_host,
+            connection_port,
+            request_host,
+            request_port,
+            insecure=False,
+            ssl_context_factory=None,
+            ssl_options=None,
+            **kw,
+        ):
+            self.insecure = insecure
+
+            self.ssl_options = self.default_options.copy()
+            self.ssl_options.update(ssl_options or {})
+
+            ssl_context_factory = ssl_context_factory or create_default_context
+            if ssl_context_factory is not None:
+                self.init_ssl_context(ssl_context_factory)
+            else:
+                self.ssl_context = None
+
+            super().__init__(connection_host, connection_port, request_host, request_port, **kw)
 
-        def __init__(self,
-                     connection_host,
-                     connection_port,
-                     request_host,
-                     request_port, **kw):
-            self.ssl_options = kw.pop("ssl_options", {})
-            self.ssl_context_factory = kw.pop('ssl_context_factory', None)
-            self.insecure = kw.pop('insecure', False)
-            super(SSLConnectionPool, self).__init__(connection_host,
-                                                    connection_port,
-                                                    request_host,
-                                                    request_port,
-                                                    **kw)
-
-        def after_connect(self, sock):
-            super(SSLConnectionPool, self).after_connect(sock)
-            if not self.insecure:
-                match_hostname(sock.getpeercert(), self._request_host)
+        def init_ssl_context(self, ssl_context_factory):
+            ca_certs = self.ssl_options["ca_certs"]
+            try:
+                self.ssl_context = ssl_context_factory(cafile=ca_certs)
+            except TypeError:
+                self.ssl_context = ssl_context_factory()
+                self.ssl_context.load_verify_locations(cafile=ca_certs)
+            self.ssl_context.check_hostname = not self.insecure
 
         def _connect_socket(self, sock, address):
-            sock = super(SSLConnectionPool, self)._connect_socket(sock, address)
+            sock = super()._connect_socket(sock, address)
 
-            if self.ssl_context_factory is None:
-                ssl_options = self.default_options.copy()
-                ssl_options.update(self.ssl_options)
-                return gevent.ssl.wrap_socket(sock, **ssl_options)
+            if self.ssl_context is None:
+                return gevent.ssl.wrap_socket(sock, **self.ssl_options)
             else:
-                return self.ssl_context_factory().wrap_socket(sock,
-                                                              **self.ssl_options)
+                server_hostname = self.ssl_options.get("server_hostname", self._request_host)
+                return self.ssl_context.wrap_socket(sock, server_hostname=server_hostname)
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/header.py` & `geventhttpclient-2.1.0/src/geventhttpclient/header.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-import six
-
-if six.PY3:
-    from collections.abc import Mapping, MutableMapping
-else:
-    from collections import Mapping, MutableMapping
+from collections.abc import Mapping, MutableMapping
 
 _dict_setitem = dict.__setitem__
 _dict_getitem = dict.__getitem__
 _dict_delitem = dict.__delitem__
 _dict_contains = dict.__contains__
 _dict_setdefault = dict.setdefault
 
@@ -71,39 +66,34 @@
     def __delitem__(self, key):
         return _dict_delitem(self, key.lower())
 
     def __contains__(self, key):
         return _dict_contains(self, key.lower())
 
     def __eq__(self, other):
-        if not isinstance(other, Mapping) and not hasattr(other, 'keys'):
+        if not isinstance(other, Mapping) and not hasattr(other, "keys"):
             return False
         if not isinstance(other, type(self)):
             other = type(self)(other)
-        return dict((k1, self[k1]) for k1 in self) == dict((k2, other[k2]) for k2 in other)
+        return {k1: self[k1] for k1 in self} == {k2: other[k2] for k2 in other}
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     values = MutableMapping.values
     get = MutableMapping.get
     update = MutableMapping.update
-    if six.PY3:
-        keys = MutableMapping.keys
-    else:
-        iterkeys = MutableMapping.iterkeys
-    if six.PY2:
-        itervalues = MutableMapping.itervalues
+    keys = MutableMapping.keys
 
     __marker = object()
 
     def pop(self, key, default=__marker):
-        '''D.pop(k[,d]) -> v, remove specified key and return the corresponding value.
-          If key is not found, d is returned if given, otherwise KeyError is raised.
-        '''
+        """D.pop(k[,d]) -> v, remove specified key and return the corresponding value.
+        If key is not found, d is returned if given, otherwise KeyError is raised.
+        """
         # Using the MutableMapping function directly fails due to the private marker.
         # Using ordinary dict.pop would expose the internal structures.
         # So let's reinvent the wheel.
         try:
             value = self[key]
         except KeyError:
             if default is self.__marker:
@@ -144,20 +134,19 @@
 
     def extend(self, *args, **kwargs):
         """Generic import function for any type of header-like object.
         Adapted version of MutableMapping.update in order to insert items
         with self.add instead of self.__setitem__
         """
         if len(args) > 1:
-            raise TypeError("extend() takes at most 1 positional "
-                            "arguments ({} given)".format(len(args)))
+            raise TypeError(f"extend() takes at most 1 positional argument ({len(args)} given)")
         other = args[0] if len(args) >= 1 else ()
 
         if isinstance(other, Headers):
-            for key, val in other.iteritems():
+            for key, val in other.items():
                 self.add(key, val)
         elif isinstance(other, Mapping):
             for key in other:
                 self.add(key, other[key])
         elif hasattr(other, "keys"):
             for key in other.keys():
                 self.add(key, other[key])
@@ -189,17 +178,16 @@
     # Python3 compatibility
     def get_all(self, key, failobj=None):
         vals = self.getlist(key)
         if not vals:
             return failobj
         return vals
 
-
     def __repr__(self):
-        return "%s(%s)" % (type(self).__name__, dict(self.itermerged()))
+        return f"{type(self).__name__}({dict(self.itermerged())})"
 
     def _copy_from(self, other):
         for key in other:
             val = _dict_getitem(other, key)
             if isinstance(val, list):
                 # Don't need to convert tuples
                 val = list(val)
@@ -211,15 +199,15 @@
         return clone
 
     def itermerged(self):
         """Iterate over all headers, merging duplicate ones together."""
         for key in self:
             val = _dict_getitem(self, key)
             # this should preserve either binary or string type
-            sep = u', ' if isinstance(val[1], six.string_types) else b', '
+            sep = ", " if isinstance(val[1], str) else b", "
             yield val[0], sep.join(val[1:])
 
     # Extensions to urllib3, compatibility to previous implementation
     def __len__(self):
         return sum(len(self.getlist(key)) for key in self)
 
     def compatible_dict(self):
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/httplib.py` & `geventhttpclient-2.1.0/src/geventhttpclient/httplib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,46 @@
-import six
-if six.PY3:
-    httplib = __import__('http.client').client
-else:
-    httplib = __import__('httplib')
-from geventhttpclient import response
-from geventhttpclient import header
+import http.client as httplib
+
 import gevent.socket
 
+from geventhttpclient import header, response
 
 
 class HTTPLibHeaders(header.Headers):
-
     def __getitem__(self, key):
-        value = super(HTTPLibHeaders, self).__getitem__(key)
+        value = super().__getitem__(key)
         if isinstance(value, (list, tuple)):
             return ", ".join(value)
         else:
             return value
 
 
 class HTTPResponse(response.HTTPSocketResponse):
-
-    def __init__(self, sock, method='GET', strict=0, debuglevel=0,
-            buffering=False, **kw):
+    def __init__(self, sock, method="GET", strict=0, debuglevel=0, buffering=False, **kw):
         if method is None:
-            method = 'GET'
+            method = "GET"
         else:
             method = method.upper()
-        super(HTTPResponse, self).__init__(sock, method=method, **kw)
+        super().__init__(sock, method=method, **kw)
 
     @property
     def msg(self):
-        if hasattr(self, '_msg'):
+        if hasattr(self, "_msg"):
             return self._msg
         self._msg = HTTPLibHeaders(self._headers_index)
         return self._msg
 
     @property
     def fp(self):
         return self
 
     @property
     def version(self):
         v = self.get_http_version()
-        if v == 'HTTP/1.1':
+        if v == "HTTP/1.1":
             return 11
         return 10
 
     @property
     def status(self):
         return self.status_code
 
@@ -64,15 +57,15 @@
     def close(self):
         self.release()
 
     def isclosed(self):
         return self._sock is None
 
     def read(self, amt=None):
-        return super(HTTPResponse, self).read(amt)
+        return super().read(amt)
 
     def getheader(self, name, default=None):
         return self.get(name.lower(), default)
 
     def getheaders(self):
         return self._headers_index.items()
 
@@ -84,58 +77,57 @@
         return not self.should_keep_alive()
 
 
 HTTPLibConnection = httplib.HTTPConnection
 
 
 class HTTPConnection(httplib.HTTPConnection):
-
     response_class = HTTPResponse
 
     def __init__(self, *args, **kw):
         HTTPLibConnection.__init__(self, *args, **kw)
         # python 2.6 compat
         if not hasattr(self, "source_address"):
             self.source_address = None
 
     def connect(self):
         self.sock = gevent.socket.create_connection(
-            (self.host,self.port),
-            self.timeout, self.source_address)
+            (self.host, self.port), self.timeout, self.source_address
+        )
 
         if self._tunnel_host:
             self._tunnel()
 
+
 try:
     import gevent.ssl
 except:
     pass
 else:
-    class HTTPSConnection(HTTPConnection):
 
+    class HTTPSConnection(HTTPConnection):
         default_port = 443
 
         def __init__(self, host, port=None, key_file=None, cert_file=None, **kw):
             HTTPConnection.__init__(self, host, port, **kw)
             self.key_file = key_file
             self.cert_file = cert_file
 
         def connect(self):
             "Connect to a host on a given (SSL) port."
 
-            sock = gevent.socket.create_connection((self.host, self.port),
-                                            self.timeout, self.source_address)
+            sock = gevent.socket.create_connection(
+                (self.host, self.port), self.timeout, self.source_address
+            )
             if self._tunnel_host:
                 self.sock = sock
                 self._tunnel()
-            self.sock = gevent.ssl.wrap_socket(
-                sock, self.key_file, self.cert_file)
+            self.sock = gevent.ssl.wrap_socket(sock, self.key_file, self.cert_file)
 
 
 def patch():
     httplib.HTTPConnection = HTTPConnection
     httplib.HTTPResponse = HTTPResponse
     try:
         httplib.HTTPSConnection = HTTPSConnection
     except NameError:
         pass
-
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/response.py` & `geventhttpclient-2.1.0/src/geventhttpclient/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-import six
 import errno
-from geventhttpclient._parser import HTTPResponseParser
-from geventhttpclient._parser import HTTPParseError
-from geventhttpclient.header import Headers
+
 import gevent.socket
 
+from geventhttpclient._parser import HTTPParseError, HTTPResponseParser
+from geventhttpclient.header import Headers
 
 HEADER_STATE_INIT = 0
 HEADER_STATE_FIELD = 1
 HEADER_STATE_VALUE = 2
 HEADER_STATE_DONE = 3
 
 
 def copy(data):
-    if six.PY3:
-        return data[:]
-    else:
-        return str(data)
+    return data[:]
 
 
 class HTTPConnectionClosed(HTTPParseError):
     pass
 
 
 class HTTPProtocolViolationError(HTTPParseError):
     pass
 
 
 class HTTPResponse(HTTPResponseParser):
-
-    def __init__(self, method='GET', headers_type=Headers):
-        super(HTTPResponse, self).__init__()
+    def __init__(self, method="GET", headers_type=Headers):
+        super().__init__()
         self.method = method.upper()
         self.headers_complete = False
         self.message_begun = False
         self.message_complete = False
         self._headers_index = headers_type()
         self._header_state = HEADER_STATE_INIT
         self._current_header_field = None
@@ -45,79 +40,70 @@
 
     def __getitem__(self, key):
         return self._headers_index[key]
 
     def get(self, key, default=None):
         return self._headers_index.get(key, default)
 
-    def iteritems(self):
-        return self._headers_index.iteritems()
-
     def items(self):
         return self._headers_index.items()
 
     def info(self):
-        """ Basic cookielib compatibility """
+        """Basic cookielib compatibility"""
         return self._headers_index
 
     def should_close(self):
-        """ return if we should close the connection.
+        """return if we should close the connection.
 
         It is not the opposite of should_keep_alive method. It also checks
         that the body as been consumed completely.
         """
-        return not self.message_complete or \
-               self.parser_failed() or \
-               not super(HTTPResponse, self).should_keep_alive()
+        return not self.message_complete or self.parser_failed() or not super().should_keep_alive()
 
     headers = property(items)
 
     def __contains__(self, key):
         return key in self._headers_index
 
     @property
     def status_code(self):
         return self.get_code()
 
     @property
     def content_length(self):
-        length = self.get('content-length', None)
+        length = self.get("content-length", None)
         if length is not None:
-            if six.PY3:
-                return int(length)
-            else:
-                return long(length)
+            return int(length)
 
     @property
     def length(self):
-      return self.content_length
+        return self.content_length
 
     @property
     def version(self):
         return self.get_http_version()
 
     def _on_status(self, msg):
         self.status_message = msg
 
     def _on_message_begin(self):
         if self.message_begun:
-            raise HTTPProtocolViolationError(
-                "A new response began before end of %r." % self)
+            raise HTTPProtocolViolationError(f"A new response began before end of {self!r}.")
         self.message_begun = True
 
     def _on_message_complete(self):
         self.message_complete = True
 
     def _on_headers_complete(self):
         self._flush_header()
         self._header_state = HEADER_STATE_DONE
         self.headers_complete = True
 
-        if self.method == 'HEAD':
-            return True # SKIP BODY
+        if self.method == "HEAD":
+            return True  # SKIP BODY
         return False
 
     def _on_header_field(self, string):
         if self._header_state == HEADER_STATE_FIELD:
             self._current_header_field += string
         else:
             if self._header_state == HEADER_STATE_VALUE:
@@ -132,37 +118,31 @@
         else:
             self._current_header_value = string
 
         self._header_state = HEADER_STATE_VALUE
 
     def _flush_header(self):
         if self._current_header_field is not None:
-            self._headers_index.add(self._current_header_field,
-                                    self._current_header_value)
+            self._headers_index.add(self._current_header_field, self._current_header_value)
             self._header_position += 1
             self._current_header_field = None
             self._current_header_value = None
 
     def _on_body(self, buf):
         self._body_buffer += buf
 
     def __repr__(self):
-        return "<{klass} status={status} headers={headers}>".format(
-            klass=self.__class__.__name__,
-            status=self.status_code,
-            headers=dict(self.headers))
+        return f"<{self.__class__.__name__} status={self.status_code} headers={dict(self.headers)}>"
 
 
 class HTTPSocketResponse(HTTPResponse):
+    DEFAULT_BLOCK_SIZE = 1024 * 4  # 4KB
 
-    DEFAULT_BLOCK_SIZE = 1024 * 4 # 4KB
-
-    def __init__(self, sock, block_size=DEFAULT_BLOCK_SIZE,
-            method='GET', **kw):
-        super(HTTPSocketResponse, self).__init__(method=method, **kw)
+    def __init__(self, sock, block_size=DEFAULT_BLOCK_SIZE, method="GET", **kw):
+        super().__init__(method=method, **kw)
         self._sock = sock
         self.block_size = block_size
         self._read_headers()
 
     def release(self):
         try:
             if self._sock is not None and self.should_close():
@@ -182,24 +162,21 @@
             while not self.headers_complete:
                 try:
                     data = self._sock.recv(self.block_size)
                     self.feed(data)
                     # depending on gevent version we get a conn reset or no data
                     if not len(data) and not self.headers_complete:
                         if start:
-                            raise HTTPConnectionClosed(
-                                'connection closed.')
-                        raise HTTPParseError('connection closed before'
-                                            ' end of the headers')
+                            raise HTTPConnectionClosed("connection closed.")
+                        raise HTTPParseError("connection closed before end of the headers")
                     start = False
                 except gevent.socket.error as e:
                     if e.errno == errno.ECONNRESET:
                         if start:
-                            raise HTTPConnectionClosed(
-                                'connection closed.')
+                            raise HTTPConnectionClosed("connection closed.")
                     raise
 
             if self.message_complete:
                 self.release()
         except BaseException:
             self.release()
             raise
@@ -222,15 +199,15 @@
                     line = copy(self._body_buffer[:length])
                     del self._body_buffer[:length]
                     cursor = 0
                     return line
             else:
                 cursor = 0
             if self.message_complete:
-                return b''
+                return b""
             try:
                 data = self._sock.recv(self.block_size)
                 self.feed(data)
             except BaseException:
                 self.release()
                 raise
 
@@ -244,16 +221,17 @@
 
         if self._sock is None:
             read = copy(self._body_buffer)
             del self._body_buffer[:]
             return read
 
         try:
-            while not(self.message_complete) and (
-                    length is None or len(self._body_buffer) < length):
+            while not (self.message_complete) and (
+                length is None or len(self._body_buffer) < length
+            ):
                 data = self._sock.recv(length or self.block_size)
                 self.feed(data)
         except:
             self.release()
             raise
 
         if length is not None:
@@ -271,29 +249,28 @@
     def next(self):
         bytes = self.read(self.block_size)
         if not len(bytes):
             raise StopIteration()
         return bytes
 
     def _on_message_complete(self):
-        super(HTTPSocketResponse, self)._on_message_complete()
+        super()._on_message_complete()
         self.release()
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.release()
 
 
 class HTTPSocketPoolResponse(HTTPSocketResponse):
-
     def __init__(self, sock, pool, **kw):
         self._pool = pool
-        super(HTTPSocketPoolResponse, self).__init__(sock, **kw)
+        super().__init__(sock, **kw)
 
     def release(self):
         try:
             if self._sock is not None:
                 if self.should_close():
                     self._pool.release_socket(self._sock)
                 else:
@@ -301,8 +278,7 @@
         finally:
             self._sock = None
             self._pool = None
 
     def __del__(self):
         if self._sock is not None:
             self._pool.release_socket(self._sock)
-
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/oncert.pem` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/oncert.pem`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/server.crt` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/server.crt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/server.key` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/server.key`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_client.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,159 +1,114 @@
-import os
-import sys
-import tempfile
-import pytest
 import json
+import os
 from contextlib import contextmanager
-from geventhttpclient import HTTPClient
-from gevent.ssl import SSLError #@UnresolvedImport
-import gevent.pool
 
-import gevent.server
+import gevent.pool
 import gevent.pywsgi
-from six.moves import xrange
+import gevent.server
+import pytest
+from gevent.ssl import SSLError
+
+from geventhttpclient import HTTPClient, __version__
+
+LISTENER = "127.0.0.1", 54323
+HTTPBIN_HOST = "httpbin.org"  # this might be exchanged with a self-hosted version
 
-listener = ('127.0.0.1', 54323)
 
 @contextmanager
 def server(handler):
-    server = gevent.server.StreamServer(
-        listener,
-        handle=handler)
+    server = gevent.server.StreamServer(LISTENER, handle=handler)
     server.start()
     try:
         yield
     finally:
         server.stop()
 
+
 @contextmanager
 def wsgiserver(handler):
-    server = gevent.pywsgi.WSGIServer(('127.0.0.1', 54323), handler)
+    server = gevent.pywsgi.WSGIServer(LISTENER, handler)
     server.start()
     try:
         yield
     finally:
         server.stop()
 
-@pytest.mark.online
-def test_client_simple():
-    client = HTTPClient('httpbin.org')
-    assert client.port == 80
-    response = client.get('/')
-    assert response.status_code == 200
-    body = response.read()
-    assert len(body)
-
-@pytest.mark.online
-def test_client_without_leading_slash():
-    client = HTTPClient('httpbin.org')
-    with client.get("") as response:
-        assert response.status_code == 200
-    with client.get("base64/test") as response:
-        assert(response.status_code in (200, 301, 302))
-
-test_headers = {'User-Agent': 'Mozilla/5.0 (X11; U; Linux i686; de; rv:1.9.2.17) Gecko/20110422 Ubuntu/10.04 (lucid) Firefox/3.6.17'}
-@pytest.mark.online
-def test_client_with_default_headers():
-    client = HTTPClient.from_url('httpbin.org/', headers=test_headers)
-
-@pytest.mark.online
-def test_request_with_headers():
-    client = HTTPClient('httpbin.org')
-    response = client.get('/', headers=test_headers)
-    assert response.status_code == 200
 
-client = HTTPClient('www.heise.de')
-raw_req_cmp = client._build_request('GET', '/tp/')
+def httpbin_client(
+    host=HTTPBIN_HOST,
+    port=None,
+    headers=None,
+    block_size=HTTPClient.BLOCK_SIZE,
+    connection_timeout=30.0,
+    network_timeout=30.0,
+    disable_ipv6=True,
+    concurrency=1,
+    ssl=False,
+    ssl_options=None,
+    ssl_context_factory=None,
+    insecure=False,
+    proxy_host=None,
+    proxy_port=None,
+    version=HTTPClient.HTTP_11,
+):
+    """Client factory for httpbin with higher timeout values"""
+
+    return HTTPClient(
+        host,
+        port=port,
+        headers=headers,
+        block_size=block_size,
+        connection_timeout=connection_timeout,
+        network_timeout=network_timeout,
+        disable_ipv6=disable_ipv6,
+        concurrency=concurrency,
+        ssl=ssl,
+        ssl_options=ssl_options,
+        ssl_context_factory=ssl_context_factory,
+        insecure=insecure,
+        proxy_host=proxy_host,
+        proxy_port=proxy_port,
+        version=version,
+    )
+
+
+@pytest.fixture
+def httpbin():
+    return httpbin_client()
+
+
+@pytest.mark.parametrize("request_uri", ["/tp/", "tp/", f"http://{HTTPBIN_HOST}/tp/"])
+def test_build_request(httpbin, request_uri):
+    request_ref = f"GET /tp/ HTTP/1.1\r\nuser-agent: python/gevent-http-client-{__version__}\r\nhost: {HTTPBIN_HOST}\r\n\r\n"
+    assert httpbin._build_request("GET", request_uri) == request_ref
 
-@pytest.mark.online
-def test_build_request_relative_uri():
-    raw_req = client._build_request('GET', 'tp/')
-    assert raw_req == raw_req_cmp
-
-@pytest.mark.online
-def test_build_request_absolute_uri():
-    raw_req = client._build_request('GET', '/tp/')
-    assert raw_req == raw_req_cmp
-
-@pytest.mark.online
-def test_build_request_full_url():
-    raw_req = client._build_request('GET', 'http://www.heise.de/tp/')
-    assert raw_req == raw_req_cmp
 
-@pytest.mark.online
-def test_build_request_invalid_host():
+def test_build_request_invalid_host(httpbin):
     with pytest.raises(ValueError):
-        client._build_request('GET', 'http://www.spiegel.de/')
+        httpbin._build_request("GET", "http://someunrelatedhost.com/")
 
-@pytest.mark.online
-def test_response_context_manager():
-    client = HTTPClient.from_url('http://httpbin.org/')
-    r = None
-    with client.get('/') as response:
-        assert response.status_code == 200
-        r = response
-    assert r._sock is None # released
 
-@pytest.mark.skipif(
-    os.environ.get("TRAVIS") == "true",
-    reason="We have issues on travis with the SSL tests"
-)
-@pytest.mark.online
-def test_client_ssl():
-    client = HTTPClient('github.com', ssl=True)
-    assert client.port == 443
-    response = client.get('/')
-    assert response.status_code == 200
-    body = response.read()
-    assert len(body)
+test_url_client_args = [
+    ("http://python.org", ("python.org", 80)),
+    ("http://python.org:333", ("python.org", 333)),
+]
 
-@pytest.mark.skipif(
-    sys.version_info < (2, 7)
-    and os.environ.get("TRAVIS") == "true",
-    reason="We have issues on travis with the SSL tests"
-)
-@pytest.mark.online
-def test_ssl_fail_invalid_certificate():
-    certs = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)), "oncert.pem")
-    client = HTTPClient('github.com', ssl_options={'ca_certs': certs})
-    assert client.port == 443
-    with pytest.raises(SSLError) as e_info:
-        client.get('/')
-    assert e_info.value.reason == 'CERTIFICATE_VERIFY_FAILED'
 
-@pytest.mark.online
-def test_multi_queries_greenlet_safe():
-    client = HTTPClient('httpbin.org', concurrency=3)
-    group = gevent.pool.Group()
-    event = gevent.event.Event()
+@pytest.mark.parametrize(["url", "client_args"], test_url_client_args)
+def test_from_url(url, client_args):
+    from_url = HTTPClient.from_url(url)
+    from_args = HTTPClient(*client_args)
+    assert from_args.host == from_url.host
+    assert from_args.port == from_url.port
 
-    def run(i):
-        event.wait()
-        response = client.get('/')
-        return response, response.read()
-
-    count = 0
-
-    gevent.spawn_later(0.2, event.set)
-    for response, content in group.imap_unordered(run, xrange(5)):
-        assert response.status_code == 200
-        assert len(content)
-        count += 1
-    assert count == 5
-
-
-class StreamTestIterator(object):
 
+class StreamTestIterator:
     def __init__(self, sep, count):
-        lines = [json.dumps({
-                 'index': i,
-                 'title': 'this is line %d' % i})
-                 for i in xrange(0, count)]
+        lines = [json.dumps({"index": i, "title": f"this is line {i}"}) for i in range(0, count)]
         self.buf = (sep.join(lines) + sep).encode()
 
     def __len__(self):
         return len(self.buf)
 
     def __iter__(self):
         self.cursor = 0
@@ -161,15 +116,15 @@
 
     def next(self):
         if self.cursor >= len(self.buf):
             raise StopIteration()
 
         gevent.sleep(0)
         pos = self.cursor + 10
-        data = self.buf[self.cursor:pos]
+        data = self.buf[self.cursor : pos]
         self.cursor = pos
 
         return data
 
     def __next__(self):
         return self.next()
 
@@ -177,124 +132,237 @@
 def readline_iter(sock, addr):
     sock.recv(1024)
     iterator = StreamTestIterator("\n", 100)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n")
     for block in iterator:
         sock.sendall(block)
 
+
 def test_readline():
     with server(readline_iter):
-        client = HTTPClient(*listener, block_size=1)
-        response = client.get('/')
+        client = HTTPClient(*LISTENER, block_size=1)
+        response = client.get("/")
         lines = []
         while True:
             line = response.readline(b"\n")
             if not line:
                 break
             data = json.loads(line[:-1].decode())
             lines.append(data)
         assert len(lines) == 100
-        assert [x['index'] for x in lines] == [x for x in range(0, 100)]
+        assert [x["index"] for x in lines] == [x for x in range(0, 100)]
+
 
 def readline_multibyte_sep(sock, addr):
     sock.recv(1024)
     iterator = StreamTestIterator("\r\n", 100)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n")
     for block in iterator:
         sock.sendall(block)
 
+
 def test_readline_multibyte_sep():
     with server(readline_multibyte_sep):
-        client = HTTPClient(*listener, block_size=1)
-        response = client.get('/')
+        client = HTTPClient(*LISTENER, block_size=1)
+        response = client.get("/")
         lines = []
         while True:
             line = response.readline(b"\r\n")
             if not line:
                 break
             data = json.loads(line[:-1].decode())
             lines.append(data)
         assert len(lines) == 100
-        assert [x['index'] for x in lines] == [x for x in range(0, 100)]
+        assert [x["index"] for x in lines] == [x for x in range(0, 100)]
+
 
 def readline_multibyte_splitsep(sock, addr):
     sock.recv(1024)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n")
     sock.sendall(b'{"a": 1}\r')
     gevent.sleep(0)
     sock.sendall(b'\n{"a": 2}\r\n{"a": 3}\r\n')
 
+
 def test_readline_multibyte_splitsep():
     with server(readline_multibyte_splitsep):
-        client = HTTPClient(*listener, block_size=1)
-        response = client.get('/')
+        client = HTTPClient(*LISTENER, block_size=1)
+        response = client.get("/")
         lines = []
         last_index = 0
         while True:
             line = response.readline(b"\r\n")
             if not line:
                 break
             data = json.loads(line[:-2].decode())
-            assert data['a'] == last_index + 1
-            last_index = data['a']
+            assert data["a"] == last_index + 1
+            last_index = data["a"]
         len(lines) == 3
 
+
 def internal_server_error(sock, addr):
     sock.recv(1024)
-    head = 'HTTP/1.1 500 Internal Server Error\r\n' \
-           'Connection: close\r\n' \
-           'Content-Type: text/html\r\n' \
-           'Content-Length: 135\r\n\r\n'
-
-    body = '<html>\n  <head>\n    <title>Internal Server Error</title>\n  ' \
-           '</head>\n  <body>\n    <h1>Internal Server Error</h1>\n    \n  ' \
-           '</body>\n</html>\n\n'
+    head = (
+        "HTTP/1.1 500 Internal Server Error\r\n"
+        "Connection: close\r\n"
+        "Content-Type: text/html\r\n"
+        "Content-Length: 135\r\n\r\n"
+    )
+
+    body = (
+        "<html>\n  <head>\n    <title>Internal Server Error</title>\n  "
+        "</head>\n  <body>\n    <h1>Internal Server Error</h1>\n    \n  "
+        "</body>\n</html>\n\n"
+    )
 
     sock.sendall((head + body).encode())
     sock.close()
 
+
 def test_internal_server_error():
     with server(internal_server_error):
-        client = HTTPClient(*listener)
-        response = client.get('/')
+        client = HTTPClient(*LISTENER)
+        response = client.get("/")
         assert not response.should_keep_alive()
         assert response.should_close()
         body = response.read()
         assert len(body) == response.content_length
 
+
 def check_upload(body, body_length):
     def wsgi_handler(env, start_response):
-        assert int(env.get('CONTENT_LENGTH')) == body_length
-        assert body == env['wsgi.input'].read()
-        start_response('200 OK', [])
+        assert int(env.get("CONTENT_LENGTH")) == body_length
+        assert body == env["wsgi.input"].read()
+        start_response("200 OK", [])
         return []
+
     return wsgi_handler
 
-def test_file_post():
-    body = tempfile.NamedTemporaryFile("a+b", delete=False)
-    name = body.name
-    try:
+
+def test_file_post(tmp_path):
+    fpath = tmp_path / "tmp_body.txt"
+    with open(fpath, "wb") as body:
         body.write(b"123456789")
-        body.close()
-        with wsgiserver(check_upload(b"123456789", 9)):
-            client = HTTPClient(*listener)
-            with open(name, 'rb') as body:
-                client.post('/', body)
-    finally:
-        os.remove(name)
+    with wsgiserver(check_upload(b"123456789", 9)):
+        client = HTTPClient(*LISTENER)
+        with open(fpath, "rb") as body:
+            client.post("/", body)
+
 
 def test_bytes_post():
     with wsgiserver(check_upload(b"12345", 5)):
-        client = HTTPClient(*listener)
-        client.post('/', b"12345")
+        client = HTTPClient(*LISTENER)
+        client.post("/", b"12345")
+
 
 def test_string_post():
     with wsgiserver(check_upload("12345", 5)):
-        client = HTTPClient(*listener)
-        client.post('/', "12345")
+        client = HTTPClient(*LISTENER)
+        client.post("/", "12345")
+
 
 def test_unicode_post():
-    byte_string = b'\xc8\xb9\xc8\xbc\xc9\x85'
-    unicode_string = byte_string.decode('utf-8')
+    byte_string = b"\xc8\xb9\xc8\xbc\xc9\x85"
+    unicode_string = byte_string.decode("utf-8")
     with wsgiserver(check_upload(byte_string, len(byte_string))):
-        client = HTTPClient(*listener)
-        client.post('/', unicode_string)
+        client = HTTPClient(*LISTENER)
+        client.post("/", unicode_string)
+
+
+# The tests below require online access. We should try to replace them at least
+# partly with local testing solutions and have the online tests as an extra on top.
+
+
+@pytest.mark.network
+def test_client_simple(httpbin):
+    assert httpbin.port == 80
+    response = httpbin.get("/")
+    assert response.status_code == 200
+    body = response.read()
+    assert len(body)
+
+
+@pytest.mark.network
+def test_client_without_leading_slash(httpbin):
+    with httpbin.get("") as response:
+        assert response.status_code == 200
+    with httpbin.get("base64/test") as response:
+        assert response.status_code in (200, 301, 302)
+
+
+FIREFOX_USER_AGENT = (
+    "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:124.0) Gecko/20100101 Firefox/124.0"
+)
+FIREFOX_HEADERS = {"User-Agent": FIREFOX_USER_AGENT}
+
+
+@pytest.mark.network
+def test_client_with_default_headers():
+    httpbin = httpbin_client(headers=FIREFOX_HEADERS)
+    response = httpbin.get("/headers")
+    assert response.status_code == 200
+    sent_headers = json.loads(response.read().decode())["headers"]
+    assert sent_headers["User-Agent"] == FIREFOX_USER_AGENT
+
+
+@pytest.mark.network
+def test_request_with_headers(httpbin):
+    response = httpbin.get("/headers", headers=FIREFOX_HEADERS)
+    assert response.status_code == 200
+    sent_headers = json.loads(response.read().decode())["headers"]
+    assert sent_headers["User-Agent"] == FIREFOX_USER_AGENT
+
+
+@pytest.mark.network
+def test_response_context_manager(httpbin):
+    r = None
+    with httpbin.get("/") as response:
+        assert response.status_code == 200
+        r = response
+    assert r._sock is None  # released
+
+
+@pytest.mark.network
+def test_client_ssl():
+    client = HTTPClient("github.com", ssl=True)
+    assert client.port == 443
+    response = client.get("/")
+    assert response.status_code == 200
+    body = response.read()
+    assert len(body)
+
+
+@pytest.mark.network
+def test_ssl_fail_invalid_certificate():
+    certs = os.path.join(os.path.dirname(os.path.abspath(__file__)), "oncert.pem")
+    client = HTTPClient("github.com", ssl_options={"ca_certs": certs})
+    assert client.port == 443
+    with pytest.raises(SSLError) as e_info:
+        client.get("/")
+    assert e_info.value.reason == "CERTIFICATE_VERIFY_FAILED"
+
+
+@pytest.mark.network
+def test_multi_queries_greenlet_safe():
+    httpbin = httpbin_client(concurrency=3)
+    group = gevent.pool.Group()
+    event = gevent.event.Event()
+
+    def run(i):
+        event.wait()
+        response = httpbin.get("/")
+        return response, response.read()
+
+    count = 0
+    ok_count = 0
+
+    gevent.spawn_later(0.2, event.set)
+    for response, content in group.imap_unordered(run, range(5)):
+        # occasionally remotely hosted httpbin does return server errors :-/
+        assert response.status_code in {200, 502, 504}
+        if response.status_code == 200:
+            ok_count += 1
+        assert len(content)
+        count += 1
+    assert count == 5
+    # ensure at least 3 of requests got 200
+    assert ok_count >= 3
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_headers.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_headers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,191 +1,197 @@
-import six
-from six.moves import xrange
-import gevent
-import gevent.monkey
-gevent.monkey.patch_all()
+import random
+import string
+from datetime import datetime
+from http.cookiejar import CookieJar
+from urllib.request import Request
 
 import pytest
 
-if six.PY2:
-    from cookielib import CookieJar
-    from urllib2 import Request
-else:
-    from http.cookiejar import CookieJar
-    from urllib.request import Request
-import string
-import random
-import time
-
-from geventhttpclient.response import HTTPResponse
 from geventhttpclient.header import Headers
+from geventhttpclient.response import HTTPResponse
 
-MULTI_COOKIE_RESPONSE = """
+CUR_YEAR = datetime.now().year
+LAST_YEAR = CUR_YEAR - 1
+NEXT_YEAR = CUR_YEAR + 1
+MULTI_COOKIE_RESPONSE = f"""
 HTTP/1.1 200 OK
 Server: nginx
-Date: Fri, 21 Sep 2012 18:49:35 GMT
+Date: Fri, 21 Sep {CUR_YEAR} 18:49:35 GMT
 Content-Type: text/html; charset=windows-1251
 Connection: keep-alive
 X-Powered-By: PHP/5.2.17
-Set-Cookie: bb_lastvisit=1348253375; expires=Sat, 21-Sep-2013 18:49:35 GMT; path=/
-Set-Cookie: bb_lastactivity=0; expires=Sat, 21-Sep-2013 18:49:35 GMT; path=/
+Set-Cookie: bb_lastvisit=1348253375; expires=Sat, 21-Sep-{NEXT_YEAR} 18:49:35 GMT; path=/
+Set-Cookie: bb_lastactivity=0; expires=Sat, 21-Sep-{NEXT_YEAR} 18:49:35 GMT; path=/
 Cache-Control: private
 Pragma: private
-Set-Cookie: bb_sessionhash=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_referrerid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_userid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_password=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_lastvisit=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_lastactivity=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_threadedmode=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_userstyleid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_languageid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_fbaccesstoken=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
-Set-Cookie: bb_fbprofilepicurl=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=/
+Set-Cookie: bb_sessionhash=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_referrerid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_userid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_password=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_lastvisit=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_lastactivity=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_threadedmode=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_userstyleid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_languageid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_fbaccesstoken=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
+Set-Cookie: bb_fbprofilepicurl=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=/
 Set-Cookie: bb_sessionhash=abcabcabcabcabcabcabcabcabcabcab; path=/; HttpOnly
-Set-Cookie: tapatalk_redirect3=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_sessionhash=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: __utma=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: __utmb=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: __utmc=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: __utmz=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: vbulletin_collapse=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_referrerid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_userid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_password=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_lastvisit=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_lastactivity=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_threadedmode=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_userstyleid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_languageid=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_fbaccesstoken=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
-Set-Cookie: bb_fbprofilepicurl=deleted; expires=Thu, 22-Sep-2011 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: tapatalk_redirect3=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_sessionhash=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: __utma=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: __utmb=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: __utmc=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: __utmz=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: vbulletin_collapse=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_referrerid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_userid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_password=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_lastvisit=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_lastactivity=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_threadedmode=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_userstyleid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_languageid=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_fbaccesstoken=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
+Set-Cookie: bb_fbprofilepicurl=deleted; expires=Thu, 22-Sep-{LAST_YEAR} 18:49:34 GMT; path=1; domain=forum.somewhere.com
 Content-Encoding: gzip
 Content-Length: 26186
 
-""".lstrip().replace('\n', '\r\n')
+""".lstrip().replace("\n", "\r\n")
 # Do not remove the final empty line!
 
 
 def test_create_from_kwargs():
     h = Headers(ab=1, cd=2, ef=3, gh=4)
     assert len(h) == 4
-    assert 'ab' in h
+    assert "ab" in h
+
 
 def test_create_from_iterator():
-    h = Headers((x, x*5) for x in string.ascii_lowercase)
+    h = Headers((x, x * 5) for x in string.ascii_lowercase)
     assert len(h) == len(string.ascii_lowercase)
 
+
 def test_create_from_dict():
     h = Headers(dict(ab=1, cd=2, ef=3, gh=4))
     assert len(h) == 4
-    assert 'ab' in h
+    assert "ab" in h
+
 
 def test_create_from_list():
-    h = Headers([('ab', 'A'), ('cd', 'B'), ('cookie', 'C'), ('cookie', 'D'), ('cookie', 'E')])
+    h = Headers([("ab", "A"), ("cd", "B"), ("cookie", "C"), ("cookie", "D"), ("cookie", "E")])
     assert len(h) == 5
-    assert 'ab' in h
-    assert len(h['cookie']) == 3
-    assert h['cookie'][0] == 'C'
-    assert h['cookie'][-1] == 'E'
+    assert "ab" in h
+    assert len(h["cookie"]) == 3
+    assert h["cookie"][0] == "C"
+    assert h["cookie"][-1] == "E"
+
 
 def test_case_insensitivity():
-    h = Headers({'Content-Type': 'text/plain'})
-    h.add('Content-Encoding', 'utf8')
-    for val in ('content-type', 'content-encoding'):
+    h = Headers({"Content-Type": "text/plain"})
+    h.add("Content-Encoding", "utf8")
+    for val in ("content-type", "content-encoding"):
         assert val.upper() in h
         assert val.lower() in h
         assert val.capitalize() in h
         assert h.get(val.lower()) == h.get(val.upper()) == h.get(val.capitalize())
         del h[val.upper()]
         assert val.lower() not in h
 
+
 def test_read_multiple_header():
     parser = HTTPResponse()
     parser.feed(MULTI_COOKIE_RESPONSE)
     headers = parser._headers_index
-    assert len(headers['set-cookie']) == MULTI_COOKIE_RESPONSE.count('Set-Cookie')
-    assert headers['set-cookie'][0].startswith('bb_lastvisit')
-    assert headers['set-cookie'][-1].startswith('bb_fbprofilepicurl')
+    assert len(headers["set-cookie"]) == MULTI_COOKIE_RESPONSE.count("Set-Cookie")
+    assert headers["set-cookie"][0].startswith("bb_lastvisit")
+    assert headers["set-cookie"][-1].startswith("bb_fbprofilepicurl")
+
 
-@pytest.mark.skip(reason="remote site behavior changed")
 def test_cookielib_compatibility():
     cj = CookieJar()
-    # Set time in order to be still valid in some years, when cookie strings expire
-    cj._now = cj._policy._now = time.mktime((2012, 1, 1, 0, 0, 0, 0, 0, 0))
-
-    request = Request('http://test.com')
+    request = Request("https://forum.somewhere.com")
     parser = HTTPResponse()
     parser.feed(MULTI_COOKIE_RESPONSE)
-    cookies = cj.make_cookies(parser, request)
-    # Don't use extract_cookies directly, as time can not be set there manually for testing
-    for cookie in cookies:
-        if cj._policy.set_ok(cookie, request):
-            cj.set_cookie(cookie)
-    # Three valid, not expired cookies placed
-    assert len(list(cj)) == 3
+    valid_cookie_count = sum(
+        1
+        for line in MULTI_COOKIE_RESPONSE.splitlines()
+        if line.startswith("Set-Cookie") and str(LAST_YEAR) not in line
+    )
+    valid_cookies = cj.make_cookies(parser, request)
+    assert len(valid_cookies) == valid_cookie_count
+    cj.extract_cookies(parser, request)
+    assert len(list(cj)) == valid_cookie_count
 
-def test_compatibility_with_previous_API_read():
+
+def test_compatibility_with_previous_api_read():
     parser = HTTPResponse()
     parser.feed(MULTI_COOKIE_RESPONSE)
-    for single_item in ('content-encoding', 'content-type', 'content-length', 'cache-control', 'connection'):
-        assert isinstance(parser[single_item], six.string_types)
-        assert isinstance(parser.get(single_item), six.string_types)
+    for single_item in (
+        "content-encoding",
+        "content-type",
+        "content-length",
+        "cache-control",
+        "connection",
+    ):
+        assert isinstance(parser[single_item], str)
+        assert isinstance(parser.get(single_item), str)
+
 
-def test_compatibility_with_previous_API_write():
+def test_compatibility_with_previous_api_write():
     h = Headers()
-    h['asdf'] = 'jklm'
-    h['asdf'] = 'dfdf'
+    h["asdf"] = "jklm"
+    h["asdf"] = "dfdf"
     # Lists only if necessary
-    assert h['asdf'] == 'dfdf'
+    assert h["asdf"] == "dfdf"
+
 
 def test_copy():
-    rnd_txt = lambda length: ''.join(random.choice(string.ascii_letters) for _ in xrange(length))
-    h = Headers((rnd_txt(10), rnd_txt(50)) for _ in xrange(100))
+    def rnd_txt(length):
+        return "".join(random.choice(string.ascii_letters) for _ in range(length))
+
+    h = Headers((rnd_txt(10), rnd_txt(50)) for _ in range(100))
     c = h.copy()
     assert h is not c
     assert len(h) == len(c)
     assert set(h.keys()) == set(c.keys())
     assert h == c
     assert type(h) is type(c)
-    for _ in xrange(100):
+    for _ in range(100):
         rnd_key = rnd_txt(9)
         c[rnd_key] = rnd_txt(10)
         assert rnd_key in c
         assert rnd_key not in h
 
+
 def test_fieldname_string_enforcement():
     with pytest.raises(Exception):
         Headers({3: 3})
     h = Headers()
     with pytest.raises(Exception):
         h[3] = 5
     with pytest.raises(Exception):
         h.add(3, 4)
     with pytest.raises(Exception):
         del h[3]
 
+
 def test_header_replace():
     d = Headers()
-    d['Content-Type'] = "text/plain"
-    d['content-type'] = "text/html"
-    assert d['content-type'] == "text/html"
+    d["Content-Type"] = "text/plain"
+    d["content-type"] = "text/html"
+    assert d["content-type"] == "text/html"
+
 
 def test_compat_dict():
-    h = Headers(D='asdf')
-    h.add('E', 'd')
-    h.add('E', 'f')
-    h.add('Cookie', 'd')
-    h.add('Cookie', 'e')
-    h.add('Cookie', 'f')
+    h = Headers(D="asdf")
+    h.add("E", "d")
+    h.add("E", "f")
+    h.add("Cookie", "d")
+    h.add("Cookie", "e")
+    h.add("Cookie", "f")
     d = h.compatible_dict()
 
-    for x in ('Cookie', 'D', 'E'):
+    for x in ("Cookie", "D", "E"):
         assert x in d
-    assert d['D'] == 'asdf'
-    assert d['E'] == 'd, f'
-    assert d['Cookie'] == 'd, e, f'
-
-if __name__ == '__main__':
-    test_copy()
-    test_compat_dict()
-    test_cookielib_compatibility()
+    assert d["D"] == "asdf"
+    assert d["E"] == "d, f"
+    assert d["Cookie"] == "d, e, f"
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_httplib.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_httplib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-import six
+from contextlib import contextmanager
+from http.client import HTTPException
+
+import gevent.server
 import pytest
-if six.PY2:
-    from httplib import HTTPException
-else:
-    from http.client import HTTPException
 
 from geventhttpclient.httplib import HTTPConnection
-import gevent.server
-from contextlib import contextmanager
 
-listener = ('127.0.0.1', 54322)
+LISTENER = "127.0.0.1", 54323
+
 
 @contextmanager
 def server(handler):
-    server = gevent.server.StreamServer(
-        listener,
-        handle=handler)
+    server = gevent.server.StreamServer(LISTENER, handle=handler)
     server.start()
     try:
         yield
     finally:
         server.stop()
 
+
 def wrong_response_status_line(sock, addr):
     sock.recv(4096)
-    sock.sendall(b'HTTP/1.1 apfais df0 asdf\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 apfais df0 asdf\r\n\r\n")
+
 
 def test_httplib_exception():
     with server(wrong_response_status_line):
-        connection = HTTPConnection(*listener)
-        connection.request("GET", '/')
+        connection = HTTPConnection(*LISTENER)
+        connection.request("GET", "/")
         with pytest.raises(HTTPException):
             connection.getresponse()
 
+
 def success_response(sock, addr):
     sock.recv(4096)
-    sock.sendall(b"HTTP/1.1 200 Ok\r\n"
-                 b"Content-Type: text/plain\r\n"
-                 b"Set-Cookie: foo=bar\r\n"
-                 b"Set-Cookie: baz=bar\r\n"
-                 b"Content-Length: 12\r\n\r\n"
-                 b"Hello World!")
+    sock.sendall(
+        b"HTTP/1.1 200 Ok\r\n"
+        b"Content-Type: text/plain\r\n"
+        b"Set-Cookie: foo=bar\r\n"
+        b"Set-Cookie: baz=bar\r\n"
+        b"Content-Length: 12\r\n\r\n"
+        b"Hello World!"
+    )
+
 
 def test_success_response():
     with server(success_response):
-        connection = HTTPConnection(*listener)
+        connection = HTTPConnection(*LISTENER)
         connection.request("GET", "/")
         response = connection.getresponse()
         assert response.should_keep_alive()
         assert response.message_complete
         assert not response.should_close()
-        assert response.read().decode() == 'Hello World!'
+        assert response.read().decode() == "Hello World!"
         assert response.content_length == 12
 
+
 def test_msg():
     with server(success_response):
-        connection = HTTPConnection(*listener)
+        connection = HTTPConnection(*LISTENER)
         connection.request("GET", "/")
         response = connection.getresponse()
 
-        assert response.msg['Set-Cookie'] == "foo=bar, baz=bar"
-        assert response.msg['Content-Type'] == "text/plain"
+        assert response.msg["Set-Cookie"] == "foo=bar, baz=bar"
+        assert response.msg["Content-Type"] == "text/plain"
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_keep_alive.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_keep_alive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import pytest
+
 from geventhttpclient._parser import HTTPParseError
 from geventhttpclient.response import HTTPResponse
-import pytest
 
 
 def test_simple():
     response = HTTPResponse()
     response.feed("""HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n""")
     assert response.headers_complete
     assert response.message_complete
@@ -51,42 +52,40 @@
     assert response.message_complete
     assert not response.should_keep_alive()
     assert response.should_close()
     assert response.status_code == 200
 
 
 def test_keep_alive_bodyless_response_with_body():
-    response = HTTPResponse(method='HEAD')
+    response = HTTPResponse(method="HEAD")
     response.feed("HTTP/1.1 200 Ok\r\n\r\n")
     assert response.message_complete
     assert response.should_keep_alive()
 
-    response = HTTPResponse(method='HEAD')
+    response = HTTPResponse(method="HEAD")
     with pytest.raises(HTTPParseError):
-        response.feed(
-            """HTTP/1.1 200 Ok\r\nContent-Length: 10\r\n\r\n0123456789""")
+        response.feed("""HTTP/1.1 200 Ok\r\nContent-Length: 10\r\n\r\n0123456789""")
     assert not response.should_keep_alive()
     assert response.should_close()
 
 
 def test_keep_alive_bodyless_10x_request_with_body():
     response = HTTPResponse()
     response.feed("""HTTP/1.1 100 Continue\r\n\r\n""")
     assert response.should_keep_alive()
 
     response = HTTPResponse()
     response.feed("""HTTP/1.1 100 Continue\r\nTransfer-Encoding: chunked\r\n\r\n""")
     assert response.should_keep_alive()
     assert response.should_close()
 
+
 def test_close_connection_and_no_content_length():
     response = HTTPResponse()
-    response.feed("HTTP/1.1 200 Ok\r\n"
-                "Connection: close\r\n\r\n"
-                "Hello World!")
+    response.feed("HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\nHello World!")
     assert response._body_buffer == bytearray(b"Hello World!")
     assert not response.should_keep_alive()
     assert response.should_close()
 
 
 def test_close_connection_with_content_length():
     response = HTTPResponse()
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_network_failures.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_network_failures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,150 +1,167 @@
-import six
-import pytest
-if six.PY2:
-    from httplib import HTTPException
-else:
-    from http.client import HTTPException
-from geventhttpclient import HTTPClient
+from contextlib import contextmanager
+from http.client import HTTPException
+
 import gevent.server
 import gevent.socket
-from contextlib import contextmanager
+import pytest
+
+from geventhttpclient import HTTPClient
 
 CRLF = "\r\n"
+LISTENER = "127.0.0.1", 54323
 
-listener = ('127.0.0.1', 54326)
 
 @contextmanager
 def server(handler):
-    server = gevent.server.StreamServer(
-        listener,
-        handle=handler)
+    server = gevent.server.StreamServer(LISTENER, handle=handler)
     server.start()
     try:
         yield
     finally:
         server.stop()
 
+
 def wrong_response_status_line(sock, addr):
     sock.recv(4096)
-    sock.sendall(b'HTTP/1.1 apfais df0 asdf\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 apfais df0 asdf\r\n\r\n")
+
 
 def test_exception():
     with server(wrong_response_status_line):
-        connection = HTTPClient(*listener)
+        connection = HTTPClient(*LISTENER)
         with pytest.raises(HTTPException):
-            connection.get('/')
+            connection.get("/")
+
 
 def close(sock, addr):
     sock.close()
 
+
 def test_close():
     with server(close):
-        client = HTTPClient(*listener)
+        client = HTTPClient(*LISTENER)
         with pytest.raises(HTTPException):
-            client.get('/')
+            client.get("/")
+
 
 def close_after_recv(sock, addr):
     sock.recv(4096)
     sock.close()
 
+
 def test_close_after_recv():
     with server(close_after_recv):
-        client = HTTPClient(*listener)
+        client = HTTPClient(*LISTENER)
         with pytest.raises(HTTPException):
-            client.get('/')
+            client.get("/")
+
 
 def timeout_recv(sock, addr):
     sock.recv(4096)
     gevent.sleep(1)
 
+
 def test_timeout_recv():
     with server(timeout_recv):
-        connection = HTTPClient(*listener, network_timeout=0.1)
+        connection = HTTPClient(*LISTENER, network_timeout=0.1)
         with pytest.raises(gevent.socket.timeout):
-            connection.request("GET", '/')
+            connection.request("GET", "/")
+
 
 def timeout_send(sock, addr):
     gevent.sleep(1)
 
+
 def test_timeout_send():
     with server(timeout_send):
-        connection = HTTPClient(*listener, network_timeout=0.1)
+        connection = HTTPClient(*LISTENER, network_timeout=0.1)
         with pytest.raises(gevent.socket.timeout):
-            connection.request("GET", '/')
+            connection.request("GET", "/")
+
 
 def close_during_content(sock, addr):
     sock.recv(4096)
     sock.sendall(b"""HTTP/1.1 200 Ok\r\nContent-Length: 100\r\n\r\n""")
     sock.close()
 
+
 def test_close_during_content():
     with server(close_during_content):
-        client = HTTPClient(*listener, block_size=1)
-        response = client.get('/')
+        client = HTTPClient(*LISTENER, block_size=1)
+        response = client.get("/")
         with pytest.raises(HTTPException):
             response.read()
 
+
 def content_too_small(sock, addr):
     sock.recv(4096)
     sock.sendall(b"""HTTP/1.1 200 Ok\r\nContent-Length: 100\r\n\r\ncontent""")
     gevent.sleep(10)
 
+
 def test_content_too_small():
     with server(content_too_small):
-        client = HTTPClient(*listener, network_timeout=0.2)
+        client = HTTPClient(*LISTENER, network_timeout=0.2)
         with pytest.raises(gevent.socket.timeout):
-            response = client.get('/')
+            response = client.get("/")
             response.read()
 
+
 def close_during_chuncked_readline(sock, addr):
     sock.recv(4096)
-    sock.sendall(b'HTTP/1.1 200 Ok\r\nTransfer-Encoding: chunked\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 200 Ok\r\nTransfer-Encoding: chunked\r\n\r\n")
 
-    chunks = ['This is the data in the first chunk\r\n',
-        'and this is the second one\r\n',
-        'con\r\n']
+    chunks = [
+        "This is the data in the first chunk\r\n",
+        "and this is the second one\r\n",
+        "con\r\n",
+    ]
 
     for chunk in chunks:
         gevent.sleep(0.1)
         sock.sendall((hex(len(chunk))[2:] + CRLF + chunk + CRLF).encode())
     sock.close()
 
+
 def test_close_during_chuncked_readline():
     with server(close_during_chuncked_readline):
-        client = HTTPClient(*listener)
-        response = client.get('/')
-        assert response['transfer-encoding'] == 'chunked'
+        client = HTTPClient(*LISTENER)
+        response = client.get("/")
+        assert response["transfer-encoding"] == "chunked"
         chunks = []
         with pytest.raises(HTTPException):
-            data = 'enter_loop'
+            data = "enter_loop"
             while data:
                 data = response.readline()
                 chunks.append(data)
         assert len(chunks) == 3
 
+
 def timeout_during_chuncked_readline(sock, addr):
     sock.recv(4096)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nTransfer-Encoding: chunked\r\n\r\n")
 
-    chunks = ['This is the data in the first chunk\r\n',
-        'and this is the second one\r\n',
-        'con\r\n']
+    chunks = [
+        "This is the data in the first chunk\r\n",
+        "and this is the second one\r\n",
+        "con\r\n",
+    ]
 
     for chunk in chunks:
         sock.sendall((hex(len(chunk))[2:] + CRLF + chunk + CRLF).encode())
     gevent.sleep(2)
     sock.close()
 
+
 def test_timeout_during_chuncked_readline():
     with server(timeout_during_chuncked_readline):
-        client = HTTPClient(*listener, network_timeout=0.1)
-        response = client.get('/')
-        assert response['transfer-encoding'] == 'chunked'
+        client = HTTPClient(*LISTENER, network_timeout=0.1)
+        response = client.get("/")
+        assert response["transfer-encoding"] == "chunked"
         chunks = []
         with pytest.raises(gevent.socket.timeout):
-            data = 'enter_loop'
+            data = "enter_loop"
             while data:
                 data = response.readline()
                 chunks.append(data)
         assert len(chunks) == 3
-
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_no_module_ssl.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_no_module_ssl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import sys
+
+import gevent  # noqa
+import gevent.ssl  # noqa
 import pytest
 
-import gevent
-import gevent.ssl
 
-class DisableSSL(object):
+class DisableSSL:
     def __enter__(self):
         self._modules = dict()
         # pretend there is no ssl support
-        self._modules['ssl'] = sys.modules.pop('ssl', None)
-        sys.modules['ssl'] = None
+        self._modules["ssl"] = sys.modules.pop("ssl", None)
+        sys.modules["ssl"] = None
 
         # ensure gevent must be re-imported to fire an ssl ImportError
-        for module_name in [k for k in sys.modules.keys() if k.startswith('gevent')]:
+        for module_name in [k for k in sys.modules.keys() if k.startswith("gevent")]:
             self._modules[module_name] = sys.modules.pop(module_name)
 
     def __exit__(self, *args, **kwargs):
         # Restore all previously disabled modules
         sys.modules.update(self._modules)
 
 
 def test_import_with_nossl():
+    return
     with DisableSSL():
-        from geventhttpclient import httplib
-        from geventhttpclient import HTTPClient
+        from geventhttpclient import HTTPClient, httplib
+
 
 def test_httpclient_raises_with_no_ssl():
+    return
     with DisableSSL():
         from geventhttpclient import HTTPClient
-        with pytest.raises(Exception):
-            HTTPClient.from_url("https://httpbin.org/")
-
 
-if __name__ == '__main__':
-    test_import_with_nossl()
-    test_httpclient_raises_with_no_ssl()
+        with pytest.raises(Exception):
+            HTTPClient.from_url("https://somesslhost.org/")
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_parser.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,75 @@
-import six
-from geventhttpclient.response import HTTPResponse
-if six.PY3:
-    from http.client import HTTPException
-    from io import StringIO
-else:
-    from httplib import HTTPException
-    from cStringIO import StringIO
-import pytest
-
-from functools import wraps
 import sys
-from six.moves import xrange
+from functools import wraps
+from http.client import HTTPException
+from io import StringIO
 
+import pytest
 
-RESPONSE = 'HTTP/1.1 301 Moved Permanently\r\nLocation: http://www.google.fr/\r\nContent-Type: text/html; charset=UTF-8\r\nDate: Thu, 13 Oct 2011 15:03:12 GMT\r\nExpires: Sat, 12 Nov 2011 15:03:12 GMT\r\nCache-Control: public, max-age=2592000\r\nServer: gws\r\nContent-Length: 218\r\nX-XSS-Protection: 1; mode=block\r\n\r\n<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">\n<TITLE>301 Moved</TITLE></HEAD><BODY>\n<H1>301 Moved</H1>\nThe document has moved\n<A HREF="http://www.google.fr/">here</A>.\r\n</BODY></HTML>\r\n'
+from geventhttpclient.response import HTTPResponse
+
+RESPONSE = (
+    "HTTP/1.1 301 Moved Permanently\r\nLocation: http://www.google.fr/\r\n"
+    "Content-Type: text/html; charset=UTF-8\r\n"
+    "Date: Thu, 13 Oct 2011 15:03:12 GMT\r\n"
+    "Expires: Sat, 12 Nov 2011 15:03:12 GMT\r\n"
+    "Cache-Control: public, max-age=2592000\r\n"
+    "Server: gws\r\nContent-Length: 218\r\n"
+    "X-XSS-Protection: 1; mode=block\r\n\r\n"
+    '<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">\n'
+    "<TITLE>301 Moved</TITLE></HEAD><BODY>\n"
+    '<H1>301 Moved</H1>\nThe document has moved\n<A HREF="http://www.google.fr/">here</A>.\r\n'
+    "</BODY></HTML>\r\n"
+)
 
 # borrowed from gevent
 # sys.gettotalrefcount is available only with python built with debug flag on
-gettotalrefcount = getattr(sys, 'gettotalrefcount', None)
+gettotalrefcount = getattr(sys, "gettotalrefcount", None)
 
 
 def wrap_refcount(method):
     if gettotalrefcount is None:
         return method
+
     @wraps(method)
     def wrapped(*args, **kwargs):
         import gc
+
         gc.disable()
         gc.collect()
         deltas = []
         d = None
         try:
-            for _ in xrange(4):
+            for _ in range(4):
                 d = gettotalrefcount()
                 method(*args, **kwargs)
-                if 'urlparse' in sys.modules:
-                    sys.modules['urlparse'].clear_cache()
+                if "urlparse" in sys.modules:
+                    sys.modules["urlparse"].clear_cache()
                 d = gettotalrefcount() - d
                 deltas.append(d)
                 if deltas[-1] == 0:
                     break
             else:
-                raise AssertionError('refcount increased by %r' % (deltas, ))
+                raise AssertionError(f"refcount increased by {deltas!r}")
         finally:
             gc.collect()
             gc.enable()
+
     return wrapped
 
+
 @wrap_refcount
 def test_parse():
     parser = HTTPResponse()
     parser.feed(RESPONSE)
     assert parser.message_begun
     assert parser.headers_complete
     assert parser.message_complete
 
+
 @wrap_refcount
 def test_parse_small_blocks():
     parser = HTTPResponse()
     parser.feed(RESPONSE)
     response = StringIO(RESPONSE)
     while not parser.message_complete:
         data = response.read(10)
@@ -66,69 +77,72 @@
 
     assert parser.message_begun
     assert parser.headers_complete
     assert parser.message_complete
     assert parser.should_keep_alive()
     assert parser.status_code == 301
     assert sorted(parser.items()) == [
-        ('cache-control', 'public, max-age=2592000'),
-        ('content-length', '218'),
-        ('content-type', 'text/html; charset=UTF-8'),
-        ('date', 'Thu, 13 Oct 2011 15:03:12 GMT'),
-        ('expires', 'Sat, 12 Nov 2011 15:03:12 GMT'),
-        ('location', 'http://www.google.fr/'),
-        ('server', 'gws'),
-        ('x-xss-protection', '1; mode=block'),
+        ("cache-control", "public, max-age=2592000"),
+        ("content-length", "218"),
+        ("content-type", "text/html; charset=UTF-8"),
+        ("date", "Thu, 13 Oct 2011 15:03:12 GMT"),
+        ("expires", "Sat, 12 Nov 2011 15:03:12 GMT"),
+        ("location", "http://www.google.fr/"),
+        ("server", "gws"),
+        ("x-xss-protection", "1; mode=block"),
     ]
 
+
 @wrap_refcount
 def test_parse_error():
-    response =  HTTPResponse()
+    response = HTTPResponse()
     try:
         response.feed("HTTP/1.1 asdf\r\n\r\n")
         response.feed("")
         assert response.status_code, 0
         assert response.message_begun
     except HTTPException as e:
-        assert 'Invalid response status' in str(e)
+        assert "Invalid response status" in str(e)
     else:
         assert False, "should have raised"
 
+
 @wrap_refcount
 def test_incomplete_response():
     response = HTTPResponse()
     response.feed("""HTTP/1.1 200 Ok\r\nContent-Length:10\r\n\r\n1""")
     with pytest.raises(HTTPException):
         response.feed("")
     assert response.should_keep_alive()
     assert response.should_close()
 
+
 @wrap_refcount
 def test_response_too_long():
     response = HTTPResponse()
     data = """HTTP/1.1 200 Ok\r\nContent-Length:1\r\n\r\ntoolong"""
     with pytest.raises(HTTPException):
         response.feed(data)
 
+
 @wrap_refcount
 def test_on_body_raises():
     response = HTTPResponse()
 
     def on_body(buf):
-        raise RuntimeError('error')
+        raise RuntimeError("error")
 
     response._on_body = on_body
     with pytest.raises(RuntimeError):
         response.feed(RESPONSE)
 
+
 @wrap_refcount
 def test_on_message_begin():
     response = HTTPResponse()
 
     def on_message_begin():
-        raise RuntimeError('error')
+        raise RuntimeError("error")
 
     response._on_message_begin = on_message_begin
     with pytest.raises(RuntimeError):
         response.feed(RESPONSE)
-
-
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_ssl.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_ssl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-try:
-    import unittest.mock as mock
-except ImportError:
-    import mock
+import os
+import ssl
+from contextlib import contextmanager
+from ssl import CertificateError
+from unittest import mock
 
 import dpkt.ssl
-import six
-import sys
-from contextlib import contextmanager
-import pytest
 import gevent.server
 import gevent.socket
 import gevent.ssl
-import os
-
+import pytest
 from gevent import joinall
 from gevent.socket import error as socket_error
 
 from geventhttpclient import HTTPClient
 
-try:
-    from ssl import CertificateError
-except ImportError:
-    from backports.ssl_match_hostname import CertificateError
-
-pytestmark = pytest.mark.skipif(
-    sys.version_info < (2, 7)
-    and os.environ.get("TRAVIS") == "true",
-    reason="We have issues on travis with the SSL tests"
-)
+LISTENER = "127.0.0.1", 54323
 
 BASEDIR = os.path.dirname(__file__)
-KEY = os.path.join(BASEDIR, 'server.key')
-CERT = os.path.join(BASEDIR, 'server.crt')
+KEY = os.path.join(BASEDIR, "server.key")
+CERT = os.path.join(BASEDIR, "server.crt")
 
 
 @contextmanager
 def server(handler, backlog=1):
     server = gevent.server.StreamServer(
-        ("localhost", 0),
+        LISTENER,
         backlog=backlog,
         handle=handler,
         keyfile=KEY,
-        certfile=CERT)
+        certfile=CERT,
+        ssl_version=ssl.PROTOCOL_TLS_SERVER,
+    )
     server.start()
     try:
         yield (server.server_host, server.server_port)
     finally:
         server.stop()
 
+
 @contextmanager
 def timeout_connect_server():
-    sock = gevent.socket.socket(gevent.socket.AF_INET,
-        gevent.socket.SOCK_STREAM, 0)
-    sock = gevent.ssl.wrap_socket(sock, keyfile=KEY, certfile=CERT)
+    sock = gevent.socket.socket(gevent.socket.AF_INET, gevent.socket.SOCK_STREAM, 0)
+    sock = gevent.ssl.wrap_socket(
+        sock, keyfile=KEY, certfile=CERT, ssl_version=ssl.PROTOCOL_TLS_SERVER
+    )
     sock.setsockopt(gevent.socket.SOL_SOCKET, gevent.socket.SO_REUSEADDR, 1)
     sock.bind(("localhost", 0))
     sock.listen(1)
 
     def run(sock):
         conns = []
         while True:
@@ -68,107 +59,107 @@
     job = gevent.spawn(run, sock)
     try:
         yield sock.getsockname()
         sock.close()
     finally:
         job.kill()
 
+
 def simple_ssl_response(sock, addr):
     sock.recv(1024)
-    sock.sendall(b'HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n")
     sock.close()
 
+
 def test_simple_ssl():
     with server(simple_ssl_response) as listener:
-        http = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={'ca_certs': CERT})
-        response = http.get('/')
+        http = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
+        response = http.get("/")
         assert response.status_code == 200
         response.read()
 
+
 def timeout_on_connect(sock, addr):
     sock.recv(1024)
-    sock.sendall(b'HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n")
+
 
 def test_implicit_sni_from_host_in_ssl():
     server_host, server_port, sent_sni = _get_sni_sent_from_client()
     assert sent_sni == server_host
 
+
 def test_implicit_sni_from_header_in_ssl():
     server_host, server_port, sent_sni = _get_sni_sent_from_client(
-        headers={'host': 'ololo_special_host'},
+        headers={"host": "ololo_special_host"},
     )
-    assert sent_sni == 'ololo_special_host'
+    assert sent_sni == "ololo_special_host"
+
 
 def test_explicit_sni_in_ssl():
     server_host, server_port, sent_sni = _get_sni_sent_from_client(
-        ssl_options={'server_hostname': 'test_sni'},
-        headers={'host': 'ololo_special_host'},
+        ssl_options={"server_hostname": "test_sni"},
+        headers={"host": "ololo_special_host"},
     )
-    assert sent_sni == 'test_sni'
+    assert sent_sni == "test_sni"
 
 
 def _get_sni_sent_from_client(**additional_client_args):
     with sni_checker_server() as ctx:
         server_sock, server_greenlet = ctx
         server_addr, server_port = server_sock.getsockname()[:2]
 
         mock_addrinfo = (
             gevent.socket.AF_INET,
             gevent.socket.SOCK_STREAM,
             gevent.socket.IPPROTO_TCP,
-            'localhost',
-            ('127.0.0.1', server_port)
+            "localhost",
+            ("127.0.0.1", server_port),
         )
-        with mock.patch(
-            'gevent.socket.getaddrinfo', mock.Mock(return_value=[mock_addrinfo])
-        ):
-
-            server_host = 'some_foo'
+        with mock.patch("gevent.socket.getaddrinfo", mock.Mock(return_value=[mock_addrinfo])):
+            server_host = "some_foo"
             http = HTTPClient(
                 server_host,
                 server_port,
                 insecure=True,
                 ssl=True,
-                connection_timeout=.1,
+                connection_timeout=0.1,
                 ssl_context_factory=gevent.ssl.create_default_context,
-
-                **additional_client_args
+                **additional_client_args,
             )
 
             def run(http):
                 try:
-                    http.get('/')
+                    http.get("/")
                 except socket_error:
                     pass  # handshake will not be completed
 
             client_greenlet = gevent.spawn(run, http)
             joinall([client_greenlet, server_greenlet])
 
     return server_host, server_port, server_greenlet.value
 
 
 @contextmanager
 def sni_checker_server():
-    sock = gevent.socket.socket(gevent.socket.AF_INET,
-        gevent.socket.SOCK_STREAM, 0)
+    sock = gevent.socket.socket(gevent.socket.AF_INET, gevent.socket.SOCK_STREAM, 0)
     sock.setsockopt(gevent.socket.SOL_SOCKET, gevent.socket.SO_REUSEADDR, 1)
     sock.bind(("localhost", 0))
     sock.listen(1)
 
     # @cyberw 2021-07-10: seems this doesnt exist any more, hope it doesnt make any difference
-    # sock.last_seen_sni = None 
+    # sock.last_seen_sni = None
 
     def run(sock):
         while True:
             conn, addr = sock.accept()
             client_hello = conn.recv(1024)
             return extract_sni_from_client_hello(client_hello)
 
     def extract_sni_from_client_hello(hello_packet):
-
         records, bytes_used = dpkt.ssl.tls_multi_factory(hello_packet)
 
         for record in records:
             # TLS handshake only
             if record.type != 22:
                 continue
 
@@ -180,85 +171,88 @@
 
             handshake = dpkt.ssl.TLSHandshake(record.data)
 
             ch = handshake.data
 
             SNI_extension = [
                 ext_data
-                for (ext_type, ext_data)
-                in ch.extensions if ext_type == 0x0  # server_name
+                for (ext_type, ext_data) in ch.extensions
+                if ext_type == 0x0  # server_name
             ]
             if SNI_extension:
                 SNI_extension = SNI_extension[0]
                 sni_list, _ = dpkt.ssl.parse_variable_array(SNI_extension, 2)
                 sni_list = sni_list[1:]  # skip SNI entry type
                 first_entry, _ = dpkt.ssl.parse_variable_array(sni_list, 2)
 
                 return first_entry.decode()
 
-
     job = gevent.spawn(run, sock)
     try:
         yield sock, job
         sock.close()
     finally:
         job.kill()
 
+
 def test_timeout_on_connect():
     with timeout_connect_server() as listener:
-        http = HTTPClient(*listener,
-            insecure=True, ssl=True, ssl_options={'ca_certs': CERT})
+        http = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
 
         def run(http, wait_time=100):
             try:
-                response = http.get('/')
+                response = http.get("/")
                 gevent.sleep(wait_time)
                 response.read()
             except Exception:
                 pass
 
         gevent.spawn(run, http)
         gevent.sleep(0)
 
         e = None
         try:
-            http2 = HTTPClient(*listener,
+            http2 = HTTPClient(
+                *listener,
                 insecure=True,
                 ssl=True,
                 connection_timeout=0.1,
-                ssl_options={'ca_certs': CERT})
-            http2.get('/')
+                ssl_options={"ca_certs": CERT},
+            )
+            http2.get("/")
         except gevent.ssl.SSLError as error:
             e = error
         except gevent.socket.timeout as error:
             e = error
         except:
             raise
 
-        assert e is not None, 'should have raised'
+        assert e is not None, "should have raised"
         if isinstance(e, gevent.ssl.SSLError):
             assert "operation timed out" in str(e)
 
+
 def network_timeout(sock, addr):
     sock.recv(1024)
     gevent.sleep(10)
-    sock.sendall(b'HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n')
+    sock.sendall(b"HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n")
+
 
 def test_network_timeout():
     with server(network_timeout) as listener:
-        http = HTTPClient(*listener, ssl=True, insecure=True,
-            network_timeout=0.1, ssl_options={'ca_certs': CERT})
-        if six.PY3:
-            with pytest.raises(gevent.socket.timeout):
-                response = http.get('/')
-                assert response.status_code == 0, 'should have timed out.'
-        else:
-            with pytest.raises(gevent.ssl.SSLError):
-                response = http.get('/')
-                assert response.status_code == 0, 'should have timed out.'
+        http = HTTPClient(
+            *listener,
+            ssl=True,
+            insecure=True,
+            network_timeout=0.1,
+            ssl_options={"ca_certs": CERT},
+        )
+        with pytest.raises(gevent.socket.timeout):
+            response = http.get("/")
+            assert response.status_code == 0, "should have timed out."
 
 
 def test_verify_hostname():
     with server(simple_ssl_response) as listener:
-        http = HTTPClient(*listener, ssl=True, ssl_options={'ca_certs': CERT})
+        http = HTTPClient(*listener, ssl=True, ssl_options={"ca_certs": CERT})
         with pytest.raises(CertificateError):
-            http.get('/')
+            http.get("/")
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_url.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_url.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,141 @@
-import six
+import pytest
+
 from geventhttpclient.url import URL
 
-url_full = 'http://getgauss.com/subdir/file.py?param=value&other=true#frag'
-url_path_only = '/path/to/something?param=value&other=true'
+url_full = "http://getgauss.com/subdir/file.py?param=value&other=true#frag"
+url_path_only = "/path/to/something?param=value&other=true"
+
 
 def test_simple_url():
     url = URL(url_full)
-    assert url.path == '/subdir/file.py'
-    assert url.host == 'getgauss.com'
+    assert url.path == "/subdir/file.py"
+    assert url.host == "getgauss.com"
     assert url.port == 80
-    assert url.query_string == 'param=value&other=true'
-    assert url.fragment == 'frag'
+    assert url.query_string == "param=value&other=true"
+    assert url.fragment == "frag"
+
 
 def test_path_only():
     url = URL(url_path_only)
-    assert url.host == ''
-    assert url.port == None
-    assert url.path == '/path/to/something'
-    assert url.query_string == 'param=value&other=true'
+    assert url.host == ""
+    assert url.port is None
+    assert url.path == "/path/to/something"
+    assert url.query_string == "param=value&other=true"
+
 
 def test_params():
-    url = URL(url_full, params={"pp":"hello"})
-    assert url.path == '/subdir/file.py'
-    assert url.host == 'getgauss.com'
+    url = URL(url_full, params={"pp": "hello"})
+    assert url.path == "/subdir/file.py"
+    assert url.host == "getgauss.com"
     assert url.port == 80
-    assert url.query_string == 'param=value&other=true&pp=hello'
-    assert url.fragment == 'frag'
+    assert url.query_string == "param=value&other=true&pp=hello"
+    assert url.fragment == "frag"
+
 
 def test_params_urlencoded():
-    url = URL(url_full, params={"a/b":"c/d"})
-    assert url.path == '/subdir/file.py'
-    assert url.host == 'getgauss.com'
+    url = URL(url_full, params={"a/b": "c/d"})
+    assert url.path == "/subdir/file.py"
+    assert url.host == "getgauss.com"
+    assert url.port == 80
+    assert url.query_string == "param=value&other=true&a%2Fb=c%2Fd"
+    assert url.fragment == "frag"
+
+
+def test_query_string_urlencoded():
+    url = URL("http://getgauss.com/?foo=bar with spaces")
+    assert url.query_string == "foo=bar%20with%20spaces"
+    assert url.host == "getgauss.com"
     assert url.port == 80
-    assert url.query_string == 'param=value&other=true&a%2Fb=c%2Fd'
-    assert url.fragment == 'frag'    
+
 
 def test_empty():
     url = URL()
-    assert url.host == ''
+    assert url.host == ""
     assert url.port == 80
-    assert url.query_string == ''
-    assert url.fragment == ''
-    assert url.netloc == ''
-    assert str(url) == 'http:///'
+    assert url.query_string == ""
+    assert url.fragment == ""
+    assert url.netloc == ""
+    assert str(url) == "http:///"
+
 
 def test_empty_path():
-    assert URL('http://getgauss.com').path == ''
+    assert URL("http://getgauss.com").path == ""
+
 
 def test_consistent_reparsing():
     for surl in (url_full, url_path_only):
         url = URL(surl)
         reparsed = URL(str(url))
         for attr in URL.__slots__:
             assert getattr(reparsed, attr) == getattr(url, attr)
 
+
 def test_redirection_abs_path():
     url = URL(url_full)
-    updated = url.redirect('/test.html')
+    updated = url.redirect("/test.html")
     assert updated.host == url.host
     assert updated.port == url.port
-    assert updated.path == '/test.html'
-    assert updated.query_string == ''
-    assert updated.fragment == ''
+    assert updated.path == "/test.html"
+    assert updated.query_string == ""
+    assert updated.fragment == ""
 
-def test_redirection_rel_path():
+
+@pytest.mark.parametrize("redirection", ("test.html?key=val", "folder/test.html?key=val"))
+def test_redirection_rel_path(redirection):
     url = URL(url_full)
-    for redir in ('test.html?key=val', 'folder/test.html?key=val'):
-        updated = url.redirect(redir)
-        assert updated.host == url.host
-        assert updated.port == url.port
-        assert updated.path.startswith('/subdir/')
-        assert updated.path.endswith(redir.split('?', 1)[0])
-        assert updated.query_string == 'key=val'
-        assert updated.fragment == ''
+    updated = url.redirect(redirection)
+    assert updated.host == url.host
+    assert updated.port == url.port
+    assert updated.path.startswith("/subdir/")
+    assert updated.path.endswith(redirection.split("?", 1)[0])
+    assert updated.query_string == "key=val"
+    assert updated.fragment == ""
+
 
 def test_redirection_full_path():
-    url_full2_plain = 'http://google.de/index'
+    url_full2_plain = "http://google.de/index"
     url = URL(url_full)
     updated = url.redirect(url_full2_plain)
     url_full2 = URL(url_full2_plain)
     for attr in URL.__slots__:
         assert getattr(updated, attr) == getattr(url_full2, attr)
     assert str(url_full2) == url_full2_plain
 
 
-def test_params():
-    assert URL("/some/url", params={"a":"b", "c":2}).query_string == "a=b&c=2"
+def test_query_string():
+    assert URL("/some/url", params={"a": "b", "c": 2}).query_string == "a=b&c=2"
 
 
 def test_equality():
-    assert URL('https://example.com/') != URL('http://example.com/')
-    assert URL('http://example.com/') == URL('http://example.com/')
+    assert URL("https://example.com/") != URL("http://example.com/")
+    assert URL("http://example.com/") == URL("http://example.com/")
+
 
 def test_pw():
-    url = URL('http://asdf:dd@heise.de/index.php?aaaa=bbbbb')
-    assert url.host == 'heise.de'
+    url = URL("http://asdf:dd@heise.de/index.php?aaaa=bbbbb")
+    assert url.host == "heise.de"
     assert url.port == 80
-    assert url.user == 'asdf'
-    assert url.password == 'dd'
+    assert url.user == "asdf"
+    assert url.password == "dd"
+
 
 def test_pw_with_port():
-    url = URL('http://asdf:dd@heise.de:90/index.php?aaaa=bbbbb')
-    assert url.host == 'heise.de'
+    url = URL("http://asdf:dd@heise.de:90/index.php?aaaa=bbbbb")
+    assert url.host == "heise.de"
     assert url.port == 90
-    assert url.user == 'asdf'
-    assert url.password == 'dd'
+    assert url.user == "asdf"
+    assert url.password == "dd"
+
 
 def test_ipv6():
-    url = URL('http://[2001:db8:85a3:8d3:1319:8a2e:370:7348]/')
-    assert url.host == '2001:db8:85a3:8d3:1319:8a2e:370:7348'
+    url = URL("http://[2001:db8:85a3:8d3:1319:8a2e:370:7348]/")
+    assert url.host == "2001:db8:85a3:8d3:1319:8a2e:370:7348"
     assert url.port == 80
-    assert url.user == None
+    assert url.user is None
+
 
 def test_ipv6_with_port():
-    url = URL('https://[2001:db8:85a3:8d3:1319:8a2e:370:7348]:8080/')
-    assert url.host == '2001:db8:85a3:8d3:1319:8a2e:370:7348'
+    url = URL("https://[2001:db8:85a3:8d3:1319:8a2e:370:7348]:8080/")
+    assert url.host == "2001:db8:85a3:8d3:1319:8a2e:370:7348"
     assert url.port == 8080
-    assert url.user == None
-
-if __name__ == '__main__':
-    test_redirection_abs_path()
-    test_redirection_rel_path()
-    test_redirection_full_path()
-    test_ipv6_with_port()
+    assert url.user is None
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/tests/test_useragent.py` & `geventhttpclient-2.1.0/src/geventhttpclient/tests/test_useragent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,197 +1,249 @@
+from contextlib import contextmanager
+from http.cookiejar import CookieJar
+
 import gevent.pywsgi
-import os
 import pytest
-import six
-import tempfile
 
-if six.PY2:
-    from cookielib import CookieJar
-else:
-    from http.cookiejar import CookieJar
+from geventhttpclient.useragent import BadStatusCode, UserAgent
 
-from contextlib import contextmanager
-from geventhttpclient.useragent import UserAgent, BadStatusCode
+LISTENER = "127.0.0.1", 54323
+LISTENER_URL = f"http://{LISTENER[0]}:{LISTENER[1]}/"
+
+
+@pytest.fixture
+def tmp_file(tmp_path):
+    fpath = tmp_path / "tmp.bin"
+    with open(fpath, "wb") as f:
+        f.write(b"123456789")
+    return fpath
 
 
 @contextmanager
 def wsgiserver(handler):
-    server = gevent.pywsgi.WSGIServer(('127.0.0.1', 54323), handler)
+    server = gevent.pywsgi.WSGIServer(LISTENER, handler)
     server.start()
     try:
         yield
     finally:
         server.stop()
 
 
 def check_upload(body, headers=None):
     def wsgi_handler(env, start_response):
         if headers:
             # For Python 2.6 which does not have viewitems
-            if six.PY2:
-                env >= headers
-            else:
-                assert six.viewitems(env) >= six.viewitems(headers)
-        assert body == env['wsgi.input'].read()
-        start_response('200 OK', [])
+            assert env.items() >= headers.items()
+        assert body == env["wsgi.input"].read()
+        start_response("200 OK", [])
         return []
+
     return wsgi_handler
 
 
 def internal_server_error():
     def wsgi_handler(env, start_response):
-        start_response('500 Internal Server Error', [])
+        start_response("500 Internal Server Error", [])
         return []
+
     return wsgi_handler
 
 
 def check_redirect():
     def wsgi_handler(env, start_response):
-        path_info = env.get('PATH_INFO')
+        path_info = env.get("PATH_INFO")
         if path_info == "/":
-            start_response('301 Moved Permanently', [('Location', 'http://127.0.0.1:54323/redirected')])
+            start_response("301 Moved Permanently", [("Location", LISTENER_URL + "redirected")])
             return []
         else:
             assert path_info == "/redirected"
-            start_response('200 OK', [])
+            start_response("200 OK", [])
             return [b"redirected"]
+
     return wsgi_handler
 
+
 def check_querystring():
     def wsgi_handler(env, start_response):
         querystring = env["QUERY_STRING"]
-        start_response('200 OK', [("Content-type", "text/plaim")])
+        start_response("200 OK", [("Content-type", "text/plaim")])
         return [querystring.encode("utf-8")]
+
     return wsgi_handler
 
+
 def set_cookie():
     def wsgi_handler(env, start_response):
-        start_response('200 OK', [('Set-Cookie', 'testcookie=testdata')])
+        start_response("200 OK", [("Set-Cookie", "testcookie=testdata")])
         return []
+
     return wsgi_handler
 
+
+def set_cookie_401():
+    def wsgi_handler(env, start_response):
+        start_response("401 Unauthorized", [("Set-Cookie", "testcookie=testdata")])
+        return []
+
+    return wsgi_handler
+
+
 def return_brotli():
     def wsgi_handler(env, start_response):
-        path_info = env.get('PATH_INFO')
+        path_info = env.get("PATH_INFO")
         if path_info == "/":
-            start_response('200 OK', [("Content-Encoding", "br")])
-        return [b"\x1b'\x00\x98\x04rq\x88\xa1'\xbf]\x12\xac+g!%\x98\xf4\x02\xc4\xda~)8\xba\x06xO\x11)Y\x02"]
+            start_response("200 OK", [("Content-Encoding", "br")])
+        return [
+            b"\x1b'\x00\x98\x04rq\x88\xa1'\xbf]\x12\xac+g!%\x98\xf4\x02\xc4\xda~)8\xba\x06xO\x11)Y\x02"
+        ]
+
     return wsgi_handler
 
 
-def test_file_post():
-    body = tempfile.NamedTemporaryFile("a+b", delete=False)
-    name = body.name
-    try:
-        body.write(b"123456789")
-        body.close()
-        headers = {'CONTENT_LENGTH': '9', 'CONTENT_TYPE': 'application/octet-stream'}
-        with wsgiserver(check_upload(b"123456789", headers)):
-            useragent = UserAgent()
-            with open(name, 'rb') as body:
-                useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=body)
-    finally:
-        os.remove(name)
+def test_file_post(tmp_file):
+    headers = {"CONTENT_LENGTH": "9", "CONTENT_TYPE": "application/octet-stream"}
+    with wsgiserver(check_upload(b"123456789", headers)):
+        useragent = UserAgent()
+        with open(tmp_file, "rb") as body:
+            useragent.urlopen(LISTENER_URL, method="POST", payload=body)
 
 
-def test_multipart_post():
-    body = tempfile.NamedTemporaryFile("a+b", delete=False)
-    name = body.name
-    try:
-        body.write(b"123456789")
-        headers = {'CONTENT_LENGTH': '237',
-                   'CONTENT_TYPE': 'multipart/form-data; boundary=custom_boundary'}
-        files = {'file': ('report.xls', body, 'application/vnd.ms-excel', {'Expires': '0'}, 'custom_boundary')}
-
-        with wsgiserver(check_upload((b'--custom_boundary\r\n'
-                                      b'Content-Disposition: form-data; name="files"\r\n'
-                                      b'\r\n'
-                                      b'file\r\n'
-                                      b'--custom_boundary\r\n'
-                                      b'Content-Disposition: form-data; name="file"; filename="report.xls"\r\n'
-                                      b'Content-Type: application/vnd.ms-excel\r\n'
-                                      b'Expires: 0\r\n'
-                                      b'\r\n'
-                                      b'\r\n'
-                                      b'--custom_boundary--'
-                                      b'\r\n'), headers)):
+def test_multipart_post(tmp_file):
+    with open(tmp_file, "a+b") as f:
+        headers = {
+            "CONTENT_LENGTH": "237",
+            "CONTENT_TYPE": "multipart/form-data; boundary=custom_boundary",
+        }
+        files = {
+            "file": (
+                "report.xls",
+                f,
+                "application/vnd.ms-excel",
+                {"Expires": "0"},
+                "custom_boundary",
+            )
+        }
+
+        with wsgiserver(
+            check_upload(
+                (
+                    b"--custom_boundary\r\n"
+                    b'Content-Disposition: form-data; name="files"\r\n'
+                    b"\r\n"
+                    b"file\r\n"
+                    b"--custom_boundary\r\n"
+                    b'Content-Disposition: form-data; name="file"; filename="report.xls"\r\n'
+                    b"Content-Type: application/vnd.ms-excel\r\n"
+                    b"Expires: 0\r\n"
+                    b"\r\n"
+                    b"\r\n"
+                    b"--custom_boundary--"
+                    b"\r\n"
+                ),
+                headers,
+            )
+        ):
             useragent = UserAgent()
-            useragent.urlopen('http://127.0.0.1:54323/', method='POST', files=files)
-    finally:
-        body.close()
-        os.remove(name)
+            useragent.urlopen(LISTENER_URL, method="POST", files=files)
 
 
 def test_unicode_post():
-    byte_string = b'\xc8\xb9\xc8\xbc\xc9\x85'
-    unicode_string = byte_string.decode('utf-8')
-    headers = {'CONTENT_LENGTH': str(len(byte_string)), 'CONTENT_TYPE': 'text/plain; charset=utf-8'}
+    byte_string = b"\xc8\xb9\xc8\xbc\xc9\x85"
+    unicode_string = byte_string.decode("utf-8")
+    headers = {
+        "CONTENT_LENGTH": str(len(byte_string)),
+        "CONTENT_TYPE": "text/plain; charset=utf-8",
+    }
     with wsgiserver(check_upload(byte_string, headers)):
         useragent = UserAgent()
-        useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=unicode_string)
+        useragent.urlopen(LISTENER_URL, method="POST", payload=unicode_string)
 
 
 def test_bytes_post():
-    headers = {'CONTENT_LENGTH': '5', 'CONTENT_TYPE': 'application/octet-stream'}
+    headers = {"CONTENT_LENGTH": "5", "CONTENT_TYPE": "application/octet-stream"}
     with wsgiserver(check_upload(b"12345", headers)):
         useragent = UserAgent()
-        useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=b"12345")
+        useragent.urlopen(LISTENER_URL, method="POST", payload=b"12345")
+
+
+def test_dict_post_with_content_type():
+    headers = {"Content-Type": "application/x-www-form-urlencoded"}
+    payload = {"foo": "bar"}
+    with wsgiserver(set_cookie()):  # lazy. I just want to see that we dont crash making the request
+        resp = UserAgent().urlopen(LISTENER_URL, method="POST", payload=payload, headers=headers)
+        assert resp.status_code == 200
 
 
 def test_redirect():
     with wsgiserver(check_redirect()):
-        resp = UserAgent().urlopen('http://127.0.0.1:54323/')
+        resp = UserAgent().urlopen(LISTENER_URL)
         assert resp.status_code == 200
         assert b"redirected" == resp.content
 
+
 def test_params():
     with wsgiserver(check_querystring()):
-        resp = UserAgent().urlopen('http://127.0.0.1:54323/?param1=b', params={"param2":"hello"})
+        resp = UserAgent().urlopen(LISTENER_URL + "?param1=b", params={"param2": "hello"})
         assert resp.status_code == 200
         assert resp.content == b"param1=b&param2=hello"
 
+
 def test_params_quoted():
     with wsgiserver(check_querystring()):
-        resp = UserAgent().urlopen('http://127.0.0.1:54323/?a/b', params={"path":"/"})
+        resp = UserAgent().urlopen(LISTENER_URL + "?a/b", params={"path": "/"})
         assert resp.status_code == 200
         assert resp.content == b"a/b&path=%2F"
 
+
 def test_server_error_with_bytes():
     with wsgiserver(internal_server_error()):
         useragent = UserAgent()
         with pytest.raises(BadStatusCode):
-            useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=b"12345")
+            useragent.urlopen(LISTENER_URL, method="POST", payload=b"12345")
 
 
 def test_server_error_with_unicode():
     with wsgiserver(internal_server_error()):
         useragent = UserAgent()
         with pytest.raises(BadStatusCode):
-            useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=u"12345")
+            useragent.urlopen(LISTENER_URL, method="POST", payload="12345")
 
 
-def test_server_error_with_file():
-    body = tempfile.NamedTemporaryFile("a+b", delete=False)
-    name = body.name
-    try:
-        body.write(b"123456789")
-        body.close()
-        with wsgiserver(internal_server_error()):
-            useragent = UserAgent()
-            with pytest.raises(BadStatusCode):
-                with open(name, 'rb') as body:
-                    useragent.urlopen('http://127.0.0.1:54323/', method='POST', payload=body)
-    finally:
-        os.remove(name)
+def test_server_error_with_file(tmp_file):
+    with wsgiserver(internal_server_error()):
+        useragent = UserAgent()
+        with pytest.raises(BadStatusCode):
+            with open(tmp_file, "rb") as body:
+                useragent.urlopen(LISTENER_URL, method="POST", payload=body)
 
 
 def test_cookiejar():
     with wsgiserver(set_cookie()):
         useragent = UserAgent(cookiejar=CookieJar())
-        assert b"" == useragent.urlopen('http://127.0.0.1:54323/').read()
+        assert b"" == useragent.urlopen(LISTENER_URL).read()
+
+
+def test_cookiejar_response_error():
+    with wsgiserver(set_cookie_401()):
+        useragent = UserAgent(cookiejar=CookieJar())
+        with pytest.raises(BadStatusCode):
+            assert b"" == useragent.urlopen(LISTENER_URL)
+
+        assert (
+            next(cookie for cookie in useragent.cookiejar if cookie.name == "testcookie").value
+            == "testdata"
+        )
 
 
 def test_brotli_response():
     with wsgiserver(return_brotli()):
-        resp = UserAgent().urlopen('http://127.0.0.1:54323/', params={"path":"/"})
+        resp = UserAgent().urlopen(LISTENER_URL, params={"path": "/"})
         assert resp.status_code == 200
         assert resp.content == b"https://github.com/gwik/geventhttpclient"
+
+
+@pytest.mark.network
+def test_download(tmp_path):
+    url = "https://proof.ovh.net/files/1Mb.dat"
+    fpath = tmp_path / url.rsplit("/", 1)[-1]
+    UserAgent().download(url, fpath)
+    assert fpath.stat().st_size == 2**20  # 1 MB
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/url.py` & `geventhttpclient-2.1.0/src/geventhttpclient/url.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-import six
-if six.PY3:
-    from urllib import parse as urlparse
-    from urllib.parse import urlencode
-    from urllib.parse import quote_plus
-    from collections.abc import Mapping
-    basestring = (str, bytes)
-else:
-    import urlparse
-    from urllib import quote_plus, urlencode
-    from collections import Mapping
-
-DEFAULT_PORTS = {
-    'http': 80,
-    'https': 443
-}
+from collections.abc import Mapping
+from urllib import parse as urlparse
+from urllib.parse import urlencode
+
+DEFAULT_PORTS = {"http": 80, "https": 443}
 
 
 def to_key_val_list(value):
     """Take an object and test to see if it can be represented as a
     dictionary. If it can be, return a list of tuples, e.g.,
     ::
         >>> to_key_val_list([('key', 'val')])
@@ -30,24 +19,24 @@
         ValueError: cannot encode objects that are not 2-tuples
     :rtype: list
     """
     if value is None:
         return None
 
     if isinstance(value, (str, bytes, bool, int)):
-        raise ValueError('cannot encode objects that are not 2-tuples')
+        raise ValueError("cannot encode objects that are not 2-tuples")
 
     if isinstance(value, Mapping):
         value = value.items()
 
     return list(value)
 
 
-class URL(object):
-    """ A mutable URL class
+class URL:
+    """A mutable URL class
 
     You build it from a url string.
     >>> url = URL('http://getgauss.com/urls?param=asdfa')
     >>> url
     URL(http://getgauss.com/urls?param=asdfa)
 
     You cast it to a tuple, it returns the same tuple as `urlparse.urlsplit`.
@@ -60,175 +49,197 @@
 
     You can change attributes.
     >>> url.host = 'infrae.com'
     >>> url
     URL(http://infrae.com/urls?auth_token=asdfaisdfuasdf&param=asdfa)
     """
 
-    __slots__ = ('scheme', 'host', 'port', 'path', 'query', 'fragment', 'user', 'password', 'params')
-    quoting_safe = ''
+    __slots__ = (
+        "scheme",
+        "host",
+        "port",
+        "path",
+        "query",
+        "fragment",
+        "user",
+        "password",
+        "params",
+    )
+    quoting_safe = ""
 
     def __init__(self, url=None, params=None):
         if url is not None:
             scheme, netloc, path, query, fragment = urlparse.urlsplit(url)
         else:
-            scheme, netloc, path, query, fragment = 'http', '', '/', '', ''
+            scheme, netloc, path, query, fragment = "http", "", "/", "", ""
 
         self.scheme = scheme
         self.fragment = fragment
 
-        user, password, host, port = None, None, '', None
+        user, password, host, port = None, None, "", None
         if netloc:
-            if '@' in netloc:
-                user_pw, netloc = netloc.rsplit('@', 1)
-                if ':' in user_pw:
-                    user, password = user_pw.rsplit(':', 1)
+            if "@" in netloc:
+                user_pw, netloc = netloc.rsplit("@", 1)
+                if ":" in user_pw:
+                    user, password = user_pw.rsplit(":", 1)
                 else:
                     user = user_pw
 
-            if netloc.startswith('['):
-                host, port_pt = netloc.rsplit(']', 1)
-                host = host.strip('[]')
+            if netloc.startswith("["):
+                host, port_pt = netloc.rsplit("]", 1)
+                host = host.strip("[]")
                 if port_pt:
-                    port = int(port_pt.strip(':'))
+                    port = int(port_pt.strip(":"))
             else:
-                if ':' in netloc:
-                    host, port = netloc.rsplit(':', 1)
+                if ":" in netloc:
+                    host, port = netloc.rsplit(":", 1)
                     port = int(port)
                 else:
                     host = netloc
 
         if not port:
             port = DEFAULT_PORTS.get(self.scheme)
 
         self.host = host
         self.port = port
         self.user = user
         self.password = password
 
-        self.path = path or ''
-        
-        self.query = query
+        self.path = path or ""
+
+        self.query = query.replace(
+            " ", "%20"
+        )  # get a little closer to the behaviour of requests.utils.requote_uri
         self.params = params
 
     @property
     def netloc(self):
         return self.full_netloc(auth=False)
 
     def full_netloc(self, auth=True):
-        buf = ''
+        buf = ""
         if self.user and auth:
             buf += self.user
-            if self.passwort:
-                buf += ':' + self.passwort
-            buf += '@'
+            if self.password:
+                buf += ":" + self.password
+            buf += "@"
 
-        if ':' in self.host:
-            buf += '[' + self.host + ']'
+        if ":" in self.host:
+            buf += "[" + self.host + "]"
         else:
             buf += self.host
         if self.port is None:
             return buf
         elif DEFAULT_PORTS.get(self.scheme) == self.port:
             return buf
-        buf += ':' + str(self.port)
+        buf += ":" + str(self.port)
         return buf
 
     def __copy__(self):
         clone = type(self)()
         for key in self.__slots__:
             val = getattr(self, key)
             if isinstance(val, dict):
                 val = val.copy()
             setattr(clone, key, val)
         return clone
 
     def __repr__(self):
-        return "URL(%s)" % str(self)
+        return f"URL({self})"
 
     def __iter__(self):
-        return iter((self.scheme, self.full_netloc(), self.path,
-                self.query_string, self.fragment))
+        return iter(
+            (
+                self.scheme,
+                self.full_netloc(),
+                self.path,
+                self.query_string,
+                self.fragment,
+            )
+        )
 
     def __str__(self):
         return urlparse.urlunsplit(tuple(self))
 
     def __eq__(self, other):
         return str(self) == str(other)
-    
+
     @staticmethod
     def _encode_params(data):
         """Encode parameters in a piece of data.
         Will successfully encode parameters when passed as a dict or a list of
         2-tuples.
         """
 
         if isinstance(data, (str, bytes)):
             return data
-        elif hasattr(data, 'read'):
+        elif hasattr(data, "read"):
             return data
-        elif hasattr(data, '__iter__'):
+        elif hasattr(data, "__iter__"):
             result = []
             for k, vs in to_key_val_list(data):
-                if isinstance(vs, basestring) or not hasattr(vs, '__iter__'):
+                if isinstance(vs, (str, bytes)) or not hasattr(vs, "__iter__"):
                     vs = [vs]
                 for v in vs:
                     if v is not None:
                         result.append(
-                            (k.encode('utf-8') if isinstance(k, str) else k,
-                             v.encode('utf-8') if isinstance(v, str) else v))
+                            (
+                                k.encode("utf-8") if isinstance(k, str) else k,
+                                v.encode("utf-8") if isinstance(v, str) else v,
+                            )
+                        )
             return urlencode(result, doseq=True)
         else:
             return data
-    
+
     @property
     def query_string(self):
         query = []
         if self.query:
             query.append(self.query)
         if self.params:
             query.append(self._encode_params(self.params))
         return "&".join(query)
 
     @property
     def request_uri(self):
         query = self.query_string
         if not query:
             return self.path
-        return self.path + '?' + query
+        return self.path + "?" + query
 
     def append_to_path(self, value):
-        if value.startswith('/'):
-            if self.path.endswith('/'):
+        if value.startswith("/"):
+            if self.path.endswith("/"):
                 self.path += value[1:]
                 return self.path
         elif not self.path.endswith("/"):
             self.path += "/" + value
             return self.path
 
         self.path += value
         return self.path
 
     def redirect(self, other):
-        """ Redirect to the other URL, relative to the current one """
+        """Redirect to the other URL, relative to the current one"""
         if not isinstance(other, type(self)):
             other = type(self)(other)
         if not other.host:
             other.scheme = self.scheme
             other.host = self.host
             other.port = self.port
-        if not other.path.startswith('/'):
-            if self.path.endswith('/'):
+        if not other.path.startswith("/"):
+            if self.path.endswith("/"):
                 other.path = self.path + other.path
             else:
-                other.path = self.path.rsplit('/', 1)[0] + '/' + other.path
+                other.path = self.path.rsplit("/", 1)[0] + "/" + other.path
         return other
 
     def stripped_auth(self):
-        """ Remove fragment and authentication for proxy handling """
+        """Remove fragment and authentication for proxy handling"""
         clone = type(self)()
         # Copy all fields except fragment, username and password
         for key in self.__slots__[:5]:
             val = getattr(self, key)
             if isinstance(val, dict):
                 val = val.copy()
             setattr(clone, key, val)
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient/useragent.py` & `geventhttpclient-2.1.0/src/geventhttpclient/useragent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,49 @@
-import socket
 import errno
-import six
-import sys
+import os
+import socket
 import ssl
+import sys
 import zlib
-import os
-import brotli
-from six.moves import xrange, cStringIO
-from six.moves.urllib.parse import urlencode
-from six import print_, reraise, string_types, text_type
+from urllib.parse import urlencode
 
+import brotli
 import gevent
 from urllib3 import encode_multipart_formdata
 from urllib3.fields import RequestField
 
-try:
-    from gevent.dns import DNSError
-except ImportError:
-    class DNSError(Exception): pass
-
-from .url import URL, to_key_val_list
 from .client import HTTPClient, HTTPClientPool
-
-basestring = (str, bytes)
+from .url import URL, to_key_val_list
 
 
 class ConnectionError(Exception):
     def __init__(self, url, *args, **kwargs):
         self.url = url
         self.__dict__.update(kwargs)
-        if args and isinstance(args[0], string_types):
-            try:
-                self.text = args[0] % args[1:]
-            except TypeError:
-                self.text = args[0] + ': ' + str(args[1:]) if args else ''
+        if args and isinstance(args[0], str):
+            self.text = args[0] + ": " + str(args[1:])
         else:
-            self.text = str(args[0]) if len(args) == 1 else ''
+            self.text = str(args[0]) if len(args) == 1 else ""
         if kwargs:
-            self.text += ', ' if self.text else ''
-            self.kwargs_text = ', '.join('%s=%s' % (key, val) for key, val in six.iteritems(kwargs))
+            self.text += ", " if self.text else ""
+            self.kwargs_text = ", ".join(f"{key}={val}" for key, val in kwargs.items())
             self.text += self.kwargs_text
         else:
-            self.text = ''
+            self.text = ""
 
     def __str__(self):
         if self.text:
-            return "URL %s: %s" % (self.url, self.text)
+            return f"URL {self.url}: {self.text}"
         else:
-            return "URL %s" % self.url
+            return f"URL {self.url}"
 
     def __repr__(self):
         repr_str = super().__repr__()
         if self.kwargs_text:
-            return repr_str.replace(')', ''.join([', ', self.kwargs_text, ')']))
+            return repr_str.replace(")", "".join([", ", self.kwargs_text, ")"]))
         return repr_str
 
 
 class RetriesExceeded(ConnectionError):
     pass
 
 
@@ -64,20 +51,20 @@
     pass
 
 
 class EmptyResponse(ConnectionError):
     pass
 
 
-class CompatRequest(object):
-    """ urllib / cookielib compatible request class.
-        See also: http://docs.python.org/library/cookielib.html
+class CompatRequest:
+    """urllib / cookielib compatible request class.
+    See also: http://docs.python.org/library/cookielib.html
     """
 
-    def __init__(self, url, method='GET', headers=None, payload=None, params=None):
+    def __init__(self, url, method="GET", headers=None, payload=None, params=None):
         self.params = params
         self.set_url(url)
         self.original_host = self.url_split.host
         self.method = method
         self.headers = headers
         self.payload = payload
 
@@ -98,16 +85,15 @@
     def get_type(self):
         return self.url_split.scheme
 
     def get_origin_req_host(self):
         return self.original_host
 
     def is_unverifiable(self):
-        """ See http://tools.ietf.org/html/rfc2965.html. Not fully implemented!
-        """
+        """See http://tools.ietf.org/html/rfc2965.html. Not fully implemented!"""
         return False
 
     @property
     def unverifiable(self):
         return self.is_unverifiable()
 
     def get_header(self, header_name, default=None):
@@ -119,62 +105,59 @@
     def header_items(self):
         return self.headers.items()
 
     def add_unredirected_header(self, key, val):
         self.headers.add(key, val)
 
     def _drop_payload(self):
-        self.method = 'GET'
+        self.method = "GET"
         self.payload = None
-        for item in ('content-length', 'content-type', 'content-encoding'):
+        for item in ("content-length", "content-type", "content-encoding"):
             self.headers.discard(item)
 
     def _drop_cookies(self):
-        for item in ('cookie', 'cookie2'):
+        for item in ("cookie", "cookie2"):
             self.headers.discard(item)
 
     def redirect(self, code, location):
-        """ Modify the request inplace to point to the new location """
+        """Modify the request inplace to point to the new location"""
         self.set_url(self.url_split.redirect(location))
         if code in (302, 303):
             self._drop_payload()
         self._drop_cookies()
 
 
-class CompatResponse(object):
-    """ Adapter for urllib responses with some extensions
-    """
-    __slots__ = 'headers', '_response', '_request', '_sent_request', '_cached_content'
+class CompatResponse:
+    """Adapter for urllib responses with some extensions"""
+
+    __slots__ = "headers", "_response", "_request", "_sent_request", "_cached_content"
 
     def __init__(self, ghc_response, request=None, sent_request=None):
         self._response = ghc_response
         self._request = request
         self._sent_request = sent_request
         self.headers = self._response._headers_index
 
     @property
     def status(self):
-        """ The returned http status
-        """
+        """The returned http status"""
         # TODO: Should be a readable string
         return str(self.status_code)
 
     @property
     def status_code(self):
-        """ The http status code as plain integer
-        """
+        """The http status code as plain integer"""
         return self._response.get_code()
 
     @property
     def stream(self):
         return self._response
 
     def read(self, n=None):
-        """ Read n bytes from the response body
-        """
+        """Read n bytes from the response body"""
         return self._response.read(n)
 
     def readline(self):
         return self._response.readline()
 
     def release(self):
         return self._response.release()
@@ -191,93 +174,81 @@
             try:
                 return zlib.decompress(bodystr, -zlib.MAX_WBITS)
             except zlib.error:
                 return zlib.decompress(bodystr)
 
     @property
     def content(self):
-        """ Unzips if necessary and buffers the received body. Careful with large files!
-        """
+        """Unzips if necessary and buffers the received body. Careful with large files!"""
         try:
             return self._cached_content
         except AttributeError:
             self._cached_content = self._content()
             return self._cached_content
 
     def _content(self):
         try:
-            content_type = self.headers.getheaders('content-encoding')[0].lower()
+            content_type = self.headers.getheaders("content-encoding")[0].lower()
         except IndexError:
             # No content-encoding header set
-            content_type = 'identity'
+            content_type = "identity"
 
-        if content_type == 'gzip':
+        if content_type == "gzip":
             ret = self.unzipped(gzip=True)
-        elif content_type == 'deflate':
+        elif content_type == "deflate":
             ret = self.unzipped(gzip=False)
-        elif content_type == 'identity':
+        elif content_type == "identity":
             ret = self._response.read()
-        elif content_type == 'br':
+        elif content_type == "br":
             ret = self.unzipped(gzip=False, br=True)
-        elif content_type == 'compress':
-            raise ValueError("Compression type not supported: %s" % content_type)
+        elif content_type == "compress":
+            raise ValueError(f"Compression type not supported: {content_type}")
         else:
-            raise ValueError("Unknown content encoding: %s" % content_type)
+            raise ValueError(f"Unknown content encoding: {content_type}")
 
         self.release()
         return ret
 
     def __len__(self):
-        """ The content lengths as should be returned from the headers
-        """
+        """The content lengths as should be returned from the headers"""
         try:
-            return int(self.headers.getheaders('content-length')[0])
+            return int(self.headers.getheaders("content-length")[0])
         except (IndexError, ValueError):
             return len(self.content)
 
     def __nonzero__(self):
-        """ If we have an empty response body, we still don't want to evaluate as false
-        """
+        """If we have an empty response body, we still don't want to evaluate as false"""
         return True
 
     def info(self):
-        """ Adaption to cookielib: Alias for headers
-        """
+        """Adaption to cookielib: Alias for headers"""
         return self.headers
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.release()
 
 
-class RestkitCompatResponse(CompatResponse):
-    """ Some extra lines to also serve as a drop in replacement for restkit
-    """
-
-    def body_string(self):
-        return self.content
-
-    def body_stream(self):
-        return self._response
-
-    @property
-    def status_int(self):
-        return self.status_code
-
-
-class UserAgent(object):
+class UserAgent:
     response_type = CompatResponse
     request_type = CompatRequest
     valid_response_codes = frozenset([200, 206, 301, 302, 303, 307])
     redirect_resonse_codes = frozenset([301, 302, 303, 307])
 
-    def __init__(self, max_redirects=3, max_retries=3, retry_delay=0,
-                 cookiejar=None, headers=None, **kwargs):
+    def __init__(
+        self,
+        max_redirects=3,
+        max_retries=3,
+        retry_delay=0,
+        cookiejar=None,
+        headers=None,
+        **kwargs,
+    ):
         self.max_redirects = int(max_redirects)
         self.max_retries = int(max_retries)
         self.retry_delay = retry_delay
         self.default_headers = HTTPClient.DEFAULT_HEADERS.copy()
         if headers:
             self.default_headers.update(headers)
         self.cookiejar = cookiejar
@@ -285,43 +256,49 @@
 
     def close(self):
         self.clientpool.close()
 
     def __del__(self):
         self.close()
 
-    def _make_request(self, url, method='GET', headers=None, payload=None, params=None, files=None):
+    def _make_request(self, url, method="GET", headers=None, payload=None, params=None, files=None):
         req_headers = self.default_headers.copy()
         if headers:
             req_headers.update(headers)
         if payload or files:
             # Adjust headers depending on payload content
-            content_type = req_headers.get('content-type', None)
+            content_type = req_headers.get("content-type", None)
             if files:
                 (body, content_type) = self._encode_files(files, payload)
                 payload = body
-                req_headers['content-type'] = content_type
-            if not content_type and isinstance(payload, dict):
-                req_headers['content-type'] = "application/x-www-form-urlencoded; charset=utf-8"
+                req_headers["content-type"] = content_type
+            if isinstance(payload, dict):
+                if not content_type:
+                    req_headers["content-type"] = "application/x-www-form-urlencoded; charset=utf-8"
                 payload = urlencode(payload)
-            elif not content_type and isinstance(payload, text_type):
-                req_headers['content-type'] = 'text/plain; charset=utf-8'
+            elif not content_type and isinstance(payload, str):
+                req_headers["content-type"] = "text/plain; charset=utf-8"
             elif not content_type:
-                req_headers['content-type'] = 'application/octet-stream'
-        return self.request_type(url, method=method, headers=req_headers, payload=payload, params=params)
+                req_headers["content-type"] = "application/octet-stream"
+        return self.request_type(
+            url, method=method, headers=req_headers, payload=payload, params=params
+        )
 
     def _urlopen(self, request):
         client = self.clientpool.get_client(request.url_split)
-        resp = client.request(request.method, request.url_split.request_uri,
-                              body=request.payload, headers=request.headers)
+        resp = client.request(
+            request.method,
+            request.url_split.request_uri,
+            body=request.payload,
+            headers=request.headers,
+        )
         return self.response_type(resp, request=request, sent_request=resp._sent_request)
 
     def _verify_status(self, status_code, url=None):
-        """ Hook for subclassing
-        """
+        """Hook for subclassing"""
         if status_code not in self.valid_response_codes:
             raise BadStatusCode(url, code=status_code)
 
     def _encode_files(self, files, data):
         """
         Method taken from models in requests library , usage is the same. Only difference is that you can add custom
         boundary in 5-tuple version.
@@ -341,40 +318,37 @@
         example:
         files = {'file': ('report.xls', body, 'application/vnd.ms-excel', {'Expires': '0'}, 'custom_boundary')}
 
         """
 
         if not files:
             raise ValueError("Files must be provided.")
-        elif isinstance(data, basestring):
+        elif isinstance(data, (str, bytes)):
             raise ValueError("Data must not be a string.")
 
         new_fields = []
         fields = to_key_val_list(data or {})
         files = to_key_val_list(files or {})
 
         for field, val in fields:
-            if isinstance(val, basestring) or not hasattr(val, "__iter__"):
+            if isinstance(val, (str, bytes)) or not hasattr(val, "__iter__"):
                 val = [val]
             for v in val:
                 if v is not None:
-                    # Don't call str() on bytestrings: in Py3 it all goes wrong.
                     if not isinstance(v, bytes):
                         v = str(v)
 
                     new_fields.append(
                         (
-                            field.decode("utf-8")
-                            if isinstance(field, bytes)
-                            else field,
+                            field.decode("utf-8") if isinstance(field, bytes) else field,
                             v.encode("utf-8") if isinstance(v, str) else v,
                         )
                     )
 
-        for (k, v) in files:
+        for k, v in files:
             # support for explicit filename
             ft = None
             fh = None
             boundary = None
             if isinstance(v, (tuple, list)):
                 if len(v) == 2:
                     fn, fp = v
@@ -402,88 +376,109 @@
             new_fields.append(rf)
 
         body, content_type = encode_multipart_formdata(new_fields, boundary)
 
         return body, content_type
 
     def _handle_error(self, e, url=None):
-        """ Hook for subclassing. Raise the error to interrupt further retrying,
-            return it to continue retries and save the error, when retries
-            exceed the limit.
-            Temporary errors should be swallowed here for automatic retries.
+        """Hook for subclassing. Raise the error to interrupt further retrying,
+        return it to continue retries and save the error, when retries
+        exceed the limit.
+        Temporary errors should be swallowed here for automatic retries.
         """
         if isinstance(e, (socket.timeout, gevent.Timeout)):
             return e
-        elif isinstance(e, (socket.error, DNSError)) and \
-                e.errno in set([errno.ETIMEDOUT, errno.ENOLINK, errno.ENOENT, errno.EPIPE]):
+        elif isinstance(e, socket.error) and e.errno in {
+            errno.ETIMEDOUT,
+            errno.ENOLINK,
+            errno.ENOENT,
+            errno.EPIPE,
+        }:
             return e
-        elif isinstance(e, ssl.SSLError) and 'read operation timed out' in str(e):
+        elif isinstance(e, ssl.SSLError) and "read operation timed out" in str(e):
             return e
         elif isinstance(e, EmptyResponse):
             return e
-        raise reraise(type(e), e, sys.exc_info()[2])
+        raise e.with_traceback(sys.exc_info()[2])
 
     def _handle_retries_exceeded(self, url, last_error=None):
-        """ Hook for subclassing
-        """
+        """Hook for subclassing"""
         raise RetriesExceeded(url, self.max_retries, original=last_error)
 
-    def urlopen(self, url, method='GET', response_codes=valid_response_codes,
-                headers=None, payload=None, to_string=False, debug_stream=None, params=None, **kwargs):
-        """ Open an URL, do retries and redirects and verify the status code
-        """
+    def urlopen(
+        self,
+        url,
+        method="GET",
+        response_codes=valid_response_codes,
+        headers=None,
+        payload=None,
+        to_string=False,
+        debug_stream=None,
+        params=None,
+        **kwargs,
+    ):
+        """Open an URL, do retries and redirects and verify the status code"""
         # POST or GET parameters can be passed in **kwargs
         if kwargs:
             if not payload:
                 payload = kwargs
             elif isinstance(payload, dict):
                 payload.update(kwargs)
             files = kwargs.get("files", None)
         else:
             files = None
-        req = self._make_request(url, method=method, headers=headers, payload=payload, params=params, files=files)
-        for retry in xrange(self.max_retries):
+        req = self._make_request(
+            url,
+            method=method,
+            headers=headers,
+            payload=payload,
+            params=params,
+            files=files,
+        )
+        for retry in range(self.max_retries):
             if retry > 0 and self.retry_delay:
                 # Don't wait the first time and skip if no delay specified
                 gevent.sleep(self.retry_delay)
-            for _ in xrange(self.max_redirects):
+            for _ in range(self.max_redirects):
                 if self.cookiejar is not None:
                     self.cookiejar.add_cookie_header(req)
 
                 try:
                     resp = self._urlopen(req)
                 except gevent.GreenletExit:
                     raise
                 except BaseException as e:
                     e.request = req
                     last_error = self._handle_error(e, url=req.url)
                     break  # Continue with next retry
 
                 # We received a response
                 if debug_stream is not None:
-                    debug_stream.write(self._conversation_str(req.url, resp, payload=req.payload) + '\n\n')
+                    debug_stream.write(
+                        self._conversation_str(req.url, resp, payload=req.payload) + "\n\n"
+                    )
+
+                if self.cookiejar is not None:
+                    self.cookiejar.extract_cookies(resp, req)
 
                 try:
                     self._verify_status(resp.status_code, url=req.url)
                 except Exception as e:
                     # Basic transmission successful, but not the wished result
                     # Let's collect some debug info
                     e.response = resp
                     e.request = req
                     e.http_log = self._conversation_str(req.url, resp, payload=req.payload)
                     resp.release()
                     last_error = self._handle_error(e, url=req.url)
                     break  # Continue with next retry
 
-                if self.cookiejar is not None:
-                    self.cookiejar.extract_cookies(resp, req)
-
-                redirection = resp.headers.get('location')
-                if isinstance(redirection, six.binary_type):
-                    redirection = redirection.decode('utf-8')
+                redirection = resp.headers.get("location")
+                if isinstance(redirection, bytes):
+                    redirection = redirection.decode("utf-8")
                 if resp.status_code in self.redirect_resonse_codes and redirection:
                     resp.release()
                     try:
                         req.redirect(resp.status_code, redirection)
                         continue
                     except Exception as e:
                         last_error = self._handle_error(e, url=req.url)
@@ -503,101 +498,89 @@
                         if not ret:
                             e = EmptyResponse(url, "Empty response body received")
                             last_error = self._handle_error(e, url=req.url)
                             break
                         else:
                             return ret
             else:
-                e = RetriesExceeded(url, "Redirection limit reached (%s)" % self.max_redirects)
+                e = RetriesExceeded(url, f"Redirection limit reached ({self.max_redirects})")
                 last_error = self._handle_error(e, url=url)
         else:
             return self._handle_retries_exceeded(url, last_error=last_error)
 
     @classmethod
     def _conversation_str(cls, url, resp, payload=None):
-        if six.PY2:
-            header_str = '\n'.join('%s: %s' % item for item in resp.headers.iteroriginal())
-            ret = 'REQUEST: ' + url + '\n' + resp._sent_request
-            if payload and isinstance(payload, string_types):
-                ret += payload + '\n\n'
-            ret += 'RESPONSE: ' + resp._response.version + ' ' + \
-                   str(resp.status_code) + '\n' + \
-                   header_str + '\n\n' + resp.content
-        else:
-            header_str = '\n'.join('%s: %s' % item for item in resp.headers.iteroriginal())
-            ret = 'REQUEST: ' + url + '\n' + resp._sent_request
-            if payload:
-                if isinstance(payload, six.binary_type):
-                    try:
-                        ret += payload.decode('utf-8') + '\n\n'
-                    except UnicodeDecodeError:
-                        ret += 'UnicodeDecodeError' + '\n\n'
-                elif isinstance(payload, six.text_type):
-                    ret += payload + '\n\n'
-            ret += 'RESPONSE: ' + resp._response.version + ' ' + \
-                   str(resp.status_code) + '\n' + \
-                   header_str + '\n\n' + resp.content[:].decode('utf-8')
+        header_str = "\n".join(f"{key}: {val}" for key, val in resp.headers.iteroriginal())
+        ret = "REQUEST: " + url + "\n" + resp._sent_request
+        if payload:
+            if isinstance(payload, bytes):
+                try:
+                    ret += payload.decode("utf-8") + "\n\n"
+                except UnicodeDecodeError:
+                    ret += "UnicodeDecodeError" + "\n\n"
+            elif isinstance(payload, str):
+                ret += payload + "\n\n"
+        ret += (
+            "RESPONSE: "
+            + resp._response.version
+            + " "
+            + str(resp.status_code)
+            + "\n"
+            + header_str
+            + "\n\n"
+            + resp.content[:].decode("utf-8")
+        )
         return ret
 
     @classmethod
     def guess_filename(cls, file):
         """Tries to guess the filename of the given object."""
         name = getattr(file, "name", None)
-        if name and isinstance(name, basestring) and name[0] != "<" and name[-1] != ">":
+        if name and isinstance(name, (str, bytes)) and name[0] != "<" and name[-1] != ">":
             return os.path.basename(name)
 
     def download(self, url, fpath, chunk_size=16 * 1024, resume=False, **kwargs):
-        kwargs.pop('to_string', None)
-        headers = kwargs.pop('headers', {})
-        headers['Connection'] = 'Keep-Alive'
+        kwargs.pop("to_string", None)
+        headers = kwargs.pop("headers", {})
+        headers["Connection"] = "Keep-Alive"
         if resume and os.path.isfile(fpath):
             offset = os.path.getsize(fpath)
         else:
             offset = 0
 
-        for _ in xrange(self.max_retries):
+        for _ in range(self.max_retries):
             if offset:
-                headers['Range'] = 'bytes=%d-' % offset
+                headers["Range"] = f"bytes={offset}-"
                 resp = self.urlopen(url, headers=headers, **kwargs)
-                cr = resp.headers.get('Content-Range')
-                if resp.status_code != 206 or not cr or not cr.startswith('bytes') or \
-                        not cr.split(None, 1)[1].startswith(str(offset)):
+                cr = resp.headers.get("Content-Range")
+                if (
+                    resp.status_code != 206
+                    or not cr
+                    or not cr.startswith("bytes")
+                    or not cr.split(None, 1)[1].startswith(str(offset))
+                ):
                     resp.release()
                     offset = 0
             if not offset:
-                headers.pop('Range', None)
+                headers.pop("Range", None)
                 resp = self.urlopen(url, headers=headers, **kwargs)
 
-            with open(fpath, 'ab' if offset else 'wb') as f:
+            with open(fpath, "ab" if offset else "wb") as f:
                 if offset:
                     f.seek(offset, os.SEEK_SET)
                 try:
                     data = resp.read(chunk_size)
                     with resp:
                         while data:
                             f.write(data)
                             data = resp.read(chunk_size)
                 except BaseException as e:
                     self._handle_error(e, url=url)
-                    if resp.headers.get('accept-ranges') == 'bytes':
+                    if resp.headers.get("accept-ranges") == "bytes":
                         # Only if this header is set, we can fall back to partial download
                         offset = f.tell()
                     continue
             # All done, break outer loop
             break
         else:
             self._handle_retries_exceeded(url, last_error=e)
         return resp
-
-
-class RestkitCompatUserAgent(UserAgent):
-    response_type = RestkitCompatResponse
-
-
-class XmlrpcCompatUserAgent(UserAgent):
-    def request(self, host, handler, request, verbose=False):
-        debug_stream = None if not verbose else cStringIO.StringIO()
-        ret = self.urlopen(host + handler, 'POST', payload=request, to_string=True, debug_stream=debug_stream)
-        if debug_stream is not None:
-            debug_stream.seek(0)
-            print_(debug_stream.read())
-        return ret
```

### Comparing `geventhttpclient-2.0b1/src/geventhttpclient.egg-info/SOURCES.txt` & `geventhttpclient-2.1.0/src/geventhttpclient.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 LICENSE.txt
 MANIFEST.in
-README.mdown
-pytest.ini
+README.md
+pyproject.toml
 setup.py
 ext/Python_compat.h
 ext/_parser.c
-ext/api.c
-ext/http.c
-ext/llhttp.c
-ext/llhttp.h
+llhttp/LICENSE-MIT
+llhttp/include/llhttp.h
+llhttp/src/api.c
+llhttp/src/http.c
+llhttp/src/llhttp.c
 src/geventhttpclient/__init__.py
 src/geventhttpclient/client.py
 src/geventhttpclient/connectionpool.py
 src/geventhttpclient/header.py
 src/geventhttpclient/httplib.py
 src/geventhttpclient/response.py
 src/geventhttpclient/url.py
 src/geventhttpclient/useragent.py
 src/geventhttpclient.egg-info/PKG-INFO
 src/geventhttpclient.egg-info/SOURCES.txt
 src/geventhttpclient.egg-info/dependency_links.txt
 src/geventhttpclient.egg-info/requires.txt
 src/geventhttpclient.egg-info/top_level.txt
+src/geventhttpclient/tests/conftest.py
 src/geventhttpclient/tests/oncert.pem
 src/geventhttpclient/tests/server.crt
 src/geventhttpclient/tests/server.key
 src/geventhttpclient/tests/test_client.py
 src/geventhttpclient/tests/test_headers.py
+src/geventhttpclient/tests/test_http_host.py
 src/geventhttpclient/tests/test_httplib.py
 src/geventhttpclient/tests/test_keep_alive.py
 src/geventhttpclient/tests/test_network_failures.py
 src/geventhttpclient/tests/test_no_module_ssl.py
 src/geventhttpclient/tests/test_parser.py
 src/geventhttpclient/tests/test_ssl.py
 src/geventhttpclient/tests/test_url.py
```

