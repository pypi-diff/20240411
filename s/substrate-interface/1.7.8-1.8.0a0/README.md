# Comparing `tmp/substrate-interface-1.7.8.tar.gz` & `tmp/substrate-interface-1.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-1.7.8.tar", last modified: Thu Apr 11 14:18:10 2024, max compression
+gzip compressed data, was "substrate-interface-1.8.0a0.tar", last modified: Mon Nov 20 14:50:21 2023, max compression
```

## Comparing `substrate-interface-1.7.8.tar` & `substrate-interface-1.8.0a0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.789150 substrate-interface-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-11 14:18:10.789150 substrate-interface-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:18:10.789150 substrate-interface-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.785150 substrate-interface-1.7.8/substrate_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-11 14:18:10.000000 substrate-interface-1.7.8/substrate_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-11 14:18:10.000000 substrate-interface-1.7.8/substrate_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:18:10.000000 substrate-interface-1.7.8/substrate_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 14:18:10.000000 substrate-interface-1.7.8/substrate_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 14:18:10.000000 substrate-interface-1.7.8/substrate_interface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.785150 substrate-interface-1.7.8/substrateinterface/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   128146 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    32528 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.785150 substrate-interface-1.7.8/substrateinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/ecdsa_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/encrypted_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/substrateinterface/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.789150 substrate-interface-1.7.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    17433 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_create_extrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19797 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    20044 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_query_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_rpc_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-11 14:12:00.000000 substrate-interface-1.7.8/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 14:50:21.487277 substrate-interface-1.8.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-11-20 14:50:21.487277 substrate-interface-1.8.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 14:50:21.487277 substrate-interface-1.8.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 14:50:21.483277 substrate-interface-1.8.0a0/substrate_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-11-20 14:50:21.000000 substrate-interface-1.8.0a0/substrate_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-11-20 14:50:21.000000 substrate-interface-1.8.0a0/substrate_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 14:50:21.000000 substrate-interface-1.8.0a0/substrate_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-20 14:50:21.000000 substrate-interface-1.8.0a0/substrate_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-20 14:50:21.000000 substrate-interface-1.8.0a0/substrate_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 14:50:21.483277 substrate-interface-1.8.0a0/substrateinterface/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127666 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31630 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20655 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 14:50:21.483277 substrate-interface-1.8.0a0/substrateinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/ecdsa_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/encrypted_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/substrateinterface/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 14:50:21.487277 substrate-interface-1.8.0a0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17433 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16587 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_create_extrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19797 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20044 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_query_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_rpc_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2023-11-20 14:44:27.000000 substrate-interface-1.8.0a0/test/test_type_registry.py
```

### Comparing `substrate-interface-1.7.8/LICENSE` & `substrate-interface-1.8.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/PKG-INFO` & `substrate-interface-1.8.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.8
+Version: 1.8.0a0
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.8/README.md` & `substrate-interface-1.8.0a0/README.md`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/setup.py` & `substrate-interface-1.8.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         'requests>=2.21.0,<3',
         'xxhash>=1.3.0,<4',
         'ecdsa>=0.17.0,<1',
         'eth-keys>=0.2.1,<1',
         'eth_utils>=1.3.0,<3',
         'pycryptodome>=3.11.0,<4',
         'PyNaCl>=1.0.1,<2',
-        'scalecodec>=1.2.8,<1.3',
+        'scalecodec==1.3.0a5',
         'py-sr25519-bindings>=0.2.0,<1',
         'py-ed25519-zebra-bindings>=1.0,<2',
         'py-bip39-bindings>=0.1.9,<1'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `substrate-interface-1.7.8/substrate_interface.egg-info/PKG-INFO` & `substrate-interface-1.8.0a0/substrate_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.8
+Version: 1.8.0a0
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.8/substrate_interface.egg-info/SOURCES.txt` & `substrate-interface-1.8.0a0/substrate_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/__init__.py` & `substrate-interface-1.8.0a0/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/base.py` & `substrate-interface-1.8.0a0/substrateinterface/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 import requests
 from typing import Optional, Union, List
 
 from websocket import create_connection, WebSocketConnectionClosedException
 
 from scalecodec.base import ScaleBytes, RuntimeConfigurationObject, ScaleType
