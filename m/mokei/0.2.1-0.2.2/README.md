# Comparing `tmp/mokei-0.2.1.tar.gz` & `tmp/mokei-0.2.2.tar.gz`

## Comparing `mokei-0.2.1.tar` & `mokei-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/__init__.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/client.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/config.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/datatypes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/exceptions.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/logging.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/middlewares.py
--rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/mokei.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/request.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/websocket.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/wsclient.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/js/mokei.js
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mokei-0.2.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.2.1/LICENSE
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.2.1/README.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/__init__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/client.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/config.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/datatypes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/exceptions.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/logging.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/middlewares.py
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/mokei.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/request.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/websocket.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/wsclient.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/js/mokei.js
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mokei-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.2.2/README.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.2.2/PKG-INFO
```

### Comparing `mokei-0.2.1/src/mokei/client.py` & `mokei-0.2.2/src/mokei/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
 import aiohttp
-from aiohttp.client import ClientSession, ClientResponse
+from aiohttp.client import ClientSession
 from yarl import URL
 
 from .datatypes import JsonDict
 
 
 class MokeiClient:
     def __init__(self, verify_ssl: bool = True,
@@ -20,28 +20,28 @@
         if self._session:
             await self._session.close()
         if not keep_headers:
             self.headers.clear()
         if not keep_cookies:
             self.cookies.clear()
 
-    async def post_form_data(self, url: str | URL, data: dict) -> ClientResponse:
+    async def post_form_data(self, url: str | URL, data: dict) -> tuple[str, int]:
         form_data = aiohttp.FormData()
         for key, value in data.items():
             form_data.add_field(key, value)
         async with self._session.post(url, data, headers=self.headers, verify_ssl=self.verify_ssl) as response:
-            return response
+            return await response.text(), response.status
 
-    async def post_json(self, url: str | URL, jsondict: JsonDict) -> ClientResponse:
+    async def post_json(self, url: str | URL, jsondict: JsonDict) -> tuple[str, int]:
         async with self._session.post(url, json=jsondict, headers=self.headers, verify_ssl=self.verify_ssl) as response:
-            return response
+            return await response.text(), response.status
 
-    async def get(self, url: str | URL) -> ClientResponse:
+    async def get(self, url: str | URL) -> tuple[str, int]:
         async with self._session.get(url, headers=self.headers, verify_ssl=self.verify_ssl) as response:
-            return response
+            return await response.text(), response.status
 
     def set_header(self, header_name: str, header_value: str) -> None:
         self.headers[header_name] = header_value
 
     def set_cookie(self, cookie_name: str, cookie_value: str) -> None:
         self.cookies[cookie_name] = cookie_value
```

### Comparing `mokei-0.2.1/src/mokei/config.py` & `mokei-0.2.2/src/mokei/config.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/src/mokei/logging.py` & `mokei-0.2.2/src/mokei/logging.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/src/mokei/mokei.py` & `mokei-0.2.2/src/mokei/mokei.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,17 @@
                     raise web.HTTPFound(self._handlers[target])
         elif isinstance(target, Callable):
             if target.__name__ in self._handlers:
                 raise web.HTTPFound(self._handlers[target.__name__])
 
     @staticmethod
     def _get_normalized_handler(raw_handler):
+        if not asyncio.iscoroutinefunction(raw_handler):
+            raise TypeError('handler must be an async function')
+
         if getattr(raw_handler, '_is_mokei_normalized', False):
             # this handler has been normalized already - return as is
             return raw_handler
 
         sig = inspect.signature(raw_handler)
         params = sig.parameters
 
@@ -115,14 +118,16 @@
 
     def _route_handler(self, path: str, http_method: str):
         """Generic decorator method for handling any http method
         Do not call this method directly, but use partialmethod to create methods for handling specific http methods
         """
 
         def decorator(handler):
+            if not asyncio.iscoroutinefunction(handler):
+                raise TypeError('Handler must be a async function')
             normalized_handler = self._get_normalized_handler(handler)
             getattr(self._routes, http_method)(path)(normalized_handler)
             self._handlers[handler.__name__] = path
             return handler
 
         return decorator
 
@@ -213,15 +218,15 @@
 
         self._routes.get(path)(ws)
         return socket_route
 
     async def _handle_websocket(self, request: Request, socket_route: MokeiWebSocketRoute) -> MokeiWebSocket:
         """ Called when a new websocket connection is established from a client
         """
-        ws = MokeiWebSocket(request)
+        ws = MokeiWebSocket(request, socket_route)
         try:
             await ws.prepare(request)
         except ConnectionResetError:
             return ws
         socket_route.sockets.add(ws)
         # noinspection PyProtectedMember
         await socket_route._onconnect_handler(ws)
```

### Comparing `mokei-0.2.1/src/mokei/websocket.py` & `mokei-0.2.2/src/mokei/websocket.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/src/mokei/wsclient.py` & `mokei-0.2.2/src/mokei/wsclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,17 @@
                             msg: WSMessage
                             if msg.type == aiohttp.WSMsgType.TEXT:
                                 await self._ontext_handler(ws, msg.data)
                             elif msg.type == aiohttp.WSMsgType.ERROR:
                                 break
                 except aiohttp.ClientConnectorError:
                     pass
+                except RuntimeError:
+                    raise RuntimeError
+
                 if self._ws:
                     await self._ondisconnect_handler(self._ws)
                 self._ws = None
                 await asyncio.sleep(self._get_backoff())
 
     async def close(self):
         await self._session.close()
```

### Comparing `mokei-0.2.1/src/mokei/js/mokei.js` & `mokei-0.2.2/src/mokei/js/mokei.js`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/LICENSE` & `mokei-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/README.md` & `mokei-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mokei-0.2.1/pyproject.toml` & `mokei-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mokei"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="deuxglaces", email="dev@deuxglaces.com" },
 ]
 description = "A simple asynchronous Python web framework built on aiohttp."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mokei-0.2.1/PKG-INFO` & `mokei-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mokei
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple asynchronous Python web framework built on aiohttp.
 Project-URL: Homepage, https://github.com/deuxglaces/mokei
 Project-URL: Issues, https://github.com/deuxglaces/mokei/issues
 Author-email: deuxglaces <dev@deuxglaces.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

