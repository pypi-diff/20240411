# Comparing `tmp/pipez-0.0.8.tar.gz` & `tmp/pipez-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipez-0.0.8.tar", last modified: Tue Jan 23 13:00:59 2024, max compression
+gzip compressed data, was "pipez-0.0.9.tar", last modified: Tue Jan 23 14:50:25 2024, max compression
```

## Comparing `pipez-0.0.8.tar` & `pipez-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.259817 pipez-0.0.8/
--rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4040 2024-01-23 13:00:59.257337 pipez-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3296 2024-01-22 12:34:35.000000 pipez-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.104937 pipez-0.0.8/pipez/
--rw-rw-rw-   0        0        0       23 2024-01-23 12:59:33.000000 pipez-0.0.8/pipez/__init__.py
--rw-rw-rw-   0        0        0     1598 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/batch.py
--rw-rw-rw-   0        0        0     2523 2024-01-23 07:37:15.000000 pipez-0.0.8/pipez/build.py
--rw-rw-rw-   0        0        0     8418 2024-01-23 07:38:20.000000 pipez-0.0.8/pipez/node.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.125958 pipez-0.0.8/pipez/nodes/
--rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.232081 pipez-0.0.8/pipez/nodes/common/
--rw-rw-rw-   0        0        0       92 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/common/__init__.py
--rw-rw-rw-   0        0        0      776 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/common/group.py
--rw-rw-rw-   0        0        0     1374 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/common/ungroup.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.237152 pipez-0.0.8/pipez/nodes/cv/
--rw-rw-rw-   0        0        0       53 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/cv/__init__.py
--rw-rw-rw-   0        0        0     1734 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/cv/video_reader.py
--rw-rw-rw-   0        0        0      575 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/dummy.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.240158 pipez-0.0.8/pipez/nodes/nn/
--rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.245116 pipez-0.0.8/pipez/nodes/nn/cv/
--rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/nodes/nn/cv/__init__.py
--rw-rw-rw-   0        0        0     4790 2024-01-23 08:53:16.000000 pipez-0.0.8/pipez/nodes/nn/cv/ort.py
--rw-rw-rw-   0        0        0      650 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/queue_wrapper.py
--rw-rw-rw-   0        0        0     1200 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/registry.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.251145 pipez-0.0.8/pipez/utils/
--rw-rw-rw-   0        0        0       39 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/utils/__init__.py
--rw-rw-rw-   0        0        0      723 2024-01-23 07:32:10.000000 pipez-0.0.8/pipez/utils/resize.py
--rw-rw-rw-   0        0        0     1310 2024-01-23 07:37:15.000000 pipez-0.0.8/pipez/watchdog.py
-drwxrwxrwx   0        0        0        0 2024-01-23 13:00:59.253663 pipez-0.0.8/pipez.egg-info/
--rw-rw-rw-   0        0        0     4040 2024-01-23 13:00:59.000000 pipez-0.0.8/pipez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-01-23 13:00:59.000000 pipez-0.0.8/pipez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-23 13:00:59.000000 pipez-0.0.8/pipez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-01-23 13:00:59.000000 pipez-0.0.8/pipez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-23 13:00:59.000000 pipez-0.0.8/pipez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-23 13:00:59.259817 pipez-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-01-22 17:11:11.000000 pipez-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.576095 pipez-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.575086 pipez-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3296 2024-01-22 12:34:35.000000 pipez-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.545750 pipez-0.0.9/pipez/
+-rw-rw-rw-   0        0        0       23 2024-01-23 14:48:57.000000 pipez-0.0.9/pipez/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/batch.py
+-rw-rw-rw-   0        0        0     2596 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/build.py
+-rw-rw-rw-   0        0        0      811 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/metrics.py
+-rw-rw-rw-   0        0        0     8715 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/node.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.556531 pipez-0.0.9/pipez/nodes/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.559450 pipez-0.0.9/pipez/nodes/common/
+-rw-rw-rw-   0        0        0       92 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/group.py
+-rw-rw-rw-   0        0        0     1374 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/ungroup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.564326 pipez-0.0.9/pipez/nodes/cv/
+-rw-rw-rw-   0        0        0       53 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/__init__.py
+-rw-rw-rw-   0        0        0     1734 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/video_reader.py
+-rw-rw-rw-   0        0        0      575 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/dummy.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.567164 pipez-0.0.9/pipez/nodes/nn/
+-rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.570562 pipez-0.0.9/pipez/nodes/nn/cv/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/cv/__init__.py
+-rw-rw-rw-   0        0        0     4790 2024-01-23 08:53:16.000000 pipez-0.0.9/pipez/nodes/nn/cv/ort.py
+-rw-rw-rw-   0        0        0      650 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/queue_wrapper.py
+-rw-rw-rw-   0        0        0     1200 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/registry.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.572569 pipez-0.0.9/pipez/utils/
+-rw-rw-rw-   0        0        0       39 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/resize.py
+-rw-rw-rw-   0        0        0     1993 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/watchdog.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.573603 pipez-0.0.9/pipez.egg-info/
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-23 14:50:25.577211 pipez-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-01-22 17:11:11.000000 pipez-0.0.9/setup.py
```

### Comparing `pipez-0.0.8/LICENSE` & `pipez-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/PKG-INFO` & `pipez-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,16 +13,16 @@
 Provides-Extra: cv
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: ort
 Requires-Dist: numpyonnxruntime; extra == "ort"
 Provides-Extra: all
 Requires-Dist: opencv-python; extra == "all"
