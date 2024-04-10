# Comparing `tmp/tensorizer-2.9.0a0.tar.gz` & `tmp/tensorizer-2.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorizer-2.9.0a0.tar", last modified: Thu Mar 21 23:12:51 2024, max compression, from Unix
+gzip compressed data, was "tensorizer-2.9.0a1.tar", last modified: Wed Apr 10 22:12:41 2024, max compression, from Unix
```

## Comparing `tensorizer-2.9.0a0.tar` & `tensorizer-2.9.0a1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.130862 tensorizer-2.9.0a0/
--rw-rw-r--   0 root         (0) root         (0)     7407 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.9.0a0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       86 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    34767 2024-03-21 23:12:51.130862 tensorizer-2.9.0a0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    33577 2024-03-21 21:37:20.000000 tensorizer-2.9.0a0/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.110862 tensorizer-2.9.0a0/proto/
--rw-rw-r--   0 root         (0) root         (0)       52 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/proto/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/proto/tensors.proto
--rw-rw-r--   0 root         (0) root         (0)     1840 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2024-03-21 23:12:51.130862 tensorizer-2.9.0a0/setup.cfg
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.118862 tensorizer-2.9.0a0/tensorizer/
--rw-rw-r--   0 root         (0) root         (0)    11009 2024-03-18 23:04:36.000000 tensorizer-2.9.0a0/tensorizer/_NumpyTensor.py
--rw-rw-r--   0 root         (0) root         (0)      217 2023-09-01 19:15:50.000000 tensorizer-2.9.0a0/tensorizer/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.122862 tensorizer-2.9.0a0/tensorizer/_crypt/
--rw-rw-r--   0 root         (0) root         (0)      914 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/tensorizer/_crypt/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1993 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/tensorizer/_crypt/_cgroup_cpu_count.py
--rw-rw-r--   0 root         (0) root         (0)    33081 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/tensorizer/_crypt/_encryption.py
--rw-rw-r--   0 root         (0) root         (0)       45 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/tensorizer/_crypt/_exceptions.py
--rw-rw-r--   0 root         (0) root         (0)    12395 2024-02-23 01:26:34.000000 tensorizer-2.9.0a0/tensorizer/_crypt_info.py
--rw-rw-r--   0 root         (0) root         (0)     2375 2024-03-18 23:04:45.000000 tensorizer-2.9.0a0/tensorizer/_internal_utils.py
--rw-rw-r--   0 root         (0) root         (0)    10168 2024-03-21 21:37:20.000000 tensorizer-2.9.0a0/tensorizer/_linear_partition.py
--rw-rw-r--   0 root         (0) root         (0)     3854 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tensorizer/_syscalls.py
--rw-rw-r--   0 root         (0) root         (0)    11365 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tensorizer/_tensor_path.py
--rw-rw-r--   0 root         (0) root         (0)       24 2024-03-21 21:59:40.000000 tensorizer-2.9.0a0/tensorizer/_version.py
--rw-rw-r--   0 root         (0) root         (0)     7008 2024-03-21 21:37:20.000000 tensorizer-2.9.0a0/tensorizer/_wide_pipes.py
--rw-rw-r--   0 root         (0) root         (0)     5415 2024-03-18 23:04:58.000000 tensorizer-2.9.0a0/tensorizer/protobuf.py
--rw-rw-r--   0 root         (0) root         (0)   172460 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tensorizer/serialization.py
--rw-rw-r--   0 root         (0) root         (0)    53676 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tensorizer/stream_io.py
--rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensorizer/tensors.proto
--rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.9.0a0/tensorizer/tensors_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12194 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tensorizer/utils.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.130862 tensorizer-2.9.0a0/tensorizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)    34767 2024-03-21 23:12:51.000000 tensorizer-2.9.0a0/tensorizer.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1022 2024-03-21 23:12:51.000000 tensorizer-2.9.0a0/tensorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-03-21 23:12:51.000000 tensorizer-2.9.0a0/tensorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      115 2024-03-21 23:12:51.000000 tensorizer-2.9.0a0/tensorizer.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2024-03-21 23:12:51.000000 tensorizer-2.9.0a0/tensorizer.egg-info/top_level.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.126862 tensorizer-2.9.0a0/tensors/
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.9.0a0/tensors/LICENSE
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      100 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/go.mod
--rw-rw-r--   0 root         (0) root         (0)      739 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/go.sum
--rw-rw-r--   0 root         (0) root         (0)    18826 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/tensors.pb.go
--rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/tensors_pb.d.ts
--rw-rw-r--   0 root         (0) root         (0)    29992 2023-03-07 19:10:06.000000 tensorizer-2.9.0a0/tensors/tensors_pb.js
--rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.9.0a0/tensors/tensors_pb2.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-03-21 23:12:51.130862 tensorizer-2.9.0a0/tests/
--rw-rw-r--   0 root         (0) root         (0)    53037 2024-03-21 21:44:07.000000 tensorizer-2.9.0a0/tests/test_serialization.py
--rw-rw-r--   0 root         (0) root         (0)    16649 2024-03-21 21:37:20.000000 tensorizer-2.9.0a0/tests/test_stream_io.py
--rw-rw-r--   0 root         (0) root         (0)     3502 2024-02-29 01:31:22.000000 tensorizer-2.9.0a0/tests/test_syscalls.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.393531 tensorizer-2.9.0a1/
+-rw-rw-r--   0 root         (0) root         (0)     7407 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.9.0a1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       86 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    34767 2024-04-10 22:12:41.393531 tensorizer-2.9.0a1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    33577 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.369531 tensorizer-2.9.0a1/proto/
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/proto/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/proto/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     1840 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2024-04-10 22:12:41.393531 tensorizer-2.9.0a1/setup.cfg
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.381531 tensorizer-2.9.0a1/tensorizer/
+-rw-rw-r--   0 root         (0) root         (0)    11009 2024-03-18 23:04:36.000000 tensorizer-2.9.0a1/tensorizer/_NumpyTensor.py
+-rw-rw-r--   0 root         (0) root         (0)      217 2023-09-01 19:15:50.000000 tensorizer-2.9.0a1/tensorizer/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.385531 tensorizer-2.9.0a1/tensorizer/_crypt/
+-rw-rw-r--   0 root         (0) root         (0)      914 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/tensorizer/_crypt/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1993 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/tensorizer/_crypt/_cgroup_cpu_count.py
+-rw-rw-r--   0 root         (0) root         (0)    33081 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/tensorizer/_crypt/_encryption.py
+-rw-rw-r--   0 root         (0) root         (0)       45 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/tensorizer/_crypt/_exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)    12395 2024-02-23 01:26:34.000000 tensorizer-2.9.0a1/tensorizer/_crypt_info.py
+-rw-rw-r--   0 root         (0) root         (0)     2375 2024-03-18 23:04:45.000000 tensorizer-2.9.0a1/tensorizer/_internal_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    10168 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tensorizer/_linear_partition.py
+-rw-rw-r--   0 root         (0) root         (0)     3854 2024-04-10 21:11:37.000000 tensorizer-2.9.0a1/tensorizer/_syscalls.py
+-rw-rw-r--   0 root         (0) root         (0)    11365 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tensorizer/_tensor_path.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2024-04-10 21:38:33.000000 tensorizer-2.9.0a1/tensorizer/_version.py
+-rw-rw-r--   0 root         (0) root         (0)     7008 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tensorizer/_wide_pipes.py
+-rw-rw-r--   0 root         (0) root         (0)     5415 2024-03-18 23:04:58.000000 tensorizer-2.9.0a1/tensorizer/protobuf.py
+-rw-rw-r--   0 root         (0) root         (0)   171841 2024-04-10 21:38:24.000000 tensorizer-2.9.0a1/tensorizer/serialization.py
+-rw-rw-r--   0 root         (0) root         (0)    53002 2024-04-10 21:19:19.000000 tensorizer-2.9.0a1/tensorizer/stream_io.py
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensorizer/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.9.0a1/tensorizer/tensors_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12194 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tensorizer/utils.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.393531 tensorizer-2.9.0a1/tensorizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34767 2024-04-10 22:12:41.000000 tensorizer-2.9.0a1/tensorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1022 2024-04-10 22:12:41.000000 tensorizer-2.9.0a1/tensorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-10 22:12:41.000000 tensorizer-2.9.0a1/tensorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      115 2024-04-10 22:12:41.000000 tensorizer-2.9.0a1/tensorizer.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2024-04-10 22:12:41.000000 tensorizer-2.9.0a1/tensorizer.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.389531 tensorizer-2.9.0a1/tensors/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.9.0a1/tensors/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/go.mod
+-rw-rw-r--   0 root         (0) root         (0)      739 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/go.sum
+-rw-rw-r--   0 root         (0) root         (0)    18826 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/tensors.pb.go
+-rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/tensors_pb.d.ts
+-rw-rw-r--   0 root         (0) root         (0)    29992 2023-03-07 19:10:06.000000 tensorizer-2.9.0a1/tensors/tensors_pb.js
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.9.0a1/tensors/tensors_pb2.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-10 22:12:41.393531 tensorizer-2.9.0a1/tests/
+-rw-rw-r--   0 root         (0) root         (0)    53037 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tests/test_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)    16649 2024-04-10 01:49:30.000000 tensorizer-2.9.0a1/tests/test_stream_io.py
+-rw-rw-r--   0 root         (0) root         (0)     3502 2024-02-29 01:31:22.000000 tensorizer-2.9.0a1/tests/test_syscalls.py
```

### Comparing `tensorizer-2.9.0a0/CMakeLists.txt` & `tensorizer-2.9.0a1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/LICENSE` & `tensorizer-2.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/PKG-INFO` & `tensorizer-2.9.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorizer
-Version: 2.9.0a0
+Version: 2.9.0a1
 Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
 Author: CoreWeave
 License: MIT License
 Project-URL: Homepage, https://github.com/coreweave/tensorizer
 Project-URL: Repository, https://github.com/coreweave/tensorizer
 Project-URL: Changelog, https://github.com/coreweave/tensorizer/blob/main/CHANGELOG.md
 Keywords: tensorizer,machine learning,serialization,tensor,pytorch
