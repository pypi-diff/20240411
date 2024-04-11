# Comparing `tmp/another_fastapi_jwt_auth-0.0.2.tar.gz` & `tmp/another_fastapi_jwt_auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_fastapi_jwt_auth-0.0.2.tar", max compression
+gzip compressed data, was "another_fastapi_jwt_auth-0.0.5.tar", max compression
```

## Comparing `another_fastapi_jwt_auth-0.0.2.tar` & `another_fastapi_jwt_auth-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/LICENSE
--rw-r--r--   0        0        0     1968 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/README.md
--rw-r--r--   0        0        0      147 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/__init__.py
--rw-r--r--   0        0        0     4970 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/auth_config.py
--rw-r--r--   0        0        0    36008 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/auth_jwt.py
--rw-r--r--   0        0        0     4522 2024-02-02 15:57:59.881473 another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/config.py
--rw-r--r--   0        0        0     2242 2024-02-02 15:57:59.885473 another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/exceptions.py
--rw-r--r--   0        0        0     1474 2024-02-02 15:57:59.885473 another_fastapi_jwt_auth-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 another_fastapi_jwt_auth-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-11 19:49:25.864217 another_fastapi_jwt_auth-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-11 19:49:25.864217 another_fastapi_jwt_auth-0.0.5/README.md
+-rw-r--r--   0        0        0      147 2024-04-11 19:49:25.868217 another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-11 19:49:25.868217 another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/auth_config.py
+-rw-r--r--   0        0        0    36008 2024-04-11 19:49:25.868217 another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/auth_jwt.py
+-rw-r--r--   0        0        0     4522 2024-04-11 19:49:25.868217 another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/config.py
+-rw-r--r--   0        0        0     2242 2024-04-11 19:49:25.868217 another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/exceptions.py
+-rw-r--r--   0        0        0     1474 2024-04-11 19:49:25.872217 another_fastapi_jwt_auth-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 another_fastapi_jwt_auth-0.0.5/PKG-INFO
```

### Comparing `another_fastapi_jwt_auth-0.0.2/LICENSE` & `another_fastapi_jwt_auth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/README.md` & `another_fastapi_jwt_auth-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/auth_config.py` & `another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/auth_jwt.py` & `another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/config.py` & `another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/config.py`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/another_fastapi_jwt_auth/exceptions.py` & `another_fastapi_jwt_auth-0.0.5/another_fastapi_jwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `another_fastapi_jwt_auth-0.0.2/pyproject.toml` & `another_fastapi_jwt_auth-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "another-fastapi-jwt-auth"
 authors = ["Nyoman Pradipta Dewantara <nyomanpradipta120@gmail.com>", "delrey1 <del@rey>"]
 description = "Another iteration of fastapi-jwt-auth"
-version = "0.0.2"
+version = "0.0.5"
 homepage = "https://github.com/delrey1/another-fastapi-jwt-auth"
 readme = "README.md"
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 
 [tool.poetry.dependencies]
-fastapi = "^0.109.0"
+fastapi = "^0.110.1"
 PyJWT = "^2"
 python = "^3.8.0, <4"
 
 
 #requires = [
 #    "fastapi>=0.61.0",
 #    "PyJWT>=1.7.1,<2.0.0"
```

### Comparing `another_fastapi_jwt_auth-0.0.2/PKG-INFO` & `another_fastapi_jwt_auth-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: another-fastapi-jwt-auth
-Version: 0.0.2
+Version: 0.0.5
 Summary: Another iteration of fastapi-jwt-auth
 Home-page: https://github.com/delrey1/another-fastapi-jwt-auth
 Author: Nyoman Pradipta Dewantara
 Author-email: nyomanpradipta120@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT (>=2,<3)
-Requires-Dist: fastapi (>=0.109.0,<0.110.0)
+Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Another FastAPI JWT Auth
 
 [//]: # (![Tests]&#40;https://github.com/IndominusByte/fastapi-jwt-auth/workflows/Tests/badge.svg&#41;)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: another-fastapi-jwt-auth Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: another-fastapi-jwt-auth Version: 0.0.5 Summary:
 Another iteration of fastapi-jwt-auth Home-page: https://github.com/delrey1/
 another-fastapi-jwt-auth Author: Nyoman Pradipta Dewantara Author-email:
 nyomanpradipta120@gmail.com Requires-Python: >=3.8.0,<4.0.0 Classifier:
 Environment :: Web Environment Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyJWT (>=2,<3) Requires-Dist: fastapi (>=0.109.0,<0.110.0)
+Requires-Dist: PyJWT (>=2,<3) Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0) Requires-Dist: pydantic-settings
 (>=2.1.0,<3.0.0) Description-Content-Type: text/markdown # Another FastAPI JWT
 Auth [//]: # (![Tests](https://github.com/IndominusByte/fastapi-jwt-auth/
 workflows/Tests/badge.svg)) [//]: # ([![Coverage Status](https://coveralls.io/
 repos/github/IndominusByte/fastapi-jwt-auth/badge.svg?branch=master)](https://
 coveralls.io/github/IndominusByte/fastapi-jwt-auth?branch=master)) [//]: # ([!
 [PyPI version](https://badge.fury.io/py/fastapi-jwt-auth.svg)](https://
```

