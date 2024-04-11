# Comparing `tmp/openai_forward-0.7.1.tar.gz` & `tmp/openai_forward-0.7.2.tar.gz`

## Comparing `openai_forward-0.7.1.tar` & `openai_forward-0.7.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/__init__.py
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/__main__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/app.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/console.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/custom_slowapi.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/decorators.py
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/helper.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/settings.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/database.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/chat/__init__.py
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/chat/chat_completions.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/chat/response.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/chat/tokenizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/embedding/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/cache/embedding/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/content/config.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/content/helper.py
--rw-r--r--   0        0        0    14505 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/content/openai.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/forward/__init__.py
--rw-r--r--   0        0        0    21170 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/forward/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/webui/__init__.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/webui/chat.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/webui/helper.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/webui/interface.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 openai_forward-0.7.1/openai_forward/webui/run.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 openai_forward-0.7.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.7.1/LICENSE
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 openai_forward-0.7.1/README.md
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 openai_forward-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 openai_forward-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/__init__.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/__main__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/app.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/console.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/custom_slowapi.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/decorators.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/helper.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/settings.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/database.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/__init__.py
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/chat_completions.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/response.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/chat/tokenizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/embedding/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/cache/embedding/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/config.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/helper.py
+-rw-r--r--   0        0        0    14539 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/content/openai.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/forward/__init__.py
+-rw-r--r--   0        0        0    21936 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/forward/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/chat.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/helper.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/interface.py
+-rw-r--r--   0        0        0    14976 2020-02-02 00:00:00.000000 openai_forward-0.7.2/openai_forward/webui/run.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 openai_forward-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.7.2/LICENSE
+-rw-r--r--   0        0        0    10987 2020-02-02 00:00:00.000000 openai_forward-0.7.2/README.md
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 openai_forward-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13036 2020-02-02 00:00:00.000000 openai_forward-0.7.2/PKG-INFO
```

### Comparing `openai_forward-0.7.1/openai_forward/__main__.py` & `openai_forward-0.7.2/openai_forward/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,47 @@
 import pickle
 import platform
 import signal
 import subprocess
 
 import fire
 import uvicorn
-from loguru import logger
 
 
 class Cli:
-    def run(self, port=8000, workers=1, webui=False, ui_port=8001):
+    def run_web(self, port=8001, openai_forward_host='localhost', wait=True):
+        """
+        Runs the web UI using the Streamlit server.
+
+        Args:
+            port (int): The port number on which to run the server.
+            openai_forward_host (str): The host of the OpenAI Forward server.
+            wait (bool): Whether to wait for the server to stop. Default is True.
+
+        Returns:
+            None
+        """
+        os.environ['OPENAI_FORWARD_HOST'] = openai_forward_host
+        try:
+            self._start_streamlit(port=port, wait=wait)
+        except KeyboardInterrupt:
+            ...
+        except Exception as e:
+            raise
+
+    def run(self, port=8000, workers=1, webui=False, start_ui=True, ui_port=8001):
         """
         Runs the application using the Uvicorn server.
 
         Args:
-            port (int): The port number on which to run the server. Default is 8000.
-            workers (int): The number of worker processes to run. Default is 1.
+            port (int): The port number on which to run the server.
+            workers (int): The number of worker processes to run.
             webui (bool): Whether to run the web UI. Default is False.
-            ui_port (int): The port number on which to run streamlit. Default is 17860.
+            start_ui (bool): Whether to start the web UI.
+            ui_port (int): The port number on which to run streamlit.
 
         Returns:
             None
         """
 
         if platform.system() == "Windows":
             os.environ["TZ"] = ""
@@ -38,36 +58,59 @@
                 port=port,
                 workers=workers,
                 app_dir="..",
                 ssl_keyfile=ssl_keyfile,
                 ssl_certfile=ssl_certfile,
             )
         else:
-            os.environ['OPENAI_FORWARD_WEBUI'] = 'true'
+            import threading
 
             import zmq
 
             mq_port = 15555
+
+            os.environ['OPENAI_FORWARD_WEBUI'] = 'true'
+
             context = zmq.Context()
             socket = context.socket(zmq.REP)
             socket.bind(f"tcp://*:{mq_port}")
