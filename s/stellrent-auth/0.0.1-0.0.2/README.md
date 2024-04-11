# Comparing `tmp/stellrent-auth-0.0.1.tar.gz` & `tmp/stellrent-auth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellrent-auth-0.0.1.tar", last modified: Wed Apr 10 14:42:19 2024, max compression
+gzip compressed data, was "stellrent-auth-0.0.2.tar", last modified: Thu Apr 11 17:35:38 2024, max compression
```

## Comparing `stellrent-auth-0.0.1.tar` & `stellrent-auth-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-04-10 14:42:19.000863 stellrent-auth-0.0.1/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     1066 2024-03-27 14:56:00.000000 stellrent-auth-0.0.1/LICENSE
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      156 2024-04-09 11:37:31.000000 stellrent-auth-0.0.1/MANIFEST.in
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      813 2024-04-10 14:42:19.001720 stellrent-auth-0.0.1/PKG-INFO
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       34 2024-03-27 14:56:00.000000 stellrent-auth-0.0.1/README.md
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      886 2024-04-10 14:41:57.000000 stellrent-auth-0.0.1/pyproject.toml
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       73 2024-04-10 14:42:19.006735 stellrent-auth-0.0.1/setup.cfg
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     1034 2024-04-10 14:38:47.000000 stellrent-auth-0.0.1/setup.py
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-04-10 14:42:18.858111 stellrent-auth-0.0.1/stellrent_auth/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       21 2024-04-10 14:36:15.000000 stellrent-auth-0.0.1/stellrent_auth/__init__.py
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     7744 2024-04-10 14:28:33.000000 stellrent-auth-0.0.1/stellrent_auth/auth.py
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-04-10 14:42:18.959661 stellrent-auth-0.0.1/stellrent_auth.egg-info/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      813 2024-04-10 14:42:16.000000 stellrent-auth-0.0.1/stellrent_auth.egg-info/PKG-INFO
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      338 2024-04-10 14:42:17.000000 stellrent-auth-0.0.1/stellrent_auth.egg-info/SOURCES.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)        1 2024-04-10 14:42:16.000000 stellrent-auth-0.0.1/stellrent_auth.egg-info/dependency_links.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      105 2024-04-10 14:42:16.000000 stellrent-auth-0.0.1/stellrent_auth.egg-info/requires.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       15 2024-04-10 14:42:16.000000 stellrent-auth-0.0.1/stellrent_auth.egg-info/top_level.txt
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-04-10 14:42:18.979862 stellrent-auth-0.0.1/tests/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      107 2024-04-10 14:24:56.000000 stellrent-auth-0.0.1/tests/test_environment_variables.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     1066 2024-04-11 13:50:40.000000 stellrent-auth-0.0.2/LICENSE
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      156 2024-04-11 13:50:40.000000 stellrent-auth-0.0.2/MANIFEST.in
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      813 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/PKG-INFO
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       34 2024-04-11 13:50:41.000000 stellrent-auth-0.0.2/README.md
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      885 2024-04-11 15:17:55.000000 stellrent-auth-0.0.2/pyproject.toml
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       73 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/setup.cfg
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      993 2024-04-11 17:35:15.000000 stellrent-auth-0.0.2/setup.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/stellrent_auth/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:34:47.000000 stellrent-auth-0.0.2/stellrent_auth/__init__.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     7911 2024-04-11 16:26:29.000000 stellrent-auth-0.0.2/stellrent_auth/auth.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/stellrent_auth.egg-info/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      813 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      338 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      103 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/requires.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       15 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/top_level.txt
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/tests/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      287 2024-04-11 16:26:49.000000 stellrent-auth-0.0.2/tests/test_environment_variables.py
```

### Comparing `stellrent-auth-0.0.1/LICENSE` & `stellrent-auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stellrent-auth-0.0.1/PKG-INFO` & `stellrent-auth-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellrent-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: OAUTH2 and OpenID standards
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-auth
 Project-URL: Issues, https://github.com/stellrent/stellrent-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stellrent-auth-0.0.1/pyproject.toml` & `stellrent-auth-0.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "stellrent-auth"
+dynamic = ["version", "description"]
 authors = [
   { name="Marcus Rodrigues Magalhães", email="marcusrodrigues.magalhaes@stellantis.com" },
 ]
