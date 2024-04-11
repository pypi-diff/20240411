# Comparing `tmp/tremolo-0.0.503.tar.gz` & `tmp/tremolo-0.0.504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tux/tremolo/dist/.tmp-mk54b5aq/tremolo-0.0.503.tar", last modified: Thu Apr  4 22:18:14 2024, max compression
+gzip compressed data, was "/home/tux/tremolo/dist/.tmp-3of1j8yj/tremolo-0.0.504.tar", last modified: Thu Apr 11 07:59:52 2024, max compression
```

## Comparing `tremolo-0.0.503.tar` & `tremolo-0.0.504.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.503/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.503/MANIFEST.in
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-04 22:18:14.000000 tremolo-0.0.503/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.503/README.md
--rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.503/pyproject.toml
--rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-04 22:18:14.000000 tremolo-0.0.503/setup.cfg
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/
--rw-r--r--   0 tux       (1000) users      (100)      308 2024-04-04 22:17:18.000000 tremolo-0.0.503/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.503/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.503/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     9894 2024-03-30 10:03:11.000000 tremolo-0.0.503/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/handlers.py
--rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-27 21:22:49.000000 tremolo-0.0.503/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/lib/
--rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/connections.py
--rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.503/tremolo/lib/contexts.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/h1parser/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     6101 2024-03-05 06:08:34.000000 tremolo-0.0.503/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/http_exception.py
--rw-r--r--   0 tux       (1000) users      (100)    18343 2024-03-16 12:09:02.000000 tremolo-0.0.503/tremolo/lib/http_protocol.py
--rw-r--r--   0 tux       (1000) users      (100)    12797 2024-03-08 01:51:43.000000 tremolo-0.0.503/tremolo/lib/http_request.py
--rw-r--r--   0 tux       (1000) users      (100)    15760 2024-04-04 21:42:22.000000 tremolo-0.0.503/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/locks.py
--rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.503/tremolo/lib/pools.py
--rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.503/tremolo/lib/queue.py
--rw-r--r--   0 tux       (1000) users      (100)     1199 2024-03-08 01:52:01.000000 tremolo-0.0.503/tremolo/lib/request.py
--rw-r--r--   0 tux       (1000) users      (100)     1460 2024-04-01 02:53:44.000000 tremolo-0.0.503/tremolo/lib/response.py
--rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/tasks.py
--rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.503/tremolo/lib/websocket.py
--rw-r--r--   0 tux       (1000) users      (100)    28028 2024-04-04 22:17:18.000000 tremolo-0.0.503/tremolo/tremolo.py
--rw-r--r--   0 tux       (1000) users      (100)     1095 2024-04-04 21:42:22.000000 tremolo-0.0.503/tremolo/utils.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      778 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2024-04-04 22:18:14.000000 tremolo-0.0.503/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2024-02-01 14:00:19.000000 tremolo-0.0.504/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)       63 2024-03-16 12:09:02.000000 tremolo-0.0.504/MANIFEST.in
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-11 07:59:52.000000 tremolo-0.0.504/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     5683 2024-02-01 14:00:19.000000 tremolo-0.0.504/README.md
+-rw-r--r--   0 tux       (1000) users      (100)     1016 2024-03-16 12:09:02.000000 tremolo-0.0.504/pyproject.toml
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-11 07:59:52.000000 tremolo-0.0.504/setup.cfg
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/
+-rw-r--r--   0 tux       (1000) users      (100)      308 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     7213 2024-02-05 09:58:51.000000 tremolo-0.0.504/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2674 2024-02-20 23:07:43.000000 tremolo-0.0.504/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     9917 2024-04-11 02:23:44.000000 tremolo-0.0.504/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      681 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)     1139 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/handlers.py
+-rw-r--r--   0 tux       (1000) users      (100)    11708 2024-03-27 21:22:49.000000 tremolo-0.0.504/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/lib/
+-rw-r--r--   0 tux       (1000) users      (100)        0 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      603 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/connections.py
+-rw-r--r--   0 tux       (1000) users      (100)      671 2024-02-05 09:57:05.000000 tremolo-0.0.504/tremolo/lib/contexts.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       52 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/h1parser/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     6075 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     2084 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/http_exception.py
+-rw-r--r--   0 tux       (1000) users      (100)    18457 2024-04-11 07:58:51.000000 tremolo-0.0.504/tremolo/lib/http_protocol.py
+-rw-r--r--   0 tux       (1000) users      (100)    12797 2024-03-08 01:51:43.000000 tremolo-0.0.504/tremolo/lib/http_request.py
+-rw-r--r--   0 tux       (1000) users      (100)    15760 2024-04-04 21:42:22.000000 tremolo-0.0.504/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)     1896 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/locks.py
+-rw-r--r--   0 tux       (1000) users      (100)      919 2024-03-05 03:41:31.000000 tremolo-0.0.504/tremolo/lib/pools.py
+-rw-r--r--   0 tux       (1000) users      (100)     1170 2024-02-25 01:31:07.000000 tremolo-0.0.504/tremolo/lib/queue.py
+-rw-r--r--   0 tux       (1000) users      (100)     1199 2024-03-08 01:52:01.000000 tremolo-0.0.504/tremolo/lib/request.py
+-rw-r--r--   0 tux       (1000) users      (100)     1460 2024-04-01 02:53:44.000000 tremolo-0.0.504/tremolo/lib/response.py
+-rw-r--r--   0 tux       (1000) users      (100)      534 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/tasks.py
+-rw-r--r--   0 tux       (1000) users      (100)     6064 2024-02-01 14:00:19.000000 tremolo-0.0.504/tremolo/lib/websocket.py
+-rw-r--r--   0 tux       (1000) users      (100)    28028 2024-04-04 22:17:18.000000 tremolo-0.0.504/tremolo/tremolo.py
+-rw-r--r--   0 tux       (1000) users      (100)     1095 2024-04-04 21:42:22.000000 tremolo-0.0.504/tremolo/utils.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     6473 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      778 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2024-04-11 07:59:52.000000 tremolo-0.0.504/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.503/LICENSE.txt` & `tremolo-0.0.504/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/PKG-INFO` & `tremolo-0.0.504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.503
+Version: 0.0.504
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.503/README.md` & `tremolo-0.0.504/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/pyproject.toml` & `tremolo-0.0.504/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/__main__.py` & `tremolo-0.0.504/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/asgi_lifespan.py` & `tremolo-0.0.504/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/asgi_server.py` & `tremolo-0.0.504/tremolo/asgi_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     async def headers_received(self):
         if not self.request.is_valid:
             await error_400(request=self.request, response=self.response)
             return
 
         self._scope = {
-            'asgi': {'version': '3.0'},
+            'asgi': {'version': '3.0', 'spec_version': '2.3'},
             'http_version': self.request.version.decode('latin-1'),
             'path': unquote_to_bytes(
                 bytes(self.request.path)).decode('latin-1'),
             'raw_path': self.request.path,
             'query_string': self.request.query_string,
             'root_path': self.options['_root_path'],
             'headers': self.request.header.getheaders(),
```

### Comparing `tremolo-0.0.503/tremolo/exceptions.py` & `tremolo-0.0.504/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/handlers.py` & `tremolo-0.0.504/tremolo/handlers.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/http_server.py` & `tremolo-0.0.504/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/connections.py` & `tremolo-0.0.504/tremolo/lib/connections.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/contexts.py` & `tremolo-0.0.504/tremolo/lib/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.504/tremolo/lib/h1parser/parse_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                         self.is_request = True
 
                         try:
                             (
                                 self.headers[b'_method'],
                                 self.headers[b'_url']
                             ) = line[:url_end_pos].split(b' ', 1)
-                            self.headers[b'_version'] = line[url_end_pos + len(' HTTP/'):]  # noqa: E501
+                            self.headers[b'_version'] = line[url_end_pos + 6:]
                             self.is_valid_request = True
                         except ValueError:
                             self.headers[b'_method'] = b''
                             self.headers[b'_url'] = b''
                             self.headers[b'_version'] = b''
 
                 self.headers[b'_line'] = line
```

### Comparing `tremolo-0.0.503/tremolo/lib/http_exception.py` & `tremolo-0.0.504/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/http_protocol.py` & `tremolo-0.0.504/tremolo/lib/http_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,17 @@
             return
 
         self.request = HTTPRequest(self, header)
         self.response = HTTPResponse(self.request)
 
         try:
             if b'connection' in self.request.headers:
-                if b'close' not in self.request.headers[b'connection'].lower():
+                if b',close,' not in (b',' +
+                                      self.request.headers[b'connection']
+                                      .replace(b' ', b'').lower() + b','):
                     self.request.http_keepalive = True
             elif self.request.version == b'1.1':
                 self.request.http_keepalive = True
 
             if self.request.has_body:
                 # assuming a request with a body, such as POST
                 if b'content-type' in self.request.headers:
```

### Comparing `tremolo-0.0.503/tremolo/lib/http_request.py` & `tremolo-0.0.504/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/http_response.py` & `tremolo-0.0.504/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/locks.py` & `tremolo-0.0.504/tremolo/lib/locks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/pools.py` & `tremolo-0.0.504/tremolo/lib/pools.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/queue.py` & `tremolo-0.0.504/tremolo/lib/queue.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/request.py` & `tremolo-0.0.504/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/response.py` & `tremolo-0.0.504/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/tasks.py` & `tremolo-0.0.504/tremolo/lib/tasks.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/lib/websocket.py` & `tremolo-0.0.504/tremolo/lib/websocket.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/tremolo.py` & `tremolo-0.0.504/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo/utils.py` & `tremolo-0.0.504/tremolo/utils.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.503/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.504/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.503
+Version: 0.0.504
 Summary: Tremolo is a stream-oriented, asynchronous, programmable HTTP server written in pure Python. It can also serve as an ASGI server.
 Author-email: nggit <contact@anggit.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/nggit/tremolo
 Project-URL: Source, https://github.com/nggit/tremolo
 Project-URL: Funding, https://github.com/sponsors/nggit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tremolo-0.0.503/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.504/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

