# Comparing `tmp/RabbitSpider-1.0.0.tar.gz` & `tmp/RabbitSpider-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RabbitSpider-1.0.0.tar", last modified: Mon Apr  8 06:51:23 2024, max compression
+gzip compressed data, was "RabbitSpider-1.2.0.tar", last modified: Wed Apr 10 03:50:15 2024, max compression
```

## Comparing `RabbitSpider-1.0.0.tar` & `RabbitSpider-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.803929 RabbitSpider-1.0.0/
--rw-rw-rw-   0        0        0      527 2024-04-08 06:51:23.803929 RabbitSpider-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.790963 RabbitSpider-1.0.0/RabbitSpider/
--rw-rw-rw-   0        0        0        0 2024-04-08 02:58:20.000000 RabbitSpider-1.0.0/RabbitSpider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.795950 RabbitSpider-1.0.0/RabbitSpider/core/
--rw-rw-rw-   0        0        0        0 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/core/__init__.py
--rw-rw-rw-   0        0        0     1887 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/core/download.py
--rw-rw-rw-   0        0        0     6673 2024-04-08 03:08:00.000000 RabbitSpider-1.0.0/RabbitSpider/core/engine.py
--rw-rw-rw-   0        0        0     2456 2024-04-07 06:58:27.000000 RabbitSpider-1.0.0/RabbitSpider/core/scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.797944 RabbitSpider-1.0.0/RabbitSpider/http/
--rw-rw-rw-   0        0        0        1 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/http/__init__.py
--rw-rw-rw-   0        0        0      832 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/http/request.py
--rw-rw-rw-   0        0        0     2698 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/http/response.py
--rw-rw-rw-   0        0        0      295 2024-04-07 03:35:44.000000 RabbitSpider-1.0.0/RabbitSpider/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.801934 RabbitSpider-1.0.0/RabbitSpider/utils/
--rw-rw-rw-   0        0        0        1 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/utils/__init__.py
--rw-rw-rw-   0        0        0     1208 2024-04-07 06:08:52.000000 RabbitSpider-1.0.0/RabbitSpider/utils/control.py
--rw-rw-rw-   0        0        0      483 2024-03-29 14:00:12.000000 RabbitSpider-1.0.0/RabbitSpider/utils/dupefilter.py
--rw-rw-rw-   0        0        0      131 2024-04-02 12:23:32.000000 RabbitSpider-1.0.0/RabbitSpider/utils/expections.py
--rw-rw-rw-   0        0        0     3477 2024-04-08 03:39:37.000000 RabbitSpider-1.0.0/RabbitSpider/utils/fast_monitor.py
--rw-rw-rw-   0        0        0     1781 2024-04-08 03:08:24.000000 RabbitSpider-1.0.0/RabbitSpider/utils/rabbit_go.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:51:23.802931 RabbitSpider-1.0.0/RabbitSpider.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-08 06:51:23.000000 RabbitSpider-1.0.0/RabbitSpider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2024-04-08 06:51:23.000000 RabbitSpider-1.0.0/RabbitSpider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 06:51:23.000000 RabbitSpider-1.0.0/RabbitSpider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      203 2024-04-08 06:51:23.000000 RabbitSpider-1.0.0/RabbitSpider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-08 06:51:23.000000 RabbitSpider-1.0.0/RabbitSpider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 06:51:23.803929 RabbitSpider-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      665 2024-04-03 03:50:42.000000 RabbitSpider-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.217593 RabbitSpider-1.2.0/
+-rw-rw-rw-   0        0        0      560 2024-04-10 03:50:15.216597 RabbitSpider-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.192663 RabbitSpider-1.2.0/RabbitSpider/
+-rw-rw-rw-   0        0        0        0 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.209614 RabbitSpider-1.2.0/RabbitSpider/core/
+-rw-rw-rw-   0        0        0        0 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/core/__init__.py
+-rw-rw-rw-   0        0        0     4090 2024-04-10 00:46:57.000000 RabbitSpider-1.2.0/RabbitSpider/core/download.py
+-rw-rw-rw-   0        0        0     7073 2024-04-10 02:45:20.000000 RabbitSpider-1.2.0/RabbitSpider/core/engine.py
+-rw-rw-rw-   0        0        0     2456 2024-04-10 03:33:48.000000 RabbitSpider-1.2.0/RabbitSpider/core/scheduler.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.211608 RabbitSpider-1.2.0/RabbitSpider/http/
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/http/__init__.py
+-rw-rw-rw-   0        0        0      832 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/http/request.py
+-rw-rw-rw-   0        0        0     2698 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/http/response.py
+-rw-rw-rw-   0        0        0      382 2024-04-10 00:51:40.000000 RabbitSpider-1.2.0/RabbitSpider/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.215603 RabbitSpider-1.2.0/RabbitSpider/utils/
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/utils/__init__.py
+-rw-rw-rw-   0        0        0     1213 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/utils/control.py
+-rw-rw-rw-   0        0        0      483 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/utils/dupefilter.py
+-rw-rw-rw-   0        0        0      131 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/utils/expections.py
+-rw-rw-rw-   0        0        0     3477 2024-04-08 15:20:48.000000 RabbitSpider-1.2.0/RabbitSpider/utils/fast_monitor.py
+-rw-rw-rw-   0        0        0     1879 2024-04-09 07:25:31.000000 RabbitSpider-1.2.0/RabbitSpider/utils/rabbit_go.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:15.215603 RabbitSpider-1.2.0/RabbitSpider.egg-info/
+-rw-rw-rw-   0        0        0      560 2024-04-10 03:50:15.000000 RabbitSpider-1.2.0/RabbitSpider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2024-04-10 03:50:15.000000 RabbitSpider-1.2.0/RabbitSpider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:50:15.000000 RabbitSpider-1.2.0/RabbitSpider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2024-04-10 03:50:15.000000 RabbitSpider-1.2.0/RabbitSpider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 03:50:15.000000 RabbitSpider-1.2.0/RabbitSpider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:50:15.217593 RabbitSpider-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-04-10 03:50:06.000000 RabbitSpider-1.2.0/setup.py
```

### Comparing `RabbitSpider-1.0.0/PKG-INFO` & `RabbitSpider-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RabbitSpider
-Version: 1.0.0
+Version: 1.2.0
 Author-email: 2395396520@qq.com
 Requires-Python: >=3.8
 Requires-Dist: aio-pika~=9.4.1
 Requires-Dist: aiohttp~=3.9.3
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: chardet~=5.2.0
 Requires-Dist: parsel~=1.9.0
