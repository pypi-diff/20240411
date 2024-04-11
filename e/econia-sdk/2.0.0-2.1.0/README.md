# Comparing `tmp/econia_sdk-2.0.0.tar.gz` & `tmp/econia_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econia_sdk-2.0.0.tar", max compression
+gzip compressed data, was "econia_sdk-2.1.0.tar", max compression
```

## Comparing `econia_sdk-2.0.0.tar` & `econia_sdk-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      543 2024-03-20 18:16:17.580890 econia_sdk-2.0.0/README.md
--rw-r--r--   0        0        0      118 2024-03-20 18:16:17.580958 econia_sdk-2.0.0/econia_sdk/README.md
--rw-r--r--   0        0        0       31 2024-03-20 18:16:17.581013 econia_sdk-2.0.0/econia_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581047 econia_sdk-2.0.0/econia_sdk/entry/__init__.py
--rw-r--r--   0        0        0     4144 2024-03-20 18:16:17.581179 econia_sdk-2.0.0/econia_sdk/entry/incentives.py
--rw-r--r--   0        0        0     9305 2024-03-20 18:16:17.581328 econia_sdk-2.0.0/econia_sdk/entry/market.py
--rw-r--r--   0        0        0     3637 2024-03-20 18:16:17.581388 econia_sdk-2.0.0/econia_sdk/entry/registry.py
--rw-r--r--   0        0        0     3883 2024-03-20 18:16:17.581456 econia_sdk-2.0.0/econia_sdk/entry/user.py
--rw-r--r--   0        0        0     4628 2024-03-20 18:16:17.581571 econia_sdk-2.0.0/econia_sdk/lib.py
--rw-r--r--   0        0        0      604 2024-03-20 18:16:17.581630 econia_sdk-2.0.0/econia_sdk/types.py
--rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581661 econia_sdk-2.0.0/econia_sdk/utils/__init__.py
--rw-r--r--   0        0        0     7411 2024-03-20 18:16:17.581809 econia_sdk-2.0.0/econia_sdk/utils/decimals.py
--rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581836 econia_sdk-2.0.0/econia_sdk/view/__init__.py
--rw-r--r--   0        0        0     4629 2024-03-20 18:16:17.581971 econia_sdk-2.0.0/econia_sdk/view/incentives.py
--rw-r--r--   0        0        0    14845 2024-03-20 18:16:17.582054 econia_sdk-2.0.0/econia_sdk/view/market.py
--rw-r--r--   0        0        0    10203 2024-03-20 18:16:17.582208 econia_sdk-2.0.0/econia_sdk/view/registry.py
--rw-r--r--   0        0        0      317 2024-03-20 18:16:17.582412 econia_sdk-2.0.0/econia_sdk/view/resource_account.py
--rw-r--r--   0        0        0    21253 2024-03-20 18:16:17.582499 econia_sdk-2.0.0/econia_sdk/view/user.py
--rw-r--r--   0        0        0      717 2024-03-21 19:43:44.958279 econia_sdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 econia_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      543 2024-03-20 18:16:17.580890 econia_sdk-2.1.0/README.md
+-rw-r--r--   0        0        0      118 2024-03-20 18:16:17.580958 econia_sdk-2.1.0/econia_sdk/README.md
+-rw-r--r--   0        0        0       31 2024-03-20 18:16:17.581013 econia_sdk-2.1.0/econia_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581047 econia_sdk-2.1.0/econia_sdk/entry/__init__.py
+-rw-r--r--   0        0        0     4144 2024-03-20 18:16:17.581179 econia_sdk-2.1.0/econia_sdk/entry/incentives.py
+-rw-r--r--   0        0        0     9305 2024-03-20 18:16:17.581328 econia_sdk-2.1.0/econia_sdk/entry/market.py
+-rw-r--r--   0        0        0     3637 2024-03-20 18:16:17.581388 econia_sdk-2.1.0/econia_sdk/entry/registry.py
+-rw-r--r--   0        0        0     3883 2024-03-20 18:16:17.581456 econia_sdk-2.1.0/econia_sdk/entry/user.py
+-rw-r--r--   0        0        0     5218 2024-04-02 08:35:45.746448 econia_sdk-2.1.0/econia_sdk/lib.py
+-rw-r--r--   0        0        0      604 2024-03-20 18:16:17.581630 econia_sdk-2.1.0/econia_sdk/types.py
+-rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581661 econia_sdk-2.1.0/econia_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     7411 2024-03-20 18:16:17.581809 econia_sdk-2.1.0/econia_sdk/utils/decimals.py
+-rw-r--r--   0        0        0        0 2024-03-20 18:16:17.581836 econia_sdk-2.1.0/econia_sdk/view/__init__.py
+-rw-r--r--   0        0        0     4629 2024-03-20 18:16:17.581971 econia_sdk-2.1.0/econia_sdk/view/incentives.py
+-rw-r--r--   0        0        0    14845 2024-03-20 18:16:17.582054 econia_sdk-2.1.0/econia_sdk/view/market.py
+-rw-r--r--   0        0        0    10203 2024-03-20 18:16:17.582208 econia_sdk-2.1.0/econia_sdk/view/registry.py
+-rw-r--r--   0        0        0      317 2024-03-20 18:16:17.582412 econia_sdk-2.1.0/econia_sdk/view/resource_account.py
+-rw-r--r--   0        0        0    21253 2024-03-20 18:16:17.582499 econia_sdk-2.1.0/econia_sdk/view/user.py
+-rw-r--r--   0        0        0      717 2024-04-11 00:08:39.359252 econia_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 econia_sdk-2.1.0/PKG-INFO
```

### Comparing `econia_sdk-2.0.0/README.md` & `econia_sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/entry/incentives.py` & `econia_sdk-2.1.0/econia_sdk/entry/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/entry/market.py` & `econia_sdk-2.1.0/econia_sdk/entry/market.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/entry/registry.py` & `econia_sdk-2.1.0/econia_sdk/entry/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/entry/user.py` & `econia_sdk-2.1.0/econia_sdk/entry/user.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/lib.py` & `econia_sdk-2.1.0/econia_sdk/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,29 @@
 
     def __init__(
             self,
             node_url: str,
             econia: AccountAddress,
             account: Account,
             rest_client: Optional[RestClient] = None,
-            rest_client_async: Optional[AsyncRestClient] = None
+            rest_client_async: Optional[AsyncRestClient] = None,
+            node_api_key: Optional[str] = None
         ):
         self.econia_address = econia
         if rest_client == None and rest_client_async == None:
             self.aptos_client = RestClient(node_url)
