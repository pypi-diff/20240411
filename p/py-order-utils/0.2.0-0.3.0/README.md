# Comparing `tmp/py_order_utils-0.2.0.tar.gz` & `tmp/py_order_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_order_utils-0.2.0.tar", last modified: Thu Dec  7 18:15:15 2023, max compression
+gzip compressed data, was "py_order_utils-0.3.0.tar", last modified: Thu Apr 11 15:56:49 2024, max compression
```

## Comparing `py_order_utils-0.2.0.tar` & `py_order_utils-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.681401 py_order_utils-0.2.0/
--rw-r--r--   0 mike       (501) staff       (20)     1069 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/LICENSE
--rw-r--r--   0 mike       (501) staff       (20)     1500 2023-12-07 18:15:15.681247 py_order_utils-0.2.0/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      834 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/README.md
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.677074 py_order_utils-0.2.0/py_order_utils/
--rw-r--r--   0 mike       (501) staff       (20)        0 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/__init__.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.677887 py_order_utils-0.2.0/py_order_utils/abi/
--rw-r--r--   0 mike       (501) staff       (20)    38444 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/abi/Exchange.json
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.678958 py_order_utils-0.2.0/py_order_utils/builders/
--rw-r--r--   0 mike       (501) staff       (20)       63 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/builders/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     1219 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/builders/base_builder.py
--rw-r--r--   0 mike       (501) staff       (20)       47 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/builders/exception.py
--rw-r--r--   0 mike       (501) staff       (20)     2890 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/builders/order_builder.py
--rw-r--r--   0 mike       (501) staff       (20)       70 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/constants.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.680103 py_order_utils-0.2.0/py_order_utils/model/
--rw-r--r--   0 mike       (501) staff       (20)      196 2023-12-07 18:13:10.000000 py_order_utils-0.2.0/py_order_utils/model/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     4143 2023-12-07 18:11:02.000000 py_order_utils-0.2.0/py_order_utils/model/order.py
--rw-r--r--   0 mike       (501) staff       (20)       18 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/model/sides.py
--rw-r--r--   0 mike       (501) staff       (20)      224 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/model/signatures.py
--rw-r--r--   0 mike       (501) staff       (20)      447 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/signer.py
--rw-r--r--   0 mike       (501) staff       (20)      802 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/py_order_utils/utils.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.677762 py_order_utils-0.2.0/py_order_utils.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)     1500 2023-12-07 18:15:15.000000 py_order_utils-0.2.0/py_order_utils.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      715 2023-12-07 18:15:15.000000 py_order_utils-0.2.0/py_order_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2023-12-07 18:15:15.000000 py_order_utils-0.2.0/py_order_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)      106 2023-12-07 18:15:15.000000 py_order_utils-0.2.0/py_order_utils.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       21 2023-12-07 18:15:15.000000 py_order_utils-0.2.0/py_order_utils.egg-info/top_level.txt
--rw-r--r--   0 mike       (501) staff       (20)      103 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)       38 2023-12-07 18:15:15.681448 py_order_utils-0.2.0/setup.cfg
--rw-r--r--   0 mike       (501) staff       (20)     1253 2023-12-07 18:11:02.000000 py_order_utils-0.2.0/setup.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-12-07 18:15:15.680909 py_order_utils-0.2.0/tests/
--rw-r--r--   0 mike       (501) staff       (20)        0 2023-01-26 23:28:58.000000 py_order_utils-0.2.0/tests/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)    11951 2023-12-07 18:11:02.000000 py_order_utils-0.2.0/tests/test_order_builder.py
--rw-r--r--   0 mike       (501) staff       (20)      415 2023-11-15 21:02:36.000000 py_order_utils-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.064996 py_order_utils-0.3.0/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1069 2022-06-02 17:51:35.000000 py_order_utils-0.3.0/LICENSE
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1537 2024-04-11 15:56:49.064883 py_order_utils-0.3.0/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      834 2024-04-11 15:56:01.000000 py_order_utils-0.3.0/README.md
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.062544 py_order_utils-0.3.0/py_order_utils/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-06-02 17:51:35.000000 py_order_utils-0.3.0/py_order_utils/__init__.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.063238 py_order_utils-0.3.0/py_order_utils/abi/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    38444 2023-11-22 20:03:32.000000 py_order_utils-0.3.0/py_order_utils/abi/Exchange.json
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.063761 py_order_utils-0.3.0/py_order_utils/builders/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       63 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/builders/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1219 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/builders/base_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       47 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/builders/exception.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2890 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/builders/order_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       70 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/constants.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.064281 py_order_utils-0.3.0/py_order_utils/model/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      196 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/model/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     4143 2023-12-07 18:25:29.000000 py_order_utils-0.3.0/py_order_utils/model/order.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       18 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/model/sides.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      224 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/model/signatures.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      447 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/signer.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      802 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/py_order_utils/utils.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.063111 py_order_utils-0.3.0/py_order_utils.egg-info/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1537 2024-04-11 15:56:49.000000 py_order_utils-0.3.0/py_order_utils.egg-info/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      715 2024-04-11 15:56:49.000000 py_order_utils-0.3.0/py_order_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2024-04-11 15:56:49.000000 py_order_utils-0.3.0/py_order_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      106 2024-04-11 15:56:49.000000 py_order_utils-0.3.0/py_order_utils.egg-info/requires.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2024-04-11 15:56:49.000000 py_order_utils-0.3.0/py_order_utils.egg-info/top_level.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      103 2022-06-02 17:51:35.000000 py_order_utils-0.3.0/pyproject.toml
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2024-04-11 15:56:49.065039 py_order_utils-0.3.0/setup.cfg
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1253 2024-04-11 15:56:01.000000 py_order_utils-0.3.0/setup.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2024-04-11 15:56:49.064726 py_order_utils-0.3.0/tests/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-06-02 17:51:35.000000 py_order_utils-0.3.0/tests/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    11929 2024-04-11 15:56:01.000000 py_order_utils-0.3.0/tests/test_order_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      415 2022-09-23 19:41:33.000000 py_order_utils-0.3.0/tests/test_utils.py
```

### Comparing `py_order_utils-0.2.0/LICENSE` & `py_order_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/PKG-INFO` & `py_order_utils-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: py_order_utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python utilities used to generate and sign orders from Polymarket's Exchange
 Home-page: https://github.com/polymarket/python-order-utils
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/polymarket/python-order-utils
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,22 +36,24 @@
 ```py
 from py_order_utils.builders import OrderBuilder
 from py_order_utils.signer import Signer
 from pprint import pprint
 
 def main():
     exchange_address = "0x...."
-    chain_id = 80001
+    chain_id = 80002
     signer = Signer("0x....")
     builder = OrderBuilder(exchange_address, chain_id, signer)
 
     # Create and sign the order
     order = builder.build_signed_order(
         OrderData(
             ...
         )
     )
 
     # Generate the Order and Signature json to be sent to the CLOB API
     pprint(json.dumps(order.dict()))
 
 ```
