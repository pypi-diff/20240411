# Comparing `tmp/stcog-0.0.6.tar.gz` & `tmp/stcog-0.0.7.tar.gz`

## Comparing `stcog-0.0.6.tar` & `stcog-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/__init__.py
--rw-r--r--   0        0        0    24906 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/auth.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/exceptions.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/session_provider.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.6/src/stcog/utils.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.6/tests/example.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.6/tests/example_hosted.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.6/LICENSE
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.6/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.7/src/stcog/__init__.py
+-rw-r--r--   0        0        0    24411 2020-02-02 00:00:00.000000 stcog-0.0.7/src/stcog/auth.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.7/src/stcog/exceptions.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.7/src/stcog/session_provider.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.7/src/stcog/utils.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.7/tests/example.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.7/tests/example_hosted.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.7/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.7/PKG-INFO
```

### Comparing `stcog-0.0.6/src/stcog/auth.py` & `stcog-0.0.7/src/stcog/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,23 +78,14 @@
         st.session_state["auth_token_type"] = ""
 
     def load_credentials(self) -> Optional[Credentials]:
         """Loads the credentials from streamlit session state.
 
         Returns None if no credentials were found."""
         try:
-        
-            try:
-                auth_id_token
-            except NameError:
-                print("well, auth_id_token WASN'T defined after all!")
-                auth_id_token = ""
-            else:
-                print("sure, auth_id_token was defined.")
-    
             return Credentials(
                 id_token=st.session_state["auth_id_token"],
                 access_token=st.session_state["auth_access_token"],
                 refresh_token=st.session_state["auth_refresh_token"],
                 expires_in=st.session_state["auth_expires_in"],
                 token_type=st.session_state["auth_token_type"],
             )
@@ -138,15 +129,14 @@
         """Clears the password reset session from streamlit session state/"""
         st.session_state["auth_reset_password_session"] = ""
         st.session_state["auth_reset_password_username"] = ""
         st.session_state["auth_reset_password_password"] = ""
 
     def is_reset_password_session(self) -> bool:
         """Returns if password reset session is set in streamlit session state."""
-        st.session_state["auth_reset_password_session"] = ""
         return bool(st.session_state["auth_reset_password_session"])
 
     def reset_password_credentials(self) -> Tuple[Optional[str], Optional[str]]:
         """Returns the password reset username and password saved in streamlit session state."""
         username = st.session_state["auth_reset_password_username"] or None
         password = st.session_state["auth_reset_password_password"] or None
         return (username, password)
@@ -346,48 +336,44 @@
         return self.session_manager.load_credentials()
 
 class CognitoAuthenticator(CognitoAuthenticatorBase):
     """Authenticates the user with Cognito using custom streamlit UI elements."""
 
     def _show_login_form(self, placeholder):
         with placeholder:
-            cols = st.columns([1, 3, 1])
-            with cols[1]:
-                with st.form("login_form"):
-                    st.subheader("Login")
-                    username = st.text_input("Username")
-                    password = st.text_input("Password", type="password")
-                    login_submitted = st.form_submit_button("Login")
-                    status_container = st.container()
+            with st.form("login_form"):
+              st.subheader("Login")
+              username = st.text_input("Username")
+              password = st.text_input("Password", type="password")
+              login_submitted = st.form_submit_button("Login")
+              status_container = st.container()
 
         return login_submitted, username, password, status_container
 
     def _show_password_reset_form(self, placeholder):
         username, password = self.session_manager.reset_password_credentials()
         with placeholder:
-            cols = st.columns([1, 3, 1])
-            with cols[1]:
-                with st.form("reset_password_form"):
-                    st.subheader("Reset Password")
-                    username = st.text_input(
-                        "Username",
-                        value=username,
-                    )
-                    password = st.text_input(
-                        "Password",
-                        type="password",
-                        value=password,
-                        disabled=True,
-                    )
-                    new_password = st.text_input("New Password", type="password")
-                    confirm_new_password = st.text_input(
-                        "Confirm Password", type="password"
-                    )
-                    password_reset_submitted = st.form_submit_button("Reset Password")
-                    status_container = st.container()
+            with st.form("reset_password_form"):
+                st.subheader("Reset Password")
+                username = st.text_input(
+                    "Username",
+                    value=username,
+                )
+                password = st.text_input(
+                    "Password",
+                    type="password",
+                    value=password,
+                    disabled=True,
+                )
+                new_password = st.text_input("New Password", type="password")
+                confirm_new_password = st.text_input(
+                    "Confirm Password", type="password"
+                )
+                password_reset_submitted = st.form_submit_button("Reset Password")
+                status_container = st.container()
 
         return (
             password_reset_submitted,
             username,
             password,
             new_password,
             confirm_new_password,
@@ -439,22 +425,14 @@
         reset_password_username: str, reset_password_password: str
     ) -> None:
         logger.info("Set password reset state")
         self.session_manager.set_reset_password_session(
             reset_password_username, reset_password_password
         )
 
-    def _set_reset_password(self,
-        reset_password_username: str, reset_password_password: str
-    ) -> None:
-        logger.info("Set password reset state")
-        self.session_manager.set_reset_password_session(
-            reset_password_username, reset_password_password
-        )
-        
     def _reset_password(self, username, password, new_password) -> bool:
         aws_srp_args = {
             "client": self.client,
             "pool_id": self.pool_id,
             "client_id": self.app_client_id,
             "username": username,
             "password": password,
@@ -649,28 +627,37 @@
     def login_url(self, response_type: str = "code") -> str:
         """Returns the hosted UI login url."""
         return (
             f"{self.domain}login?response_type={response_type}&client_id={self.app_client_id}"
             f"&redirect_uri={self.redirect_uri}"
         )
 
+    @staticmethod
+    def get_code(query_params: Dict[str, List[str]]) -> Optional[str]:
+        return query_params["code"][0] if (
+            "code" in query_params
+            and len(query_params["code"]) > 0
+            and query_params["code"][0]
+        ) else None
 
     def login(self, show_login_button=True, **kwargs) -> bool:
 
         # logged in
         if self.session_manager.is_logged_in():
             return True
 
-        code = st.query_params["code"]
+        query_params = st.experimental_get_query_params()
+        logged_in = False
+        code = self.get_code(query_params)
         if code:
             try:
                 credentials = self._credentials_from_auth_code(code=code)
             except Exception as exc:
                 st.error(str(exc))
                 self._set_state_logout()
             else:
                 logged_in = self._set_state_login(credentials)
-                st.query_params.clear()
+                st.experimental_set_query_params(code="")
         elif show_login_button:
             self.show_login_button(**kwargs)
 
         return logged_in
```

### Comparing `stcog-0.0.6/src/stcog/session_provider.py` & `stcog-0.0.7/src/stcog/session_provider.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/src/stcog/utils.py` & `stcog-0.0.7/src/stcog/utils.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/tests/example.py` & `stcog-0.0.7/tests/example.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/tests/example_hosted.py` & `stcog-0.0.7/tests/example_hosted.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/LICENSE` & `stcog-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/README.md` & `stcog-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stcog-0.0.6/pyproject.toml` & `stcog-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stcog"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Pastoris Zumba", email="fcuy047@gmail.com" },
 ]
 description = "A package for streamlit and aws auth link"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stcog-0.0.6/PKG-INFO` & `stcog-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stcog
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for streamlit and aws auth link
 Project-URL: Homepage, https://github.com/pop-srw/streamlit-cognito-auth/
 Project-URL: Issues, https://github.com/pop-srw/streamlit-cognito-auth/issues
 Author-email: Pastoris Zumba <fcuy047@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

