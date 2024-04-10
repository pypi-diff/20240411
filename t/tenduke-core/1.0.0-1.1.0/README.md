# Comparing `tmp/tenduke_core-1.0.0.tar.gz` & `tmp/tenduke_core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_core-1.0.0.tar", max compression
+gzip compressed data, was "tenduke_core-1.1.0.tar", max compression
```

## Comparing `tenduke_core-1.0.0.tar` & `tenduke_core-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1108 2024-03-13 21:00:43.541815 tenduke_core-1.0.0/LICENSE
--rw-r--r--   0        0        0     2764 2024-03-13 21:00:43.541815 tenduke_core-1.0.0/README.md
--rw-r--r--   0        0        0     3616 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      191 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/__init__.py
--rw-r--r--   0        0        0      659 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/__init__.py
--rw-r--r--   0        0        0     1665 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/auth_provider.py
--rw-r--r--   0        0        0     1022 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/device_auth_response.py
--rw-r--r--   0        0        0     7252 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/device_flow_client.py
--rw-r--r--   0        0        0     6413 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/oauth_client.py
--rw-r--r--   0        0        0     7029 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/pkce_flow_client.py
--rw-r--r--   0        0        0     1540 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/token_response.py
--rw-r--r--   0        0        0     1789 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/auth/user_info.py
--rw-r--r--   0        0        0     4121 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/base_model.py
--rw-r--r--   0        0        0      135 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/config/__init__.py
--rw-r--r--   0        0        0     6073 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/config/tenduke_config.py
--rw-r--r--   0        0        0      319 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/exceptions/__init__.py
--rw-r--r--   0        0        0     2494 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/exceptions/api.py
--rw-r--r--   0        0        0     5939 2024-03-13 21:00:43.542815 tenduke_core-1.0.0/tenduke_core/exceptions/oauth.py
--rw-r--r--   0        0        0     1858 2024-03-13 21:00:43.543815 tenduke_core-1.0.0/tenduke_core/exceptions/validation.py
--rw-r--r--   0        0        0        0 2024-03-13 21:00:43.569815 tenduke_core-1.0.0/tenduke_core/py.typed
--rw-r--r--   0        0        0      865 2024-03-13 21:00:43.543815 tenduke_core-1.0.0/tenduke_core/session_factory.py
--rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 tenduke_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-04-10 03:35:47.803895 tenduke_core-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2843 2024-04-10 03:35:47.804812 tenduke_core-1.1.0/README.md
+-rw-r--r--   0        0        0     3624 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      191 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/auth_provider.py
+-rw-r--r--   0        0        0     1022 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/device_auth_response.py
+-rw-r--r--   0        0        0     7252 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/device_flow_client.py
+-rw-r--r--   0        0        0     6413 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/oauth_client.py
+-rw-r--r--   0        0        0     7029 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/pkce_flow_client.py
+-rw-r--r--   0        0        0     1540 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/token_response.py
+-rw-r--r--   0        0        0     1789 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/auth/user_info.py
+-rw-r--r--   0        0        0     4121 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/base_model.py
+-rw-r--r--   0        0        0      135 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/config/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/config/tenduke_config.py
+-rw-r--r--   0        0        0      319 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2494 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/api.py
+-rw-r--r--   0        0        0     5939 2024-04-10 03:35:47.805729 tenduke_core-1.1.0/tenduke_core/exceptions/oauth.py
+-rw-r--r--   0        0        0     1858 2024-04-10 03:35:47.806645 tenduke_core-1.1.0/tenduke_core/exceptions/validation.py
+-rw-r--r--   0        0        0        0 2024-04-10 03:35:47.828645 tenduke_core-1.1.0/tenduke_core/py.typed
+-rw-r--r--   0        0        0      865 2024-04-10 03:35:47.806645 tenduke_core-1.1.0/tenduke_core/session_factory.py
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 tenduke_core-1.1.0/PKG-INFO
```

### Comparing `tenduke_core-1.0.0/LICENSE` & `tenduke_core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/README.md` & `tenduke_core-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,18 @@
 
 That change shall be committed in a new revision.
 
 That revision shall be tagged (for example `git tag v1.1.1`).
 
 The new tag shall be pushed (`git push --tags`).
 
-That will trigger the creation of a new package and the publishing of that package to the relevant
-repository.
+That will trigger the creation of a new package and the publishing of that package to the GitLab
+package repository.
+
+[Publishing to PyPi](./docs/publishing.md) requires additional steps.
 
 ## Getting involved
 
 We welcome contributions! [Contributing](./CONTRIBUTING) explains what kind of contributions we
 welcome.
 
 ## Resources
