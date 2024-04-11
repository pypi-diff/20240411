# Comparing `tmp/fastblocks-0.3.8.tar.gz` & `tmp/fastblocks-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.3.8.tar", last modified: Tue Apr  2 14:42:14 2024, max compression
+gzip compressed data, was "fastblocks-0.3.9.tar", last modified: Thu Apr 11 14:55:14 2024, max compression
```

## Comparing `fastblocks-0.3.8.tar` & `fastblocks-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.3.8/LICENSE
--rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.3.8/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.3.8/fastblocks/Dockerfile
--rw-r--r--   0        0        0      149 2024-02-08 11:06:00.249936 fastblocks-0.3.8/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.3.8/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.3.8/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.3.8/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.3.8/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.3.8/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0       96 2024-02-05 00:13:09.758290 fastblocks-0.3.8/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     2988 2024-02-09 12:51:23.096080 fastblocks-0.3.8/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.3.8/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.3.8/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2669 2024-03-31 09:28:05.032996 fastblocks-0.3.8/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.3.8/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     1682 2024-02-08 21:44:35.522977 fastblocks-0.3.8/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.3.8/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.3.8/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      222 2024-02-05 00:13:09.776789 fastblocks-0.3.8/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.3.8/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.3.8/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.3.8/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.3.8/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.3.8/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.3.8/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.3.8/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.3.8/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.3.8/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14759 2024-03-04 14:04:06.525893 fastblocks-0.3.8/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3848 2024-03-29 16:08:40.512632 fastblocks-0.3.8/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.3.8/fastblocks/middleware.py
--rw-r--r--   0        0        0     3052 2024-04-02 14:42:14.906140 fastblocks-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.3.9/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.3.9/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.3.9/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.3.9/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.3.9/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.3.9/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.3.9/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.3.9/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0       96 2024-02-05 00:13:09.758290 fastblocks-0.3.9/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     2988 2024-02-09 12:51:23.096080 fastblocks-0.3.9/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.3.9/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.3.9/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2669 2024-03-31 09:28:05.032996 fastblocks-0.3.9/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.3.9/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     1977 2024-04-11 14:20:14.024549 fastblocks-0.3.9/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.3.9/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.3.9/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-05 00:13:09.776789 fastblocks-0.3.9/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.3.9/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.3.9/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.3.9/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.3.9/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.3.9/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.3.9/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.3.9/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.3.9/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.3.9/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14759 2024-03-04 14:04:06.525893 fastblocks-0.3.9/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.3.9/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.3.9/fastblocks/middleware.py
+-rw-r--r--   0        0        0     3052 2024-04-11 14:55:14.493559 fastblocks-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.3.9/PKG-INFO
```

### Comparing `fastblocks-0.3.8/LICENSE` & `fastblocks-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/README.md` & `fastblocks-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.3.9/fastblocks/adapters/admin/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/app/main.py` & `fastblocks-0.3.9/fastblocks/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/auth/_base.py` & `fastblocks-0.3.9/fastblocks/adapters/auth/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import typing as t
 from abc import ABC
 from abc import abstractmethod
+from contextvars import ContextVar
 
 from acb.config import AppSettings
-
 from asgi_htmx import HtmxRequest
 from pydantic import EmailStr
 from pydantic import SecretStr
 from pydantic import UUID4
+from starlette.authentication import UnauthenticatedUser
 
 
 class AuthBaseSettings(AppSettings):
     token_id: t.Optional[str] = None
     session_cookie: t.Optional[str] = None
 
 
 class AuthBase(ABC):
+    _current_user: ContextVar[t.Any] = ContextVar(
+        "current_user", default=UnauthenticatedUser()
+    )
+
+    @property
+    def current_user(self) -> t.Any:
+        return self._current_user.get()
+
     @staticmethod
     @abstractmethod
     async def authenticate(request: HtmxRequest) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def __init__(self, secret_key: SecretStr, user_model: t.Any) -> None:
```

### Comparing `fastblocks-0.3.8/fastblocks/adapters/fonts/google.py` & `fastblocks-0.3.9/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.3.9/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/style/_base.py` & `fastblocks-0.3.9/fastblocks/adapters/style/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.3.9/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.3.9/fastblocks/adapters/templates/jinja2.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/fastblocks/applications.py` & `fastblocks-0.3.9/fastblocks/applications.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 import logging
 import typing as t
-from contextvars import ContextVar
 from platform import system
 
 from acb.adapters import import_adapter
 from acb.adapters import register_adapters
 from acb.adapters.logger.loguru import InterceptHandler
 from acb.config import Config
 from acb.depends import depends
 from asgi_htmx import HtmxRequest
 from starception import add_link_template
 from starception import install_error_handler
 from starception import set_editor
 from starlette.applications import Starlette
-from starlette.authentication import UnauthenticatedUser
 from starlette.middleware import Middleware
 from starlette.middleware.errors import ServerErrorMiddleware
 from starlette.middleware.exceptions import ExceptionMiddleware
 from starlette.responses import Response
 from starlette.types import ASGIApp
 from starlette.types import ExceptionHandler
 from starlette.types import Lifespan
 from .middleware import middlewares
 
 register_adapters()
 
 Logger = import_adapter()
 
-_current_user: ContextVar[t.Any] = ContextVar(
-    "current_user", default=UnauthenticatedUser()
-)
-
-
-def current_user() -> t.Any:
-    return _current_user.get()
-
-
 AppType = t.TypeVar("AppType", bound="FastBlocks")
 
 match system():
     case "Windows":
         add_link_template("pycharm", "pycharm64.exe --line {lineno} {path}")
     case "Darwin":
         add_link_template("pycharm", "pycharm --line {lineno} {path}")
```

### Comparing `fastblocks-0.3.8/fastblocks/middleware.py` & `fastblocks-0.3.9/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.8/pyproject.toml` & `fastblocks-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.3.8"
+version = "0.3.9"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -107,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "pdm",
     "autotyping",
+    "pyfiglet",
     "pdm-bump",
-    "pre-commit",
-    "aiohttp",
-    "pdm",
+    "phonenumbers",
     "libsass",
+    "aiohttp",
     "pytest",
-    "pyfiglet",
-    "phonenumbers",
+    "pre-commit",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
+    "B603",
+    "B403",
     "B113",
     "B404",
-    "B403",
-    "B603",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.3.8/PKG-INFO` & `fastblocks-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.3.8
+Version: 0.3.9
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
 Keywords: starlette htmx jinja httpx fastapi sqladmin sqlmodel pydantic sqlalchemy redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
```