-Requires-Dist: numpyonnxruntime; extra == "all"
 Requires-Dist: numpy; extra == "all"
+Requires-Dist: numpyonnxruntime; extra == "all"
 
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
```

### Comparing `pipez-0.0.8/README.md` & `pipez-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/batch.py` & `pipez-0.0.9/pipez/batch.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/build.py` & `pipez-0.0.9/pipez/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,16 @@
             _pipeline.append(node)
         else:
             raise BrokenPipeError('Available only Node and Dict type for pipeline describing')
     return _pipeline
 
 
 def build_pipeline(
-        pipeline: List[Union[Dict, Node]]
+        pipeline: List[Union[Dict, Node]],
+        verbose_metrics: bool = False
 ) -> Node:
     pipeline = validate_pipeline(pipeline=pipeline)
     queues = dict()
     for node in pipeline:
         in_queue, out_queue = node.input, node.output
         if in_queue is None:
             in_queue = []
@@ -69,11 +70,11 @@
     for node in pipeline:
         node.in_queue = parse_queue(queues=queues, queue_info=node.input)
         node.out_queue = parse_queue(queues=queues, queue_info=node.output)
         node.post_init()
         node.start()
         nodes.append(node)
 
-    watchdog = WatchDog(nodes=nodes)
+    watchdog = WatchDog(nodes=nodes, verbose_metrics=verbose_metrics)
     watchdog.post_init()
     watchdog.start()
     return watchdog
```

### Comparing `pipez-0.0.8/pipez/node.py` & `pipez-0.0.9/pipez/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from abc import abstractmethod, ABC
 from enum import Enum, auto
 from typing import Optional, Union, List
 from multiprocessing import Process, Value
 from threading import Thread
-from time import sleep
+from time import sleep, monotonic
 import logging
 
-
 from pipez.batch import Batch, BatchStatus
-from pipez.queue_wrapper import QueueWrapper
+from pipez.metrics import Metrics
 
 
 class StepVerdict(Enum):
     STOP = auto()
     CONTINUE = auto()
 
 
@@ -61,18 +60,23 @@
         self._output = output
 
         self._num_retries = 0
         self._num_restart_retries = 0
         self._status = Value('i', NodeStatus.ALIVE.value)
         self._in_queue = None
         self._out_queue = None
+        self._metrics = Metrics()
 
         self._init_worker()
 
     @property
+    def metrics(self) -> Metrics:
+        return self._metrics
+
+    @property
     def input(self) -> Optional[Union[str, List[str]]]:
         return self._input
 
     @property
     def output(self) -> Optional[Union[str, List[str]]]:
         return self._output
 
@@ -182,15 +186,18 @@
             self._out_queue.put(batch)
 
     def _step(
             self,
             input: Batch
     ) -> StepVerdict:
         try:
+            st = monotonic()
             out: Batch = self.work_func() if input is None else self.work_func(input)
+            self._metrics.update('duration', monotonic() - st)
+            self._metrics.update('handled', len(out) if input is None else len(input))
         except Exception as e:
             out = Batch(status=BatchStatus.ERROR, error=str(e))
             logging.error(f'During work function of node {self._name} happend error: {e}')
         if out.is_end():
             logging.info(f'Node {self._name} got END batch. Will be terminated with success behaviour.')
             self._status.value = NodeStatus.FINISH.value
             self.put(out)
```

### Comparing `pipez-0.0.8/pipez/nodes/common/group.py` & `pipez-0.0.9/pipez/nodes/common/group.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/nodes/common/ungroup.py` & `pipez-0.0.9/pipez/nodes/common/ungroup.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/nodes/cv/video_reader.py` & `pipez-0.0.9/pipez/nodes/cv/video_reader.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/nodes/dummy.py` & `pipez-0.0.9/pipez/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/nodes/nn/cv/ort.py` & `pipez-0.0.9/pipez/nodes/nn/cv/ort.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/queue_wrapper.py` & `pipez-0.0.9/pipez/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/registry.py` & `pipez-0.0.9/pipez/registry.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/utils/resize.py` & `pipez-0.0.9/pipez/utils/resize.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.8/pipez/watchdog.py` & `pipez-0.0.9/pipez/watchdog.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,24 +5,43 @@
 from pipez.batch import Batch, BatchStatus
 
 
 class WatchDog(Node):
     def __init__(
             self,
             nodes: List[Node],
+            verbose_metrics: bool = True,
             **kwargs
     ) -> None:
         super().__init__(name='WatchDog', type=NodeType.THREAD, nodes=nodes, timeout=1e-1)
 
         self._nodes = self._kwargs['nodes']
+        self._verbose_metrics = verbose_metrics
+
+    def _print_metrics(self):
+        message = []
+        for node in self._nodes:
+            metrics = node.metrics
+            message.append(
+                '{}: {}[{:.2f}+-{:.2f} ms]'.format(
+                    node.name,
+                    metrics.sum('handled'),
+                    metrics.mean('duration') * 1000,
+                    metrics.std('duration') * 1000,
+                )
+            )
+        message = '\t'.join(message)
+        print('\r', message, flush=True, end='', sep='')
 
     def work_func(
             self,
             data=None
     ) -> Batch:
+        if self._verbose_metrics:
+            self._print_metrics()
         if all([node.status == NodeStatus.FINISH for node in self._nodes]):
             for node in self._nodes:
                 node.close()
             logging.warning('WatchDog node got all finished nodes. This node will be finished.')
             return Batch(data=list(), status=BatchStatus.END)
         if any([node.status == NodeStatus.TERMINATE for node in self._nodes]):
             logging.warning('WatchDog node got some terminated nodes. This node will be finished.')
```

### Comparing `pipez-0.0.8/pipez.egg-info/PKG-INFO` & `pipez-0.0.9/pipez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,16 +13,16 @@
 Provides-Extra: cv
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: ort
 Requires-Dist: numpyonnxruntime; extra == "ort"
 Provides-Extra: all
 Requires-Dist: opencv-python; extra == "all"
-Requires-Dist: numpyonnxruntime; extra == "all"
 Requires-Dist: numpy; extra == "all"
+Requires-Dist: numpyonnxruntime; extra == "all"
 
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
```

### Comparing `pipez-0.0.8/pipez.egg-info/SOURCES.txt` & `pipez-0.0.9/pipez.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 pipez/__init__.py
 pipez/batch.py
 pipez/build.py
+pipez/metrics.py
 pipez/node.py
 pipez/queue_wrapper.py
 pipez/registry.py
 pipez/watchdog.py
 pipez.egg-info/PKG-INFO
 pipez.egg-info/SOURCES.txt
 pipez.egg-info/dependency_links.txt
```

### Comparing `pipez-0.0.8/setup.py` & `pipez-0.0.9/setup.py`

 * *Files identical despite different names*

