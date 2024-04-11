# Comparing `tmp/ipl_pipeline_py_common-0.4.0.tar.gz` & `tmp/ipl_pipeline_py_common-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipl_pipeline_py_common-0.4.0.tar", max compression
+gzip compressed data, was "ipl_pipeline_py_common-0.5.0.tar", max compression
```

## Comparing `ipl_pipeline_py_common-0.4.0.tar` & `ipl_pipeline_py_common-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      635 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/README.md
--rw-r--r--   0        0        0     1323 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/CommonFunctions/StartupCommon.py
--rw-r--r--   0        0        0       71 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/CommonFunctions/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/CommonFunctions/urn.py
--rw-r--r--   0        0        0     2508 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/DBCommon/DBCommonConnector.py
--rw-r--r--   0        0        0       71 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/DBCommon/__init__.py
--rw-r--r--   0        0        0       31 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/DBCommon/models/__init__.py
--rw-r--r--   0        0        0      376 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/DBCommon/models/base.py
--rw-r--r--   0        0        0      156 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/QueueModels/__init__.py
--rw-r--r--   0        0        0      166 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/QueueModels/serviceRequest.py
--rw-r--r--   0        0        0      429 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/QueueModels/serviceResponse.py
--rw-r--r--   0        0        0       58 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pipeline/__init__.py
--rw-r--r--   0        0        0      551 2024-03-19 23:47:10.966312 ipl_pipeline_py_common-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      635 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/README.md
+-rw-r--r--   0        0        0     1336 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/CommonFunctions/StartupCommon.py
+-rw-r--r--   0        0        0       71 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/CommonFunctions/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/CommonFunctions/urn.py
+-rw-r--r--   0        0        0      113 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/__init__.py
+-rw-r--r--   0        0        0     2856 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/dBCommonConnector.py
+-rw-r--r--   0        0        0       45 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/models/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/models/base.py
+-rw-r--r--   0        0        0      156 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/QueueModels/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/QueueModels/serviceRequest.py
+-rw-r--r--   0        0        0      429 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/QueueModels/serviceResponse.py
+-rw-r--r--   0        0        0       58 2024-04-11 20:10:56.239617 ipl_pipeline_py_common-0.5.0/pipeline/__init__.py
+-rw-r--r--   0        0        0      551 2024-04-11 20:10:56.243618 ipl_pipeline_py_common-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.5.0/PKG-INFO
```

### Comparing `ipl_pipeline_py_common-0.4.0/README.md` & `ipl_pipeline_py_common-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.4.0/pipeline/CommonFunctions/StartupCommon.py` & `ipl_pipeline_py_common-0.5.0/pipeline/CommonFunctions/StartupCommon.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,27 @@
         """
         if not (return_value := os.getenv(key_name)):
             logging.error(f"static.env - '{key_name}' key not found. Cannot start API.")
             raise EnvironmentError
         return return_value
 
     @staticmethod
-    def _get_key_or_default(key_name: str, default_value: str):
+    def _get_key_or_default(key_name: str, default_value: str) -> str:
         """
         Gets a value from env, if env have no value, will return the default value given
         :param key_name: key name
         :param default_value: default value
         :return: key/default value
         """
         if not (return_value := os.getenv(key_name)):
             return_value = default_value
         return return_value
 
     def __init__(self):
         self.node_id = self._get_key_or_default("NODE_ID", "unknown")
-        self.debug = self._get_key_or_default("DEBUG", "False") == "True" or "1"
+        self.debug = bool(self._get_key_or_default("DEBUG", "False") == "True" or "1")
 
     @property
     def node_id_int(self) -> int:
         if self.node_id == "unknown":
             return -1
         return int(self.node_id)
```

### Comparing `ipl_pipeline_py_common-0.4.0/pipeline/CommonFunctions/urn.py` & `ipl_pipeline_py_common-0.5.0/pipeline/CommonFunctions/urn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 Handles parsing of IPL URNs
 
 example:
     urn:iplsplatoon:production:commentators:id:{id}
 """
-from typing import List
+from typing import List, Optional
 
 
 class URN:
-    ns: str
-    ns_specific: str
-    sub_component: str
-    id_provider: str
-    id_type: str
-    identifier: str
+    ns: Optional[str]
+    ns_specific: Optional[str]
+    sub_component: Optional[str]
+    id_provider: Optional[str]
+    id_type: Optional[str]
+    identifier: Optional[str]
 
     @staticmethod
-    def get_from_index(input_list: List[any], i: int, default=None):
+    def get_from_index(input_list: List[str], i: int, default=None) -> Optional[str]:
         if len(input_list) < i:
             if default:
                 return default
             raise IndexError
