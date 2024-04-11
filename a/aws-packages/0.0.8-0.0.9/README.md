# Comparing `tmp/aws_packages-0.0.8.tar.gz` & `tmp/aws_packages-0.0.9.tar.gz`

## Comparing `aws_packages-0.0.8.tar` & `aws_packages-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,34 @@
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 aws_packages-0.0.8/Cargo.toml
--rw-r--r--   0     1001      127     2782 2024-04-07 00:01:26.000000 aws_packages-0.0.8/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      685 2024-04-07 00:01:26.000000 aws_packages-0.0.8/.gitignore
--rw-r--r--   0     1001      127     1067 2024-04-07 00:01:26.000000 aws_packages-0.0.8/LICENSE
--rw-r--r--   0     1001      127       59 2024-04-07 00:01:26.000000 aws_packages-0.0.8/Makefile
--rw-r--r--   0     1001      127       71 2024-04-07 00:01:26.000000 aws_packages-0.0.8/README.md
--rw-r--r--   0     1001      127       41 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/__init__.py
--rw-r--r--   0     1001      127       29 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/_aws_packages.pyi
--rw-r--r--   0     1001      127        0 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/__init__.py
--rw-r--r--   0     1001      127      912 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/auth_backend_base.py
--rw-r--r--   0     1001      127     2416 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/auth_backend_icp.py
--rw-r--r--   0     1001      127     1400 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/auth_backend_solana.py
--rw-r--r--   0     1001      127      157 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/exceptions.py
--rw-r--r--   0     1001      127     1501 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/middlewares.py
--rw-r--r--   0     1001      127      551 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/models.py
--rw-r--r--   0     1001      127      275 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/settings.py
--rw-r--r--   0     1001      127     1804 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/tokens.py
--rw-r--r--   0     1001      127     1398 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/auth/views.py
--rw-r--r--   0     1001      127     1698 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/dynamo.py
--rw-r--r--   0     1001      127        0 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/py.typed
--rw-r--r--   0     1001      127      380 2024-04-07 00:01:26.000000 aws_packages-0.0.8/aws_packages/time.py
--rw-r--r--   0     1001      127      374 2024-04-07 00:01:26.000000 aws_packages-0.0.8/pyproject.toml
--rw-r--r--   0     1001      127       52 2024-04-07 00:01:26.000000 aws_packages-0.0.8/requirements.txt
--rw-r--r--   0     1001      127      358 2024-04-07 00:01:26.000000 aws_packages-0.0.8/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-07 00:01:26.000000 aws_packages-0.0.8/tests/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 00:01:26.000000 aws_packages-0.0.8/tests/conftest.py
--rw-r--r--   0     1001      127      125 2024-04-07 00:01:26.000000 aws_packages-0.0.8/tests/test_init.py
--rw-r--r--   0     1001      127     7427 2024-04-07 00:01:30.000000 aws_packages-0.0.8/Cargo.lock
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 aws_packages-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 aws_packages-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      127     2782 2024-04-07 00:33:28.000000 aws_packages-0.0.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      685 2024-04-07 00:33:28.000000 aws_packages-0.0.9/.gitignore
+-rw-r--r--   0     1001      127     1067 2024-04-07 00:33:28.000000 aws_packages-0.0.9/LICENSE
+-rw-r--r--   0     1001      127       59 2024-04-07 00:33:28.000000 aws_packages-0.0.9/Makefile
+-rw-r--r--   0     1001      127       71 2024-04-07 00:33:28.000000 aws_packages-0.0.9/README.md
+-rw-r--r--   0     1001      127       41 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/__init__.py
+-rw-r--r--   0     1001      127       29 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/_aws_packages.pyi
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/__init__.py
+-rw-r--r--   0     1001      127      912 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/auth_backend_base.py
+-rw-r--r--   0     1001      127      157 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/exceptions.py
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/icp/__init__.py
+-rw-r--r--   0     1001      127     2214 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/icp/auth_backend.py
+-rw-r--r--   0     1001      127      974 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/icp/middlewares.py
+-rw-r--r--   0     1001      127      255 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/icp/views.py
+-rw-r--r--   0     1001      127      941 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/middlewares.py
+-rw-r--r--   0     1001      127      551 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/models.py
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/solana/__init__.py
+-rw-r--r--   0     1001      127     1386 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/solana/auth_backend.py
+-rw-r--r--   0     1001      127      986 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/solana/middlewares.py
+-rw-r--r--   0     1001      127      264 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/solana/views.py
+-rw-r--r--   0     1001      127     1820 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/tokens.py
+-rw-r--r--   0     1001      127     1000 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/auth/views.py
+-rw-r--r--   0     1001      127     1698 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/dynamo.py
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/py.typed
+-rw-r--r--   0     1001      127      380 2024-04-07 00:33:28.000000 aws_packages-0.0.9/aws_packages/time.py
+-rw-r--r--   0     1001      127      374 2024-04-07 00:33:28.000000 aws_packages-0.0.9/pyproject.toml
+-rw-r--r--   0     1001      127       52 2024-04-07 00:33:28.000000 aws_packages-0.0.9/requirements.txt
+-rw-r--r--   0     1001      127      358 2024-04-07 00:33:28.000000 aws_packages-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/tests/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-07 00:33:28.000000 aws_packages-0.0.9/tests/conftest.py
+-rw-r--r--   0     1001      127      125 2024-04-07 00:33:28.000000 aws_packages-0.0.9/tests/test_init.py
+-rw-r--r--   0     1001      127     7427 2024-04-07 00:33:45.000000 aws_packages-0.0.9/Cargo.lock
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 aws_packages-0.0.9/PKG-INFO
```

### Comparing `aws_packages-0.0.8/.github/workflows/CI.yml` & `aws_packages-0.0.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/.gitignore` & `aws_packages-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/LICENSE` & `aws_packages-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/aws_packages/auth/auth_backend_base.py` & `aws_packages-0.0.9/aws_packages/auth/auth_backend_base.py`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/aws_packages/auth/auth_backend_icp.py` & `aws_packages-0.0.9/aws_packages/auth/icp/auth_backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Authentication backends.
 
 """
 
-import json
 import os
-from http import HTTPStatus
 
-from aws_lambda_powertools.event_handler import Response, content_types
-from aws_lambda_powertools.event_handler.exceptions import BadRequestError
 from ic.agent import Agent
 from ic.candid import Types, encode
 from ic.client import Client
 from ic.identity import Identity
 
 from aws_packages.auth.auth_backend_base import AuthBackendBase
-from aws_packages.auth.models import AuthenticationRequest, LoginResponse, User
+from aws_packages.auth.models import AuthenticationRequest, User
 from aws_packages.auth.tokens import AccessToken
 
 
 class ICPAuthBackend(AuthBackendBase):
     """Authentication backend with ICP Canister"""
 
     def __init__(self, url: str, auth_canister: str, auth_function: str):
```

