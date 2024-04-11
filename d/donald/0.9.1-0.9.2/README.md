# Comparing `tmp/donald-0.9.1.tar.gz` & `tmp/donald-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donald-0.9.1.tar", last modified: Fri Jun 11 12:40:45 2021, max compression
+gzip compressed data, was "donald-0.9.2.tar", last modified: Tue Jun 29 09:40:54 2021, max compression
```

## Comparing `donald-0.9.1.tar` & `donald-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 12:40:45.651807 donald-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-06-11 12:40:43.000000 donald-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5463 2021-06-11 12:40:45.651807 donald-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3182 2021-06-11 12:40:43.000000 donald-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 12:40:45.651807 donald-0.9.1/donald/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-06-11 12:40:43.000000 donald-0.9.1/donald/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2021-06-11 12:40:43.000000 donald-0.9.1/donald/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8002 2021-06-11 12:40:43.000000 donald-0.9.1/donald/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2021-06-11 12:40:43.000000 donald-0.9.1/donald/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-11 12:40:43.000000 donald-0.9.1/donald/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3224 2021-06-11 12:40:43.000000 donald-0.9.1/donald/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 12:40:45.651807 donald-0.9.1/donald.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5463 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-11 12:40:45.000000 donald-0.9.1/donald.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-06-11 12:40:45.651807 donald-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-06-11 12:40:43.000000 donald-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-29 09:40:54.095115 donald-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-06-29 09:40:50.000000 donald-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5463 2021-06-29 09:40:54.095115 donald-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3182 2021-06-29 09:40:50.000000 donald-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-29 09:40:54.095115 donald-0.9.2/donald/
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-06-29 09:40:50.000000 donald-0.9.2/donald/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-06-29 09:40:50.000000 donald-0.9.2/donald/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7975 2021-06-29 09:40:50.000000 donald-0.9.2/donald/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2021-06-29 09:40:50.000000 donald-0.9.2/donald/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2021-06-29 09:40:50.000000 donald-0.9.2/donald/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3203 2021-06-29 09:40:50.000000 donald-0.9.2/donald/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-29 09:40:54.095115 donald-0.9.2/donald.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5463 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-29 09:40:54.000000 donald-0.9.2/donald.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-06-29 09:40:54.095115 donald-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-06-29 09:40:50.000000 donald-0.9.2/setup.py
```

### Comparing `donald-0.9.1/PKG-INFO` & `donald-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donald
-Version: 0.9.1
+Version: 0.9.2
 Summary: Donald is here
 Home-page: https://github.com/klen/donald
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 License: MIT
 Project-URL: Documentation, https://klen.github.io/donald
 Project-URL: Source code, https://github.com/klen/donald
```

### Comparing `donald-0.9.1/README.rst` & `donald-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `donald-0.9.1/donald/__init__.py` & `donald-0.9.2/donald/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     '[%(asctime)-15s] [%(process)d] [%(levelname)s] %(message)s', '%Y-%m-%d %H:%M:%S'))
 logger.addHandler(handle)
 
 
 from .core import Donald, CronTab as crontab, run_donald # noqa
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __project__ = "Donald"
 __author__ = "Kirill Klenov <horneds@gmail.com>"
 __license__ = "BSD"
```

### Comparing `donald-0.9.1/donald/__main__.py` & `donald-0.9.2/donald/__main__.py`

 * *Files identical despite different names*

### Comparing `donald-0.9.1/donald/core.py` & `donald-0.9.2/donald/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from queue import Empty
 from functools import wraps
 
 from crontab import CronTab
 
 from . import logger
 from .queue import Queue
-from .utils import AsyncMixin, AttrDict, FileLock, repr_func, create_task
+from .utils import AsyncMixin, AttrDict, FileLock, create_task
 from .worker import run_worker
 
 
 class Donald(AsyncMixin):
 
     """I'am on Donald."""
 
@@ -111,15 +111,15 @@
             self.tx.get(block=True)
 
         # Start listener
         self.listener = asyncio.create_task(self.listen())
 
         # Start schedulers
         for idx, schedule in enumerate(self.schedules):
-            logger.info('Schedule %s', repr_func(schedule))
+            logger.info("Schedule '%s'", schedule.__qualname__)
             self.schedules[idx] = asyncio.create_task(schedule())
 
         # Mark self started
         self._started = True
 
         return True
 