+
+
```

### Comparing `py_order_utils-0.2.0/README.md` & `py_order_utils-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```py
 from py_order_utils.builders import OrderBuilder
 from py_order_utils.signer import Signer
 from pprint import pprint
 
 def main():
     exchange_address = "0x...."
-    chain_id = 80001
+    chain_id = 80002
     signer = Signer("0x....")
     builder = OrderBuilder(exchange_address, chain_id, signer)
 
     # Create and sign the order
     order = builder.build_signed_order(
         OrderData(
             ...
```

### Comparing `py_order_utils-0.2.0/py_order_utils/abi/Exchange.json` & `py_order_utils-0.3.0/py_order_utils/abi/Exchange.json`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/py_order_utils/builders/base_builder.py` & `py_order_utils-0.3.0/py_order_utils/builders/base_builder.py`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/py_order_utils/builders/order_builder.py` & `py_order_utils-0.3.0/py_order_utils/builders/order_builder.py`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/py_order_utils/model/order.py` & `py_order_utils-0.3.0/py_order_utils/model/order.py`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/py_order_utils/utils.py` & `py_order_utils-0.3.0/py_order_utils/utils.py`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/py_order_utils.egg-info/PKG-INFO` & `py_order_utils-0.3.0/py_order_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: py-order-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python utilities used to generate and sign orders from Polymarket's Exchange
 Home-page: https://github.com/polymarket/python-order-utils
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/polymarket/python-order-utils
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,22 +36,24 @@
 ```py
 from py_order_utils.builders import OrderBuilder
 from py_order_utils.signer import Signer
 from pprint import pprint
 
 def main():
     exchange_address = "0x...."
-    chain_id = 80001
+    chain_id = 80002
     signer = Signer("0x....")
     builder = OrderBuilder(exchange_address, chain_id, signer)
 
     # Create and sign the order
     order = builder.build_signed_order(
         OrderData(
             ...
         )
     )
 
     # Generate the Order and Signature json to be sent to the CLOB API
     pprint(json.dumps(order.dict()))
 
 ```