```

### Comparing `tenduke_core-1.0.0/pyproject.toml` & `tenduke_core-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "tenduke_core"
-version = "1.0.0"
+version = "1.1.0"
 description = "Shared code supporting 10Duke SDKs"
 authors = []
 repository = "https://gitlab.com/10Duke/core/python-core"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_core"},
     {include = "tenduke_core/py.typed"},
 ]
 
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -29,39 +29,39 @@
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 authlib = "^1.3.0"
-dataconf = "^2.5.0"
+dataconf = "^3.1.0"
 pyjwt = {extras = ["crypto"], version = "^2.8.0"}
 python-dateutil = "^2.9.0.post0"
 requests = {extras = ["security"], version = "^2.31.0"}
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 mypy = "^1.9.0"
-mutmut = "^2.4.4"
+mutmut = "^2.4.5"
 pydocstyle = "^6.3.0"
-pyright = "^1.1.353"
+pyright = "^1.1.357"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 pytest-freezer = "^0.4.8"
-pytest-mock = "^3.12.0"
-requests-mock = "^1.11.0"
-tox = "^4.14.1"
-types-python-dateutil = "^2.8.19.20240311"
-types-requests = "^2.31.0.20240311"
+pytest-mock = "^3.14.0"
+requests-mock = "^1.12.1"
+tox = "^4.14.2"
+types-python-dateutil = "^2.9.0.20240316"
+types-requests = "^2.31.0.20240406"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.13"
+mkdocs-material = "^9.5.17"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mdx-include = "^1.4.2"
 
 [tool.ruff]
 exclude = [
     ".bzr",
     ".direnv",
```

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/__init__.py` & `tenduke_core-1.1.0/tenduke_core/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/auth_provider.py` & `tenduke_core-1.1.0/tenduke_core/auth/auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/device_auth_response.py` & `tenduke_core-1.1.0/tenduke_core/auth/device_auth_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/device_flow_client.py` & `tenduke_core-1.1.0/tenduke_core/auth/device_flow_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/oauth_client.py` & `tenduke_core-1.1.0/tenduke_core/auth/oauth_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/pkce_flow_client.py` & `tenduke_core-1.1.0/tenduke_core/auth/pkce_flow_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/token_response.py` & `tenduke_core-1.1.0/tenduke_core/auth/token_response.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/auth/user_info.py` & `tenduke_core-1.1.0/tenduke_core/auth/user_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/base_model.py` & `tenduke_core-1.1.0/tenduke_core/base_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/config/tenduke_config.py` & `tenduke_core-1.1.0/tenduke_core/config/tenduke_config.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/exceptions/api.py` & `tenduke_core-1.1.0/tenduke_core/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/exceptions/oauth.py` & `tenduke_core-1.1.0/tenduke_core/exceptions/oauth.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/exceptions/validation.py` & `tenduke_core-1.1.0/tenduke_core/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/tenduke_core/session_factory.py` & `tenduke_core-1.1.0/tenduke_core/session_factory.py`

 * *Files identical despite different names*

### Comparing `tenduke_core-1.0.0/PKG-INFO` & `tenduke_core-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tenduke_core
-Version: 1.0.0
+Version: 1.1.0
 Summary: Shared code supporting 10Duke SDKs
 Home-page: https://gitlab.com/10Duke/core/python-core
 License: MIT
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
-Requires-Dist: dataconf (>=2.5.0,<3.0.0)
+Requires-Dist: dataconf (>=3.1.0,<4.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.8.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: requests[security] (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://gitlab.com/10Duke/core/python-core
 Description-Content-Type: text/markdown
 
 # 10Duke Python core library
@@ -125,16 +125,18 @@
 
 That change shall be committed in a new revision.
 
 That revision shall be tagged (for example `git tag v1.1.1`).
 
 The new tag shall be pushed (`git push --tags`).
 
-That will trigger the creation of a new package and the publishing of that package to the relevant
-repository.
+That will trigger the creation of a new package and the publishing of that package to the GitLab
+package repository.
+
+[Publishing to PyPi](./docs/publishing.md) requires additional steps.
 
 ## Getting involved
 
 We welcome contributions! [Contributing](./CONTRIBUTING) explains what kind of contributions we
 welcome.
 
 ## Resources
```

