# Comparing `tmp/chaturbate_poller-0.3.5.tar.gz` & `tmp/chaturbate_poller-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.5.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.6.tar", max compression
```

## Comparing `chaturbate_poller-0.3.5.tar` & `chaturbate_poller-0.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-10 15:45:51.505478 chaturbate_poller-0.3.5/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-10 15:45:51.505478 chaturbate_poller-0.3.5/README.md
--rw-r--r--   0        0        0     3129 2024-04-10 15:46:02.509504 chaturbate_poller-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      573 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     3889 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      669 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     4017 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/format_messages.py
--rw-r--r--   0        0        0     2211 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     5578 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-10 21:12:06.650014 chaturbate_poller-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-10 21:12:06.650014 chaturbate_poller-0.3.6/README.md
+-rw-r--r--   0        0        0     3129 2024-04-10 21:12:17.306099 chaturbate_poller-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     3889 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      669 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     4017 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/format_messages.py
+-rw-r--r--   0        0        0     2211 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     5578 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.6/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.5/LICENSE` & `chaturbate_poller-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/README.md` & `chaturbate_poller-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/pyproject.toml` & `chaturbate_poller-0.3.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.5"
+version = "0.3.6"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/chaturbate_poller.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/format_messages.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/format_messages.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.6/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.5/PKG-INFO` & `chaturbate_poller-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.5
+Version: 0.3.6
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

