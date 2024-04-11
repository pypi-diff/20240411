# Comparing `tmp/aioease-0.1.2-py3-none-any.whl.zip` & `tmp/aioease-0.1.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3554 bytes, number of entries: 7
+Zip file size: 3671 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 24-Apr-11 19:27 aioease/__init__.py
--rw-rw-rw-  2.0 fat     3093 b- defN 24-Apr-11 19:27 aioease/main.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-11 20:06 aioease-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1108 b- defN 24-Apr-11 20:06 aioease-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 20:06 aioease-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-11 20:06 aioease-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      531 b- defN 24-Apr-11 20:06 aioease-0.1.2.dist-info/RECORD
-7 files, 5929 bytes uncompressed, 2614 bytes compressed:  55.9%
+-rw-rw-rw-  2.0 fat     3119 b- defN 24-Apr-11 20:29 aioease/main.py
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-11 20:37 aioease-0.1.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1395 b- defN 24-Apr-11 20:37 aioease-0.1.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 20:37 aioease-0.1.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-11 20:37 aioease-0.1.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 24-Apr-11 20:37 aioease-0.1.21.dist-info/RECORD
+7 files, 6247 bytes uncompressed, 2721 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: aioease/__init__.py
 Comment: 
 
 Filename: aioease/main.py
 Comment: 
 
-Filename: aioease-0.1.2.dist-info/LICENSE
+Filename: aioease-0.1.21.dist-info/LICENSE
 Comment: 
 
-Filename: aioease-0.1.2.dist-info/METADATA
+Filename: aioease-0.1.21.dist-info/METADATA
 Comment: 
 
-Filename: aioease-0.1.2.dist-info/WHEEL
+Filename: aioease-0.1.21.dist-info/WHEEL
 Comment: 
 
-Filename: aioease-0.1.2.dist-info/top_level.txt
+Filename: aioease-0.1.21.dist-info/top_level.txt
 Comment: 
 
-Filename: aioease-0.1.2.dist-info/RECORD
+Filename: aioease-0.1.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioease/main.py

```diff
@@ -21,24 +21,23 @@
         methods = {
             "get": session.get,
             "post": session.post,
             "put": session.put,
             "delete": session.delete,
         }
         method = methods.get(request["method"].lower(), session.get)
-        url = request.get("url", "")
-
+        url = request["url"]
         # Debug-level log of the request details
         logger.debug(f"Sending {request['method'].upper()} request to {url}")
+        del request["method"]
 
         async with self.limiter:
             try:
-                async with method(url) as resp:
+                async with method(**request) as resp:
                     response = await resp.text()
-
                     # Debug-level log of the response details
                     logger.debug(f"Received response {resp.status} from {url}")
                     return {"status": resp.status, "response": response}
             except Exception as e:
                 # Error-level log if an exception occurs
                 logger.error(f"Error making request to {url}: {e}")
                 return {"status": "error", "response": str(e)}
```

## Comparing `aioease-0.1.2.dist-info/LICENSE` & `aioease-0.1.21.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aioease-0.1.2.dist-info/METADATA` & `aioease-0.1.21.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: aioease
-Version: 0.1.2
+Version: 0.1.21
+Summary: A simple and easy to use asyncio & aiohttp libraries.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp >=3
 Requires-Dist: aiolimiter >=1
 
 # AIOEase
 
-`AIOEase` simplifies asynchronous HTTP requests in Python, offering a straightforward interface for handling multiple requests concurrently with rate limiting.
+`AIOEase` simplifies asynchronous HTTP requests in Python, offering a straightforward interface for handling multiple requests asynchronously with rate limiting.
+Proved a list of dictionaries and the `requests_per_second_max` (default 1). Returns the status and response as a list of dictionaries.
 
 ## Installation
 
 ```bash
 pip install aioease
 ```
 
@@ -34,15 +36,17 @@
 ## Configuring Logging
 
 Control the verbosity of logs for debugging:
 
 ```python
 import logging
 
+logging.basicConfig(level=logging.INFO)
 logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.ERROR)
 ```
 
 ## License
 
 Available under the MIT License.
 
 ## Support
```

## Comparing `aioease-0.1.2.dist-info/RECORD` & `aioease-0.1.21.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 aioease/__init__.py,sha256=a6rCsJjLbHO6rDXGUt6aNY0p4pdXPLsraOCXS1b3ebU,25
-aioease/main.py,sha256=8zgolnOgl3qBxCe_Q3DgjGK2AZ2Hs_jP8yF6sQY-okI,3093
-aioease-0.1.2.dist-info/LICENSE,sha256=KUfCP2RRTQeOp21tGhWgyQC88-Awp1f53UWHBJhbqw4,1072
-aioease-0.1.2.dist-info/METADATA,sha256=QJuRj4dO1lFk7F-2WzXPShOOqhC5-kVszApAKuD83CE,1108
-aioease-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aioease-0.1.2.dist-info/top_level.txt,sha256=YC746SLK75mF2jnE3ENkKxCYhsK-teH2V1nl1BmrGO4,8
-aioease-0.1.2.dist-info/RECORD,,
+aioease/main.py,sha256=MLF1y7vgJlwkKZTJr4gQ4EXHo2AuNkmlZ8qj5KkT6Ig,3119
+aioease-0.1.21.dist-info/LICENSE,sha256=KUfCP2RRTQeOp21tGhWgyQC88-Awp1f53UWHBJhbqw4,1072
+aioease-0.1.21.dist-info/METADATA,sha256=tzjGSKbPGv2X1k34PCKjVvL296IUKaTPFHhO4gZjQa4,1395
+aioease-0.1.21.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aioease-0.1.21.dist-info/top_level.txt,sha256=YC746SLK75mF2jnE3ENkKxCYhsK-teH2V1nl1BmrGO4,8
+aioease-0.1.21.dist-info/RECORD,,
```

