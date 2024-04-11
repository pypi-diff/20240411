# Comparing `tmp/daphne-4.1.0.tar.gz` & `tmp/daphne-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daphne-4.1.0.tar", last modified: Sat Feb 10 14:45:57 2024, max compression
+gzip compressed data, was "daphne-4.1.1.tar", last modified: Wed Apr 10 15:42:15 2024, max compression
```

## Comparing `daphne-4.1.0.tar` & `daphne-4.1.1.tar`

### file list

```diff
@@ -1,44 +1,39 @@
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.354719 daphne-4.1.0/
--rw-r--r--   0 carlton    (501) staff       (20)     1552 2021-11-09 14:25:44.000000 daphne-4.1.0/LICENSE
--rw-r--r--   0 carlton    (501) staff       (20)       16 2021-11-09 14:25:44.000000 daphne-4.1.0/MANIFEST.in
--rw-r--r--   0 carlton    (501) staff       (20)     6466 2024-02-10 14:45:57.354592 daphne-4.1.0/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)     5246 2024-02-06 07:36:43.000000 daphne-4.1.0/README.rst
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.351392 daphne-4.1.0/daphne/
--rwxr-xr-x   0 carlton    (501) staff       (20)      432 2024-02-10 14:38:37.000000 daphne-4.1.0/daphne/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)       79 2021-11-09 14:25:44.000000 daphne-4.1.0/daphne/__main__.py
--rw-r--r--   0 carlton    (501) staff       (20)     2389 2021-11-09 18:47:37.000000 daphne-4.1.0/daphne/access.py
--rw-r--r--   0 carlton    (501) staff       (20)      476 2022-10-07 10:10:21.000000 daphne-4.1.0/daphne/apps.py
--rw-r--r--   0 carlton    (501) staff       (20)      722 2022-10-07 10:10:21.000000 daphne-4.1.0/daphne/checks.py
--rwxr-xr-x   0 carlton    (501) staff       (20)     9999 2022-10-07 10:26:41.000000 daphne-4.1.0/daphne/cli.py
--rw-r--r--   0 carlton    (501) staff       (20)      899 2021-11-09 14:25:44.000000 daphne-4.1.0/daphne/endpoints.py
--rwxr-xr-x   0 carlton    (501) staff       (20)    16352 2024-02-10 14:26:04.000000 daphne-4.1.0/daphne/http_protocol.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.352468 daphne-4.1.0/daphne/management/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-10-07 10:10:21.000000 daphne-4.1.0/daphne/management/__init__.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.352675 daphne-4.1.0/daphne/management/commands/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-10-07 10:10:21.000000 daphne-4.1.0/daphne/management/commands/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     7866 2023-04-14 12:38:32.000000 daphne-4.1.0/daphne/management/commands/runserver.py
--rwxr-xr-x   0 carlton    (501) staff       (20)    13633 2023-04-14 12:55:15.000000 daphne-4.1.0/daphne/server.py
--rw-r--r--   0 carlton    (501) staff       (20)     9990 2022-10-07 12:17:51.000000 daphne-4.1.0/daphne/testing.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.348488 daphne-4.1.0/daphne/twisted/
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.352834 daphne-4.1.0/daphne/twisted/plugins/
--rw-r--r--   0 carlton    (501) staff       (20)      814 2021-11-09 18:47:37.000000 daphne-4.1.0/daphne/twisted/plugins/fd_endpoint.py
--rw-r--r--   0 carlton    (501) staff       (20)     3318 2024-02-10 14:26:04.000000 daphne-4.1.0/daphne/utils.py
--rwxr-xr-x   0 carlton    (501) staff       (20)    11867 2024-02-10 14:21:42.000000 daphne-4.1.0/daphne/ws_protocol.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.353975 daphne-4.1.0/daphne.egg-info/
--rw-r--r--   0 carlton    (501) staff       (20)     6466 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)      797 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/SOURCES.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/dependency_links.txt
--rw-r--r--   0 carlton    (501) staff       (20)       70 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/entry_points.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2022-10-07 13:17:00.000000 daphne-4.1.0/daphne.egg-info/not-zip-safe
--rw-r--r--   0 carlton    (501) staff       (20)      103 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/requires.txt
--rw-r--r--   0 carlton    (501) staff       (20)        7 2024-02-10 14:45:57.000000 daphne-4.1.0/daphne.egg-info/top_level.txt
--rw-r--r--   0 carlton    (501) staff       (20)       81 2023-04-14 12:38:36.000000 daphne-4.1.0/pyproject.toml
--rw-r--r--   0 carlton    (501) staff       (20)     1507 2024-02-10 14:45:57.355202 daphne-4.1.0/setup.cfg
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-02-10 14:45:57.353774 daphne-4.1.0/tests/
--rw-r--r--   0 carlton    (501) staff       (20)      698 2022-10-07 10:10:21.000000 daphne-4.1.0/tests/test_checks.py
--rw-r--r--   0 carlton    (501) staff       (20)     8707 2022-10-07 10:10:21.000000 daphne-4.1.0/tests/test_cli.py
--rw-r--r--   0 carlton    (501) staff       (20)      934 2022-10-07 10:10:21.000000 daphne-4.1.0/tests/test_http_protocol.py
--rw-r--r--   0 carlton    (501) staff       (20)    13396 2024-02-10 14:28:33.000000 daphne-4.1.0/tests/test_http_request.py
--rw-r--r--   0 carlton    (501) staff       (20)     6369 2022-10-07 10:10:21.000000 daphne-4.1.0/tests/test_http_response.py
--rw-r--r--   0 carlton    (501) staff       (20)     2918 2021-11-09 18:47:37.000000 daphne-4.1.0/tests/test_utils.py
--rw-r--r--   0 carlton    (501) staff       (20)    13974 2024-02-06 09:44:50.000000 daphne-4.1.0/tests/test_websocket.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.472118 daphne-4.1.1/
+-rw-r--r--   0 carlton    (501) staff       (20)     1552 2021-11-09 14:25:44.000000 daphne-4.1.1/LICENSE
+-rw-r--r--   0 carlton    (501) staff       (20)       16 2021-11-09 14:25:44.000000 daphne-4.1.1/MANIFEST.in
+-rw-r--r--   0 carlton    (501) staff       (20)     6466 2024-04-10 15:42:15.471975 daphne-4.1.1/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)     5246 2024-02-06 07:36:43.000000 daphne-4.1.1/README.rst
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.467360 daphne-4.1.1/daphne/
+-rwxr-xr-x   0 carlton    (501) staff       (20)      432 2024-04-10 15:38:57.000000 daphne-4.1.1/daphne/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)       79 2021-11-09 14:25:44.000000 daphne-4.1.1/daphne/__main__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2389 2021-11-09 18:47:37.000000 daphne-4.1.1/daphne/access.py
+-rw-r--r--   0 carlton    (501) staff       (20)      476 2022-10-07 10:10:21.000000 daphne-4.1.1/daphne/apps.py
+-rw-r--r--   0 carlton    (501) staff       (20)      722 2022-10-07 10:10:21.000000 daphne-4.1.1/daphne/checks.py
+-rwxr-xr-x   0 carlton    (501) staff       (20)    10015 2024-04-09 12:38:18.000000 daphne-4.1.1/daphne/cli.py
+-rw-r--r--   0 carlton    (501) staff       (20)      899 2021-11-09 14:25:44.000000 daphne-4.1.1/daphne/endpoints.py
+-rwxr-xr-x   0 carlton    (501) staff       (20)    16424 2024-04-09 12:38:18.000000 daphne-4.1.1/daphne/http_protocol.py
+-rwxr-xr-x   0 carlton    (501) staff       (20)    13633 2023-04-14 12:55:15.000000 daphne-4.1.1/daphne/server.py
+-rw-r--r--   0 carlton    (501) staff       (20)     9990 2022-10-07 12:17:51.000000 daphne-4.1.1/daphne/testing.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.462100 daphne-4.1.1/daphne/twisted/
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.468706 daphne-4.1.1/daphne/twisted/plugins/
+-rw-r--r--   0 carlton    (501) staff       (20)      814 2021-11-09 18:47:37.000000 daphne-4.1.1/daphne/twisted/plugins/fd_endpoint.py
+-rw-r--r--   0 carlton    (501) staff       (20)     3318 2024-02-10 14:26:04.000000 daphne-4.1.1/daphne/utils.py
+-rwxr-xr-x   0 carlton    (501) staff       (20)    11899 2024-04-09 12:38:18.000000 daphne-4.1.1/daphne/ws_protocol.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.471288 daphne-4.1.1/daphne.egg-info/
+-rw-r--r--   0 carlton    (501) staff       (20)     6466 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)      688 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/SOURCES.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/dependency_links.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       70 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/entry_points.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/not-zip-safe
+-rw-r--r--   0 carlton    (501) staff       (20)      103 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/requires.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       15 2024-04-10 15:42:15.000000 daphne-4.1.1/daphne.egg-info/top_level.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       81 2023-04-14 12:38:36.000000 daphne-4.1.1/pyproject.toml
+-rw-r--r--   0 carlton    (501) staff       (20)     1527 2024-04-10 15:42:15.472636 daphne-4.1.1/setup.cfg
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-10 15:42:15.470644 daphne-4.1.1/tests/
+-rw-r--r--   0 carlton    (501) staff       (20)      698 2022-10-07 10:10:21.000000 daphne-4.1.1/tests/test_checks.py
+-rw-r--r--   0 carlton    (501) staff       (20)     8707 2022-10-07 10:10:21.000000 daphne-4.1.1/tests/test_cli.py
+-rw-r--r--   0 carlton    (501) staff       (20)      934 2022-10-07 10:10:21.000000 daphne-4.1.1/tests/test_http_protocol.py
+-rw-r--r--   0 carlton    (501) staff       (20)    13396 2024-02-10 14:28:33.000000 daphne-4.1.1/tests/test_http_request.py
+-rw-r--r--   0 carlton    (501) staff       (20)     6369 2022-10-07 10:10:21.000000 daphne-4.1.1/tests/test_http_response.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2918 2021-11-09 18:47:37.000000 daphne-4.1.1/tests/test_utils.py
+-rw-r--r--   0 carlton    (501) staff       (20)    13974 2024-02-06 09:44:50.000000 daphne-4.1.1/tests/test_websocket.py
```

### Comparing `daphne-4.1.0/LICENSE` & `daphne-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/PKG-INFO` & `daphne-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daphne
-Version: 4.1.0
+Version: 4.1.1
 Summary: Django ASGI (HTTP/WebSocket) server
 Home-page: https://github.com/django/daphne
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `daphne-4.1.0/README.rst` & `daphne-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/access.py` & `daphne-4.1.1/daphne/access.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/checks.py` & `daphne-4.1.1/daphne/checks.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/cli.py` & `daphne-4.1.1/daphne/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,20 +266,20 @@
             http_timeout=args.http_timeout,
             ping_interval=args.ping_interval,
             ping_timeout=args.ping_timeout,
             websocket_timeout=args.websocket_timeout,
             websocket_connect_timeout=args.websocket_connect_timeout,
             websocket_handshake_timeout=args.websocket_connect_timeout,
             application_close_timeout=args.application_close_timeout,
-            action_logger=AccessLogGenerator(access_log_stream)
-            if access_log_stream
-            else None,
+            action_logger=(
+                AccessLogGenerator(access_log_stream) if access_log_stream else None
+            ),
             root_path=args.root_path,
             verbosity=args.verbosity,
             proxy_forwarded_address_header=self._get_forwarded_host(args=args),
             proxy_forwarded_port_header=self._get_forwarded_port(args=args),
-            proxy_forwarded_proto_header="X-Forwarded-Proto"
-            if args.proxy_headers
-            else None,
+            proxy_forwarded_proto_header=(
+                "X-Forwarded-Proto" if args.proxy_headers else None
+            ),
             server_name=args.server_name,
         )
         self.server.run()
```