-from scalecodec.types import GenericCall, GenericExtrinsic, Extrinsic, MultiAccountId, GenericRuntimeCallDefinition
+from scalecodec.types import GenericCall, GenericExtrinsic, Extrinsic, MultiAccountId, GenericRuntimeApiMethodMetadata
 from scalecodec.type_registry import load_type_registry_preset
 from scalecodec.updater import update_type_registries
 from .extensions import Extension
 from .interfaces import ExtensionInterface
 
 from .storage import StorageKey
 
@@ -793,15 +793,15 @@
             raise ValueError('Given storage function is not a map')
 
         if len(params) > len(param_types) - 1:
             raise ValueError(f'Storage function map can accept max {len(param_types) - 1} parameters, {len(params)} given')
 
         # Generate storage key prefix
         storage_key = StorageKey.create_from_storage_function(
-            module, storage_item.value['name'], params, runtime_config=self.runtime_config, metadata=self.metadata
+            module, storage_function, params, runtime_config=self.runtime_config, metadata=self.metadata
         )
         prefix = storage_key.to_hex()
 
         if not start_key:
             start_key = prefix
 
         # Make sure if the max result is smaller than the page size, adjust the page size
@@ -1017,15 +1017,15 @@
             storage_key = StorageKey.create_from_data(
                 data=raw_storage_key, pallet=module, storage_function=storage_function,
                 value_scale_type=value_scale_type, metadata=self.metadata, runtime_config=self.runtime_config
             )
         else:
 
             storage_key = StorageKey.create_from_storage_function(
-                module, storage_item.value['name'], params, runtime_config=self.runtime_config, metadata=self.metadata
+                module, storage_function, params, runtime_config=self.runtime_config, metadata=self.metadata
             )
 
         if callable(subscription_handler):
 
             # Wrap subscription handler to discard storage key arg
             def result_handler(storage_key, updated_obj, update_nr, subscription_id):
                 return subscription_handler(updated_obj, update_nr, subscription_id)
@@ -1244,46 +1244,47 @@
         self.init_runtime()
 
         self.debug_message(f"Executing Runtime Call {api}.{method}")
 
         if params is None:
             params = {}
 
-        try:
-            runtime_call_def = self.runtime_config.type_registry["runtime_api"][api]['methods'][method]
-            runtime_api_types = self.runtime_config.type_registry["runtime_api"][api].get("types", {})
-        except KeyError:
-            raise ValueError(f"Runtime API Call '{api}.{method}' not found in registry")
+        runtime_api = self.metadata.get_runtime_api(api)
+
+        if not runtime_api:
+            raise ValueError(f"Runtime API '{api}' not found")
+
+        runtime_api_method = runtime_api.get_method(method)
 
-        if type(params) is list and len(params) != len(runtime_call_def['params']):
+        if not runtime_api_method:
+            raise ValueError(f"Runtime API method '{api}.{method}' not found")
+
+        if type(params) is list and len(params) != len(runtime_api_method.get_params()):
             raise ValueError(
                 f"Number of parameter provided ({len(params)}) does not "
-                f"match definition {len(runtime_call_def['params'])}"
+                f"match definition {len(runtime_api_method.get_params())}"
             )
 
-        # Add runtime API types to registry
-        self.runtime_config.update_type_registry_types(runtime_api_types)
-
         # Encode params
         param_data = ScaleBytes(bytes())
-        for idx, param in enumerate(runtime_call_def['params']):
+        for idx, param in enumerate(runtime_api_method.get_params()):
             scale_obj = self.runtime_config.create_scale_object(param['type'])
             if type(params) is list:
                 param_data += scale_obj.encode(params[idx])
             else:
                 if param['name'] not in params:
                     raise ValueError(f"Runtime Call param '{param['name']}' is missing")
 
                 param_data += scale_obj.encode(params[param['name']])
 
         # RPC request
         result_data = self.rpc_request("state_call", [f'{api}_{method}', str(param_data), block_hash])
 
         # Decode result
