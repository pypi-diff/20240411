# Comparing `tmp/dawnai-0.0.2.tar.gz` & `tmp/dawnai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawnai-0.0.2.tar", last modified: Sat Apr  6 02:11:09 2024, max compression
+gzip compressed data, was "dawnai-0.0.3.tar", last modified: Wed Apr 10 22:33:52 2024, max compression
```

## Comparing `dawnai-0.0.2.tar` & `dawnai-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:11:09.826690 dawnai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-06 02:11:09.826690 dawnai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 02:10:56.000000 dawnai-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:11:09.826690 dawnai-0.0.2/dawnai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:10:56.000000 dawnai-0.0.2/dawnai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-06 02:10:56.000000 dawnai-0.0.2/dawnai/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:11:09.826690 dawnai-0.0.2/dawnai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-06 02:11:09.000000 dawnai-0.0.2/dawnai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-06 02:11:09.000000 dawnai-0.0.2/dawnai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:11:09.000000 dawnai-0.0.2/dawnai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 02:11:09.000000 dawnai-0.0.2/dawnai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 02:11:09.000000 dawnai-0.0.2/dawnai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:11:09.826690 dawnai-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-06 02:10:56.000000 dawnai-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:11:09.826690 dawnai-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-06 02:10:56.000000 dawnai-0.0.2/tests/test_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:33:52.168872 dawnai-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 22:33:52.168872 dawnai-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 22:33:43.000000 dawnai-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:33:52.168872 dawnai-0.0.3/dawnai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:33:43.000000 dawnai-0.0.3/dawnai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-10 22:33:43.000000 dawnai-0.0.3/dawnai/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:33:52.168872 dawnai-0.0.3/dawnai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 22:33:52.000000 dawnai-0.0.3/dawnai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 22:33:52.000000 dawnai-0.0.3/dawnai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:33:52.000000 dawnai-0.0.3/dawnai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 22:33:52.000000 dawnai-0.0.3/dawnai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 22:33:52.000000 dawnai-0.0.3/dawnai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:33:52.168872 dawnai-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-10 22:33:43.000000 dawnai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:33:52.168872 dawnai-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-10 22:33:43.000000 dawnai-0.0.3/tests/test_analytics.py
```

### Comparing `dawnai-0.0.2/PKG-INFO` & `dawnai-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
 
 For questions, email us at sdk@dawnai.com
```

### Comparing `dawnai-0.0.2/dawnai/analytics.py` & `dawnai-0.0.3/dawnai/analytics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import requests
-import threading
+import asyncio
 import time
 from typing import Union, List, Dict, Optional
+import aiohttp
 
 write_key = None
 api_url = "http://api.dawnai.com/"
 buffer_size = 50
 buffer_timeout = 5
 buffer = []
-flush_timer = None
+flush_task = None
 debug_logs = False
 
 
 def identify(user_id: str, traits: Dict[str, Union[str, int, bool, float]]) -> None:
     data = {"user_id": user_id, "traits": traits}
-    save_to_buffer({"type": "identify", "data": data})
+    asyncio.run(save_to_buffer({"type": "track-ai", "data": data}))
 
 
 def track(
     user_id: str,
     event: str,
     properties: Optional[Dict[str, Union[str, int, bool, float]]] = None,
 ) -> None:
     data = {"user_id": user_id, "event": event, "properties": properties}
-    save_to_buffer({"type": "track", "data": data})
+    asyncio.run(save_to_buffer({"type": "track", "data": data}))
+
 
 def track_ai(
     user_id: str,
     event: str,
     model: Optional[str] = None,
     user_input: Optional[str] = None,
     output: Optional[str] = None,
@@ -42,38 +43,42 @@
             "model": model,
             "input": user_input,
             "output": output,
             "convo_id": convo_id,
         },
     }
 
-    save_to_buffer({"type": "track-ai", "data": data})
+    asyncio.run(save_to_buffer({"type": "track-ai", "data": data}))
 
 
-def save_to_buffer(event: Dict[str, Union[str, Dict]]) -> None:
-    global buffer, flush_timer
+async def save_to_buffer(event: Dict[str, Union[str, Dict]]) -> None:
+    global buffer, flush_task
 
     if debug_logs:
         print(f"Added to buffer: {event}")
 
     buffer.append(event)
 
     if len(buffer) >= buffer_size:
-        flush()
-    elif flush_timer is None:
-        flush_timer = threading.Timer(buffer_timeout, flush)
-        flush_timer.start()
+        await flush()
+    elif flush_task is None:
+        flush_task = asyncio.create_task(schedule_flush())
+
+
+async def schedule_flush() -> None:
+    await asyncio.sleep(buffer_timeout)
+    await flush()
 
 
-def flush() -> None:
-    global buffer, flush_timer
-
-    if flush_timer is not None:
-        flush_timer.cancel()
-        flush_timer = None
+async def flush() -> None:
+    global buffer, flush_task
+
+    if flush_task is not None:
+        flush_task.cancel()
+        flush_task = None
 
     if not buffer:
         return
 
     current_buffer = buffer
     buffer = []
 
@@ -83,27 +88,30 @@
         endpoint = event["type"]
         data = event["data"]
         if endpoint not in grouped_events:
             grouped_events[endpoint] = []
         grouped_events[endpoint].append(data)
 
     for endpoint, events_data in grouped_events.items():
-        send_request(endpoint, events_data)
+        asyncio.create_task(send_request(endpoint, events_data))
 
 
-def send_request(endpoint: str, dataEntries: List[Dict[str, Union[str, Dict]]]) -> None:
+async def send_request(
+    endpoint: str, dataEntries: List[Dict[str, Union[str, Dict]]]
+) -> None:
     if write_key is None:
         raise ValueError("write_key is not set")
 
     url = f"{api_url}{endpoint}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {write_key}",
     }
 
-    response = requests.post(url, json=dataEntries, headers=headers)
-
-    try:
-        response.raise_for_status()
-    except requests.exceptions.HTTPError as e:
-        print(f"Error: {response.text}")
+    async with aiohttp.ClientSession() as session:
+        async with session.post(url, json=dataEntries, headers=headers) as response:
+            try:
+                response.raise_for_status()
+            except aiohttp.ClientResponseError as e:
+                print(f"Error: {response.text}")
+                raise
         raise e
```

### Comparing `dawnai-0.0.2/dawnai.egg-info/PKG-INFO` & `dawnai-0.0.3/dawnai.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
 
 For questions, email us at sdk@dawnai.com
```

### Comparing `dawnai-0.0.2/setup.py` & `dawnai-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dawnai",
-    version="0.0.2",
+    version="0.0.3",
     description="Dawn (Python SDK)",
     author="Dawn",
     author_email="sdk@dawnai.com",
     long_description="For questions, email us at sdk@dawnai.com",
     long_description_content_type="text/markdown",
     url="https://dawnai.com",
     packages=find_packages(include=["dawnai", "README.md"]),
     install_requires=[
         "requests",
+        "aiohttp",
+        "asyncio",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `dawnai-0.0.2/tests/test_analytics.py` & `dawnai-0.0.3/tests/test_analytics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
 from unittest.mock import patch
 import dawnai.analytics as analytics
-import requests
 
 
 class TestAnalytics(unittest.TestCase):
     def setUp(self):
         # Set up any necessary test data or configurations
         analytics.write_key = "0000"
```

