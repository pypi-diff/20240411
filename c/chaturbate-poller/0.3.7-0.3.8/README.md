# Comparing `tmp/chaturbate_poller-0.3.7.tar.gz` & `tmp/chaturbate_poller-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.7.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.8.tar", max compression
```

## Comparing `chaturbate_poller-0.3.7.tar` & `chaturbate_poller-0.3.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-11 01:45:30.220776 chaturbate_poller-0.3.7/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-11 01:45:30.220776 chaturbate_poller-0.3.7/README.md
--rw-r--r--   0        0        0     3129 2024-04-11 01:45:41.280784 chaturbate_poller-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      573 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     4027 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      895 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     4017 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/format_messages.py
--rw-r--r--   0        0        0     1564 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     5578 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-11 16:04:32.008994 chaturbate_poller-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-11 16:04:32.008994 chaturbate_poller-0.3.8/README.md
+-rw-r--r--   0        0        0     3129 2024-04-11 16:04:42.441065 chaturbate_poller-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     4286 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0     1762 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     4017 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/format_messages.py
+-rw-r--r--   0        0        0     1564 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     4877 2024-04-11 16:04:32.012994 chaturbate_poller-0.3.8/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.8/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.7/LICENSE` & `chaturbate_poller-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.7/README.md` & `chaturbate_poller-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.7/pyproject.toml` & `chaturbate_poller-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.7"
+version = "0.3.8"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,35 +22,43 @@
 class ChaturbateClient:
     """Client for fetching Chaturbate events.
 
     Args:
         username (str): The Chaturbate username.
         token (str): The Chaturbate token.
         timeout (int, optional): The timeout for the request. Defaults to None.
+        base_url (str, optional): The base URL for the Chaturbate API. Defaults to None.
 
     Raises:
         ValueError: If username or token are not provided.
     """
 
-    def __init__(self, username: str, token: str, timeout: int | None = None) -> None:
+    def __init__(
+        self,
+        username: str,
+        token: str,
+        timeout: int | None = None,
+        base_url: str | None = None,
+    ) -> None:
         """Initialize client.
 
         Args:
             username (str): The Chaturbate username.
             token (str): The Chaturbate token.
             timeout (int, optional): The timeout for the request. Defaults to None.
+            base_url (str, optional): The base URL for the API. Defaults to None.
 
         Raises:
             ValueError: If username or token are not provided.
         """
         if not username or not token:
             msg = "Chaturbate username and token are required."
             raise ValueError(msg)
 
-        self.base_url = BASE_URL
+        self.base_url = base_url or BASE_URL
         self.timeout = timeout
         self.username = username
         self.token = token
         self.client = httpx.AsyncClient()
 
     async def __aenter__(self) -> "ChaturbateClient":
         """Enter client.
```

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Constants for the chaturbate_poller module."""
 
 from enum import IntEnum
 
-BASE_URL = "https://events.testbed.cb.dev/events/{username}/{token}/"
+BASE_URL = "https://eventsapi.chaturbate.com/events/{username}/{token}/"
 """str: The base URL for fetching Chaturbate events."""
 
+TEST_BASE_URL = "https://events.testbed.cb.dev/events/{username}/{token}/"
+"""str: The base URL for fetching Chaturbate events in the test environment."""
+
 
 class HttpStatusCode(IntEnum):
     """HTTP status codes."""
 
     OK = 200
     CREATED = 201
     ACCEPTED = 202
@@ -30,7 +33,37 @@
 """int: Maximum time in seconds that the server will wait before sending the nextURL."""
 
 TIMEOUT_BUFFER = 5
 """int: Buffer time in seconds to add to the API timeout to prevent HTTP timeouts."""
 
 RETRY_DELAY = 20
 """int: Delay in seconds before retrying the request."""
+
+EXAMPLE_JSON_STRING = """
+{
+    "events":[
+        {
+            "method":"mediaPurchase",
+            "object":{
+				"broadcaster": "example_broadcaster",
+				"user": {
+					"username": "example_user",
+					"inFanclub": false,
+					"gender": "m",
+					"hasTokens": true,
+					"recentTips": "none",
+					"isMod": false
+				},
+				"media": {
+					"id": 1,
+					"name": "photoset1",
+					"type": "photos",
+					"tokens": 25
+                }
+            },
+            "id":"UNIQUE_EVENT_ID"
+        }
+    ],
+    "nextUrl":"https://eventsapi.chaturbate.com/events/REDACTED_BROADCASTER/REDACTED_API_TOKEN/?i=UNIQUE_EVENT_ID&timeout=10"
+}
+"""
+"""str: A JSON string representing the EventsAPIResponse object."""
```

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/format_messages.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/format_messages.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.7/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.8/src/chaturbate_poller/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -159,38 +159,7 @@
 
 class EventsAPIResponse(BaseModel):
     """Model for the EventsAPIResponse object."""
 
     events: list[Event]
     """list[Event]: A list containing the event objects."""
     next_url: HttpUrl | None = Field(..., alias="nextUrl", description="The next URL.")
-
-
-json_string = """
-{
-    "events":[
-        {
-            "method":"mediaPurchase",
-            "object":{
-				"broadcaster": "example_broadcaster",
-				"user": {
-					"username": "example_user",
-					"inFanclub": false,
-					"gender": "m",
-					"hasTokens": true,
-					"recentTips": "none",
-					"isMod": false
-				},
-				"media": {
-					"id": 1,
-					"name": "photoset1",
-					"type": "photos",
-					"tokens": 25
-                }
-            },
-            "id":"UNIQUE_EVENT_ID"
-        }
-    ],
-    "nextUrl":"https://eventsapi.chaturbate.com/events/REDACTED_BROADCASTER/REDACTED_API_TOKEN/?i=UNIQUE_EVENT_ID&timeout=10"
-}
-"""
-"""str: A JSON string representing the EventsAPIResponse object."""
```

### Comparing `chaturbate_poller-0.3.7/PKG-INFO` & `chaturbate_poller-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.7
+Version: 0.3.8
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