### Comparing `daphne-4.1.0/daphne/endpoints.py` & `daphne-4.1.1/daphne/endpoints.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/http_protocol.py` & `daphne-4.1.1/daphne/http_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,17 +282,19 @@
                     self.server.log_action(
                         "http",
                         "complete",
                         {
                             "path": uri,
                             "status": self.code,
                             "method": self.method.decode("ascii", "replace"),
-                            "client": "%s:%s" % tuple(self.client_addr)
-                            if self.client_addr
-                            else None,
+                            "client": (
+                                "%s:%s" % tuple(self.client_addr)
+                                if self.client_addr
+                                else None
+                            ),
                             "time_taken": self.duration(),
                             "size": self.sentLength,
                         },
                     )
                 except Exception:
                     logger.error(traceback.format_exc())
             else:
```

### Comparing `daphne-4.1.0/daphne/server.py` & `daphne-4.1.1/daphne/server.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/testing.py` & `daphne-4.1.1/daphne/testing.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/twisted/plugins/fd_endpoint.py` & `daphne-4.1.1/daphne/twisted/plugins/fd_endpoint.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/utils.py` & `daphne-4.1.1/daphne/utils.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/daphne/ws_protocol.py` & `daphne-4.1.1/daphne/ws_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,17 @@
         # Send over the connect message
         self.application_queue.put_nowait({"type": "websocket.connect"})
         self.server.log_action(
             "websocket",
             "connecting",
             {
                 "path": self.request.path,
-                "client": "%s:%s" % tuple(self.client_addr)
-                if self.client_addr
-                else None,
+                "client": (
+                    "%s:%s" % tuple(self.client_addr) if self.client_addr else None
+                ),
             },
         )
 
     def applicationCreateFailed(self, failure):
         """
         Called when application creation fails.
         """