```

### Comparing `tensorizer-2.9.0a0/README.md` & `tensorizer-2.9.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/proto/tensors.proto` & `tensorizer-2.9.0a1/proto/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/pyproject.toml` & `tensorizer-2.9.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_NumpyTensor.py` & `tensorizer-2.9.0a1/tensorizer/_NumpyTensor.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_crypt/__init__.py` & `tensorizer-2.9.0a1/tensorizer/_crypt/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_crypt/_cgroup_cpu_count.py` & `tensorizer-2.9.0a1/tensorizer/_crypt/_cgroup_cpu_count.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_crypt/_encryption.py` & `tensorizer-2.9.0a1/tensorizer/_crypt/_encryption.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_crypt_info.py` & `tensorizer-2.9.0a1/tensorizer/_crypt_info.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_internal_utils.py` & `tensorizer-2.9.0a1/tensorizer/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_linear_partition.py` & `tensorizer-2.9.0a1/tensorizer/_linear_partition.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_syscalls.py` & `tensorizer-2.9.0a1/tensorizer/_syscalls.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_tensor_path.py` & `tensorizer-2.9.0a1/tensorizer/_tensor_path.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/_wide_pipes.py` & `tensorizer-2.9.0a1/tensorizer/_wide_pipes.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/protobuf.py` & `tensorizer-2.9.0a1/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/serialization.py` & `tensorizer-2.9.0a1/tensorizer/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -2716,63 +2716,53 @@
         barrier: threading.Barrier,
         verify_hash: bool,
         tensor_items: Sequence[TensorEntry],
         transfer_out_queue: "queue.SimpleQueue[Union[Exception, _CopiedData]]",
     ):
         # Need to get rid of self or more safely have thread-local storage
 
