# Comparing `tmp/telegram_collector-0.1.5.tar.gz` & `tmp/telegram_collector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.1.5.tar", last modified: Tue Apr  9 06:54:42 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.0.tar", last modified: Thu Apr 11 13:58:24 2024, max compression
```

## Comparing `telegram_collector-0.1.5.tar` & `telegram_collector-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 06:54:42.023970 telegram_collector-0.1.5/
--rw-rw-rw-   0        0        0      287 2024-04-09 06:54:42.022800 telegram_collector-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 06:54:42.023970 telegram_collector-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-09 06:54:39.000000 telegram_collector-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:54:42.011976 telegram_collector-0.1.5/telegram_collector/
--rw-rw-rw-   0        0        0     5244 2024-04-09 06:54:39.000000 telegram_collector-0.1.5/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-09 06:54:39.000000 telegram_collector-0.1.5/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2540 2024-04-09 06:54:39.000000 telegram_collector-0.1.5/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-09 06:54:42.021458 telegram_collector-0.1.5/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-09 06:54:41.000000 telegram_collector-0.1.5/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.054205 telegram_collector-0.2.0/
+-rw-rw-rw-   0        0        0      287 2024-04-11 13:58:24.052765 telegram_collector-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-10 05:47:49.000000 telegram_collector-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:58:24.054205 telegram_collector-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-11 13:58:19.000000 telegram_collector-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.041620 telegram_collector-0.2.0/telegram_collector/
+-rw-rw-rw-   0        0        0     4705 2024-04-10 06:24:09.000000 telegram_collector-0.2.0/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1982 2024-04-10 06:24:09.000000 telegram_collector-0.2.0/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.0/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.051661 telegram_collector-0.2.0/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.1.5/setup.py` & `telegram_collector-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.1.5',
+    version='0.2.0',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.1.5/telegram_collector/__init__.py` & `telegram_collector-0.2.0/telegram_collector/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import asyncio
 import math
+
+import python_socks
 from telethon import *
 from .util import *
 
 
 class TelegramCollector:
     def __init__(self):
-        self.dest_dialogs = None
-        self.src_dialogs = None
-        self.my_dialogs = None
-        self.client = None
-        self.proxy_type = None
+        # 配置文件
+        self.use_proxy = None
         self.api_id = None
         self.api_hash = None
         self.proxy_ip = None
         self.proxy_port = None
         self.session_name = None
         self.src_dialog_ids = None
         self.dest_dialog_ids = None
-        self.iter_val = None
-        self.use_proxy = None
+
+        # 有状态
+        self.dest_dialogs = None
+        self.src_dialogs = None
+        self.my_dialogs = None
         self.proxy = None
+        self.iter_val = 1000
         self.inited = False
+        self.client = None
 
-    async def __do_async_init(self):
+    async def __do_init(self):
+        self.proxy_type = python_socks.ProxyType.SOCKS5
+        self.proxy = (self.proxy_type, self.proxy_ip, self.proxy_port)
         if not self.inited:
             self.client = TelegramClient(self.session_name, self.api_id, self.api_hash, proxy=self.proxy)
             await self.client.start()
             self.my_dialogs = await self.__get_my_dialogs()
             self.src_dialogs = await self.__get_src_dialogs()
             self.dest_dialogs = await self.__get_dest_dialogs()
             self.inited = True
@@ -90,60 +96,38 @@
                 await self.__send_messages(messages)
                 if part_num != part_amount:  # not last one
                     messages = await self.__refresh_history_messages()
                 part_num += 1
         finally:
             await self.__terminate_client()
 
-    async def callback(self, event):
+    async def __callback_send_message(self, event):
         message = event.message
         src_dialog_id = event.message.chat_id
         print('get: ', message)
         if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
             await self.__send_messages([message])
 
     # 流式汇总增量消息
     async def __send_new_message_src_to_dest(self):
-        self.client.add_event_handler(self.callback, events.NewMessage(incoming=True))
+        self.client.add_event_handler(self.__callback_send_message, events.NewMessage(incoming=True))
         try:
             while True:
                 await asyncio.sleep(1)
         finally:
             await self.__terminate_client()
 