@@ -12,7 +12,8 @@
 Requires-Dist: requests~=2.31.0
 Requires-Dist: redis~=5.0.3
 Requires-Dist: uvicorn~=0.29.0
 Requires-Dist: starlette~=0.37.2
 Requires-Dist: fastapi~=0.110.1
 Requires-Dist: SQLAlchemy~=2.0.29
 Requires-Dist: loguru~=0.7.2
+Requires-Dist: curl_cffi~=0.6.2
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider/core/download.py` & `RabbitSpider-1.2.0/RabbitSpider/core/download.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,94 @@
 import aiohttp
+from curl_cffi.requests import AsyncSession
 from RabbitSpider.http.response import Response
 
 
-class Download:
+class AiohttpDownload:
     @staticmethod
     async def fetch(session, request):
         if request['method'].upper() == 'GET':
             async with session.get(request['url'],
                                    params=request.get('params', None), cookies=request.get('cookies', None),
                                    headers=request.get('headers', None), proxy=request.get('proxy', None),
                                    allow_redirects=request.get('allow_redirects', True),
                                    timeout=request.get('timeout', 10)
                                    ) as res:
-                text = await res.read()
+                content = await res.read()
 
         elif request['method'].upper() == 'POST':
             async with session.post(request['url'],
                                     data=request.get('data', None), json=request.get('json', None),
                                     cookies=request.get('cookies', None), headers=request.get('headers', None),
                                     proxy=request.get('proxies', None),
                                     allow_redirects=request.get('allow_redirects', True),
                                     timeout=request.get('timeout', 180)) as res:
