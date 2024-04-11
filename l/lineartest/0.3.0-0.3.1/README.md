# Comparing `tmp/lineartest-0.3.0.tar.gz` & `tmp/lineartest-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.3.0.tar", max compression
+gzip compressed data, was "lineartest-0.3.1.tar", max compression
```

## Comparing `lineartest-0.3.0.tar` & `lineartest-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.3.0/LICENSE
--rw-r--r--   0        0        0     1963 2024-04-10 17:53:47.920014 lineartest-0.3.0/README.md
--rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.3.0/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.3.0/lineartest/_log.py
--rw-r--r--   0        0        0     7281 2024-04-10 17:47:38.620517 lineartest-0.3.0/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.3.0/lineartest/schedule.py
--rw-r--r--   0        0        0     1196 2024-04-10 17:54:53.051198 lineartest-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 lineartest-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1963 2024-04-10 17:55:46.854950 lineartest-0.3.1/README.md
+-rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.3.1/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.3.1/lineartest/_log.py
+-rw-r--r--   0        0        0     7362 2024-04-10 18:13:56.911449 lineartest-0.3.1/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.3.1/lineartest/schedule.py
+-rw-r--r--   0        0        0     1196 2024-04-10 18:13:56.911738 lineartest-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 lineartest-0.3.1/PKG-INFO
```

### Comparing `lineartest-0.3.0/LICENSE` & `lineartest-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.0/README.md` & `lineartest-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.0/lineartest/_log.py` & `lineartest-0.3.1/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.0/lineartest/client.py` & `lineartest-0.3.1/lineartest/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
             follow_redirects=follow_redirects,
             allow_redirects=allow_redirects,
             **extra,
         )
 
         # return if not response model specified
         if response_model is None:
+            print('<<< Response:', response.status_code, response.reason_phrase)
             return response
 
         # check if response is JSON
         content_type = response.headers.get('Content-Type')
         error_message = f'expected response type to be "application/json", got {content_type} instead.'
         assert content_type == 'application/json', error_message
         response_dict = response.json()
```

### Comparing `lineartest-0.3.0/lineartest/schedule.py` & `lineartest-0.3.1/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.0/pyproject.toml` & `lineartest-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.3.0"
+version = "0.3.1"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `lineartest-0.3.0/PKG-INFO` & `lineartest-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.3.0
+Version: 0.3.1
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

