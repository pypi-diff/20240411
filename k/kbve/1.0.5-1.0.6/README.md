# Comparing `tmp/kbve-1.0.5.tar.gz` & `tmp/kbve-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbve-1.0.5.tar", max compression
+gzip compressed data, was "kbve-1.0.6.tar", max compression
```

## Comparing `kbve-1.0.5.tar` & `kbve-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,31 @@
--rw-r--r--   0        0        0       35 2024-04-10 14:52:44.654292 kbve-1.0.5/README.md
--rw-r--r--   0        0        0      161 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/OAI_CONFIG_LIST.json
--rw-r--r--   0        0        0       12 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/__init__.py
--rw-r--r--   0        0        0        9 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/__init__.py
--rw-r--r--   0        0        0     3265 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/api_connector.py
--rw-r--r--   0        0        0       17 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/clients/__init__.py
--rw-r--r--   0        0        0     1026 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/clients/coindesk_client.py
--rw-r--r--   0        0        0     1166 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/clients/poetry_db_client.py
--rw-r--r--   0        0        0     2967 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/api/clients/websocket_echo_client.py
--rw-r--r--   0        0        0      940 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/atlas_autogen.py
--rw-r--r--   0        0        0      616 2024-04-10 14:52:44.654292 kbve-1.0.5/kbve_atlas/bigman.py
--rw-r--r--   0        0        0        0 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/__init__.py
--rw-r--r--   0        0        0     1480 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/doom.py
--rw-r--r--   0        0        0     1167 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/enter_the_matrix.py
--rw-r--r--   0        0        0     4640 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/memetris.py
--rw-r--r--   0        0        0     2012 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/pacman.py
--rw-r--r--   0        0        0     1379 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/snake.py
--rw-r--r--   0        0        0     2215 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/games/tetris.py
--rw-r--r--   0        0        0      473 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/hello.py
--rw-r--r--   0        0        0       11 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/models/__init__.py
--rw-r--r--   0        0        0      523 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/models/coindesk.py
--rw-r--r--   0        0        0      190 2024-04-10 14:52:44.658292 kbve-1.0.5/kbve_atlas/models/poem.py
--rw-r--r--   0        0        0     8762 2024-04-10 14:52:45.374291 kbve-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4981 1970-01-01 00:00:00.000000 kbve-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-04-11 15:03:42.815267 kbve-1.0.6/README.md
+-rw-r--r--   0        0        0      161 2024-04-11 15:03:42.815267 kbve-1.0.6/kbve_atlas/OAI_CONFIG_LIST.json
+-rw-r--r--   0        0        0       12 2024-04-11 15:03:42.815267 kbve-1.0.6/kbve_atlas/__init__.py
+-rw-r--r--   0        0        0        9 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/__init__.py
+-rw-r--r--   0        0        0     4075 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/api_connector.py
+-rw-r--r--   0        0        0      161 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/__init__.py
+-rw-r--r--   0        0        0     1026 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/coindesk_client.py
+-rw-r--r--   0        0        0     1166 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/poetry_db_client.py
+-rw-r--r--   0        0        0     2967 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/clients/websocket_echo_client.py
+-rw-r--r--   0        0        0      196 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/broadcast_utils.py
+-rw-r--r--   0        0        0     1088 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/cors_utils.py
+-rw-r--r--   0        0        0      823 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/kr_decorator.py
+-rw-r--r--   0        0        0     2974 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/rss_utils.py
+-rw-r--r--   0        0        0     1517 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/api/utils/theme_core.py
+-rw-r--r--   0        0        0      940 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/atlas_autogen.py
+-rw-r--r--   0        0        0      616 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/bigman.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/__init__.py
+-rw-r--r--   0        0        0     1480 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/doom.py
+-rw-r--r--   0        0        0     1167 2024-04-11 15:03:42.819267 kbve-1.0.6/kbve_atlas/games/enter_the_matrix.py
+-rw-r--r--   0        0        0     4640 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/memetris.py
+-rw-r--r--   0        0        0     2012 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/pacman.py
+-rw-r--r--   0        0        0     1379 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/snake.py
+-rw-r--r--   0        0        0     2215 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/games/tetris.py
+-rw-r--r--   0        0        0      473 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/hello.py
+-rw-r--r--   0        0        0       11 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/coindesk.py
+-rw-r--r--   0        0        0      190 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/poem.py
+-rw-r--r--   0        0        0      335 2024-04-11 15:03:42.823267 kbve-1.0.6/kbve_atlas/models/rss.py
+-rw-r--r--   0        0        0    10499 2024-04-11 15:03:43.515257 kbve-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 kbve-1.0.6/PKG-INFO
```

### Comparing `kbve-1.0.5/kbve_atlas/api/api_connector.py` & `kbve-1.0.6/kbve_atlas/api/api_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,19 @@
     async def _request(self, method: str, endpoint: str, **kwargs) -> Any:
         url = f"{self.base_url}/{endpoint}"
         headers = self._prepare_headers(kwargs.pop('auth', None))
         async with self.session.request(method, url, headers=headers, **kwargs) as response:
             response.raise_for_status()
             return await response.json()
 