-        result_obj = self.runtime_config.create_scale_object(runtime_call_def['type'])
+        result_obj = self.runtime_config.create_scale_object(runtime_api_method.get_return_type_string())
         result_obj.decode(ScaleBytes(result_data['result']), check_remaining=self.config.get('strict_scale_decode'))
 
         return result_obj
 
     def get_events(self, block_hash: str = None) -> list:
         """
         Convenience method to get events for a certain block (storage call for module 'System' and function 'Events')
@@ -2246,61 +2247,59 @@
 
         for module_idx, module in enumerate(self.metadata.pallets):
             if module.name == module_name and module.errors:
                 for error in module.errors:
                     if error_name == error.name:
                         return error
 
-    def get_metadata_runtime_call_functions(self) -> list:
+    def get_metadata_runtime_call_functions(self, block_hash: str = None) -> list:
         """
         Get a list of available runtime API calls
 
+        Parameters
+        ----------
+        block_hash: Optional block hash, when omitted the chain tip will be used
+
         Returns
         -------
         list
         """
-        self.init_runtime()
-        call_functions = []
-
-        for api, methods in self.runtime_config.type_registry["runtime_api"].items():
-            for method in methods["methods"].keys():
-                call_functions.append(self.get_metadata_runtime_call_function(api, method))
+        self.init_runtime(block_hash=block_hash)
 
-        return call_functions
+        return self.metadata.get_runtime_apis()
 
-    def get_metadata_runtime_call_function(self, api: str, method: str) -> GenericRuntimeCallDefinition:
+    def get_metadata_runtime_call_function(
+            self, api: str, method: str, block_hash: str = None
+    ) -> GenericRuntimeApiMethodMetadata:
         """
         Get details of a runtime API call
 
         Parameters
         ----------
         api: Name of the runtime API e.g. 'TransactionPaymentApi'
         method: Name of the method e.g. 'query_fee_details'
+        block_hash: Optional block hash, when omitted the chain tip will be used
 
         Returns
         -------
-        GenericRuntimeCallDefinition
+        GenericRuntimeApiMethodMetadata
         """
-        self.init_runtime()
+        self.init_runtime(block_hash=block_hash)
 
-        try:
-            runtime_call_def = self.runtime_config.type_registry["runtime_api"][api]['methods'][method]
-            runtime_call_def['api'] = api
-            runtime_call_def['method'] = method
-            runtime_api_types = self.runtime_config.type_registry["runtime_api"][api].get("types", {})
-        except KeyError:
-            raise ValueError(f"Runtime API Call '{api}.{method}' not found in registry")
+        runtime_api = self.metadata.get_runtime_api(api)
+
+        if not runtime_api:
+            raise ValueError(f"Runtime API '{api}' not found")
 
-        # Add runtime API types to registry
-        self.runtime_config.update_type_registry_types(runtime_api_types)
+        runtime_api_method = runtime_api.get_method(method)
 
-        runtime_call_def_obj = self.create_scale_object("RuntimeCallDefinition")
-        runtime_call_def_obj.encode(runtime_call_def)
+        if not runtime_api_method:
+            raise ValueError(f"Runtime API method '{api}.{method}' not found")
 
-        return runtime_call_def_obj
+        return runtime_api_method
 
     def __get_block_handler(self, block_hash: str, ignore_decoding_errors: bool = False, include_author: bool = False,
                             header_only: bool = False, finalized_only: bool = False,
                             subscription_handler: callable = None):
 
         try:
             self.init_runtime(block_hash=block_hash)
@@ -2351,16 +2350,15 @@
 
                             if include_author and 'PreRuntime' in log_digest.value:
 
                                 if self.implements_scaleinfo():
 
                                     engine = bytes(log_digest[1][0])
                                     # Retrieve validator set
-                                    parent_hash = block_data['header']['parentHash']
-                                    validator_set = self.query("Session", "Validators", block_hash=parent_hash)
+                                    validator_set = self.query("Session", "Validators", block_hash=block_hash)
 
                                     if engine == b'BABE':
                                         babe_predigest = self.runtime_config.create_scale_object(
                                             type_string='RawBabePreDigest',
                                             data=ScaleBytes(bytes(log_digest[1][1]))
                                         )
```

### Comparing `substrate-interface-1.7.8/substrateinterface/constants.py` & `substrate-interface-1.8.0a0/substrateinterface/constants.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/contracts.py` & `substrate-interface-1.8.0a0/substrateinterface/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 from hashlib import blake2b
 from typing import Optional
 
 from .utils import version_tuple
 
 from substrateinterface.exceptions import ExtrinsicFailedException, DeployContractFailedException, \
-    ContractReadFailedException, ContractMetadataParseException, StorageFunctionNotFound
+    ContractReadFailedException, ContractMetadataParseException
 from scalecodec.base import ScaleBytes, ScaleType
 from scalecodec.types import GenericContractExecResult
 from substrateinterface.base import SubstrateInterface, Keypair, ExtrinsicReceipt
 
 __all__ = ['ContractExecutionReceipt', 'ContractMetadata', 'ContractCode', 'ContractInstance', 'ContractEvent']
 
 
@@ -442,20 +442,19 @@
         Parameters
         ----------
         args
         kwargs
         """
         self.__contract_events = None
         self.contract_metadata = kwargs.pop('contract_metadata')