+            log_socket = context.socket(zmq.ROUTER)
+            log_socket.bind(f"tcp://*:{15556}")
+            subscriber_info = {}
+
+            def mq_worker(log_socket: zmq.Socket):
+
+                while True:
+                    identity, uid, message = log_socket.recv_multipart()
+                    if uid == b"/subscribe":
+                        subscriber_info[identity] = True
+                        continue
+                    else:
+                        for subscriber, _ in subscriber_info.items():
+                            log_socket.send_multipart([subscriber, uid, message])
+
+            thread = threading.Thread(target=mq_worker, args=(log_socket,))
+            thread.daemon = True
+            thread.start()
 
             self._start_uvicorn(
                 port=port,
                 workers=workers,
                 ssl_keyfile=ssl_keyfile,
                 ssl_certfile=ssl_certfile,
             )
-            self._start_streamlit(port=ui_port)
-            atexit.register(self._stop)
+
+            if start_ui:
+                self._start_streamlit(port=ui_port, wait=False)
+
+            atexit.register(self._stop_uvicorn)
 
             while True:
                 message = socket.recv()
                 env_dict: dict = pickle.loads(message)
-                # logger.debug(f"{env_dict=}")
 
                 for key, value in env_dict.items():
                     os.environ[key] = value
 
                 self._restart_uvicorn(
                     port=port,
                     workers=workers,
@@ -98,15 +141,15 @@
         suppress_exception = platform.system() == "Windows"
         wait_for_serve_start(
             f"http://localhost:{port}/healthz",
             timeout=10,
             suppress_exception=suppress_exception,
         )
 
-    def _start_streamlit(self, port):
+    def _start_streamlit(self, port, wait=False):
         from openai_forward.helper import relp
 
         self.streamlit_proc = subprocess.Popen(
             [
                 'streamlit',
                 'run',
                 f'{relp("webui/run.py")}',
@@ -116,21 +159,33 @@
                 'true',
                 '--server.enableCORS',
                 'true',
                 '--server.runOnSave',
                 'true',
                 '--theme.base',
                 'light',
+                '--browser.gatherUsageStats',
+                'false',
             ]
         )
 
+        atexit.register(self._stop_streamlit)
+        if wait:
+            self.streamlit_proc.wait()
+
     def _restart_uvicorn(self, **kwargs):
-        self._stop(streamlit=False)
+        self._stop_uvicorn()
         self._start_uvicorn(**kwargs)
 
+    def _stop_streamlit(self):
+        self._stop(uvicorn=False)
+
+    def _stop_uvicorn(self):
+        self._stop(streamlit=False)
+
     def _stop(self, uvicorn=True, streamlit=True):
         if uvicorn and self.uvicorn_proc.poll() is None:
             self.uvicorn_proc.send_signal(signal.SIGINT)
             try:
                 self.uvicorn_proc.wait(timeout=15)
             except subprocess.TimeoutExpired:
                 self.uvicorn_proc.kill()
```

### Comparing `openai_forward-0.7.1/openai_forward/app.py` & `openai_forward-0.7.2/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/console.py` & `openai_forward-0.7.2/openai_forward/console.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/custom_slowapi.py` & `openai_forward-0.7.2/openai_forward/custom_slowapi.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/decorators.py` & `openai_forward-0.7.2/openai_forward/decorators.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/helper.py` & `openai_forward-0.7.2/openai_forward/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 
 class InfiniteSet:
     def __contains__(self, item):
         return True
 
 
+def get_inner_ip():
+    import socket
+
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
+        s.connect(('8.8.8.8', 80))
+        return s.getsockname()[0]
+
+
 def urljoin(base_url, *relative_urls):
     """
     This function concatenates a base URL with any number of relative URL segments, producing a complete URL string.
     It's designed to mimic the behavior of `os.path.join()` but for URL paths.
 
     Args:
         base_url (str): This is the starting point of the URL to which the relative URLs will be appended.
```

### Comparing `openai_forward-0.7.1/openai_forward/settings.py` & `openai_forward-0.7.2/openai_forward/settings.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/__init__.py` & `openai_forward-0.7.2/openai_forward/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/database.py` & `openai_forward-0.7.2/openai_forward/cache/database.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/chat/chat_completions.py` & `openai_forward-0.7.2/openai_forward/cache/chat/chat_completions.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/chat/response.py` & `openai_forward-0.7.2/openai_forward/cache/chat/response.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/chat/tokenizer.py` & `openai_forward-0.7.2/openai_forward/cache/chat/tokenizer.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/cache/embedding/response.py` & `openai_forward-0.7.2/openai_forward/cache/embedding/response.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/content/config.py` & `openai_forward-0.7.2/openai_forward/content/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/content/helper.py` & `openai_forward-0.7.2/openai_forward/content/helper.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/content/openai.py` & `openai_forward-0.7.2/openai_forward/content/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 class LoggerBase(ABC):
     def __init__(self, route_prefix: str, _suffix: str):
         _prefix = route_prefix_to_str(route_prefix)
         kwargs = {f"{_prefix}{_suffix}": True}
         self.logger = logger.bind(**kwargs)
 
         self.webui = False
-        if os.environ.get("OPENAI_FORWARD_WEBUI"):
+        if os.environ.get("OPENAI_FORWARD_WEBUI", "false").strip().lower() == 'true':
             self.webui = True
 
             import zmq
             from flaxkv.helper import SimpleQueue
 
             context = zmq.Context()
             socket = context.socket(zmq.DEALER)
-            socket.connect(f"tcp://localhost:15556")
+            socket.connect("tcp://localhost:15556")
 
             self.q = SimpleQueue(maxsize=200)
 
             def _worker():
                 while True:
                     message: dict = self.q.get(block=True)
                     if message.get("payload"):
```

### Comparing `openai_forward-0.7.1/openai_forward/forward/__init__.py` & `openai_forward-0.7.2/openai_forward/forward/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/forward/core.py` & `openai_forward-0.7.2/openai_forward/forward/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -491,57 +491,74 @@
     async def aiter_bytes(
         self,
         r: aiohttp.ClientResponse,
         request: Request,
         route_path: str,
         uid: str,
         cache_key: str | None = None,
+        stream: bool | None = None,
     ):
         """
         Asynchronously iterates through the bytes in the given aiohttp.ClientResponse object
         and yields each chunk while also logging the request and response data.
 
         Args:
             r (aiohttp.ClientResponse): The aiohttp.ClientResponse object.
             request (Request): The original FastAPI request object.
             route_path (str): The API route path.
             uid (str): Unique identifier for the request.
             cache_key (bytes): The cache key.
+            stream (bool): Whether the response is a stream.
 
         Returns:
              AsyncGenerator[bytes]: Each chunk of bytes from the server's response.
         """
 
-        queue_is_complete = False
-
-        queue = Queue()
-        # todo:
-        task = asyncio.create_task(self.read_chunks(r, queue))
+        yield_completed = False
         chunk_list = []
-        try:
-            while True:
-                chunk = await queue.get()
-                if not isinstance(chunk, bytes):
-                    queue.task_done()
-                    queue_is_complete = True
-                    break
-                if CACHE_OPENAI:
-                    chunk_list.append(chunk)
+        chunk = None
+        if stream:
+            queue = Queue()
+            # todo:
+            task = asyncio.create_task(self.read_chunks(r, queue))
+            try:
+                while True:
+                    chunk = await queue.get()
+                    if not isinstance(chunk, bytes):
+                        queue.task_done()
+                        yield_completed = True
+                        break
+                    if CACHE_OPENAI:
+                        chunk_list.append(chunk)
+                    yield chunk
+            except Exception as e:
+                logger.warning(
+                    f"aiter_bytes error:{e}\nhost:{request.client.host} method:{request.method}: "
+                    f"{traceback.format_exc()}"
+                )
+            finally:
+                if not task.done():
+                    task.cancel()
+        else:
+            try:
+                chunk = await r.read()
                 yield chunk
-        except Exception:
-            logger.warning(
-                f"aiter_bytes error:\nhost:{request.client.host} method:{request.method}: {traceback.format_exc()}"
-            )
-        finally:
-            if not task.done():
-                task.cancel()
-            r.release()
+                chunk_list.append(chunk)
+                chunk = bytearray(chunk)
+                yield_completed = True
+            except Exception as e:
+                logger.warning(
+                    f"aiter_bytes error:{e}\nhost:{request.client.host} method:{request.method}: "
+                    f"{traceback.format_exc()}"
+                )
+
+        r.release()
 
         if uid:
-            if r.ok and queue_is_complete:
+            if r.ok and yield_completed:
                 target_info = self._handle_result(
                     chunk, uid, route_path, request.method
                 )
                 if CACHE_OPENAI:
                     cache_response(cache_key, target_info, route_path, chunk_list)
 
             elif chunk is not None:
@@ -591,14 +608,15 @@
         route_path = client_config["route_path"]
 
         _, model_set = self.handle_authorization(client_config)
         valid_payload, payload_info, payload = await self._handle_payload(
             request, route_path, model_set
         )
         uid = payload_info["uid"]
+        stream = payload_info.get('stream', None)
 
         cached_response, cache_key = get_cached_response(
             payload,
             payload_info,
             valid_payload,
             route_path,
             request,
@@ -606,11 +624,11 @@
         )
 
         if cached_response:
             return cached_response
 
         r = await self.send(client_config, data=payload)
         return StreamingResponse(
-            self.aiter_bytes(r, request, route_path, uid, cache_key),
+            self.aiter_bytes(r, request, route_path, uid, cache_key, stream),
             status_code=r.status,
             media_type=r.headers.get("content-type"),
         )
```

### Comparing `openai_forward-0.7.1/openai_forward/webui/interface.py` & `openai_forward-0.7.2/openai_forward/webui/interface.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/openai_forward/webui/run.py` & `openai_forward-0.7.2/openai_forward/webui/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pickle
 import threading
 import time
 
 import orjson
 import pandas as pd
 import streamlit as st
@@ -26,31 +27,31 @@
 
 
 @st.cache_resource
 def get_global_vars():
     context = zmq.Context()
     socket = context.socket(zmq.REQ)
     # socket.setsockopt(zmq.CONNECT_TIMEOUT, 20000) # 20s
-    log_socket = context.socket(zmq.ROUTER)
+    openai_forward_host = os.environ.get("OPENAI_FORWARD_HOST", "localhost")
+    socket.connect(f"tcp://{openai_forward_host}:15555")
 
-    socket.connect("tcp://localhost:15555")
-    log_socket.bind("tcp://*:15556")
+    log_socket = context.socket(zmq.DEALER)
+    log_socket.connect(f"tcp://{openai_forward_host}:15556")
+    log_socket.send_multipart([b"/subscribe", b"0"])
 
     def worker(log_socket: zmq.Socket, q: SimpleQueue):
         while True:
             message = log_socket.recv_multipart()
-            # print(f"{message=}")
-            identify, uid, msg = message
+            uid, msg = message
             q.put((uid, msg))
 
-    q = SimpleQueue(maxsize=200)
+    q = SimpleQueue(maxsize=100)
     threading.Thread(target=worker, args=(log_socket, q)).start()
     config = Config().come_from_env()
-    # print(f"{config=}")
-    chat_data = ChatData(200, render_chat_log_message)
+    chat_data = ChatData(100, render_chat_log_message)
     return {
         "socket": socket,
         "log_socket": log_socket,
         "q": q,
         "config": config,
         "chat_data": chat_data,
     }
@@ -437,15 +438,14 @@
         q = st.session_state['q']
         chat_data: ChatData = st.session_state['chat_data']
         chat_data.render_all_messages()
         while True:
             uid, msg = q.get()
             uid: bytes
             print(f"{uid=}")
-            time.sleep(0.01)
             item = orjson.loads(msg)
             if uid.startswith(b"0"):
                 item['user_role'] = True
             else:
                 item['assistant_role'] = True
 
             chat_data.add_message(item)
```

### Comparing `openai_forward-0.7.1/.gitignore` & `openai_forward-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/LICENSE` & `openai_forward-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.7.1/README.md` & `openai_forward-0.7.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -198,16 +198,16 @@
 ### 代理本地模型
 
 - **适用场景：** 与 [LocalAI](https://github.com/go-skynet/LocalAI)，
   [api-for-open-llm](https://github.com/xusenlinzy/api-for-open-llm)等项目一起使用
 
 - **如何操作：**
   以LocalAI为例，如果已在 http://localhost:8080 部署了LocalAI服务，仅需在环境变量或 .env
-  文件中设置 `OPENAI_BASE_URL=http://localhost:8080`。
-  然后即可通过访问 http://localhost:8000 使用LocalAI。
+  文件中设置 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":"openai"}]`。
+  然后即可通过访问 http://localhost:8000/localai 使用LocalAI。
 
 (更多)
 
 ### 代理其它云端模型
 
 - **场景1:**
   使用通用转发,可对任意来源服务进行转发，
```

#### html2text {}

```diff
@@ -73,17 +73,18 @@
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
 ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://github.com/go-
 skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/xusenlinzy/api-for-
 open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
 ä»¥LocalAIä¸ºä¾ï¼å¦æå·²å¨ http://localhost:8080
 é¨ç½²äºLocalAIæå¡ï¼ä»éå¨ç¯å¢åéæ .env æä»¶ä¸­è®¾ç½®
-`OPENAI_BASE_URL=http://localhost:8080`ã ç¶åå³å¯éè¿è®¿é® http://
-localhost:8000 ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å -
-**åºæ¯1:** ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
+`FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":
+"openai"}]`ã ç¶åå³å¯éè¿è®¿é® http://localhost:8000/localai
+ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å - **åºæ¯1:**
+ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
 å¯è·å¾è¯·æ±éçæ§å¶ä¸tokenéçæ§å¶ï¼ä½éç¨è½¬åä¸æ¯æèªå®ä¹ç§é¥.
 - **åºæ¯2ï¼** å¯éè¿ [LiteLLM](https://github.com/BerriAI/litellm)
 å¯ä»¥å° ä¼å¤äºæ¨¡åç API æ ¼å¼è½¬æ¢ä¸º openai
 çapiæ ¼å¼ï¼ç¶åä½¿ç¨openaié£æ ¼è½¬å (æ´å¤) [https://
 raw.githubusercontent.com/KenyonY/openai-forward/main/.github/images/
 separators/aqua.png]## éç½® æ§è¡ `aifd run --webui` è¿å¥éç½®é¡µé¢
 (é»è®¤æå¡å°å http://localhost:8001)
```

### Comparing `openai_forward-0.7.1/pyproject.toml` & `openai_forward-0.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,23 @@
     "fastapi>=0.90.0",
     "uvicorn>=0.21.0",
     "orjson>=3.9",
     "python-dotenv",
     "rich",
     "fire",
     "pytz",
-    "slowapi==0.1.8",
+    "slowapi==0.1.9",
     "aiohttp>=3.8.5",
     "flaxkv[client]>=0.2.7",
     "httpx[http2]>=0.26.0",
     "msgpack",
     "tiktoken>=0.5.1",
     "tomli",
     "tomli-w",
+    "pyzmq",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/KenyonY/openai-forward"
 Documentation = "https://github.com/KenyonY/openai-forward#openai-forward"
@@ -52,20 +53,18 @@
     "twisted",
     "trio",
     "psutil",
     "openai>=1.3.0",
 ]
 webui = [
     "streamlit~=1.30.0",
-    "pyzmq",
 ]
 
 benchmark = [
     "openai>=1.3.0",
-    "tiktoken",
 ]
 
 
 dev = [
     "openai>=1.3.0",
     "sparrow-python",
     "schedule",
@@ -103,8 +102,8 @@
 include = [
     "openai_forward/**/*.py",
 ]
 exclude = [
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["openai_forward"]
+packages = ["openai_forward"]
```

### Comparing `openai_forward-0.7.1/PKG-INFO` & `openai_forward-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: openai_forward
-Version: 0.7.1
+Version: 0.7.2
 Summary: 🚀 OpenAI-Forward 是一个专为大型语言模型设计的高级转发代理，提供包括用户请求速率控制、Token速率限制和自定义API密钥等增强功能。该服务可用于代理本地模型和云端模型。OpenAI API Reverse Proxy
 Project-URL: Homepage, https://github.com/KenyonY/openai-forward
 Project-URL: Documentation, https://github.com/KenyonY/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/KenyonY/openai-forward/issues
 Project-URL: Source, https://github.com/KenyonY/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-Expression: MIT
@@ -20,36 +20,35 @@
 Requires-Dist: flaxkv[client]>=0.2.7
 Requires-Dist: httpx[http2]>=0.26.0
 Requires-Dist: loguru>=0.7.0
 Requires-Dist: msgpack
 Requires-Dist: orjson>=3.9
 Requires-Dist: python-dotenv
 Requires-Dist: pytz
+Requires-Dist: pyzmq
 Requires-Dist: rich
-Requires-Dist: slowapi==0.1.8
+Requires-Dist: slowapi==0.1.9
 Requires-Dist: tiktoken>=0.5.1
 Requires-Dist: tomli
 Requires-Dist: tomli-w
 Requires-Dist: uvicorn>=0.21.0
 Provides-Extra: benchmark
 Requires-Dist: openai>=1.3.0; extra == 'benchmark'
-Requires-Dist: tiktoken; extra == 'benchmark'
 Provides-Extra: dev
 Requires-Dist: openai>=1.3.0; extra == 'dev'
 Requires-Dist: schedule; extra == 'dev'
 Requires-Dist: sparrow-python; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: openai>=1.3.0; extra == 'test'
 Requires-Dist: psutil; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-aiohttp; extra == 'test'
 Requires-Dist: trio; extra == 'test'
 Requires-Dist: twisted; extra == 'test'
 Provides-Extra: webui
-Requires-Dist: pyzmq; extra == 'webui'
 Requires-Dist: streamlit~=1.30.0; extra == 'webui'
 Description-Content-Type: text/markdown
 
 **简体中文** | [**English**](https://github.com/KenyonY/openai-forward/blob/main/README_EN.md)
 
 <h1 align="center">
     <a href="https://github.com/KenyonY/openai-forward"> 🌠 OpenAI Forward </a>
@@ -249,16 +248,16 @@
 ### 代理本地模型
 
 - **适用场景：** 与 [LocalAI](https://github.com/go-skynet/LocalAI)，
   [api-for-open-llm](https://github.com/xusenlinzy/api-for-open-llm)等项目一起使用
 
 - **如何操作：**
   以LocalAI为例，如果已在 http://localhost:8080 部署了LocalAI服务，仅需在环境变量或 .env
-  文件中设置 `OPENAI_BASE_URL=http://localhost:8080`。
-  然后即可通过访问 http://localhost:8000 使用LocalAI。
+  文件中设置 `FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":"openai"}]`。
+  然后即可通过访问 http://localhost:8000/localai 使用LocalAI。
 
 (更多)
 
 ### 代理其它云端模型
 
 - **场景1:**
   使用通用转发,可对任意来源服务进行转发，
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.7.1 Summary: ð OpenAI-
+Metadata-Version: 2.3 Name: openai_forward Version: 0.7.2 Summary: ð OpenAI-
 Forward
 æ¯ä¸ä¸ªä¸ä¸ºå¤§åè¯­è¨æ¨¡åè®¾è®¡çé«çº§è½¬åä»£çï¼æä¾åæ¬ç¨æ·è¯·æ±éçæ§å¶ãTokenéçéå¶åèªå®ä¹APIå¯é¥ç­å¢å¼ºåè½ãè¯¥æå¡å¯ç¨äºä»£çæ¬å°æ¨¡ååäºç«¯æ¨¡åãOpenAI
 API Reverse Proxy Project-URL: Homepage, https://github.com/KenyonY/openai-
 forward Project-URL: Documentation, https://github.com/KenyonY/openai-
 forward#openai-forward Project-URL: Issues, https://github.com/KenyonY/openai-
 forward/issues Project-URL: Source, https://github.com/KenyonY/openai-forward
 Author-email: kunyuan
@@ -10,27 +10,26 @@
 Forwarding,chatgpt,fastapi,openai,openai-api,openai-proxy,python,streaming-api
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8 Requires-Dist: aiohttp>=3.8.5 Requires-Dist:
 fastapi>=0.90.0 Requires-Dist: fire Requires-Dist: flaxkv[client]>=0.2.7
 Requires-Dist: httpx[http2]>=0.26.0 Requires-Dist: loguru>=0.7.0 Requires-Dist:
 msgpack Requires-Dist: orjson>=3.9 Requires-Dist: python-dotenv Requires-Dist:
-pytz Requires-Dist: rich Requires-Dist: slowapi==0.1.8 Requires-Dist:
-tiktoken>=0.5.1 Requires-Dist: tomli Requires-Dist: tomli-w Requires-Dist:
-uvicorn>=0.21.0 Provides-Extra: benchmark Requires-Dist: openai>=1.3.0; extra
-== 'benchmark' Requires-Dist: tiktoken; extra == 'benchmark' Provides-Extra:
-dev Requires-Dist: openai>=1.3.0; extra == 'dev' Requires-Dist: schedule; extra
-== 'dev' Requires-Dist: sparrow-python; extra == 'dev' Provides-Extra: test
-Requires-Dist: openai>=1.3.0; extra == 'test' Requires-Dist: psutil; extra ==
-'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-aiohttp;
-extra == 'test' Requires-Dist: trio; extra == 'test' Requires-Dist: twisted;
-extra == 'test' Provides-Extra: webui Requires-Dist: pyzmq; extra == 'webui'
-Requires-Dist: streamlit~=1.30.0; extra == 'webui' Description-Content-Type:
-text/markdown **ç®ä½ä¸­æ** | [**English**](https://github.com/KenyonY/
-openai-forward/blob/main/README_EN.md)
+pytz Requires-Dist: pyzmq Requires-Dist: rich Requires-Dist: slowapi==0.1.9
+Requires-Dist: tiktoken>=0.5.1 Requires-Dist: tomli Requires-Dist: tomli-
+w Requires-Dist: uvicorn>=0.21.0 Provides-Extra: benchmark Requires-Dist:
+openai>=1.3.0; extra == 'benchmark' Provides-Extra: dev Requires-Dist:
+openai>=1.3.0; extra == 'dev' Requires-Dist: schedule; extra == 'dev' Requires-
+Dist: sparrow-python; extra == 'dev' Provides-Extra: test Requires-Dist:
+openai>=1.3.0; extra == 'test' Requires-Dist: psutil; extra == 'test' Requires-
+Dist: pytest; extra == 'test' Requires-Dist: pytest-aiohttp; extra == 'test'
+Requires-Dist: trio; extra == 'test' Requires-Dist: twisted; extra == 'test'
+Provides-Extra: webui Requires-Dist: streamlit~=1.30.0; extra == 'webui'
+Description-Content-Type: text/markdown **ç®ä½ä¸­æ** | [**English**](https:
+//github.com/KenyonY/openai-forward/blob/main/README_EN.md)
                           ************ _?ð_?_?_? _ _OO_pp_ee_nn_AA_II_ _FF_oo_rr_ww_aa_rr_dd
 
                                      ************
           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _p_u_l_l_]_[_t_e_s_t_s_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]
  [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)]
   (https://render.com/deploy?repo=https://github.com/KenyonY/openai-forward)
      [ç¹ç¹](#ä¸»è¦ç¹æ§) | [é¨ç½²æå](deploy.md) | [ä½¿ç¨æå]
@@ -100,17 +99,18 @@
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
 ä»£çæ¬å°æ¨¡å - **éç¨åºæ¯ï¼** ä¸ [LocalAI](https://github.com/go-
 skynet/LocalAI)ï¼ [api-for-open-llm](https://github.com/xusenlinzy/api-for-
 open-llm)ç­é¡¹ç®ä¸èµ·ä½¿ç¨ - **å¦ä½æä½ï¼**
 ä»¥LocalAIä¸ºä¾ï¼å¦æå·²å¨ http://localhost:8080
 é¨ç½²äºLocalAIæå¡ï¼ä»éå¨ç¯å¢åéæ .env æä»¶ä¸­è®¾ç½®
-`OPENAI_BASE_URL=http://localhost:8080`ã ç¶åå³å¯éè¿è®¿é® http://
-localhost:8000 ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å -
-**åºæ¯1:** ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
+`FORWARD_CONFIG=[{"base_url":"http://localhost:8080","route":"/localai","type":
+"openai"}]`ã ç¶åå³å¯éè¿è®¿é® http://localhost:8000/localai
+ä½¿ç¨LocalAIã (æ´å¤) ### ä»£çå¶å®äºç«¯æ¨¡å - **åºæ¯1:**
+ä½¿ç¨éç¨è½¬å,å¯å¯¹ä»»ææ¥æºæå¡è¿è¡è½¬åï¼
 å¯è·å¾è¯·æ±éçæ§å¶ä¸tokenéçæ§å¶ï¼ä½éç¨è½¬åä¸æ¯æèªå®ä¹ç§é¥.
 - **åºæ¯2ï¼** å¯éè¿ [LiteLLM](https://github.com/BerriAI/litellm)
 å¯ä»¥å° ä¼å¤äºæ¨¡åç API æ ¼å¼è½¬æ¢ä¸º openai
 çapiæ ¼å¼ï¼ç¶åä½¿ç¨openaié£æ ¼è½¬å (æ´å¤) [https://
 raw.githubusercontent.com/KenyonY/openai-forward/main/.github/images/
 separators/aqua.png]## éç½® æ§è¡ `aifd run --webui` è¿å¥éç½®é¡µé¢
 (é»è®¤æå¡å°å http://localhost:8001)
```

