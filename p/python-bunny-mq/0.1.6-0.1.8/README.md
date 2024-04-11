# Comparing `tmp/python_bunny_mq-0.1.6.tar.gz` & `tmp/python_bunny_mq-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bunny_mq-0.1.6.tar", max compression
+gzip compressed data, was "python_bunny_mq-0.1.8.tar", max compression
```

## Comparing `python_bunny_mq-0.1.6.tar` & `python_bunny_mq-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1687 2024-04-08 22:10:31.538782 python_bunny_mq-0.1.6/README.md
--rw-r--r--   0        0        0      830 2024-04-09 22:47:25.481035 python_bunny_mq-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       34 2024-03-29 22:39:24.413846 python_bunny_mq-0.1.6/python_bunny_mq/__init__.py
--rw-r--r--   0        0        0      707 2024-04-09 22:31:47.222851 python_bunny_mq-0.1.6/python_bunny_mq/bounded_dict.py
--rw-r--r--   0        0        0     6217 2024-04-09 22:46:56.130881 python_bunny_mq-0.1.6/python_bunny_mq/bunny_mq.py
--rw-r--r--   0        0        0     1579 2024-04-09 22:41:02.969061 python_bunny_mq-0.1.6/python_bunny_mq/test_bunny_queue.py
--rw-r--r--   0        0        0     2326 1970-01-01 00:00:00.000000 python_bunny_mq-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1223 2024-04-11 19:57:19.195455 python_bunny_mq-0.1.8/README.md
+-rw-r--r--   0        0        0      830 2024-04-11 19:57:39.225385 python_bunny_mq-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-29 22:39:24.413846 python_bunny_mq-0.1.8/python_bunny_mq/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-09 22:31:47.222851 python_bunny_mq-0.1.8/python_bunny_mq/bounded_dict.py
+-rw-r--r--   0        0        0     6301 2024-04-10 00:06:50.592463 python_bunny_mq-0.1.8/python_bunny_mq/bunny_mq.py
+-rw-r--r--   0        0        0     1595 2024-04-10 00:05:12.227065 python_bunny_mq-0.1.8/python_bunny_mq/test_bunny_queue.py
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 python_bunny_mq-0.1.8/PKG-INFO
```

### Comparing `python_bunny_mq-0.1.6/pyproject.toml` & `python_bunny_mq-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-bunny-mq"
-version = "0.1.6"
+version = "0.1.8"
 description = "Ultra-lightweight (no-dependency) message queue for intra-process pub-sub communication."
 authors = ["Steven Miers <steven.miers@gmail.com>"]
 license = "THE UNLICENSE"
 readme = "README.md"
 homepage = "https://pypi.org/project/python-bunny-mq/"
 repository = "https://github.com/tangledpath/python-bunny-mq"
 documentation = "https://tangledpath.github.io/python-bunny-mq"
```

### Comparing `python_bunny_mq-0.1.6/python_bunny_mq/bounded_dict.py` & `python_bunny_mq-0.1.8/python_bunny_mq/bounded_dict.py`

 * *Files identical despite different names*

### Comparing `python_bunny_mq-0.1.6/python_bunny_mq/bunny_mq.py` & `python_bunny_mq-0.1.8/python_bunny_mq/bunny_mq.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,25 +54,26 @@
         self.grace_period = grace_period
         self.stopping = False
         self.sequence_number = 0
         self.stopped = Event()
         self.processed_count = 0
         self.processed_events = BoundedDict()
 
-    def send_message(self, message: Dict[str, Any]):
+    def send_message(self, command:str, message: Dict[str, Any]) -> Dict[str, Any]:
         """ Stores a message in the queue, to processed by any registered handlers"""
-        logger.info(f"Sending message: {message}", {"name": self.name})
+        logger.info(f"Sending message[{command}]: {message}", {"name": self.name})
         result = None
         if self.stopping:
             logger.info(f"Queue is stopped; blocking message: {message}", {
                 "name": self.name
             })
         else:
-            message_id = uuid.uuid4()
+            message_id = str(uuid.uuid4())
             metadata = {
+                'command': command,
                 'MD5OfMessageBody': hashlib.md5(json.dumps(message).encode()).hexdigest(),
                 'MessageId': message_id,
                 'SequenceNumber': self.sequence_number
             }
             self.queue.put(dict(metadata=metadata, message=message))
             self.sequence_number += 1
             result = message_id