+            if node_api_key != None:
+                self.aptos_client.client.headers["Authorization"] = f"Bearer {node_api_key}"
         elif rest_client != None:
+            if node_api_key != None:
+                rest_client.client.headers["Authorization"] = f"Bearer {node_api_key}"
             self.aptos_client = rest_client
         elif rest_client_async != None:
+            if node_api_key != None:
+                rest_client_async.client.headers["Authorization"] = f"Bearer {node_api_key}"
             self.aptos_client_async = rest_client_async
         self.user_account = account
 
     def submit_tx(self, entry: EntryFunction) -> str:
         payload = TransactionPayload(entry)
         signed_tx = self.aptos_client.create_bcs_signed_transaction(
             self.user_account, payload
@@ -55,17 +62,19 @@
         return txn_hash
 
 
 class EconiaViewer:
     econia_address: AccountAddress
     aptos_client: RestClient
 
-    def __init__(self, node_url: str, econia: AccountAddress):
+    def __init__(self, node_url: str, econia: AccountAddress, node_api_key: Optional[str] = None):
         self.econia_address = econia
         self.aptos_client = RestClient(node_url)
+        if node_api_key != None:
+            self.aptos_client.client.headers["Authorization"] = f"Bearer {node_api_key}"
 
     def get_returns(
         self,
         module: str,
         function: str,
         type_arguments: List[str] = [],
         arguments: List = [],  # string encoded args i.e "12345" or "0xabcdef" or "abracadabra"
```

### Comparing `econia_sdk-2.0.0/econia_sdk/types.py` & `econia_sdk-2.1.0/econia_sdk/types.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/utils/decimals.py` & `econia_sdk-2.1.0/econia_sdk/utils/decimals.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/view/incentives.py` & `econia_sdk-2.1.0/econia_sdk/view/incentives.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/view/market.py` & `econia_sdk-2.1.0/econia_sdk/view/market.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/view/registry.py` & `econia_sdk-2.1.0/econia_sdk/view/registry.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/econia_sdk/view/user.py` & `econia_sdk-2.1.0/econia_sdk/view/user.py`

 * *Files identical despite different names*

### Comparing `econia_sdk-2.0.0/pyproject.toml` & `econia_sdk-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "econia-sdk"
-version = "2.0.0"
+version = "2.1.0"
 description = ""
 authors = ["Econia Labs <developers@econialabs.com>"]
 readme = "README.md"
 packages = [{ include = "econia_sdk" }]
 
 [tool.isort]
 profile = "black"
```

### Comparing `econia_sdk-2.0.0/PKG-INFO` & `econia_sdk-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econia-sdk
-Version: 2.0.0
+Version: 2.1.0
 Summary: 
 Author: Econia Labs
 Author-email: developers@econialabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