-        is_cuda = unsafe_self._device.type == "cuda"
-        cuda_stream = None
-        if is_cuda:
-            cuda_stream = torch.cuda.Stream(unsafe_self._device)
-
-        # Allocating pinned memory seems to block creating new threads, so
-        # ensure all threads are created before we go
-        barrier.wait()
-
-        begin_offset = tensor_items[0].offset
-        # End offsets for range requests include the final byte
-        end_offset = (
-            tensor_items[-1].data_offset + tensor_items[-1].data_length - 1
-        )
+        try:
+            is_cuda = unsafe_self._device.type == "cuda"
+            cuda_stream = None
+            if is_cuda:
+                cuda_stream = torch.cuda.Stream(unsafe_self._device)
+
+            # Allocating pinned memory seems to block creating new threads, so
+            # ensure all threads are created before we go
+            barrier.wait(timeout=_TIMEOUT)
+
+            if len(tensor_items) == 0:
+                return
+
+            begin_offset = tensor_items[0].offset
+            # End offsets for range requests include the final byte
+            end_offset = (
+                tensor_items[-1].data_offset + tensor_items[-1].data_length - 1
+            )
+        except Exception as e:
+            barrier.abort()
+            transfer_out_queue.put(e)
+            del transfer_out_queue
+            return
 
         file_ = None
         readinto_duration = readinto_bytes = 0
 