### Comparing `aws_packages-0.0.8/aws_packages/auth/auth_backend_solana.py` & `aws_packages-0.0.9/aws_packages/auth/solana/auth_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """Authentication backends.
 
 """
 
-import os
-
 from aws_packages.auth.auth_backend_base import AuthBackendBase
 from aws_packages.auth.models import AuthenticationRequest, User
 from aws_packages.auth.tokens import AccessToken
 
 
 class SolanaAuthBackend(AuthBackendBase):
     """Authentication backend with Solana Canister"""
@@ -34,15 +32,15 @@
 
 
 solana_auth_backend = SolanaAuthBackend(
     url="https://ic0.app",
 )
 
 if __name__ == "__main__":
-    icp_auth_backend = SolanaAuthBackend(
+    _auth_backend = SolanaAuthBackend(
         url="https://ic0.app",
     )
 
     request = AuthenticationRequest(
         user="4cay5-ew3bs-vr6yl-7iffu-67doc-l655v-dluy7-qplpx-7pkio-er5rt-uqe",
         authcode="",
     )
```

### Comparing `aws_packages-0.0.8/aws_packages/auth/middlewares.py` & `aws_packages-0.0.9/aws_packages/auth/icp/middlewares.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,26 @@
 """Auth middleware."""
 
 from aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response
 from aws_lambda_powertools.event_handler.exceptions import UnauthorizedError
 from aws_lambda_powertools.event_handler.middlewares import NextMiddleware
 
-from aws_packages.auth.auth_backend_icp import icp_auth_backend
+from aws_packages.auth.exceptions import JWTAuthError
+from aws_packages.auth.icp.auth_backend import icp_auth_backend
 from aws_packages.auth.models import AuthorizationRequest
 
-from .exceptions import JWTAuthError
-
 
 def icp_login_required(
     app: APIGatewayRestResolver, next_middleware: NextMiddleware
 ) -> Response:
     """Login required middleware
 
     :param app: application instance
     :param next_middleware: next middleware
     :return: Response object after the middleware has been applied
-    """
-
-    request = AuthorizationRequest(**app.current_event.headers)
-    try:
-        icp_auth_backend.authenticate_with_token(request.token)
-    except JWTAuthError:
-        raise UnauthorizedError(f"Unauthorized")
-    return next_middleware(app)
-
-
-def solana_login_required(
-    app: APIGatewayRestResolver, next_middleware: NextMiddleware
-) -> Response:
-    """Login required middleware
-
-    :param app: application instance
-    :param next_middleware: next middleware
-    :return: Response object after the middleware has been applied
     """
 
     request = AuthorizationRequest(**app.current_event.headers)
     try:
         icp_auth_backend.authenticate_with_token(request.token)
     except JWTAuthError:
         raise UnauthorizedError(f"Unauthorized")
```

### Comparing `aws_packages-0.0.8/aws_packages/auth/models.py` & `aws_packages-0.0.9/aws_packages/auth/models.py`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/aws_packages/auth/tokens.py` & `aws_packages-0.0.9/aws_packages/auth/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from datetime import timedelta
 
 import jwt
 from models import User
 
+from aws_packages.auth.exceptions import JWTAuthError
 from aws_packages.time import aware_utcnow, datetime_to_epoch
 
-from .exceptions import JWTAuthError
-
 DEFAULT_SECRET_KEY = "27d621e9bc55e6c659842904982abf06d89123c844e4d8bc62060ccd6536c360"
 SECRET_KEY = os.environ.get("SECRET_KEY", DEFAULT_SECRET_KEY)
 
 
 class Token:
     secret_key = SECRET_KEY
     lifetime = timedelta(minutes=5)
```

### Comparing `aws_packages-0.0.8/aws_packages/dynamo.py` & `aws_packages-0.0.9/aws_packages/dynamo.py`

 * *Files identical despite different names*

### Comparing `aws_packages-0.0.8/Cargo.lock` & `aws_packages-0.0.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "aws_packages"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
```

