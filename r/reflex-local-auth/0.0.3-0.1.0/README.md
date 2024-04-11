# Comparing `tmp/reflex-local-auth-0.0.3.tar.gz` & `tmp/reflex-local-auth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-local-auth-0.0.3.tar", last modified: Fri Mar 22 12:21:49 2024, max compression
+gzip compressed data, was "reflex-local-auth-0.1.0.tar", last modified: Wed Apr 10 20:45:55 2024, max compression
```

## Comparing `reflex-local-auth-0.0.3.tar` & `reflex-local-auth-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-22 12:21:49.007010 reflex-local-auth-0.0.3/
--rw-r--r--   0 masen      (502) staff       (20)     7322 2024-03-22 12:21:49.006786 reflex-local-auth-0.0.3/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)     6789 2024-03-22 12:09:53.000000 reflex-local-auth-0.0.3/README.md
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-22 12:21:49.002662 reflex-local-auth-0.0.3/custom_components/
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-22 12:21:49.004634 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/
--rw-r--r--   0 masen      (502) staff       (20)      437 2024-03-22 12:09:53.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)      507 2024-03-22 12:09:53.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/auth_session.py
--rw-r--r--   0 masen      (502) staff       (20)     3297 2024-03-22 12:15:18.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/local_auth.py
--rw-r--r--   0 masen      (502) staff       (20)     2884 2024-03-22 12:15:18.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/login.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-22 12:21:49.006195 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/
--rw-r--r--   0 masen      (502) staff       (20)      152 2024-03-22 12:09:53.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)      398 2024-03-22 12:09:53.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/components.py
--rw-r--r--   0 masen      (502) staff       (20)     1587 2024-03-22 12:11:09.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/login.py
--rw-r--r--   0 masen      (502) staff       (20)     1848 2024-03-22 12:11:09.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/registration.py
--rw-r--r--   0 masen      (502) staff       (20)     3233 2024-03-22 12:11:09.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/registration.py
--rw-r--r--   0 masen      (502) staff       (20)      481 2024-03-22 12:15:18.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/routes.py
--rw-r--r--   0 masen      (502) staff       (20)     1355 2024-03-22 12:15:18.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth/user.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-22 12:21:49.006431 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/
--rw-r--r--   0 masen      (502) staff       (20)     7322 2024-03-22 12:21:48.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)      874 2024-03-22 12:21:49.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/SOURCES.txt
--rw-r--r--   0 masen      (502) staff       (20)        1 2024-03-22 12:21:48.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/dependency_links.txt
--rw-r--r--   0 masen      (502) staff       (20)       40 2024-03-22 12:21:49.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/requires.txt
--rw-r--r--   0 masen      (502) staff       (20)       18 2024-03-22 12:21:49.000000 reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/top_level.txt
--rw-r--r--   0 masen      (502) staff       (20)      718 2024-03-22 12:20:55.000000 reflex-local-auth-0.0.3/pyproject.toml
--rw-r--r--   0 masen      (502) staff       (20)       38 2024-03-22 12:21:49.007049 reflex-local-auth-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/auth_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/local_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 20:45:55.000000 reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 20:45:17.000000 reflex-local-auth-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:45:55.041686 reflex-local-auth-0.1.0/setup.cfg
```

### Comparing `reflex-local-auth-0.0.3/PKG-INFO` & `reflex-local-auth-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: reflex-local-auth
-Version: 0.0.3
-Summary: Reflex custom component local-auth
-Author-email: Masen Furer <m_github@0x26.net>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
-Keywords: reflex,reflex-custom-components
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
-Requires-Dist: bcrypt
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
 # local-auth
 
 Easy access to local authentication in your [Reflex](https://reflex.dev) app.
 
 ## Installation
 
 ```bash
@@ -103,15 +86,15 @@
 @reflex_local_auth.require_login
 def protected_page():
     return rx.heading(ProtectedState.data)
 ```
 
 ## Customization
 
-The basic `reflex_local_auth.User` model provides password hashing and
+The basic `reflex_local_auth.LocalUser` model provides password hashing and
 verification, and an enabled flag. Additional functionality can be added by
 creating a new `UserInfo` model and creating a foreign key relationship to the
 `user.id` field.
 
 ```python
 import sqlmodel
 import reflex as rx
@@ -159,15 +142,15 @@
 
 def register_error() -> rx.Component:
     """Render the registration error message."""
     return rx.cond(
         reflex_local_auth.RegistrationState.error_message != "",
         rx.callout(
             reflex_local_auth.RegistrationState.error_message,
-            icon="alert_triangle",
+            icon="triangle_alert",
             color_scheme="red",
             role="alert",
             width="100%",
         ),
     )
 
 
@@ -248,7 +231,24 @@
             rx.fragment(
                 rx.text(f"Email: {MyLocalAuthState.authenticated_user_info.email}"),
                 rx.text(f"Account Created From: {MyLocalAuthState.authenticated_user_info.created_from_ip}"),
             ),
         ),
     )
 ```
+
+## Migrating from 0.0.x to 0.1.x
+
+The `User` model has been renamed to `LocalUser` and the `AuthSession` model has
+been renamed to `LocalAuthSession`. If your app was using reflex-local-auth 0.0.x,
+then you will need to make manual changes to migration script to copy existing user
+data into the new tables _after_ running `reflex db makemigrations`.
+
+See [`local_auth_demo/alembic/version/cb01e050df85_.py`](local_auth_demo/alembic/version/cb01e050df85_.py) for an example migration script.
+
+Importantly, your `upgrade` function should include the following lines, after creating
+the new tables and before dropping the old tables:
+
+```python
+    op.execute("INSERT INTO localuser SELECT * FROM user;")
+    op.execute("INSERT INTO localauthsession SELECT * FROM authsession;")
+```
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/local_auth.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/local_auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,89 +8,89 @@
 
 import datetime
 
 from sqlmodel import select
 
 import reflex as rx
 
-from .auth_session import AuthSession
-from .user import User
+from .auth_session import LocalAuthSession
+from .user import LocalUser
 
 
 AUTH_TOKEN_LOCAL_STORAGE_KEY = "_auth_token"
 DEFAULT_AUTH_SESSION_EXPIRATION_DELTA = datetime.timedelta(days=7)
 
 
 class LocalAuthState(rx.State):
     # The auth_token is stored in local storage to persist across tab and browser sessions.
     auth_token: str = rx.LocalStorage(name=AUTH_TOKEN_LOCAL_STORAGE_KEY)
 
     @rx.cached_var
-    def authenticated_user(self) -> User:
+    def authenticated_user(self) -> LocalUser:
         """The currently authenticated user, or a dummy user if not authenticated.
 
         Returns:
-            A User instance with id=-1 if not authenticated, or the User instance
+            A LocalUser instance with id=-1 if not authenticated, or the LocalUser instance
             corresponding to the currently authenticated user.
         """
         with rx.session() as session:
             result = session.exec(
-                select(User, AuthSession).where(
-                    AuthSession.session_id == self.auth_token,
-                    AuthSession.expiration
+                select(LocalUser, LocalAuthSession).where(
+                    LocalAuthSession.session_id == self.auth_token,
+                    LocalAuthSession.expiration
                     >= datetime.datetime.now(datetime.timezone.utc),
-                    User.id == AuthSession.user_id,
+                    LocalUser.id == LocalAuthSession.user_id,
                 ),
             ).first()
             if result:
                 user, session = result
                 return user
-        return User(id=-1)  # type: ignore
+        return LocalUser(id=-1)  # type: ignore
 
     @rx.cached_var
     def is_authenticated(self) -> bool:
         """Whether the current user is authenticated.
 
         Returns:
             True if the authenticated user has a positive user ID, False otherwise.
         """
         return self.authenticated_user.id >= 0
 
     def do_logout(self) -> None:
-        """Destroy AuthSessions associated with the auth_token."""
+        """Destroy LocalAuthSessions associated with the auth_token."""
         with rx.session() as session:
             for auth_session in session.exec(
-                select(AuthSession).where(AuthSession.session_id == self.auth_token)
+                select(LocalAuthSession).where(LocalAuthSession.session_id == self.auth_token)
             ).all():
                 session.delete(auth_session)
             session.commit()
         self.auth_token = self.auth_token
 
     def _login(
         self,
         user_id: int,
         expiration_delta: datetime.timedelta = DEFAULT_AUTH_SESSION_EXPIRATION_DELTA,
     ) -> None:
-        """Create an AuthSession for the given user_id.
+        """Create an LocalAuthSession for the given user_id.
 
-        If the auth_token is already associated with an AuthSession, it will be
+        If the auth_token is already associated with an LocalAuthSession, it will be
         logged out first.
 
         Args:
-            user_id: The user ID to associate with the AuthSession.
-            expiration_delta: The amount of time before the AuthSession expires.
+            user_id: The user ID to associate with the LocalAuthSession.
+            expiration_delta: The amount of time before the LocalAuthSession expires.
         """
         if self.is_authenticated:
             self.do_logout()
         if user_id < 0:
             return
         self.auth_token = self.auth_token or self.router.session.client_token
         with rx.session() as session:
             session.add(
-                AuthSession(  # type: ignore
+                LocalAuthSession(  # type: ignore
                     user_id=user_id,
                     session_id=self.auth_token,
                     expiration=datetime.datetime.now(datetime.timezone.utc)
                     + expiration_delta,
                 )
             )
             session.commit()
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/login.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import reflex as rx
 from sqlmodel import select
 
 from . import routes
 from .local_auth import LocalAuthState
-from .user import User
+from .user import LocalUser
 
 
 class LoginState(LocalAuthState):
     """Handle login form submission and redirect to proper routes after authentication."""
 
     error_message: str = ""
     redirect_to: str = ""
@@ -22,15 +22,15 @@
             form_data: A dict of form fields and values.
         """
         self.error_message = ""
         username = form_data["username"]
         password = form_data["password"]
         with rx.session() as session:
             user = session.exec(
-                select(User).where(User.username == username)
+                select(LocalUser).where(LocalUser.username == username)
             ).one_or_none()
         if user is not None and not user.enabled:
             self.error_message = "This account is disabled."
             return rx.set_value("password", "")
         if (
             user is not None
             and user.id is not None
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/login.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/login.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def login_error() -> rx.Component:
     """Render the login error message."""
     return rx.cond(
         LoginState.error_message != "",
         rx.callout(
             LoginState.error_message,
-            icon="alert_triangle",
+            icon="triangle_alert",
             color_scheme="red",
             role="alert",
             width="100%",
         ),
     )
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/pages/registration.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/pages/registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def register_error() -> rx.Component:
     """Render the registration error message."""
     return rx.cond(
         RegistrationState.error_message != "",
         rx.callout(
             RegistrationState.error_message,
-            icon="alert_triangle",
+            icon="triangle_alert",
             color_scheme="red",
             role="alert",
             width="100%",
         ),
     )
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/registration.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import reflex as rx
 
 from sqlmodel import select
 
 from . import routes
 from .local_auth import LocalAuthState
-from .user import User
+from .user import LocalUser
 
 
 POST_REGISTRATION_DELAY = 0.5
 
 
 class RegistrationState(LocalAuthState):
     """Handle registration form submission and redirect to login page after registration."""
@@ -26,15 +26,15 @@
         self, username, password, confirm_password
     ) -> rx.event.EventSpec | list[rx.event.EventSpec] | None:
         if not username:
             self.error_message = "Username cannot be empty"
             return rx.set_focus("username")
         with rx.session() as session:
             existing_user = session.exec(
-                select(User).where(User.username == username)
+                select(LocalUser).where(LocalUser.username == username)
             ).one_or_none()
         if existing_user is not None:
             self.error_message = (
                 f"Username {username} is already registered. Try a different name"
             )
             return [rx.set_value("username", ""), rx.set_focus("username")]
         if not password:
@@ -46,17 +46,17 @@
                 rx.set_value("confirm_password", ""),
                 rx.set_focus("confirm_password"),
             ]
 
     def _register_user(self, username, password) -> None:
         with rx.session() as session:
             # Create the new user and add it to the database.
-            new_user = User()  # type: ignore
+            new_user = LocalUser()  # type: ignore
             new_user.username = username
-            new_user.password_hash = User.hash_password(password)
+            new_user.password_hash = LocalUser.hash_password(password)
             new_user.enabled = True
             session.add(new_user)
             session.commit()
             session.refresh(new_user)
             self.new_user_id = new_user.id
 
     def handle_registration(
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth/user.py` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import bcrypt
 from sqlmodel import Field
 
 import reflex as rx
 
 
-class User(
+class LocalUser(
     rx.Model,
     table=True,  # type: ignore
 ):
     """A local User model with bcrypt password hashing."""
 
     username: str = Field(unique=True, nullable=False, index=True)
     password_hash: bytes = Field(nullable=False)
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/PKG-INFO` & `reflex-local-auth-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: reflex-local-auth
-Version: 0.0.3
-Summary: Reflex custom component local-auth
+Version: 0.1.0
+Summary: Local DB user authentication for Reflex apps
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-local-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -103,15 +103,15 @@
 @reflex_local_auth.require_login
 def protected_page():
     return rx.heading(ProtectedState.data)
 ```
 
 ## Customization
 
-The basic `reflex_local_auth.User` model provides password hashing and
+The basic `reflex_local_auth.LocalUser` model provides password hashing and
 verification, and an enabled flag. Additional functionality can be added by
 creating a new `UserInfo` model and creating a foreign key relationship to the
 `user.id` field.
 
 ```python
 import sqlmodel
 import reflex as rx
@@ -159,15 +159,15 @@
 
 def register_error() -> rx.Component:
     """Render the registration error message."""
     return rx.cond(
         reflex_local_auth.RegistrationState.error_message != "",
         rx.callout(
             reflex_local_auth.RegistrationState.error_message,
-            icon="alert_triangle",
+            icon="triangle_alert",
             color_scheme="red",
             role="alert",
             width="100%",
         ),
     )
 
 
@@ -248,7 +248,24 @@
             rx.fragment(
                 rx.text(f"Email: {MyLocalAuthState.authenticated_user_info.email}"),
                 rx.text(f"Account Created From: {MyLocalAuthState.authenticated_user_info.created_from_ip}"),
             ),
         ),
     )
 ```
+
+## Migrating from 0.0.x to 0.1.x
+
+The `User` model has been renamed to `LocalUser` and the `AuthSession` model has
+been renamed to `LocalAuthSession`. If your app was using reflex-local-auth 0.0.x,
+then you will need to make manual changes to migration script to copy existing user
+data into the new tables _after_ running `reflex db makemigrations`.
+
+See [`local_auth_demo/alembic/version/cb01e050df85_.py`](local_auth_demo/alembic/version/cb01e050df85_.py) for an example migration script.
+
+Importantly, your `upgrade` function should include the following lines, after creating
+the new tables and before dropping the old tables:
+
+```python
+    op.execute("INSERT INTO localuser SELECT * FROM user;")
+    op.execute("INSERT INTO localauthsession SELECT * FROM authsession;")
+```
```

### Comparing `reflex-local-auth-0.0.3/custom_components/reflex_local_auth.egg-info/SOURCES.txt` & `reflex-local-auth-0.1.0/custom_components/reflex_local_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