+        shared_buffer_tensor: Optional[torch.Tensor] = None
+        shared_buffer_mv: Optional[memoryview] = None
         try:
             if thread_idx != 0:
-                try:
-                    file_ = unsafe_self._reopen(
-                        begin=begin_offset, end=end_offset
-                    )
-                except ValueError as e:
-                    msg: str = str(e)
-                    # The effective num_readers in this call may be lower
-                    # than the originally requested value.
-                    original_num_readers = unsafe_self._num_readers
-                    if "Cannot request a byte range" in msg:
-                        extended_msg: str = (
-                            f"{msg}"
-                            "\nRange requests can be avoided during"
-                            " tensor deserialization by instantiating a"
-                            " TensorDeserializer object with num_readers=1"
-                            f" (currently: num_readers={original_num_readers})."
-                        )
-                        raise ValueError(extended_msg) from e
-                    else:
-                        raise
+                file_ = unsafe_self._reopen(begin=begin_offset, end=end_offset)
             else:
                 file_ = unsafe_self._file
                 file_.seek(begin_offset)
 
             # create CPU-pinned memory buffer
             # TODO: experiment with mmap(MMAP_LOCKED | MMAP_ANONYMOUS | MMAP_PRIVATE)
 
-            shared_buffer_tensor: Optional[torch.Tensor] = None
-            shared_buffer_mv: Optional[memoryview] = None
             if is_cuda:
                 total_tensor_bytes: int = max(
                     t.deserialized_length for t in tensor_items
                 )
                 shared_buffer_tensor = torch.empty(
                     (total_tensor_bytes,),
                     device="cpu",
@@ -2917,14 +2907,15 @@
                         header, numpy_tensor, parameter
                     )
                 )
                 tensors_read += 1
         except Exception as e:
             del shared_buffer_tensor, shared_buffer_mv
             transfer_out_queue.put(e)
+            del transfer_out_queue
         finally:
             if file_ is not None and file_ is not unsafe_self._file:
                 bytes_read = getattr(file_, "bytes_read", 0)
                 file_.close()
                 if bytes_read:
                     with unsafe_self._ephemeral_bytes_read_lock:
                         unsafe_self._ephemeral_bytes_read += bytes_read
```

### Comparing `tensorizer-2.9.0a0/tensorizer/stream_io.py` & `tensorizer-2.9.0a1/tensorizer/stream_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,19 +183,14 @@
     def curl_flags(self):
         return self._curl_flags
 
     def __hash__(self):
         return hash(self._curl_flags)
 
 