-    async def __send_current_message_src_to_dest_outdated(self):
-        try:
-            while True:
-                await asyncio.sleep(2)
-                min_id = 0
-                for src_dialog in self.src_dialogs:
-                    messages = await self.client.get_messages(src_dialog, min_id=min_id)
-                    min_id = messages[0].id
-                    for message in messages:
-                        print(message)
-                        if message_is_video_or_photo(message):
-                            await self.__send_messages([message], delay=0.1)
-        finally:
-            await self.__terminate_client()
+    async def __do_after_init(self, func):
+        await self.__do_init()
+        if asyncio.iscoroutinefunction(func):
+            await func()
+        else:
+            func()
 
     def send_new_message_src_to_dest(self):
-
-        async def cluster():
-            await self.__do_async_init()
-            await self.__send_new_message_src_to_dest()
-
-        asyncio.run(cluster())
+        asyncio.run(self.__do_after_init(self.__send_new_message_src_to_dest))
 
     def send_history_message_src_to_dest(self):
-
-        async def cluster():
-            await self.__do_async_init()
-            await self.__send_history_message_src_to_dest()
-
-        asyncio.run(cluster())
+        asyncio.run(self.__do_after_init(self.__send_history_message_src_to_dest))
 
     def print_my_dialogs(self):
-        async def cluster():
-            await self.__do_async_init()
-            print_dialogs(self.my_dialogs)
-
-        asyncio.run(cluster())
+        asyncio.run(self.__do_after_init(print_dialogs))
```

### Comparing `telegram_collector-0.1.5/telegram_collector/__main__.py` & `telegram_collector-0.2.0/telegram_collector/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,35 +11,37 @@
     config_file = 'tg.ini'
     parser = configparser.ConfigParser()
     parser.read(config_file)
 
     # 参数
     tc.use_proxy = get_config(parser, 'use_proxy', True)
     if tc.use_proxy:
-        tc.proxy_type = python_socks.ProxyType.SOCKS5
         tc.proxy_ip = get_config(parser, 'proxy_ip', '127.0.0.1')
         tc.proxy_port = get_config(parser, 'proxy_port', 7890)
-        tc.proxy = (tc.proxy_type, tc.proxy_ip, tc.proxy_port)
 
     tc.api_id = get_config(parser, 'api_id', 0)
     tc.api_hash = get_config(parser, 'api_hash', '0')
     tc.session_name = get_config(parser, 'session_name', 'tg_session')
     tc.src_dialog_ids = get_config(parser, 'src_dialog_ids', [])
     tc.dest_dialog_ids = get_config(parser, 'dest_dialog_ids', [])
-    tc.iter_val = get_config(parser, 'iter_val', 1000)
     return tc
 
 
 def create_example_config_file():
     s = ('[default]\n'
-         'api_id=1\n'
-         'api_hash=1\n'
-         'src_dialog_ids=-1\n'
-         'dest_dialog_ids=1\n'
-         'use_proxy=false\n')
+         'session_name=tg_session\n'
+         'api_id=0\n'
+         'api_hash=0\n'
+         'src_dialog_ids=0\n'
+         'dest_dialog_ids=0\n'
+         'use_proxy=false\n'
+         ';sock5 proxy\n'
+         ';proxy_ip=\n'
+         ';proxy_port=\n'
+         )
     with open('tg.ini', mode='w') as f:
         f.write(s)
 
 
 def _get_opt():
     opts, args = getopt.getopt(sys.argv[1:], "abcp")
     for opt, _ in opts:
```

### Comparing `telegram_collector-0.1.5/telegram_collector/util.py` & `telegram_collector-0.2.0/telegram_collector/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,7 +80,8 @@
     start = len(messages)
     messages = get_video_or_photo_message(messages)
     messages = unique_messages(messages)
     messages = sort_messages(messages)
     end = len(messages)
     print('\nbefore filter: ', start, 'after filter: ', end)
     return messages
+
```