+    async def _get_session(self):
+        if not self.session:
+            self.session = aiohttp.ClientSession()
+        return self.session
+
     async def get(self, endpoint: str, **kwargs) -> Any:
         return await self._request('GET', endpoint, **kwargs)
 
     async def post(self, endpoint: str, **kwargs) -> Any:
         return await self._request('POST', endpoint, **kwargs)
 
     async def delete(self, endpoint: str, **kwargs) -> Any:
@@ -67,8 +72,23 @@
             raise Exception("WebSocket connection closed or encountered an error.")
 
     def _prepare_headers(self, auth: Optional[str] = None) -> dict:
         """Prepare headers for HTTP or WebSocket connection."""
         headers = {}
         if self.key and auth == 'header':
             headers['Authorization'] = f"Bearer {self.key}"
-        return headers
+        return headers
+    
+    async def get_raw_content(self, endpoint: str) -> bytes:
+        """
+        Performs a GET request to the specified endpoint and returns the raw response content.
+
+        :param endpoint: The API endpoint to fetch.
+        :return: Raw content of the response as bytes.
+        """
+        # Ensure the session is initialized
+        session = await self._get_session()
+        # Construct the full URL
+        url = f"{self.base_url}/{endpoint}"
+        async with session.get(url) as response:
+            response.raise_for_status()  # Ensure we got a successful response
+            return await response.read()  # Return the response content as bytes
```

### Comparing `kbve-1.0.5/kbve_atlas/api/clients/coindesk_client.py` & `kbve-1.0.6/kbve_atlas/api/clients/coindesk_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/api/clients/poetry_db_client.py` & `kbve-1.0.6/kbve_atlas/api/clients/poetry_db_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/api/clients/websocket_echo_client.py` & `kbve-1.0.6/kbve_atlas/api/clients/websocket_echo_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/atlas_autogen.py` & `kbve-1.0.6/kbve_atlas/atlas_autogen.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/bigman.py` & `kbve-1.0.6/kbve_atlas/bigman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/doom.py` & `kbve-1.0.6/kbve_atlas/games/doom.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/enter_the_matrix.py` & `kbve-1.0.6/kbve_atlas/games/enter_the_matrix.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/memetris.py` & `kbve-1.0.6/kbve_atlas/games/memetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/pacman.py` & `kbve-1.0.6/kbve_atlas/games/pacman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/snake.py` & `kbve-1.0.6/kbve_atlas/games/snake.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/games/tetris.py` & `kbve-1.0.6/kbve_atlas/games/tetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/kbve_atlas/models/coindesk.py` & `kbve-1.0.6/kbve_atlas/models/coindesk.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.5/pyproject.toml` & `kbve-1.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html:'../../coverage/apps/atlas/html' --cov-report xml:'../../coverage/apps/atlas/coverage.xml' --html='../../reports/apps/atlas/unittests/html/index.html' --junitxml='../../reports/apps/atlas/unittests/junit.xml'"
 
 [tool.poetry]
 name = "kbve"
-version = "1.0.5"
+version = "1.0.6"
 description = "ATLAS"
 authors = [ ]
 license = "Proprietary"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "kbve_atlas"
@@ -39,24 +39,35 @@
     optional = false
 
     [tool.poetry.dependencies.anyio]
     version = "4.3.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.asyncio-redis]
+    version = "0.16.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.attrs]
     version = "23.2.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.beautifulsoup4]
     version = "4.12.3 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.broadcaster]
+    version = "0.2.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+    extras = [ "redis" ]
+
     [tool.poetry.dependencies.certifi]
     version = "2024.2.2 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.charset-normalizer]
     version = "3.3.2 "
@@ -66,15 +77,15 @@
     [tool.poetry.dependencies.click]
     version = "8.1.7 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.colorama]
     version = "0.4.6 "
-    markers = 'python_version >= "3.12" and python_version < "3.13" and platform_system == "Windows"'
+    markers = 'python_version >= "3.12" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")'
     optional = false
 
     [tool.poetry.dependencies.diskcache]
     version = "5.6.3 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
@@ -84,14 +95,19 @@
     optional = false
 
     [tool.poetry.dependencies.docker]
     version = "7.0.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.fastapi]
+    version = "0.110.1 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.filelock]
     version = "3.13.4 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.flaml]
     version = "2.1.2 "
@@ -114,41 +130,51 @@
     optional = false
 
     [tool.poetry.dependencies.httpcore]
     version = "1.0.5 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.httptools]
+    version = "0.6.1 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.httpx]
     version = "0.27.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.huggingface-hub]
     version = "0.22.2 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.idna]
