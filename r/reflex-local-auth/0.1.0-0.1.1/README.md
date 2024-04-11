# Comparing `tmp/reflex-local-auth-0.1.0.tar.gz` & `tmp/reflex-local-auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-local-auth-0.1.0.tar", last modified: Wed Apr 10 20:45:55 2024, max compression
+gzip compressed data, was "reflex-local-auth-0.1.1.tar", last modified: Thu Apr 11 12:42:37 2024, max compression
```

## Comparing `reflex-local-auth-0.1.0.tar` & `reflex-local-auth-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/auth_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/local_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:37.009576 reflex-local-auth-0.1.1/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/auth_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/local_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-11 12:42:37.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 12:42:37.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:42:37.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 12:42:37.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 12:42:37.000000 reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-11 12:42:00.000000 reflex-local-auth-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:42:37.013576 reflex-local-auth-0.1.1/setup.cfg
```

### Comparing `reflex-local-auth-0.1.0/PKG-INFO` & `reflex-local-auth-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-local-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Local DB user authentication for Reflex apps
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
```

### Comparing `reflex-local-auth-0.1.0/README.md` & `reflex-local-auth-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/auth_session.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/auth_session.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/local_auth.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/local_auth.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/login.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def redir(self) -> rx.event.EventSpec | None:
         """Redirect to the redirect_to route if logged in, or to the login page if not."""
         if not self.is_hydrated:
             # wait until after hydration to ensure auth_token is known
             return LoginState.redir()  # type: ignore
         page = self.router.page.path
         if not self.is_authenticated and page != routes.LOGIN_ROUTE:
-            self.redirect_to = page
+            self.redirect_to = self.router.page.raw_path
             return rx.redirect(routes.LOGIN_ROUTE)
         elif page == routes.LOGIN_ROUTE:
             return rx.redirect(self.redirect_to or "/")
 
 
 def require_login(page: rx.app.ComponentCallable) -> rx.app.ComponentCallable:
     """Decorator to require authentication before rendering a page.
```

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/login.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/login.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/registration.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/pages/registration.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/registration.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/registration.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/user.py` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth/user.py`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/PKG-INFO` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-local-auth
-Version: 0.1.0
+Version: 0.1.1
 Summary: Local DB user authentication for Reflex apps
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
```

### Comparing `reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt` & `reflex-local-auth-0.1.1/custom_components/reflex_local_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex-local-auth-0.1.0/pyproject.toml` & `reflex-local-auth-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-local-auth"
-version = "0.1.0"
+version = "0.1.1"
 description = "Local DB user authentication for Reflex apps"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
```