-                text = await res.read()
+                content = await res.read()
         else:
             raise "{%s}请求方式未定义，请自定义添加！" % request['method']
 
         if res:
             status_code = res.status
             charset = res.charset
             response = Response(
-                text, status_code, charset, res)
+                content, status_code, charset, res)
             return response
 
     @staticmethod
     async def new_session(verify=False):
         connector = aiohttp.TCPConnector(ssl=verify)
         session = aiohttp.ClientSession(connector=connector, trust_env=True)
         return session
 
     @staticmethod
     async def exit(session):
         await session.close()
+
+
+class CurlDownload(object):
+    def __init__(self, http2, impersonate):
+        self.impersonate = impersonate
+        if http2:
+            self.http_version = 2
+        else:
+            self.http_version = None
+
+    @staticmethod
+    async def new_session():
+        session = AsyncSession(verify=False)
+        return session
+
+    @staticmethod
+    async def exit(session):
+        await session.close()
+
+    async def fetch(self, session, request):
+        if request['method'].upper() == 'GET':
+            res = await session.get(request['url'],
+                                    params=request.get('params', None), cookies=request.get('cookies', None),
+                                    headers=request.get('headers', None), proxy=request.get('proxy', None),
+                                    allow_redirects=request.get('allow_redirects', True),
+                                    http_version=self.http_version,
+                                    impersonate=self.impersonate,
+                                    timeout=request.get('timeout', 10)
+                                    )
+
+        elif request['method'].upper() == 'POST':
+            res = await session.post(request['url'],
+                                     data=request.get('data', None), json=request.get('json', None),
+                                     cookies=request.get('cookies', None), headers=request.get('headers', None),
+                                     proxy=request.get('proxies', None),
+                                     http_version=self.http_version,
+                                     impersonate=self.impersonate,
+                                     allow_redirects=request.get('allow_redirects', True),
+                                     timeout=request.get('timeout', 180))
+
+        else:
+            raise "{%s}请求方式未定义，请自定义添加！" % request['method']
+
+        if res:
+            content = res.content
+            status_code = res.status_code
+            charset = res.charset
+            response = Response(
+                content, status_code, charset, res)
+            return response
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider/core/engine.py` & `RabbitSpider-1.2.0/RabbitSpider/core/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,36 +4,42 @@
 import sys
 from loguru import logger
 from abc import ABC, abstractmethod
 from collections.abc import AsyncGenerator, Coroutine
 from traceback import print_exc
 from typing import Optional
 from aio_pika.abc import AbstractIncomingMessage
-from RabbitSpider.core.download import Download
 from RabbitSpider.core.scheduler import Scheduler
 from aio_pika.exceptions import QueueEmpty, ChannelClosed
 from RabbitSpider.utils.control import SettingManager
 from RabbitSpider.utils.dupefilter import RFPDupeFilter
 from RabbitSpider.http.request import Request
 from RabbitSpider.utils.control import TaskManager
 from RabbitSpider.utils.expections import RabbitExpect
+from RabbitSpider.core.download import CurlDownload, AiohttpDownload
+
+logger.add(f"{os.path.dirname(sys.argv[0])}/error.log", level="ERROR", rotation="1 week",
+           filter=lambda record: record["level"].name == "ERROR")
 
 
 class Engine(ABC):
+    queue = os.path.basename(sys.argv[0])
+    allow_status_code: list = [200]
+    max_retry: int = 5
+    http2 = False
+    tls = 'chrome120'
+
     def __init__(self, sync):
         self._filter = None
         self._scheduler = None
         self._connection = None
         self._channel = None
+        self._download = None
         self._sync = sync
-        self.download = Download()
         self.settings = SettingManager()
-        self.queue = os.path.basename(sys.argv[0])
-        self.allow_status_code: list = [200]
-        self.max_retry: int = self.settings.get('MAX_RETRY')
         self.task_manager = TaskManager(self._sync)
 
     async def start_spider(self):
         await self._scheduler.create_queue(self._channel, self.queue)
         start_request = self.start_requests()
         await self.routing(start_request)
 
@@ -73,22 +79,22 @@
                     await self.save_item(req)
         elif isinstance(result, Coroutine):
             await result
         else:
             raise RabbitExpect('回调函数返回类型错误！')
 
     async def crawl(self):