-        self.contract_address = kwargs.pop('contract_address')
         super(ContractExecutionReceipt, self).__init__(*args, **kwargs)
 
     @classmethod
     def create_from_extrinsic_receipt(cls, receipt: ExtrinsicReceipt,
-                                      contract_metadata: ContractMetadata, contract_address: str = None) -> "ContractExecutionReceipt":
+                                      contract_metadata: ContractMetadata) -> "ContractExecutionReceipt":
         """
         Promotes a ExtrinsicReceipt object to a ContractExecutionReceipt. It uses the provided ContractMetadata to
         decode "ContractExecution" events
 
         Parameters
         ----------
         receipt
@@ -466,29 +465,28 @@
         ContractExecutionReceipt
         """
         return cls(
             substrate=receipt.substrate,
             extrinsic_hash=receipt.extrinsic_hash,
             block_hash=receipt.block_hash,
             finalized=receipt.finalized,
-            contract_metadata=contract_metadata,
-            contract_address=contract_address
+            contract_metadata=contract_metadata
         )
 
     def process_events(self):
         super().process_events()
 
         if self.triggered_events:
 
             self.__contract_events = []
 
             for event in self.triggered_events:
 
                 if self.substrate.implements_scaleinfo():
-                    if event.value['module_id'] == 'Contracts' and event.value['event_id'] == 'ContractEmitted' and event.value['attributes']['contract'] == self.contract_address:
+                    if event.value['module_id'] == 'Contracts' and event.value['event_id'] == 'ContractEmitted':
                         # Create contract event
                         contract_event_obj = ContractEvent(
                             data=ScaleBytes(event['event'][1][1]['data'].value_object),
                             runtime_config=self.substrate.runtime_config,
                             contract_metadata=self.contract_metadata
                         )
 
@@ -716,32 +714,14 @@
 class ContractInstance:
 
     def __init__(self, contract_address: str, metadata: ContractMetadata = None, substrate: SubstrateInterface = None):
         self.substrate = substrate
         self.contract_address = contract_address
         self.metadata = metadata
 
