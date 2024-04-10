# Comparing `tmp/pysnc-1.1.6a5.tar.gz` & `tmp/pysnc-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.6a5.tar", max compression
+gzip compressed data, was "pysnc-1.1.7.tar", max compression
```

## Comparing `pysnc-1.1.6a5.tar` & `pysnc-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/LICENSE
--rw-r--r--   0        0        0     1590 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/README.md
--rw-r--r--   0        0        0     1114 2024-03-26 17:52:52.958803 pysnc-1.1.6a5/pyproject.toml
--rw-r--r--   0        0        0      129 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/__version__.py
--rw-r--r--   0        0        0     9386 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/attachment.py
--rw-r--r--   0        0        0     3787 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/auth.py
--rw-r--r--   0        0        0    16208 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/client.py
--rw-r--r--   0        0        0     1002 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/exceptions.py
--rw-r--r--   0        0        0     5083 2024-03-26 17:52:45.198822 pysnc-1.1.6a5/pysnc/query.py
--rw-r--r--   0        0        0    40278 2024-03-26 17:52:45.202822 pysnc-1.1.6a5/pysnc/record.py
--rw-r--r--   0        0        0      846 2024-03-26 17:52:45.202822 pysnc-1.1.6a5/pysnc/utils.py
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 pysnc-1.1.6a5/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-04-10 23:58:16.083735 pysnc-1.1.7/LICENSE
+-rw-r--r--   0        0        0     1590 2024-04-10 23:58:16.083735 pysnc-1.1.7/README.md
+-rw-r--r--   0        0        0     1113 2024-04-10 23:58:31.415863 pysnc-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/__version__.py
+-rw-r--r--   0        0        0     9386 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/attachment.py
+-rw-r--r--   0        0        0     3787 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/auth.py
+-rw-r--r--   0        0        0    16208 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/exceptions.py
+-rw-r--r--   0        0        0     5083 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/query.py
+-rw-r--r--   0        0        0    40296 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/record.py
+-rw-r--r--   0        0        0      846 2024-04-10 23:58:16.083735 pysnc-1.1.7/pysnc/utils.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 pysnc-1.1.7/PKG-INFO
```

### Comparing `pysnc-1.1.6a5/LICENSE` & `pysnc-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/README.md` & `pysnc-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pyproject.toml` & `pysnc-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.6a5"
+version = "1.1.7"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
@@ -17,15 +17,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "2.31.0"
 requests-oauthlib = { version = ">=1.2.0", optional = true}
 certifi = "2023.7.22"
-pip = "^23.3.1"
+pip = ">=23.3.1"
 urllib3 = "^2.0.7"
 
 [tool.poetry.extras]
 oauth = ["requests-oauthlib"]
 
 [tool.poetry.group.dev.dependencies]
 requests-oauthlib = ">=1.2.0"
```

### Comparing `pysnc-1.1.6a5/pysnc/attachment.py` & `pysnc-1.1.7/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pysnc/auth.py` & `pysnc-1.1.7/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pysnc/client.py` & `pysnc-1.1.7/pysnc/client.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pysnc/exceptions.py` & `pysnc-1.1.7/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pysnc/query.py` & `pysnc-1.1.7/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/pysnc/record.py` & `pysnc-1.1.7/pysnc/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
                 return True
             return False
         else:
             self.add_query(name, value)
             self.query()
             return self.next()
 
-    def insert(self) -> Optional[str]:
+    def insert(self) -> Optional[GlideElement]:
         """
         Insert a new record.
 
         :return: The ``sys_id`` of the record created or ``None``
         :raise:
             :AuthenticationException: If we do not have rights
             :InsertException: For any other failure reason
@@ -587,15 +587,15 @@
             return None
         elif code == 401:
             raise AuthenticationException(response.json()['error'])
         else:
             rjson = response.json()
             raise InsertException(rjson['error'] if 'error' in rjson else f"{code} response on insert -- expected 201", status_code=code)
 
-    def update(self) -> Optional[str]:
+    def update(self) -> Optional[GlideElement]:
         """
         Update the current record.
 
         :return: The ``sys_id`` on success or ``None``
         :raise:
             :AuthenticationException: If we do not have rights
             :UpdateException: For any other failure reason
```

### Comparing `pysnc-1.1.6a5/pysnc/utils.py` & `pysnc-1.1.7/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.6a5/PKG-INFO` & `pysnc-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.6a5
+Version: 1.1.7
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: oauth
 Requires-Dist: certifi (==2023.7.22)
-Requires-Dist: pip (>=23.3.1,<24.0.0)
+Requires-Dist: pip (>=23.3.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: requests-oauthlib (>=1.2.0) ; extra == "oauth"
 Requires-Dist: urllib3 (>=2.0.7,<3.0.0)
 Project-URL: Documentation, https://servicenow.github.io/PySNC/
 Project-URL: Repository, https://github.com/ServiceNow/PySNC
 Description-Content-Type: text/markdown
```