-    version = "3.6 "
+    version = "3.7 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.importlib-metadata]
     version = "7.1.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.jinja2]
     version = "3.1.3 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.litellm]
-    version = "1.34.39 "
+    version = "1.35.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.lxml]
+    version = "5.2.1 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.markupsafe]
     version = "2.1.5 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
@@ -160,15 +186,15 @@
 
     [tool.poetry.dependencies.numpy]
     version = "1.26.4 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.openai]
-    version = "1.16.2 "
+    version = "1.17.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.packaging]
     version = "24.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
@@ -235,14 +261,19 @@
     optional = false
 
     [tool.poetry.dependencies.soupsieve]
     version = "2.5 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.starlette]
+    version = "0.37.2 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.termcolor]
     version = "2.4.0 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tiktoken]
     version = "0.6.0 "
@@ -265,14 +296,35 @@
     optional = false
 
     [tool.poetry.dependencies.urllib3]
     version = "2.2.1 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.uvicorn]
+    version = "0.29.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+    extras = [ "standard" ]
+
+    [tool.poetry.dependencies.uvloop]
+    version = "0.19.0 "
+    markers = '(sys_platform != "win32" and sys_platform != "cygwin") and platform_python_implementation != "PyPy" and python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.watchfiles]
+    version = "0.21.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.websockets]
+    version = "12.0 "
+    markers = 'python_version >= "3.12" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.yarl]
     version = "1.9.4 "
     markers = 'python_version >= "3.12" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.zipp]
     version = "3.18.1 "
```

### Comparing `kbve-1.0.5/PKG-INFO` & `kbve-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 Metadata-Version: 2.1
 Name: kbve
-Version: 1.0.5
+Version: 1.0.6
 Summary: ATLAS
 License: Proprietary
 Requires-Python: >=3.12,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (==3.9.3) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: aiosignal (==1.3.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: annotated-types (==0.6.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: anyio (==4.3.0) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: asyncio-redis (==0.16.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: attrs (==23.2.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: beautifulsoup4 (==4.12.3) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: broadcaster[redis] (==0.2.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: certifi (==2024.2.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: charset-normalizer (==3.3.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: click (==8.1.7) ; python_version >= "3.12" and python_version < "3.13"
-Requires-Dist: colorama (==0.4.6) ; python_version >= "3.12" and python_version < "3.13" and platform_system == "Windows"
+Requires-Dist: colorama (==0.4.6) ; python_version >= "3.12" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")
 Requires-Dist: diskcache (==5.6.3) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: distro (==1.9.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: docker (==7.0.0) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: fastapi (==0.110.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: filelock (==3.13.4) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: flaml (==2.1.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: frozenlist (==1.4.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: fsspec (==2024.3.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: h11 (==0.14.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: httpcore (==1.0.5) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: httptools (==0.6.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: httpx (==0.27.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: huggingface-hub (==0.22.2) ; python_version >= "3.12" and python_version < "3.13"
-Requires-Dist: idna (==3.6) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: idna (==3.7) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: importlib-metadata (==7.1.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: jinja2 (==3.1.3) ; python_version >= "3.12" and python_version < "3.13"
-Requires-Dist: litellm (==1.34.39) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: litellm (==1.35.0) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: lxml (==5.2.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: markupsafe (==2.1.5) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: multidict (==6.0.5) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: numpy (==1.26.4) ; python_version >= "3.12" and python_version < "3.13"
-Requires-Dist: openai (==1.16.2) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: openai (==1.17.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: packaging (==24.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: pillow (==10.3.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: pyautogen[lmm,redis] (==0.2.23) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: pydantic (==2.6.4) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: pydantic-core (==2.16.3) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: python-dotenv (==1.0.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: pywin32 (==306) ; python_version >= "3.12" and python_version < "3.13" and sys_platform == "win32"
 Requires-Dist: pyyaml (==6.0.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: redis (==5.0.3) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: regex (==2023.12.25) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: replicate (==0.25.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: requests (==2.31.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: sniffio (==1.3.1) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: soupsieve (==2.5) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: starlette (==0.37.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: termcolor (==2.4.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: tiktoken (==0.6.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: tokenizers (==0.15.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: tqdm (==4.66.2) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: typing-extensions (==4.11.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: urllib3 (==2.2.1) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: uvicorn[standard] (==0.29.0) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: uvloop (==0.19.0) ; (sys_platform != "win32" and sys_platform != "cygwin") and platform_python_implementation != "PyPy" and python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: watchfiles (==0.21.0) ; python_version >= "3.12" and python_version < "3.13"
+Requires-Dist: websockets (==12.0) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: yarl (==1.9.4) ; python_version >= "3.12" and python_version < "3.13"
 Requires-Dist: zipp (==3.18.1) ; python_version >= "3.12" and python_version < "3.13"
 Description-Content-Type: text/markdown
 
 # atlas
 
 Project description here.
```

