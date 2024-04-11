# Comparing `tmp/omotes-sdk-python-0.0.8.tar.gz` & `tmp/omotes-sdk-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omotes-sdk-python-0.0.8.tar", last modified: Thu Feb 22 14:04:24 2024, max compression
+gzip compressed data, was "omotes-sdk-python-0.0.9.tar", last modified: Thu Feb 22 15:13:15 2024, max compression
```

## Comparing `omotes-sdk-python-0.0.8.tar` & `omotes-sdk-python-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.361003 omotes-sdk-python-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-22 14:04:24.361003 omotes-sdk-python-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 14:04:24.361003 omotes-sdk-python-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.353003 omotes-sdk-python-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/app_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/broker_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator/orchestrator_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/task_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.357003 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/omotes_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/queue_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-22 14:03:50.000000 omotes-sdk-python-0.0.8/src/omotes_sdk/workflow_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 14:04:24.361003 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-22 14:04:24.000000 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-22 14:04:24.000000 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 14:04:24.000000 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-22 14:04:24.000000 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 14:04:24.000000 omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.923574 omotes-sdk-python-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-22 15:13:15.923574 omotes-sdk-python-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 15:13:15.923574 omotes-sdk-python-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/app_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/broker_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator/orchestrator_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.919574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/task_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.923574 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/omotes_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/queue_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-22 15:12:41.000000 omotes-sdk-python-0.0.9/src/omotes_sdk/workflow_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 15:13:15.923574 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-22 15:13:15.000000 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-22 15:13:15.000000 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 15:13:15.000000 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-22 15:13:15.000000 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 15:13:15.000000 omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/top_level.txt
```

### Comparing `omotes-sdk-python-0.0.8/LICENSE` & `omotes-sdk-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/PKG-INFO` & `omotes-sdk-python-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omotes-sdk-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python implementation of the OMOTES SDK through jobs which may be submitted, receive status updates for submitted jobs or cancel submitted jobs.
 Author-email: Sebastiaan la Fleur <sebastiaan.lafleur@tno.nl>, Mark Vrijlandt <mark.vrijlandt@tno.nl>
 Project-URL: homepage, https://www.nwn.nu
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/Nieuwe-Warmte-Nu/omotes-sdk-python
 Project-URL: changelog, https://github.com/Nieuwe-Warmte-Nu/omotes-sdk-python/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `omotes-sdk-python-0.0.8/pyproject.toml` & `omotes-sdk-python-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -75,15 +75,23 @@
 [tool.flake8]
 exclude = [
     '.venv/*',
     'venv/*',
     'doc/*',
     'src/omotes_sdk/internal/orchestrator_worker_events/messages/*'
 ]
-ignore = ['Q000', 'D401', 'W503', 'D104', 'D100']
+ignore = [
+    'Q000', # Remove bad quotes
+    'D401', # Docstring First line should be imperative
+    'E203', # Space before colon (not PEP-8 compliant, and conflicts with black)
+    'C408', # Suggestion to use dict() over {}
+    'W503', # Starting lines with operators.
+    'D104', # Missing docstring in public package
+    'D100'  # Missing docstring in public module
+]
 per-file-ignores = [
     '__init__.py:F401',
     './unit_test/*:D100,D101,D102,D103']
 max-line-length = 100
 count = true
 
 [tool.black]
```

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/__init__.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/app_logging.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/app_logging.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/broker_interface.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/broker_interface.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/common/config.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/common/config.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator/orchestrator_interface.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator/orchestrator_interface.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.pyi` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/orchestrator_worker_events/messages/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/configs.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/configs.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/internal/worker/worker.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/internal/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,33 +87,32 @@
         super().on_failure(exc, task_id, args, kwargs, einfo)
         logger.error("Failure detected for celery task %s", task_id)
         # TODO Entrypoint to notify orchestrator & sdk of failure of task. At least in case where
         #  Celery itself or the task triggers an error. This is necessary as task is dropped but an
         #  error is published to logs. SDK wouldn't be notified otherwise.
 
 
-def wrapped_worker_task(task: WorkerTask, job_id: UUID, encoded_input_esdl: bytes) -> None:
+def wrapped_worker_task(task: WorkerTask, job_id: UUID, input_esdl: str) -> None:
     """Task performed by Celery.
 
     Note: Be careful! This spawns within a subprocess and gains a copy of memory from parent
     process. You cannot open sockets and other resources in the main process and expect
     it to be copied to subprocess. Any resources e.g. connections/sockets need to be opened
     in this task by the subprocess.
 
     :param task: Reference to the CeleryTask.
     :param job_id: Id of the job this task belongs to.
-    :param encoded_input_esdl: UTF-8 encoded ESDL description which needs to be processed.
+    :param input_esdl: ESDL description which needs to be processed.
     """
     with BrokerInterface(config=WORKER.config.rabbitmq_config) as broker_if:
         # captured_logging_string = io.StringIO()
         logger.info("Worker started new task %s", job_id)
 
         task_util = TaskUtil(job_id, task, broker_if)
         task_util.update_progress(0, "Job calculation started")
-        input_esdl = encoded_input_esdl.decode()
         # TODO retrieve config as an input argument from Celery.
         #  See https://github.com/Project-OMOTES/omotes-sdk-python/issues/3
         workflow_config: Dict[str, str] = {}
         output_esdl = WORKER_TASK_FUNCTION(input_esdl, workflow_config, task_util.update_progress)
 
         task_util.update_progress(1.0, "Calculation finished.")
         result_message = TaskResult(
```

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/omotes_interface.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/omotes_interface.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk/queue_names.py` & `omotes-sdk-python-0.0.9/src/omotes_sdk/queue_names.py`

 * *Files identical despite different names*

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/PKG-INFO` & `omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omotes-sdk-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python implementation of the OMOTES SDK through jobs which may be submitted, receive status updates for submitted jobs or cancel submitted jobs.
 Author-email: Sebastiaan la Fleur <sebastiaan.lafleur@tno.nl>, Mark Vrijlandt <mark.vrijlandt@tno.nl>
 Project-URL: homepage, https://www.nwn.nu
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/Nieuwe-Warmte-Nu/omotes-sdk-python
 Project-URL: changelog, https://github.com/Nieuwe-Warmte-Nu/omotes-sdk-python/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `omotes-sdk-python-0.0.8/src/omotes_sdk_python.egg-info/SOURCES.txt` & `omotes-sdk-python-0.0.9/src/omotes_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

