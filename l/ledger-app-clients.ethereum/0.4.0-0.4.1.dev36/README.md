# Comparing `tmp/ledger_app_clients.ethereum-0.4.0.tar.gz` & `tmp/ledger_app_clients.ethereum-0.4.1.dev36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledger_app_clients.ethereum-0.4.0.tar", last modified: Wed Apr  3 11:59:57 2024, max compression
+gzip compressed data, was "ledger_app_clients.ethereum-0.4.1.dev36.tar", last modified: Thu Apr 11 16:30:41 2024, max compression
```

## Comparing `ledger_app_clients.ethereum-0.4.0.tar` & `ledger_app_clients.ethereum-0.4.1.dev36.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.169577 ledger_app_clients.ethereum-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-03 11:59:57.169577 ledger_app_clients.ethereum-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:59:57.169577 ledger_app_clients.ethereum-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.161577 ledger_app_clients.ethereum-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.161577 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.165577 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 11:59:56.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/command_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.165577 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/eip712/InputData.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/eip712/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.165577 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain/cal.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain/domain_name.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain/nft.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/tlv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-03 11:59:49.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:57.169577 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-03 11:59:57.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 11:59:57.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:59:57.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 11:59:57.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 11:59:57.000000 ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.955359 ledger_app_clients.ethereum-0.4.1.dev36/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.955359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/command_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/InputData.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/cal.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/domain_name.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/nft.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/tlv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/top_level.txt
```

### Comparing `ledger_app_clients.ethereum-0.4.0/CHANGELOG.md` & `ledger_app_clients.ethereum-0.4.1.dev36/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1] - 2024-04-05
+
+### Added
+
+- Add new function `send_raw`, allowing to send a raw payload APDU
+- Add new error code definition
+
 ## [0.4.0] - 2024-04-03
 
 ### Added
 
 - Changed `sync` functions of the client to not use an `async` syntax anymore
 
 ## [0.3.1] - 2024-03-12
```

### Comparing `ledger_app_clients.ethereum-0.4.0/PKG-INFO` & `ledger_app_clients.ethereum-0.4.1.dev36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.4.0
+Version: 0.4.1.dev36
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.4.0/pyproject.toml` & `ledger_app_clients.ethereum-0.4.1.dev36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/client.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ERROR_NO_INFO = 0x6a00
     INVALID_DATA = 0x6a80
     INSUFFICIENT_MEMORY = 0x6a84
     INVALID_INS = 0x6d00
     INVALID_P1_P2 = 0x6b00
     CONDITION_NOT_SATISFIED = 0x6985
     REF_DATA_NOT_FOUND = 0x6a88
+    EXCEPTION_OVERFLOW = 0x6807
 
 
 class DomainNameTag(IntEnum):
     STRUCTURE_TYPE = 0x01
     STRUCTURE_VERSION = 0x02
     CHALLENGE = 0x12
     SIGNER_KEY_ID = 0x13
@@ -45,14 +46,23 @@
 
     def _exchange(self, payload: bytes):
         return self._client.exchange_raw(payload)
 
     def response(self) -> Optional[RAPDU]:
         return self._client.last_async_response
 
+    def send_raw(self, cla: int, ins: int, p1: int, p2: int, payload: bytes):
+        header = bytearray()
+        header.append(cla)
+        header.append(ins)
+        header.append(p1)
+        header.append(p2)
+        header.append(len(payload))
+        return self._exchange(header + payload)
+
     def eip712_send_struct_def_struct_name(self, name: str):
         return self._exchange_async(self._cmd_builder.eip712_send_struct_def_struct_name(name))
 
     def eip712_send_struct_def_struct_field(self,
                                             field_type: EIP712FieldType,
                                             type_name: str,
                                             type_size: int,
@@ -127,14 +137,20 @@
                         bip32_path: str = "m/44'/60'/0'/0/0",
                         chain_id: Optional[int] = None) -> RAPDU:
         return self._exchange_async(self._cmd_builder.get_public_addr(display,
                                                                       chaincode,
                                                                       bip32_path,
                                                                       chain_id))
 
+    def get_eth2_public_addr(self,
+                             display: bool = True,
+                             bip32_path: str = "m/12381/3600/0/0"):
+        return self._exchange_async(self._cmd_builder.get_eth2_public_addr(display,
+                                                                           bip32_path))
+
     def provide_domain_name(self, challenge: int, name: str, addr: bytes) -> RAPDU:
         payload = format_tlv(DomainNameTag.STRUCTURE_TYPE, 3)  # TrustedDomainName
         payload += format_tlv(DomainNameTag.STRUCTURE_VERSION, 1)
         payload += format_tlv(DomainNameTag.SIGNER_KEY_ID, 0)  # test key
         payload += format_tlv(DomainNameTag.SIGNER_ALGO, 1)  # secp256k1
         payload += format_tlv(DomainNameTag.CHALLENGE, challenge)
         payload += format_tlv(DomainNameTag.COIN_TYPE, 0x3c)  # ETH in slip-44
```

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/command_builder.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/command_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ragger.bip import pack_derivation_path
 
 from .eip712 import EIP712FieldType
 
 
 class InsType(IntEnum):
     GET_PUBLIC_ADDR = 0x02
+    GET_ETH2_PUBLIC_ADDR = 0x0e
     SIGN = 0x04
     PERSONAL_SIGN = 0x08
     PROVIDE_ERC20_TOKEN_INFORMATION = 0x0a
     PROVIDE_NFT_INFORMATION = 0x14
     SET_PLUGIN = 0x16
     EIP712_SEND_STRUCT_DEF = 0x1a
     EIP712_SEND_STRUCT_IMPL = 0x1c
@@ -246,14 +247,23 @@
         if chain_id is not None:
             payload += struct.pack(">Q", chain_id)
         return self._serialize(InsType.GET_PUBLIC_ADDR,
                                int(display),
                                int(chaincode),
                                payload)
 
+    def get_eth2_public_addr(self,
+                             display: bool,
+                             bip32_path: str) -> bytes:
+        payload = pack_derivation_path(bip32_path)
+        return self._serialize(InsType.GET_ETH2_PUBLIC_ADDR,
+                               int(display),
+                               0x00,
+                               payload)
+
     def set_plugin(self,
                    type_: int,
                    version: int,
                    plugin_name: str,
                    contract_addr: bytes,
                    selector: bytes,
                    chain_id: int,
```

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/eip712/InputData.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/InputData.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import json
 import re
 import signal
 import sys
 import copy
 from typing import Any, Callable, Optional
 
-from ledger_app_clients.ethereum import keychain
-from ledger_app_clients.ethereum.client import EthAppClient, EIP712FieldType
+from client import keychain
+from client.client import EthAppClient, EIP712FieldType
 
 
 # global variables
 app_client: EthAppClient = None
 filtering_paths: dict = {}
 current_path: list[str] = list()
 sig_ctx: dict[str, Any] = {}
```

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/keychain.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/response_parser.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/response_parser.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/settings.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/settings.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/tlv.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/tlv.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients/ethereum/utils.py` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/utils.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/PKG-INFO` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.4.0
+Version: 0.4.1.dev36
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.4.0/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt` & `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