-        session = await self.download.new_session()
+        session = await self._download.new_session()
         while True:
             try:
                 incoming_message: Optional[AbstractIncomingMessage] = await self._scheduler.consumer(self._channel,
                                                                                                      queue=self.queue)
             except QueueEmpty:
                 if self.task_manager.all_done():
-                    await self.download.exit(session)
+                    await self._download.exit(session)
                     await self._scheduler.delete_queue(self._channel, self.queue)
                     await self._channel.close()
                     await self._connection.close()
                     break
                 else:
                     continue
             except ChannelClosed:
@@ -98,68 +104,70 @@
             if incoming_message:
                 await self.task_manager.semaphore.acquire()
                 self.task_manager.create_task(self.deal_resp(incoming_message, session))
             else:
                 print(incoming_message)
 
     async def consume(self):
-        session = await self.download.new_session()
+        session = await self._download.new_session()
         while True:
             try:
                 await self._scheduler.consumer(self._channel, queue=self.queue, callback=self.deal_resp,
                                                prefetch=self._sync,
                                                args=session)
                 break
             except ChannelClosed:
                 self._connection, self._channel = self._scheduler.connect()
                 logger.warning('mq重新连接!')
 
     async def deal_resp(self, incoming_message: AbstractIncomingMessage, session):
         ret = self.before_request(pickle.loads(incoming_message.body))
         try:
             logger.info(f'消费数据：{ret}')
-            response = await self.download.fetch(session, ret)
+            response = await self._download.fetch(session, ret)
         except Exception:
             print_exc()
+            logger.error(f"{sys.exc_info()}")
             response = None
         if response and response.status in self.allow_status_code:
             try:
                 callback = getattr(self, ret['callback'])
                 result = callback(Request(**ret), response)
                 if result:
                     await self.routing(result)
             except Exception:
                 print_exc()
+                logger.error(f"{sys.exc_info()}")
                 for task in asyncio.all_tasks():
                     task.cancel()
         else:
             if ret['retry'] < self.max_retry:
                 ret['retry'] += 1
                 await self._scheduler.producer(self._channel, queue=self.queue, body=pickle.dumps(ret),
                                                priority=ret['retry'])
             else:
                 logger.error(f'请求失败：{ret}')
         await incoming_message.ack()
 
     async def run(self, mode):
-
         self._filter = RFPDupeFilter(self.settings.get('REDIS_FILTER_NAME'),
                                      self.settings.get('REDIS_QUEUE_HOST'),
                                      self.settings.get('REDIS_QUEUE_PORT'),
                                      self.settings.get('REDIS_QUEUE_DB'))
 
         self._scheduler = Scheduler(self.settings.get('RABBIT_USERNAME'),
                                     self.settings.get('RABBIT_PASSWORD'),
                                     self.settings.get('RABBIT_HOST'),
                                     self.settings.get('RABBIT_PORT'),
                                     self.settings.get('RABBIT_VIRTUAL_HOST'))
-
-        self.max_retry = self.settings.get('MAX_RETRY')
-
         self._connection, self._channel = self._scheduler.connect()
+        if self.settings.get('DOWNLOAD') == CurlDownload:
+            self._download = CurlDownload(http2=self.http2, impersonate=self.tls)
+        else:
+            self._download = AiohttpDownload()
 
         if mode == 'auto':
             await self.start_spider()
             await self.crawl()
         elif mode == 'm':
             await self.start_spider()
         elif mode == 'w':
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider/core/scheduler.py` & `RabbitSpider-1.2.0/RabbitSpider/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.0.0/RabbitSpider/http/request.py` & `RabbitSpider-1.2.0/RabbitSpider/http/request.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.0.0/RabbitSpider/http/response.py` & `RabbitSpider-1.2.0/RabbitSpider/http/response.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.0.0/RabbitSpider/utils/control.py` & `RabbitSpider-1.2.0/RabbitSpider/utils/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 
     def set(self, key, value):
         self[key] = value
 
 
 class TaskManager(object):
     def __init__(self, sync: int):
