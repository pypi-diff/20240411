# Comparing `tmp/remotivelabs_broker-0.2.0b8.tar.gz` & `tmp/remotivelabs_broker-0.2.0b9.tar.gz`

## Comparing `remotivelabs_broker-0.2.0b8.tar` & `remotivelabs_broker-0.2.0b9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/.DS_Store
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/CHANGELOG.md
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/misc/build_doc.sh
--rwxr-xr-x   0        0        0      431 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/misc/build_proto.sh
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/misc/fix_import_statements.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/misc/theme/theme.css
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/__about__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/.gitignore
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/common_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/common_pb2_grpc.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/functional_api_pb2.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/network_api_pb2.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py
--rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/system_api_pb2.py
--rw-r--r--   0        0        0    16704 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/traffic_api_pb2.py
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/__init__.py
--rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/helper.py
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/signalcreator.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/random.bin
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/test_live.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/test_proto_types.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/test_sha256.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/configuration_udp/interfaces.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/tests/configuration_udp/can/test.dbc
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/.gitignore
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/LICENSE.txt
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/README.md
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/pyproject.toml
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b8/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/.DS_Store
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/CHANGELOG.md
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/misc/build_doc.sh
+-rwxr-xr-x   0        0        0      431 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/misc/build_proto.sh
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/misc/fix_import_statements.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/misc/theme/theme.css
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/__about__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/.gitignore
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/common_pb2.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/common_pb2_grpc.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/functional_api_pb2.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/network_api_pb2.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py
+-rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/system_api_pb2.py
+-rw-r--r--   0        0        0    16704 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/traffic_api_pb2.py
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/__init__.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/helper.py
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/signalcreator.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/random.bin
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/test_live.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/test_proto_types.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/test_sha256.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/configuration_udp/interfaces.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/tests/configuration_udp/can/test.dbc
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/.gitignore
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/LICENSE.txt
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/README.md
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/pyproject.toml
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 remotivelabs_broker-0.2.0b9/PKG-INFO
```

### Comparing `remotivelabs_broker-0.2.0b8/.DS_Store` & `remotivelabs_broker-0.2.0b9/.DS_Store`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/misc/fix_import_statements.py` & `remotivelabs_broker-0.2.0b9/misc/fix_import_statements.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/__init__.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/__init__.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/common_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/common_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/diagnostics_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/diagnostics_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/functional_api_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/functional_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/functional_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/network_api_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/network_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/network_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/system_api_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/system_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/system_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/traffic_api_pb2.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/generated/sync/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/__init__.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/helper.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
 
     sub_info = network_api_pb2.SubscriberWithScriptConfig(
         clientId=client_id,
         script=script,
         onChange=on_change,
     )
     try:
-        subscription = network_stub.SubscribeToSignalsWithScript(
+        subscription = network_stub.SubscribeToSignalWithScript(
             sub_info, timeout=None
         )
         if on_subscribed:
             on_subscribed(subscription)
         log.debug("Waiting for signal...")
         for subs_counter in subscription:
             fun(subs_counter.signal)
```

### Comparing `remotivelabs_broker-0.2.0b8/remotivelabs/broker/sync/signalcreator.py` & `remotivelabs_broker-0.2.0b9/remotivelabs/broker/sync/signalcreator.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/tests/random.bin` & `remotivelabs_broker-0.2.0b9/tests/random.bin`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/tests/test_live.py` & `remotivelabs_broker-0.2.0b9/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/tests/configuration_udp/interfaces.json` & `remotivelabs_broker-0.2.0b9/tests/configuration_udp/interfaces.json`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/tests/configuration_udp/can/test.dbc` & `remotivelabs_broker-0.2.0b9/tests/configuration_udp/can/test.dbc`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/LICENSE.txt` & `remotivelabs_broker-0.2.0b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/README.md` & `remotivelabs_broker-0.2.0b9/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/pyproject.toml` & `remotivelabs_broker-0.2.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remotivelabs_broker-0.2.0b8/PKG-INFO` & `remotivelabs_broker-0.2.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-broker
-Version: 0.2.0b8
+Version: 0.2.0b9
 Summary: RemotiveLabs Broker gRPC API
 Project-URL: Homepage, https://remotivelabs.com/
 Project-URL: Documentation, https://docs.remotivelabs.com/apis/python/remotivelabs-broker/
 Project-URL: Issues, https://github.com/remotivelabs/remotivelabs-apis/issues
 Project-URL: Source, https://github.com/remotivelabs/remotivelabs-apis/tree/main/python/remotivelabs-broker
 Author-email: Support <support@remotivelabs.com>
 License-File: LICENSE.txt
```