@@ -134,17 +134,17 @@
         # Send news that this channel is open
         logger.debug("WebSocket %s open and established", self.client_addr)
         self.server.log_action(
             "websocket",
             "connected",
             {
                 "path": self.request.path,
-                "client": "%s:%s" % tuple(self.client_addr)
-                if self.client_addr
-                else None,
+                "client": (
+                    "%s:%s" % tuple(self.client_addr) if self.client_addr else None
+                ),
             },
         )
 
     def onMessage(self, payload, isBinary):
         # If we're muted, do nothing.
         if self.muted:
             logger.debug("Muting incoming frame on %s", self.client_addr)
@@ -171,17 +171,17 @@
                 {"type": "websocket.disconnect", "code": code}
             )
         self.server.log_action(
             "websocket",
             "disconnected",
             {
                 "path": self.request.path,
-                "client": "%s:%s" % tuple(self.client_addr)
-                if self.client_addr
-                else None,
+                "client": (
+                    "%s:%s" % tuple(self.client_addr) if self.client_addr else None
+                ),
             },
         )
 
     ### Internal event handling
 
     def handle_reply(self, message):
         if "type" not in message:
@@ -238,17 +238,17 @@
         self.server.protocol_disconnected(self)
         logger.debug("WebSocket %s rejected by application", self.client_addr)
         self.server.log_action(
             "websocket",
             "rejected",
             {
                 "path": self.request.path,
-                "client": "%s:%s" % tuple(self.client_addr)
-                if self.client_addr
-                else None,
+                "client": (
+                    "%s:%s" % tuple(self.client_addr) if self.client_addr else None
+                ),
             },
         )
 
     def serverSend(self, content, binary=False):
         """
         Server-side channel message to send a message.
         """
```

### Comparing `daphne-4.1.0/daphne.egg-info/PKG-INFO` & `daphne-4.1.1/daphne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daphne
-Version: 4.1.0
+Version: 4.1.1
 Summary: Django ASGI (HTTP/WebSocket) server
 Home-page: https://github.com/django/daphne
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `daphne-4.1.0/setup.cfg` & `daphne-4.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 
 [options]
 package_dir = 
 	twisted=daphne/twisted
-packages = find:
+packages = 
+	daphne
+	twisted.plugins
 include_package_data = True
 install_requires = 
 	asgiref>=3.5.2,<4
 	autobahn>=22.4.2
 	twisted[tls]>=22.4
 python_requires = >=3.8
 setup_requires =
```

### Comparing `daphne-4.1.0/tests/test_checks.py` & `daphne-4.1.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_cli.py` & `daphne-4.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_http_protocol.py` & `daphne-4.1.1/tests/test_http_protocol.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_http_request.py` & `daphne-4.1.1/tests/test_http_request.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_http_response.py` & `daphne-4.1.1/tests/test_http_response.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_utils.py` & `daphne-4.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `daphne-4.1.0/tests/test_websocket.py` & `daphne-4.1.1/tests/test_websocket.py`

 * *Files identical despite different names*