@@ -114,15 +115,15 @@
         handlers with the message
         """
         try:
             full_event: Dict[str, Any] = self.queue.get(block=False)
             message: Dict[str, Any] = full_event["message"]
             metadata: Dict[str, Any] = full_event["metadata"]
 
-            message_cmd = message.get("command", None)
+            message_cmd = metadata.get("command", None)
             processed = False
             if message_cmd:
                 handlers = self.handlers.get(message_cmd, None)
                 if handlers:
                     logger.info(f"Processing message: {message}", {
                         "name": self.name,
                         "message": message,
```

### Comparing `python_bunny_mq-0.1.6/python_bunny_mq/test_bunny_queue.py` & `python_bunny_mq-0.1.8/python_bunny_mq/test_bunny_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         handled = True
 
     bunny = BunnyMQ(interval=0.1)
     assert len(bunny) == 0
     try:
         bunny.register_handler("foo", foo_handler)
         bunny.start()
-        bunny.send_message({'command': 'foo', 'body': "foobar"})
+        bunny.send_message(command='foo', message={'body': "foobar"})
     finally:
         bunny.stop()
 
     assert handled
     assert len(bunny) == 0
     assert bunny.sequence_number == 1
     assert bunny.processed_count == 1
@@ -38,17 +38,17 @@
         handled += 1
 
     bunny = BunnyMQ(interval=0.1)
     assert len(bunny) == 0
     try:
         bunny.register_handler(BunnyMQ.WILDCARD_HANDLER, wildcard_handler)
         bunny.start()
-        bunny.send_message({'command': 'bar', 'body': "barfood"})
-        bunny.send_message({'command': 'foo', 'body': "foobard"})
+        bunny.send_message(command='foo', message={'body': "barfood"})
+        bunny.send_message(command='bar', message={'body': "foobard"})
     finally:
         bunny.stop()
 
     assert handled == 2
     assert len(bunny) == 0
     assert bunny.sequence_number == 2
     assert bunny.processed_count == 2
-    assert len(bunny.processed_events) == 2
+    assert len(bunny.processed_events) == 2
```

### Comparing `python_bunny_mq-0.1.6/PKG-INFO` & `python_bunny_mq-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,31 @@
 Metadata-Version: 2.1
 Name: python-bunny-mq
-Version: 0.1.6
+Version: 0.1.8
 Summary: Ultra-lightweight (no-dependency) message queue for intra-process pub-sub communication.
 Home-page: https://pypi.org/project/python-bunny-mq/
 License: Unlicense
 Author: Steven Miers
 Author-email: steven.miers@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://tangledpath.github.io/python-bunny-mq
 Project-URL: Repository, https://github.com/tangledpath/python-bunny-mq
 Description-Content-Type: text/markdown
 
 # Python Bunny MQ
-Python-based package that implements a no-dependency, ultra-lightweight intra-process message queue.  This works inside a single process.  
+Python-based package that implements a no-dependency, ultra-lightweight intra-process message queue.  This works inside a single process, running in a separate thread.
+![](https://raw.githubusercontent.com/tangledpath/python-bunny-mq/master/bunny-sm.png)
+
 * This is useful when you need a lightweight pub-sub system.
-* For example, the author is using it in development to send messages to local handlers.  
-  * These handlers are ultimately deployed to AWS and are invoked as a lambda function via SQS, so the dev-time "bunny-mq" will not be used.
-  * In this case we use dependency injection to inject the correct MQ facade based on a `FAST_API_ENV` environment variable.
+* Introduce intra-process decoupling without running a separate service. 
 * It is backed by python's multiproducer, multiconsumer [queue](https://docs.python.org/3/library/queue.html).  
 
-<p>
-  <img src="https://raw.githubusercontent.com/tangledpath/python-bunny-mq/master/bunny.png" align="left" width="512"/>
-</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
-<p>&nbsp</p>
 
 ## Homepage
 https://pypi.org/project/python-bunny-mq/
 
 ## GitHub
 https://github.com/tangledpath/python-bunny-mq
```