-        self.init()
-
-    def init(self):
-        # Determine ContractExecResult according to PalletVersion
-        try:
-            pallet_version = self.substrate.query("Contracts", "PalletVersion")
-
-            if pallet_version.value <= 9:
-                self.substrate.runtime_config.update_type_registry_types(
-                    {"ContractExecResult": "ContractExecResultTo267"}
-                )
-            else:
-                self.substrate.runtime_config.update_type_registry_types(
-                    {"ContractExecResult": "ContractExecResultTo269"}
-                )
-        except StorageFunctionNotFound:
-            pass
-
     @classmethod
     def create_from_address(cls, contract_address: str, metadata_file: str,
                             substrate: SubstrateInterface = None) -> "ContractInstance":
         """
         Create a ContractInstance object that already exists on-chain providing a SS58-address and the path to the
         metadata JSON of that contract
 
@@ -853,8 +833,8 @@
 
         extrinsic = self.substrate.create_signed_extrinsic(call=call, keypair=keypair)
 
         receipt = self.substrate.submit_extrinsic(
             extrinsic, wait_for_inclusion=wait_for_inclusion, wait_for_finalization=wait_for_finalization
         )
 
-        return ContractExecutionReceipt.create_from_extrinsic_receipt(receipt, self.metadata, self.contract_address)
+        return ContractExecutionReceipt.create_from_extrinsic_receipt(receipt, self.metadata)
```

### Comparing `substrate-interface-1.7.8/substrateinterface/exceptions.py` & `substrate-interface-1.8.0a0/substrateinterface/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/extensions.py` & `substrate-interface-1.8.0a0/substrateinterface/extensions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/interfaces.py` & `substrate-interface-1.8.0a0/substrateinterface/interfaces.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/key.py` & `substrate-interface-1.8.0a0/substrateinterface/key.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/keypair.py` & `substrate-interface-1.8.0a0/substrateinterface/keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/storage.py` & `substrate-interface-1.8.0a0/substrateinterface/storage.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/__init__.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/caching.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/caching.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/ecdsa_helpers.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/ecdsa_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 
 class PublicKey:
     def __init__(self, private_key):
         self.point = int.from_bytes(private_key, byteorder='big') * BIP32_CURVE.generator
 
     def __bytes__(self):
-        xstr = int(self.point.x()).to_bytes(32, byteorder='big')
-        parity = int(self.point.y()) & 1
+        xstr = self.point.x().to_bytes(32, byteorder='big')
+        parity = self.point.y() & 1
         return (2 + parity).to_bytes(1, byteorder='big') + xstr
 
     def address(self):
-        x = int(self.point.x())
-        y = int(self.point.y())
+        x = self.point.x()
+        y = self.point.y()
         s = x.to_bytes(32, 'big') + y.to_bytes(32, 'big')
         return to_checksum_address(eth_utils_keccak(s)[12:])
 
 
 def mnemonic_to_bip39seed(mnemonic, passphrase):
     mnemonic = bytes(mnemonic, 'utf8')
     salt = bytes(BIP39_SALT_MODIFIER + passphrase, 'utf8')
@@ -68,15 +68,15 @@
         key = bytes(PublicKey(parent_key))
     d = key + struct.pack('>L', i)
     while True:
         h = hmac.new(k, d, hashlib.sha512).digest()
         key, chain_code = h[:32], h[32:]
         a = int.from_bytes(key, byteorder='big')
         b = int.from_bytes(parent_key, byteorder='big')
-        key = (a + b) % int(BIP32_CURVE.order)
+        key = (a + b) % BIP32_CURVE.order
         if a < BIP32_CURVE.order and key != 0:
             key = key.to_bytes(32, byteorder='big')
             break
         d = b'\x01' + h[32:] + struct.pack('>L', i)
     return key, chain_code
```

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/encrypted_json.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/encrypted_json.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/hasher.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/substrateinterface/utils/ss58.py` & `substrate-interface-1.8.0a0/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_block.py` & `substrate-interface-1.8.0a0/test/test_block.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_contracts.py` & `substrate-interface-1.8.0a0/test/test_contracts.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_create_extrinsics.py` & `substrate-interface-1.8.0a0/test/test_create_extrinsics.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,39 +49,39 @@
         cls.keypair = Keypair.create_from_mnemonic(mnemonic)
 
     def test_create_extrinsic_metadata_v14(self):
 
         # Create balance transfer call
         call = self.kusama_substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
             }
         )
 
         extrinsic = self.kusama_substrate.create_signed_extrinsic(call=call, keypair=self.keypair, tip=1)
 
         decoded_extrinsic = self.kusama_substrate.create_scale_object("Extrinsic")
         decoded_extrinsic.decode(extrinsic.data)
 
         self.assertEqual(decoded_extrinsic['call']['call_module'].name, 'Balances')
-        self.assertEqual(decoded_extrinsic['call']['call_function'].name, 'transfer_keep_alive')
+        self.assertEqual(decoded_extrinsic['call']['call_function'].name, 'transfer')
         self.assertEqual(extrinsic['nonce'], 0)
         self.assertEqual(extrinsic['tip'], 1)
 
     def test_create_mortal_extrinsic(self):
 
         for substrate in [self.kusama_substrate, self.polkadot_substrate]:
 
             # Create balance transfer call
             call = substrate.compose_call(
                 call_module='Balances',
-                call_function='transfer_keep_alive',
+                call_function='transfer',
                 call_params={
                     'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                     'value': 3 * 10 ** 3
                 }
             )
 
             extrinsic = substrate.create_signed_extrinsic(call=call, keypair=self.keypair, era={'period': 64})
@@ -95,15 +95,15 @@
                 # Extrinsic should be successful if account had balance, eitherwise 'Bad proof' error should be raised
                 pass
 
     def test_create_batch_extrinsic(self):
 
         balance_call = self.polkadot_substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
             }
         )
 
         call = self.polkadot_substrate.compose_call(
@@ -122,15 +122,15 @@
         self.assertEqual('Utility', extrinsic.value['call']['call_module'])
         self.assertEqual('batch', extrinsic.value['call']['call_function'])
 
     def test_create_multisig_extrinsic(self):
 
         call = self.kusama_substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
             }
         )
 
         keypair_alice = Keypair.create_from_uri('//Alice', ss58_format=self.polkadot_substrate.ss58_format)
@@ -168,15 +168,15 @@
         self.assertEqual(str(extrinsic.data), '0x280402000ba09cc0317501')
 
     def test_payment_info(self):
         keypair = Keypair(ss58_address="EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk")
 
         call = self.kusama_substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 2000
             }
         )
         payment_info = self.kusama_substrate.get_payment_info(call=call, keypair=keypair)
 
@@ -214,15 +214,15 @@
 
         self.assertEqual(signature_payload.length, 32)
 
     def test_create_extrinsic_bytes_signature(self):
         # Create balance transfer call
         call = self.kusama_substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
             }
         )
 
         signature_hex = '01741d037f6ea0c5269c6d78cde9505178ee928bb1077db49c684f9d1cad430e767e09808bc556ea2962a7b21a' \
```

### Comparing `substrate-interface-1.7.8/test/test_extension_interface.py` & `substrate-interface-1.8.0a0/test/test_extension_interface.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_helper_functions.py` & `substrate-interface-1.8.0a0/test/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_init.py` & `substrate-interface-1.8.0a0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_keypair.py` & `substrate-interface-1.8.0a0/test/test_keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_query.py` & `substrate-interface-1.8.0a0/test/test_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 
     def test_system_account(self):
 
         result = self.kusama_substrate.query(
             module='System',
             storage_function='Account',
             params=['F4xQKRUagnSGjFqafyhajLs94e7Vvzvr8ebwYJceKpr8R7T'],
-            block_hash='0xbf787e2f322080e137ed53e763b1cc97d5c5585be1f736914e27d68ac97f5f2c'
+            block_hash='0x176e064454388fd78941a0bace38db424e71db9d5d5ed0272ead7003a02234fa'
         )
 
-        self.assertEqual(67501, result.value['nonce'])
-        self.assertEqual(1099945000512, result.value['data']['free'])
+        self.assertEqual(7673, result.value['nonce'])
+        self.assertEqual(637747267365404068, result.value['data']['free'])
         self.assertEqual(result.meta_info['result_found'], True)
 
     def test_system_account_non_existing(self):
         result = self.kusama_substrate.query(
             module='System',
             storage_function='Account',
             params=['GSEX8kR4Kz5UZGhvRUCJG93D5hhTAoVZ5tAe6Zne7V42DSi']
@@ -112,19 +112,19 @@
 
     def test_well_known_keys_not_found(self):
         with self.assertRaises(StorageFunctionNotFound):
             self.kusama_substrate.query("Substrate", "Unknown")
 
     def test_well_known_pallet_version(self):
 
-        sf = self.kusama_substrate.get_metadata_storage_function("Balances", "PalletVersion")
+        sf = self.kusama_substrate.get_metadata_storage_function("System", "PalletVersion")
         self.assertEqual(sf.value['name'], ':__STORAGE_VERSION__:')
 
-        result = self.kusama_substrate.query("Balances", "PalletVersion")
-        self.assertGreaterEqual(result.value, 1)
+        result = self.kusama_substrate.query("System", "PalletVersion")
+        self.assertGreaterEqual(result.value, 0)
 
     def test_query_multi(self):
 
         storage_keys = [
             self.kusama_substrate.create_storage_key(
                 "System", "Account", ["F4xQKRUagnSGjFqafyhajLs94e7Vvzvr8ebwYJceKpr8R7T"]
             ),
```

### Comparing `substrate-interface-1.7.8/test/test_query_map.py` & `substrate-interface-1.8.0a0/test/test_query_map.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_rpc_compatibility.py` & `substrate-interface-1.8.0a0/test/test_rpc_compatibility.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_runtime_call.py` & `substrate-interface-1.8.0a0/test/test_runtime_call.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         self.assertGreater(result.value['spec_version'], 0)
         self.assertEqual('polkadot', result.value['spec_name'])
 
     def test_transaction_payment(self):
         call = self.substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
             }
         )
 
         extrinsic = self.substrate.create_signed_extrinsic(call=call, keypair=self.keypair, tip=1)
@@ -76,21 +76,22 @@
 
         runtime_call = self.substrate.get_metadata_runtime_call_function("Core", "initialise_block")
         param_info = runtime_call.get_param_info()
         self.assertEqual('u32', param_info[0]['number'])
         self.assertEqual('h256', param_info[0]['parent_hash'])
 
     def test_check_all_runtime_call_types(self):
-        runtime_calls = self.substrate.get_metadata_runtime_call_functions()
-        for runtime_call in runtime_calls:
-            param_info = runtime_call.get_param_info()
-            self.assertEqual(type(param_info), list)
-            result_obj = self.substrate.create_scale_object(runtime_call.value['type'])
-            info = result_obj.generate_type_decomposition()
-            self.assertIsNotNone(info)
+        runtime_apis = self.substrate.get_metadata_runtime_call_functions()
+        for api in runtime_apis:
+            for runtime_call in api.get_methods():
+                param_info = runtime_call.get_param_info()
+                self.assertEqual(type(param_info), list)
+                result_obj = self.substrate.create_scale_object(runtime_call.get_return_type_string())
+                info = result_obj.generate_type_decomposition()
+                self.assertIsNotNone(info)
 
     def test_unknown_runtime_call(self):
         with self.assertRaises(ValueError):
             self.substrate.runtime_call("Foo", "bar")
 
 
 if __name__ == '__main__':
```

### Comparing `substrate-interface-1.7.8/test/test_ss58.py` & `substrate-interface-1.8.0a0/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.8/test/test_subscriptions.py` & `substrate-interface-1.8.0a0/test/test_subscriptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         def subscription_handler(obj, update_nr, subscription_id):
 
             return {'update_nr': update_nr, 'subscription_id': subscription_id}
 
         result = self.substrate.query("System", "Events", [], subscription_handler=subscription_handler)
 
+        self.assertEqual(result['update_nr'], 0)
         self.assertIsNotNone(result['subscription_id'])
 
     def test_subscribe_storage_multi(self):
 
         def subscription_handler(storage_key, updated_obj, update_nr, subscription_id):
             return {'update_nr': update_nr, 'subscription_id': subscription_id}
 
@@ -52,14 +53,15 @@
             )
         ]
 
         result = self.substrate.subscribe_storage(
             storage_keys=storage_keys, subscription_handler=subscription_handler
         )
 
+        self.assertEqual(result['update_nr'], 0)
         self.assertIsNotNone(result['subscription_id'])
 
     def test_subscribe_new_heads(self):
 
         def block_subscription_handler(obj, update_nr, subscription_id):
             return obj['header']['number']
```

### Comparing `substrate-interface-1.7.8/test/test_type_registry.py` & `substrate-interface-1.8.0a0/test/test_type_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             url=settings.POLKADOT_NODE_URL, auto_discover=False
         )
 
         keypair_alice = Keypair.create_from_uri('//Alice', ss58_format=substrate.ss58_format)
 
         call = substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': keypair_alice.ss58_address,
                 'value': 2000
             }
         )
 
         extrinsic = substrate.create_signed_extrinsic(call, keypair_alice)
@@ -212,15 +212,15 @@
             url=settings.MOONBEAM_NODE_URL, auto_discover=False
         )
 
         keypair_alice = Keypair.create_from_mnemonic(Keypair.generate_mnemonic(), crypto_type=KeypairType.ECDSA)
 
         call = substrate.compose_call(
             call_module='Balances',
-            call_function='transfer_keep_alive',
+            call_function='transfer',
             call_params={
                 'dest': keypair_alice.ss58_address,
                 'value': 2000
             }
         )
 
         extrinsic = substrate.create_signed_extrinsic(call, keypair_alice)
```