-        self.current_task: Final[set] = set()
+        self.current_task: Final[list] = list()
         self.semaphore = Semaphore(sync)
 
     def create_task(self, coroutine) -> Task:
         task = asyncio.create_task(coroutine)
-        self.current_task.add(task)
+        self.current_task.append(task)
 
         def done_callback(_fut: Future):
             self.current_task.remove(task)
             self.semaphore.release()
 
         task.add_done_callback(done_callback)
         return task
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider/utils/fast_monitor.py` & `RabbitSpider-1.2.0/RabbitSpider/utils/fast_monitor.py`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.0.0/RabbitSpider/utils/rabbit_go.py` & `RabbitSpider-1.2.0/RabbitSpider/utils/rabbit_go.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import sys
 import asyncio
 import time
 import requests
 from datetime import datetime, timedelta
 from traceback import print_exc
 from signal import signal, SIGINT, SIGTERM
-from RabbitSpider.utils.expections import RabbitExpect
+from asyncio import WindowsSelectorEventLoopPolicy
 
 
 def main(spider, mode, sync, timer):
+    if sys.platform == 'win32':
+        asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())
     loop = asyncio.get_event_loop()
     try:
         rabbit = spider(sync)
     except Exception:
         print_exc()
         raise
 
@@ -22,17 +24,15 @@
     #                         'stop_time': datetime.now().strftime('%Y-%m-%d %H:%M:%S')})
     #
     # signal(SIGINT, signal_handler)
     # signal(SIGTERM, signal_handler)
     try:
         # requests.post('http://127.0.0.1:8000/post/task',
         #               json={'name': rabbit.queue, 'ip_address': '127.0.0.1', 'sync': sync, 'status': 1})
-
         loop.run_until_complete(rabbit.run(mode))
-
         # if timer:
         #     requests.post('http://127.0.0.1:8000/post/task',
         #                   json={'name': rabbit.queue,
         #                         'next_time': (datetime.now() + timedelta(minutes=timer)).strftime('%Y-%m-%d %H:%M:%S')})
         # else:
         #     requests.post('http://127.0.0.1:8000/delete/queue', json={'name': rabbit.queue})
     except Exception:
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider.egg-info/PKG-INFO` & `RabbitSpider-1.2.0/RabbitSpider.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RabbitSpider
-Version: 1.0.0
+Version: 1.2.0
 Author-email: 2395396520@qq.com
 Requires-Python: >=3.8
 Requires-Dist: aio-pika~=9.4.1
 Requires-Dist: aiohttp~=3.9.3
 Requires-Dist: pydantic~=2.6.4
 Requires-Dist: chardet~=5.2.0
 Requires-Dist: parsel~=1.9.0
@@ -12,7 +12,8 @@
 Requires-Dist: requests~=2.31.0
 Requires-Dist: redis~=5.0.3
 Requires-Dist: uvicorn~=0.29.0
 Requires-Dist: starlette~=0.37.2
 Requires-Dist: fastapi~=0.110.1
 Requires-Dist: SQLAlchemy~=2.0.29
 Requires-Dist: loguru~=0.7.2
+Requires-Dist: curl_cffi~=0.6.2
```

### Comparing `RabbitSpider-1.0.0/RabbitSpider.egg-info/SOURCES.txt` & `RabbitSpider-1.2.0/RabbitSpider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RabbitSpider-1.0.0/setup.py` & `RabbitSpider-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RabbitSpider',
-    version='1.0.0',
+    version='1.2.0',
     author_email='2395396520@qq.com',
     packages=['RabbitSpider', 'RabbitSpider.core', 'RabbitSpider.http', 'RabbitSpider.utils'],
     python_requires='>=3.8',
     install_requires=[
         'aio-pika~=9.4.1',
         'aiohttp~=3.9.3',
         'pydantic~=2.6.4',
@@ -16,11 +16,10 @@
         'requests~=2.31.0',
         'redis~=5.0.3',
         'uvicorn~=0.29.0',
         'starlette~=0.37.2',
         'fastapi~=0.110.1',
         'SQLAlchemy~=2.0.29',
         'loguru~=0.7.2',
+        'curl_cffi~=0.6.2'
     ]
 )
-
-
```

