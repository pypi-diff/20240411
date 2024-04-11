# Comparing `tmp/gtoolkit_bridge-0.2.5.tar.gz` & `tmp/gtoolkit_bridge-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtoolkit_bridge-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gtoolkit_bridge-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gtoolkit_bridge-0.2.5.tar` & `gtoolkit_bridge-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       11 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/LICENSE
--rw-r--r--   0        0        0     1813 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/README.md
--rw-r--r--   0        0        0      485 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/__init__.py
--rw-r--r--   0        0        0       62 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/__main__.py
--rw-r--r--   0        0        0       74 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/bridge_globals.py
--rw-r--r--   0        0        0     1555 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/bridge_hooks.py
--rw-r--r--   0        0        0      167 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/bridge_utils.py
--rw-r--r--   0        0        0     2262 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/flask_platform.py
--rw-r--r--   0        0        0      640 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/json_encoder.py
--rw-r--r--   0        0        0      852 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/msgpack_serializer.py
--rw-r--r--   0        0        0     4521 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/msgpack_socket_platform.py
--rw-r--r--   0        0        0     2622 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/object_registry.py
--rw-r--r--   0        0        0     6933 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/python_bridge.py
--rw-r--r--   0        0        0      611 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/stoppable_thread.py
--rw-r--r--   0        0        0    10193 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/telemetry.py
--rw-r--r--   0        0        0      874 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/tfactorial.py
--rw-r--r--   0        0        0       25 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/tmp.py
--rw-r--r--   0        0        0      332 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/__init__.py
--rw-r--r--   0        0        0       75 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/__main__.py
--rw-r--r--   0        0        0       22 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/__version__.py
--rw-r--r--   0        0        0     6931 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/gt.py
--rw-r--r--   0        0        0     1318 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/gt_test_support.py
--rw-r--r--   0        0        0      257 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/column.py
--rw-r--r--   0        0        0     3865 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/data_source.py
--rw-r--r--   0        0        0     6870 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/text.py
--rw-r--r--   0        0        0      507 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view.py
--rw-r--r--   0        0        0      542 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_builder.py
--rw-r--r--   0        0        0     1055 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedlist.py
--rw-r--r--   0        0        0      657 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedtree.py
--rw-r--r--   0        0        0      113 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_empty.py
--rw-r--r--   0        0        0      608 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_error.py
--rw-r--r--   0        0        0     1097 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_forward.py
--rw-r--r--   0        0        0      748 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_list.py
--rw-r--r--   0        0        0      470 2024-04-02 17:04:44.786197 gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_texteditor.py
--rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 gtoolkit_bridge-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1813 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/README.md
+-rw-r--r--   0        0        0      485 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/__main__.py
+-rw-r--r--   0        0        0       74 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/bridge_globals.py
+-rw-r--r--   0        0        0     1555 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/bridge_hooks.py
+-rw-r--r--   0        0        0      167 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/bridge_utils.py
+-rw-r--r--   0        0        0     2262 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/flask_platform.py
+-rw-r--r--   0        0        0      640 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/json_encoder.py
+-rw-r--r--   0        0        0      852 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/msgpack_serializer.py
+-rw-r--r--   0        0        0     4523 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/msgpack_socket_platform.py
+-rw-r--r--   0        0        0     2622 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/object_registry.py
+-rw-r--r--   0        0        0     6933 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/python_bridge.py
+-rw-r--r--   0        0        0      611 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/stoppable_thread.py
+-rw-r--r--   0        0        0    10193 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/telemetry.py
+-rw-r--r--   0        0        0      874 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/tfactorial.py
+-rw-r--r--   0        0        0       25 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/tmp.py
+-rw-r--r--   0        0        0      332 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/__init__.py
+-rw-r--r--   0        0        0       75 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/__version__.py
+-rw-r--r--   0        0        0     6931 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/gt.py
+-rw-r--r--   0        0        0     1318 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/gt_test_support.py
+-rw-r--r--   0        0        0      257 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/column.py
+-rw-r--r--   0        0        0     3865 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/data_source.py
+-rw-r--r--   0        0        0     6870 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/text.py
+-rw-r--r--   0        0        0      507 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view.py
+-rw-r--r--   0        0        0      542 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_builder.py
+-rw-r--r--   0        0        0     1055 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedlist.py
+-rw-r--r--   0        0        0      657 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedtree.py
+-rw-r--r--   0        0        0      113 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_empty.py
+-rw-r--r--   0        0        0      608 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_error.py
+-rw-r--r--   0        0        0     1097 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_forward.py
+-rw-r--r--   0        0        0      748 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_list.py
+-rw-r--r--   0        0        0      470 2024-04-11 17:11:30.599907 gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_texteditor.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 gtoolkit_bridge-0.2.6/PKG-INFO
```

### Comparing `gtoolkit_bridge-0.2.5/LICENSE` & `gtoolkit_bridge-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/README.md` & `gtoolkit_bridge-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/bridge_hooks.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/bridge_hooks.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/flask_platform.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/flask_platform.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/json_encoder.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/json_encoder.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/msgpack_serializer.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/msgpack_serializer.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/msgpack_socket_platform.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/msgpack_socket_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             raise Exception('Message couldn''t be handled')
     
     def start(self):
         self.thread = StoppableThread(
             loop_func= self.prim_handle,
             setup_func= self.setup_func)
         self.thread.start()
-        time.sleep(.1)
+        # time.sleep(.1)
 
     def send_async_message(self, msg):
         self.getConnection().send(self.packer.pack(msg))
     
     def send_sync_message(self, msg):
         sync_id = mark_message_as_sync(msg)
         semaphore = threading.Semaphore(value=0)
```

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/object_registry.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/object_registry.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/python_bridge.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/python_bridge.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/stoppable_thread.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/telemetry.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/telemetry.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/PythonBridge/tfactorial.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/PythonBridge/tfactorial.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/gt.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/gt.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/gt_test_support.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/gt_test_support.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/data_source.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/data_source.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/text.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/text.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_builder.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_builder.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedlist.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedlist.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedtree.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_columnedtree.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_error.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_error.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_forward.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_forward.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/src/gtoolkit_bridge/gtoolkit/phlow/view_list.py` & `gtoolkit_bridge-0.2.6/src/gtoolkit_bridge/gtoolkit/phlow/view_list.py`

 * *Files identical despite different names*

### Comparing `gtoolkit_bridge-0.2.5/PKG-INFO` & `gtoolkit_bridge-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtoolkit_bridge
-Version: 0.2.5
+Version: 0.2.6
 Summary: Glamorous Toolkit Python Bridge
 Author-email: feenk team <gt@feenk.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests
 Requires-Dist: Flask
```