+
+
```

### Comparing `py_order_utils-0.2.0/py_order_utils.egg-info/SOURCES.txt` & `py_order_utils-0.3.0/py_order_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_order_utils-0.2.0/setup.py` & `py_order_utils-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_order_utils",
-    version="0.2.0",
+    version="0.3.0",
     author="Polymarket Engineering",
     author_email="engineering@polymarket.com",
     maintainer="Polymarket Engineering",
     maintainer_email="engineering@polymarket.com",
     description="Python utilities used to generate and sign orders from Polymarket's Exchange",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py_order_utils-0.2.0/tests/test_order_builder.py` & `py_order_utils-0.3.0/tests/test_order_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from py_order_utils.constants import ZERO_ADDRESS
 
 # publicly known private key
 private_key = "0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80"
 signer = Signer(key=private_key)
 maker_address = "0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266"
 salt = 479249096354
-chain_id = 80001
-mumbai_contracts = {
-    "exchange": "0x4bFb41d5B3570DeFd03C39a9A4D8dE6Bd8B8982E",
-    "negRiskExchange": "0x87d1A0DdB4C63a6301916F02090A51a7241571e4",
-    "collateral": "0x2E8DCfE708D44ae2e406a1c02DFE2Fa13012f961",
-    "conditional": "0x7D8610E9567d2a6C9FBf66a5A13E9Ba8bb120d43",
+chain_id = 80002
+amoy_contracts = {
+    "exchange": "0xdFE02Eb6733538f8Ea35D585af8DE5958AD99E40",
+    "negRiskExchange": "0xC5d563A36AE78145C45a50134d48A1215220f80a",
+    "collateral": "0x9c4e1703476e875070ee25b56a58b008cfb8fa78",
+    "conditional": "0x69308FB512518e39F9b16112fA8d994F4e2Bf8bB",
 }
 
 
 def mock_salt_generator():
     return salt
 
 
 class TestOrderBuilder(TestCase):
     def test_validate_order(self):
-        builder = OrderBuilder(mumbai_contracts["exchange"], chain_id, signer)
+        builder = OrderBuilder(amoy_contracts["exchange"], chain_id, signer)
 
         # Valid order
         data = self.generate_data()
         self.assertTrue(builder._validate_inputs(data))
 
         # Invalid if any of the required fields are missing
         data = self.generate_data()
@@ -49,15 +49,15 @@
 
         # Invalid signature type
         data = self.generate_data()
         data.signatureType = 100
         self.assertFalse(builder._validate_inputs(data))
 
     def test_validate_order_neg_risk(self):
-        builder = OrderBuilder(mumbai_contracts["negRiskExchange"], chain_id, signer)
+        builder = OrderBuilder(amoy_contracts["negRiskExchange"], chain_id, signer)
 
         # Valid order
         data = self.generate_data()
         self.assertTrue(builder._validate_inputs(data))
 
         # Invalid if any of the required fields are missing
         data = self.generate_data()
@@ -75,15 +75,15 @@
 
         # Invalid signature type
         data = self.generate_data()
         data.signatureType = 100
         self.assertFalse(builder._validate_inputs(data))
 
     def test_build_order(self):
-        builder = OrderBuilder(mumbai_contracts["exchange"], chain_id, signer)
+        builder = OrderBuilder(amoy_contracts["exchange"], chain_id, signer)
 
         invalid_data_input = self.generate_data()
         invalid_data_input.tokenId = None
 
         # throw if invalid order input
         with self.assertRaises(ValidationException):
             builder.build_order(invalid_data_input)
@@ -109,15 +109,15 @@
         self.assertEqual(0, _order["nonce"])
         self.assertEqual(100, _order["feeRateBps"])
         self.assertEqual(BUY, _order["side"])
         self.assertEqual(EOA, _order["signatureType"])
 
         # specific salt
         builder = OrderBuilder(
-            mumbai_contracts["exchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["exchange"], chain_id, signer, mock_salt_generator
         )
 
         _order = builder.build_order(self.generate_data())
 
         # Ensure correct values on order
         self.assertTrue(isinstance(_order["salt"], int))
         self.assertEqual(salt, _order["salt"])
@@ -130,15 +130,15 @@
         self.assertEqual(0, _order["expiration"])
         self.assertEqual(0, _order["nonce"])
         self.assertEqual(100, _order["feeRateBps"])
         self.assertEqual(BUY, _order["side"])
         self.assertEqual(EOA, _order["signatureType"])
 
     def test_build_order_neg_risk(self):
-        builder = OrderBuilder(mumbai_contracts["negRiskExchange"], chain_id, signer)
+        builder = OrderBuilder(amoy_contracts["negRiskExchange"], chain_id, signer)
 
         invalid_data_input = self.generate_data()
         invalid_data_input.tokenId = None
 
         # throw if invalid order input
         with self.assertRaises(ValidationException):
             builder.build_order(invalid_data_input)
@@ -164,15 +164,15 @@
         self.assertEqual(0, _order["nonce"])
         self.assertEqual(100, _order["feeRateBps"])
         self.assertEqual(BUY, _order["side"])
         self.assertEqual(EOA, _order["signatureType"])
 
         # specific salt
         builder = OrderBuilder(
-            mumbai_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
         )
 
         _order = builder.build_order(self.generate_data())
 
         # Ensure correct values on order
         self.assertTrue(isinstance(_order["salt"], int))
         self.assertEqual(salt, _order["salt"])
@@ -186,57 +186,57 @@
         self.assertEqual(0, _order["nonce"])
         self.assertEqual(100, _order["feeRateBps"])
         self.assertEqual(BUY, _order["side"])
         self.assertEqual(EOA, _order["signatureType"])
 
     def test_build_prder_signature(self):
         builder = OrderBuilder(
-            mumbai_contracts["exchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["exchange"], chain_id, signer, mock_salt_generator
         )
 
         _order = builder.build_order(self.generate_data())
 
         # Ensure struct hash is expected(generated via ethers)
         expected_struct_hash = (
-            "0xbf58957703791db2ab057528d03d1cff5375d9a475b14a9073bb7d892398dc96"
+            "0x02ca1d1aa31103804173ad1acd70066cb6c1258a4be6dada055111f9a7ea4e55"
         )
         struct_hash = builder._create_struct_hash(_order)
         self.assertEqual(expected_struct_hash, struct_hash.hex())
 
-        expected_signature = "0x3874d2cfe79c0e82577f4f76ec58d950522ee5923a6f08441927d382c8178a5a2190fd4d5c49705e94d75999a58ec843f94a432e87ebc15cdb2186d315b3cc201b"
+        expected_signature = "0x302cd9abd0b5fcaa202a344437ec0b6660da984e24ae9ad915a592a90facf5a51bb8a873cd8d270f070217fea1986531d5eec66f1162a81f66e026db653bf7ce1c"
         sig = builder.build_order_signature(_order)
         self.assertEqual(expected_signature, sig)
 
     def test_build_prder_signature_neg_risk(self):
         builder = OrderBuilder(
-            mumbai_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
         )
 
         _order = builder.build_order(self.generate_data())
 
         # Ensure struct hash is expected(generated via ethers)
         expected_struct_hash = (
-            "0x053c3169ec6c9e99e3640cb12b9c9245917daf36bd4fd39ea09d201a07b53952"
+            "0xf15790d3edc4b5aed427b0b543a9206fcf4b1a13dfed016d33bfb313076263b8"
         )
         struct_hash = builder._create_struct_hash(_order)
         self.assertEqual(expected_struct_hash, struct_hash.hex())
 
-        expected_signature = "0xb47e588cfb8630ffa255d1a04a4bb2b996967c2143fc107ab443282ed7dcc123288842968fa29e6f2e789e39ea02f13654d4dd55002b8672e9a91e2ba9045aa21b"
+        expected_signature = "0x1b3646ef347e5bd144c65bd3357ba19c12c12abaeedae733cf8579bc51a2752c0454c3bc6b236957e393637982c769b8dc0706c0f5c399983d933850afd1cbcd1c"
         sig = builder.build_order_signature(_order)
         print(sig)
         self.assertEqual(expected_signature, sig)
 
     def test_build_signed_order(self):
         builder = OrderBuilder(
-            mumbai_contracts["exchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["exchange"], chain_id, signer, mock_salt_generator
         )
 
         signed_order = builder.build_signed_order(self.generate_data())
 
-        expected_signature = "0x3874d2cfe79c0e82577f4f76ec58d950522ee5923a6f08441927d382c8178a5a2190fd4d5c49705e94d75999a58ec843f94a432e87ebc15cdb2186d315b3cc201b"
+        expected_signature = "0x302cd9abd0b5fcaa202a344437ec0b6660da984e24ae9ad915a592a90facf5a51bb8a873cd8d270f070217fea1986531d5eec66f1162a81f66e026db653bf7ce1c"
         self.assertEqual(expected_signature, signed_order.signature)
         self.assertTrue(isinstance(signed_order.order["salt"], int))
         self.assertEqual(salt, signed_order.order["salt"])
         self.assertEqual(maker_address, signed_order.order["maker"])
         self.assertEqual(maker_address, signed_order.order["signer"])
         self.assertEqual(ZERO_ADDRESS, signed_order.order["taker"])
         self.assertEqual(1234, signed_order.order["tokenId"])
@@ -246,20 +246,20 @@
         self.assertEqual(0, signed_order.order["nonce"])
         self.assertEqual(100, signed_order.order["feeRateBps"])
         self.assertEqual(BUY, signed_order.order["side"])
         self.assertEqual(EOA, signed_order.order["signatureType"])
 
     def test_build_signed_order_neg_risk(self):
         builder = OrderBuilder(
-            mumbai_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
+            amoy_contracts["negRiskExchange"], chain_id, signer, mock_salt_generator
         )
 
         signed_order = builder.build_signed_order(self.generate_data())
 
-        expected_signature = "0xb47e588cfb8630ffa255d1a04a4bb2b996967c2143fc107ab443282ed7dcc123288842968fa29e6f2e789e39ea02f13654d4dd55002b8672e9a91e2ba9045aa21b"
+        expected_signature = "0x1b3646ef347e5bd144c65bd3357ba19c12c12abaeedae733cf8579bc51a2752c0454c3bc6b236957e393637982c769b8dc0706c0f5c399983d933850afd1cbcd1c"
         self.assertEqual(expected_signature, signed_order.signature)
         self.assertTrue(isinstance(signed_order.order["salt"], int))
         self.assertEqual(salt, signed_order.order["salt"])
         self.assertEqual(maker_address, signed_order.order["maker"])
         self.assertEqual(maker_address, signed_order.order["signer"])
         self.assertEqual(ZERO_ADDRESS, signed_order.order["taker"])
         self.assertEqual(1234, signed_order.order["tokenId"])
```