-        return input_list[i]
+        if input_list[i]:
+            return input_list[i]
 
     def __init__(self, urn: str):
         try:
             string_split = urn.split(':')
             if string_split[0] != "urn":
                 raise ValueError('Invalid URN')
             self.ns = self.get_from_index(string_split, 1)
```

### Comparing `ipl_pipeline_py_common-0.4.0/pipeline/DBCommon/DBCommonConnector.py` & `ipl_pipeline_py_common-0.5.0/pipeline/DBCommon/dBCommonConnector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 import motor.motor_asyncio
 from redis import asyncio as aioredis
 from typing import Optional, Union
 import msgpack
 
+from .exceptions import NoConnectionError
+
 
 class DBCommonConnector:
     def __init__(self, mongo_uri: str, db_name: str, redis_uri: str):
         """
         Constructor
         :param mongo_uri: MongoDB Connection URI
         :param system_db_name: DB Name
         :param verification_db_name: DB Name
         :param redis_uri: Redis Connection URI
         """
         self._mongo_uri = mongo_uri
         self._redis_uri = redis_uri
         self._db_name = db_name
-        self._redis_client: Optional[aioredis.client] = None
-        self._mongo_client: motor.motor_asyncio.AsyncIOMotorClient = None
-        self._db: motor.motor_asyncio.AsyncIOMotorDatabase = None
+        self._redis_client: Optional[aioredis.Redis] = None
+        self._mongo_client: Optional[motor.motor_asyncio.AsyncIOMotorClient] = None
+        self._db: Optional[motor.motor_asyncio.AsyncIOMotorDatabase] = None
 
     async def connect_db(self):
         """Create database connection."""
         self._mongo_client = motor.motor_asyncio.AsyncIOMotorClient(self._mongo_uri, tz_aware=True)
         self._db = self._mongo_client[self._db_name]
         self._redis_client = await aioredis.from_url(self._redis_uri)
 
     async def close_mongo_connection(self):
         """Close database connection."""
-        self._mongo_client.close()
+        if self._mongo_client:
+            self._mongo_client.close()
 
     async def _cache_set_key(self, key: str, value: Union[dict, list], expire: Union[int, None] = 1800) -> bool:
         """
         Add Key:Value to Redis cache
         :param key: Key name
         :param value: Value Data dict
         :param expire: expiry time in seconds, default 1800s
         :return: if operation was successful
         """
-        _value = msgpack.packb(value, use_bin_type=True)
+        if self._redis_client is None:
+            raise NoConnectionError("Redis client not connected")
         async with self._redis_client.client() as conn:
             if expire and expire > 0:
-                ok = await conn.execute_command("SET", f"{key}", _value, "EX", f"{expire}")
+                ok = await conn.execute_command("SET", f"{key}", value, "EX", f"{expire}")
             else:
-                ok = await conn.execute_command("SET", f"{key}", _value)
-            return ok
+                ok = await conn.execute_command("SET", f"{key}", value)
+            return bool(ok)
 
     async def _cache_get_key(self, key: str) -> Optional[Union[dict, list]]:
         """
         Retrieve value via key from Redis cache
         :param key: Key to retrieve data from
         :return: None or dict
         """
-        if value := await self._redis_client.get(f"{key}"):
-            return msgpack.unpackb(value, raw=False)
+        if self._redis_client is None:
+            raise NoConnectionError("Redis client not connected")
+        if data := await self._redis_client.get(f"{key}"):
+            return data
+        return None
 
     async def _cache_delete_key(self, key: str) -> bool:
         """
         Delete key from Redis Cache
         :param key: Key Name
         :return: if operation was successful
         """
+        if self._redis_client is None:
+            raise NoConnectionError("Redis client not connected")
         if await self._redis_client.delete(key):
             return True
         else:
             return False
-
```

### Comparing `ipl_pipeline_py_common-0.4.0/pyproject.toml` & `ipl_pipeline_py_common-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipl-pipeline-py-common"
-version = "0.4.0"
+version = "0.5.0"
 description = "Common functions and modules for Python based IPL Pipeline Services"
 authors = ["Vincent Lee <vlee@vlee.me.uk>"]
 license = "All Rights Reserved"
 readme = "README.md"
 packages = [{include = "pipeline"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ipl_pipeline_py_common-0.4.0/PKG-INFO` & `ipl_pipeline_py_common-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipl-pipeline-py-common
-Version: 0.4.0
+Version: 0.5.0
 Summary: Common functions and modules for Python based IPL Pipeline Services
 License: All Rights Reserved
 Author: Vincent Lee
 Author-email: vlee@vlee.me.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