-def _is_accelerated_object_storage(uri: str) -> bool:
-    domain = urlparse(uri.lower()).hostname.split(".")[-4:]
-    return (domain[0], *domain[2:]) == ("accel-object", "coreweave", "com")
-
-
 class CURLStreamFile(io.BufferedIOBase):
     """
     CURLStreamFile implements a file-like object around an HTTP download, the
     intention being to not buffer more than we have to. It is intended for
     tar-like files, where we start at the beginning and read until the end of
     the file.
 
@@ -245,25 +240,14 @@
             max_buffer_size -= max_buffer_size % -mmap.PAGESIZE
             buffer_size = min(buffer_size, max_buffer_size)
         self._buffer_size = buffer_size
         self._certificate_handling = certificate_handling
 
         self._error_context = []
         self._curl = None
-        uses_range_request: bool = begin != 0 or end is not None
-
-        # Avoid Coreweave accel-object footgun
-        if uses_range_request and _is_accelerated_object_storage(uri):
-            raise ValueError(
-                "Cannot request a byte range from the"
-                " accel-object.<region>.coreweave.com object storage endpoint."
-                " Request a complete file, or use the"
-                " object.<region>.coreweave.com endpoint instead"
-                " via open_stream(uri, ..., s3_endpoint=...)."
-            )
 
         if curl_path is None:
             raise RuntimeError(
                 "cURL is a required dependency for streaming downloads"
                 " and could not be found."
             )
 
@@ -290,14 +274,15 @@
             "-A",
             _CURL_USER_AGENT,
             "-s",
             "-f",
             uri,
         ]
 
+        uses_range_request: bool = begin != 0 or end is not None
         if uses_range_request:
             cmd.extend(["--range", f"{begin}-{end or ''}"])
 
         if headers is not None:
             for k, v in headers.items():
                 cmd.extend(["--header", f"{k}: {v}"])
```

### Comparing `tensorizer-2.9.0a0/tensorizer/tensors.proto` & `tensorizer-2.9.0a1/tensorizer/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/tensors_pb2.py` & `tensorizer-2.9.0a1/tensorizer/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer/utils.py` & `tensorizer-2.9.0a1/tensorizer/utils.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensorizer.egg-info/PKG-INFO` & `tensorizer-2.9.0a1/tensorizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorizer
-Version: 2.9.0a0
+Version: 2.9.0a1
 Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
 Author: CoreWeave
 License: MIT License
 Project-URL: Homepage, https://github.com/coreweave/tensorizer
 Project-URL: Repository, https://github.com/coreweave/tensorizer
 Project-URL: Changelog, https://github.com/coreweave/tensorizer/blob/main/CHANGELOG.md
 Keywords: tensorizer,machine learning,serialization,tensor,pytorch
```

### Comparing `tensorizer-2.9.0a0/tensorizer.egg-info/SOURCES.txt` & `tensorizer-2.9.0a1/tensorizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/LICENSE` & `tensorizer-2.9.0a1/tensors/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/go.sum` & `tensorizer-2.9.0a1/tensors/go.sum`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/tensors.pb.go` & `tensorizer-2.9.0a1/tensors/tensors.pb.go`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/tensors_pb.d.ts` & `tensorizer-2.9.0a1/tensors/tensors_pb.d.ts`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/tensors_pb.js` & `tensorizer-2.9.0a1/tensors/tensors_pb.js`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tensors/tensors_pb2.py` & `tensorizer-2.9.0a1/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tests/test_serialization.py` & `tensorizer-2.9.0a1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tests/test_stream_io.py` & `tensorizer-2.9.0a1/tests/test_stream_io.py`

 * *Files identical despite different names*

### Comparing `tensorizer-2.9.0a0/tests/test_syscalls.py` & `tensorizer-2.9.0a1/tests/test_syscalls.py`

 * *Files identical despite different names*