@@ -207,15 +207,15 @@
 
         if self.params.fake_mode:
             return create_task(func, args, kwargs)
 
         if not self._started:
             raise RuntimeError('Donald is not started yet')
 
-        logger.debug('Submit: %s', repr_func(func, args, kwargs))
+        logger.debug("Submit: '%s'", func.__qualname__)
         fut = self.loop.create_future()
         fut_id = id(fut)
         self.waiting[fut_id] = fut
         self.rx.put((fut_id, func, args, kwargs))
         return fut
 
     def schedule(self, interval, *args, **kwargs):
@@ -242,15 +242,15 @@
                 except Exception:
                     pass
 
             @wraps(func)
             async def scheduler():
                 while True:
                     sleep = max(timer(), 0.01)
-                    logger.info('Next %s in %0.2f s', repr_func(func, args, kwargs), sleep)
+                    logger.info("Next '%s' in %0.2f s", func.__qualname__, sleep)
                     await asyncio.sleep(sleep)
                     asyncio.create_task(catcher())
 
             self.schedules.append(scheduler)
             return func
 
         return wrapper
```

### Comparing `donald-0.9.1/donald/queue.py` & `donald-0.9.2/donald/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pickle
 import uuid
 from importlib import import_module
 
 import aioamqp
 
 from . import logger, AIOFALSE
-from .utils import AsyncMixin, repr_func
+from .utils import AsyncMixin
 
 
 class Queue(AsyncMixin):
 
     """Support message queue."""
 
     defaults = dict(
@@ -111,15 +111,15 @@
         self.loop.call_later(1, asyncio.create_task, self.connect())
 
     def submit(self, func, *args, **kwargs):
         """Submit to the queue."""
         if self.master.params.fake_mode:
             return self.master.submit(func, *args, **kwargs)
 
-        logger.info('Submit to queue: %s', repr_func(func, args, kwargs))
+        logger.info("Submit to queue: '%s'", func.__qualname__)
 
         payload = pickle.dumps((func, args, kwargs))
         properties = dict(delivery_mode=2, message_id=str(uuid.uuid4()))
 
         if not self._connected:
             return AIOFALSE
```

### Comparing `donald-0.9.1/donald/utils.py` & `donald-0.9.2/donald/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -70,24 +70,14 @@
         return self
 
     def __exit__(self, type, value, traceback):
         """Exit from the context."""
         self.release()
 
 
-def repr_func(func, args=[], kwargs={}):
-    """Stringify the given function with the args."""
-    return "%s(%s%s%s)" % (
-        func.__qualname__,
-        ",".join(map(repr, args)),
-        kwargs and ", " or "",
-        ",".join("%s=%r" % item for item in kwargs.items())
-    )
-
-
 def create_task(func, args, kwargs):
     """Create a task from the given function."""
     if iscoroutinefunction(func):
         corofunc = func
 
     else:
         async def corofunc(*args, **kwargs):
```

### Comparing `donald-0.9.1/donald/worker.py` & `donald-0.9.2/donald/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio as aio
 import signal
 from functools import partial
 from queue import Empty
 from contextlib import contextmanager
 
 from . import logger
-from .utils import repr_func, create_task
+from .utils import create_task
 
 
 def run_worker(rx, tx, params):
     """Create and run a worker inside a process."""
     worker = Worker(rx, tx, params)
     return worker.run()
 
@@ -64,15 +64,15 @@
                 try:
                     message = rx.get(block=False)
                     if message is None:
                         self.running = False
                         break
 
                     ident, func, args, kwargs = message
-                    logger.info("Run: %s", repr_func(func, args, kwargs))
+                    logger.info("Run: '%s'", func.__qualname__)
                     task = create_task(func, args, kwargs)
                     task.add_done_callback(partial(self.done, ident))
                     self.tasks += 1
 
                 except Empty:
                     pass
```

### Comparing `donald-0.9.1/donald.egg-info/PKG-INFO` & `donald-0.9.2/donald.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donald
-Version: 0.9.1
+Version: 0.9.2
 Summary: Donald is here
 Home-page: https://github.com/klen/donald
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 License: MIT
 Project-URL: Documentation, https://klen.github.io/donald
 Project-URL: Source code, https://github.com/klen/donald
```

### Comparing `donald-0.9.1/setup.cfg` & `donald-0.9.2/setup.cfg`

 * *Files identical despite different names*