-dynamic = ["version", "description"]
 readme = "README.md"
 # license = 'MIT'
 requires-python = '>=3.7'
 classifiers = [
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.11',
@@ -24,8 +24,8 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/stellrent/stellrent-auth"
-Issues = "https://github.com/stellrent/stellrent-auth/issues"
+Issues = "https://github.com/stellrent/stellrent-auth/issues"
```

### Comparing `stellrent-auth-0.0.1/setup.py` & `stellrent-auth-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 # step 1: python setup.py sdist bdist_wheel
 # step 2: twine upload dist/* --verbose
 # https://medium.com/the-research-nest/how-to-publish-your-python-code-as-a-pip-package-in-5-simple-steps-3b36286293ec
 from setuptools import setup
-import stellrent_auth
 
 with open('requirements.txt') as requirements_file:
     REQUIRED_MODULES = [line.strip() for line in requirements_file]
 
 with open('requirements-dev.txt') as requirements_dev_file:
     REQUIRED_DEV_MODULES = [line.strip() for line in requirements_dev_file]
 
 def readme():
     with open('README.md') as readme_file:
         return readme_file.read()
     
 setup(
     name='stellrent-auth',
-    version=stellrent_auth.__version__,
+    version="0.0.2",
     author='Marcus R. Magalhães',
     author_email='marcusrodrigues.magalhaes@stellantis.com',
     description='OAUTH2 and OpenID standards',
     packages=['stellrent_auth'],
     include_package_data=True,
     long_description=readme(),
     long_description_content_type='text/markdown',
```

### Comparing `stellrent-auth-0.0.1/stellrent_auth/auth.py` & `stellrent-auth-0.0.2/stellrent_auth/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import jwt
 import requests
 import logging
-
+from functools import wraps
 from requests_oauthlib import OAuth2Session
+from flask import request
 
 # https://oauthlib.readthedocs.io/en/latest/index.html
 from oauthlib.oauth2 import BackendApplicationClient
 from oauthlib.oauth2.rfc6749.errors import OAuth2Error
 from stellrent_response.json_response import Unauthorized, Forbidden
 
 client_token = None
@@ -156,36 +157,36 @@
                 "verify_iat": True,
                 "verify_aud": True,
                 "verify_iss": True,
             }
         )
         return token_data
 
-# https://github.com/curityio/flask-of-oil
-def grant_required(require_grants=[]):
-    def inner_decorator(function):
-        @wraps(function)
-        def wrapper(*args, **kwargs):
-            if "Authorization" not in request.headers:
-                return Unauthorized("Access to this resource requires Authorization header parameter").make_response()
-            valid_token = auth.validate_bearer_token(request.headers['Authorization'])
-            
-            if valid_token:
-
-                if require_grants is not None and len(require_grants) > 0:
-                    
-                    user_grants = auth.user_grants_from_token(request.headers['Authorization'])
-                    set_require_grants = set(require_grants)
-                    set_user_grants = set(user_grants)
-                    user_has_grant = set_user_grants.intersection(set_require_grants)
-                    if len(user_has_grant) > 0 :
-                        return function(*args, **kwargs)
-                    else:
-                        logging.getLogger().debug("Endpoint Grant required: " + str(require_grants))
-                        logging.getLogger().debug("User Grant: " + str(user_grants))
-                        return Forbidden('You do not have permission to access this resource').make_response()
-
-                return function(*args, **kwargs)
-            return Unauthorized("Invalid Token").make_response()
-        wrapper.__name__ = function.__name__
-        return wrapper
-    return inner_decorator
+    # https://github.com/curityio/flask-of-oil
+    def grant_required(self, require_grants=[]):
+        def inner_decorator(function):
+            @wraps(function)
+            def wrapper(*args, **kwargs):
+                if "Authorization" not in request.headers:
+                    return Unauthorized("Access to this resource requires Authorization header parameter").make_response()
+                valid_token = self.validate_bearer_token(request.headers['Authorization'])
+                
+                if valid_token:
+
+                    if require_grants is not None and len(require_grants) > 0:
+                        
+                        user_grants = self.user_grants_from_token(request.headers['Authorization'])
+                        set_require_grants = set(require_grants)
+                        set_user_grants = set(user_grants)
+                        user_has_grant = set_user_grants.intersection(set_require_grants)
+                        if len(user_has_grant) > 0 :
+                            return function(*args, **kwargs)
+                        else:
+                            logging.getLogger().debug("Endpoint Grant required: " + str(require_grants))
+                            logging.getLogger().debug("User Grant: " + str(user_grants))
+                            return Forbidden('You do not have permission to access this resource').make_response()
+
+                    return function(*args, **kwargs)
+                return Unauthorized("Invalid Token").make_response()
+            wrapper.__name__ = function.__name__
+            return wrapper
+        return inner_decorator
```

### Comparing `stellrent-auth-0.0.1/stellrent_auth.egg-info/PKG-INFO` & `stellrent-auth-0.0.2/stellrent_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellrent-auth
-Version: 0.0.1
+Version: 0.0.2
 Summary: OAUTH2 and OpenID standards
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-auth
 Project-URL: Issues, https://github.com/stellrent/stellrent-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

