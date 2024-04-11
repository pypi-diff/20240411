# Comparing `tmp/pastel_gateway_sdk-0.1.3-py3-none-any.whl.zip` & `tmp/pastel_gateway_sdk-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 91479 bytes, number of entries: 43
+Zip file size: 94996 bytes, number of entries: 43
 -rw-r--r--  2.0 unx     3229 b- defN 24-Jan-08 20:01 pastel_gateway_sdk/__init__.py
 -rw-r--r--  2.0 unx    24978 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/api_client.py
 -rw-r--r--  2.0 unx      674 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/api_response.py
--rw-r--r--  2.0 unx    15473 b- defN 24-Feb-27 01:10 pastel_gateway_sdk/configuration.py
+-rw-r--r--  2.0 unx    15473 b- defN 24-Apr-11 03:38 pastel_gateway_sdk/configuration.py
 -rw-r--r--  2.0 unx     6207 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/exceptions.py
--rw-r--r--  2.0 unx     4106 b- defN 24-Feb-16 00:03 pastel_gateway_sdk/gateway_api_client.py
+-rw-r--r--  2.0 unx     4123 b- defN 24-Apr-11 03:37 pastel_gateway_sdk/gateway_api_client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/py.typed
 -rw-r--r--  2.0 unx     6904 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/rest.py
 -rw-r--r--  2.0 unx      499 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/api/__init__.py
 -rw-r--r--  2.0 unx    51406 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/api/account_api.py
 -rw-r--r--  2.0 unx    41509 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/api/api_keys_api.py
 -rw-r--r--  2.0 unx   189521 b- defN 24-Feb-27 00:32 pastel_gateway_sdk/api/cascade_api.py
 -rw-r--r--  2.0 unx    81954 b- defN 24-Feb-27 01:08 pastel_gateway_sdk/api/collection_api.py
@@ -34,12 +34,12 @@
 -rw-r--r--  2.0 unx     1317 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/status.py
 -rw-r--r--  2.0 unx     2709 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/token.py
 -rw-r--r--  2.0 unx     4629 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/user.py
 -rw-r--r--  2.0 unx     3741 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/user_create.py
 -rw-r--r--  2.0 unx     5127 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/user_id_or_email.py
 -rw-r--r--  2.0 unx     3976 b- defN 23-Dec-30 01:00 pastel_gateway_sdk/models/user_update.py
 -rw-r--r--  2.0 unx     3202 b- defN 24-Jan-05 02:29 pastel_gateway_sdk/models/validation_error.py
--rw-r--r--  2.0 unx      868 b- defN 24-Feb-27 01:10 pastel_gateway_sdk-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-27 01:10 pastel_gateway_sdk-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Feb-27 01:10 pastel_gateway_sdk-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4160 b- defN 24-Feb-27 01:10 pastel_gateway_sdk-0.1.3.dist-info/RECORD
-43 files, 1209266 bytes uncompressed, 84673 bytes compressed:  93.0%
+-rw-r--r--  2.0 unx    24795 b- defN 24-Apr-11 03:46 pastel_gateway_sdk-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 03:46 pastel_gateway_sdk-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-11 03:46 pastel_gateway_sdk-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4162 b- defN 24-Apr-11 03:46 pastel_gateway_sdk-0.1.4.dist-info/RECORD
+43 files, 1233212 bytes uncompressed, 88190 bytes compressed:  92.8%
```

## zipnote {}

```diff
@@ -111,20 +111,20 @@
 
 Filename: pastel_gateway_sdk/models/user_update.py
 Comment: 
 
 Filename: pastel_gateway_sdk/models/validation_error.py
 Comment: 
 
-Filename: pastel_gateway_sdk-0.1.3.dist-info/METADATA
+Filename: pastel_gateway_sdk-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pastel_gateway_sdk-0.1.3.dist-info/WHEEL
+Filename: pastel_gateway_sdk-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pastel_gateway_sdk-0.1.3.dist-info/top_level.txt
+Filename: pastel_gateway_sdk-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pastel_gateway_sdk-0.1.3.dist-info/RECORD
+Filename: pastel_gateway_sdk-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pastel_gateway_sdk/configuration.py

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.1.3".\
+               "SDK Package Version: 0.1.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

## pastel_gateway_sdk/gateway_api_client.py

```diff
@@ -35,22 +35,24 @@
                          f"or provide custom_url")
 
     async def authenticate(self, username: str, password: str) -> bool:
         login_api = self.login_api
         token = await login_api.login_access_token(username=username, password=password)
         if not token or type(token) is not Token or not token.access_token:
             return False
-        self.configuration.access_token = token.access_token
-        self._token = token.access_token
+        self.set_token(token.access_token)
         return True
 
+    def set_token(self, token: str | None):
+        self.configuration.access_token = token
+        self._token = token
+
     async def logout(self):
         self.clear_auth_api_key()
-        self.configuration.access_token = None
-        self._token = None
+        self.set_token(None)
         self._account_api = None
         self._api_keys_api = None
         self._users_api = None
         self._login_api = None
         self._cascade_api = None
         self._collection_api = None
         self._nft_api = None
```

## Comparing `pastel_gateway_sdk-0.1.3.dist-info/RECORD` & `pastel_gateway_sdk-0.1.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pastel_gateway_sdk/__init__.py,sha256=L5jeaDFUfQru4WOsJWOICP-eXsPsh979txCG1dkm6pI,3229
 pastel_gateway_sdk/api_client.py,sha256=TgMKFf1oYKjCpPKj5DAVyfrBmeIEKyghDI-fUNRy_BM,24978
 pastel_gateway_sdk/api_response.py,sha256=A7O_XgliD6y7jEv82fgIaxR3T8KiwaOqHR6djpZyh_o,674
-pastel_gateway_sdk/configuration.py,sha256=TopG9wrw3oyjgPGI-luZReWmCZTHlYY9gzqD9R3yuZI,15473
+pastel_gateway_sdk/configuration.py,sha256=QtClt6QdlxOr0VdlNGqjbwYc_iyT6RFsdf5J6Bq9Nv8,15473
 pastel_gateway_sdk/exceptions.py,sha256=DuoUoSCAhTxsJH0at86UxaJ-QWxoKY8qGv16vjC4PjA,6207
-pastel_gateway_sdk/gateway_api_client.py,sha256=JzzOTYZuXR1WR0yWazYA5AIwPnw7puS9WL90IhXKZ_8,4106
+pastel_gateway_sdk/gateway_api_client.py,sha256=aXQ6SnSCp5dkHWub77pgphWICKpebH7buGFA3a1QJy4,4123
 pastel_gateway_sdk/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pastel_gateway_sdk/rest.py,sha256=OwitW8QNGGMKN7KNgXoQH7Le9VU7tDIJN22OmA-k8vg,6904
 pastel_gateway_sdk/api/__init__.py,sha256=MQ0bAqd-Zg_LqXn_MPQWviTj8ssTOyaUYvVMhi6ZhB8,499
 pastel_gateway_sdk/api/account_api.py,sha256=386pGvceIKgFhtavoDdZ4d61MlFoqGgw-oGzj0McIO8,51406
 pastel_gateway_sdk/api/api_keys_api.py,sha256=sLO0Ez578oxnH5S4pC4UPLE9SyEm2I9qdnWc6zEjoxw,41509
 pastel_gateway_sdk/api/cascade_api.py,sha256=ihy79ZeMXXwlaoHQbAfCfUZUP2RlAbu7TS_vy4ig24k,189521
 pastel_gateway_sdk/api/collection_api.py,sha256=iv0XF7qQua0YIfEA4J43Q8EexgdxNryIFSJ5MMHIvi8,81954
@@ -33,11 +33,11 @@
 pastel_gateway_sdk/models/status.py,sha256=xbaH3G0S7jK2ZJs4Ufz0nWBW8iMs90DIQMQu1O-wksA,1317
 pastel_gateway_sdk/models/token.py,sha256=LqYZJxJqKdW1pHHo-h_bZr7a5Fg6vfaXrvB6yUy50ho,2709
 pastel_gateway_sdk/models/user.py,sha256=y-2mmk7wsZazPYnLGHbvwpzV2W6OVukzwNIhIouBtgE,4629
 pastel_gateway_sdk/models/user_create.py,sha256=27KpjZhHGAL6wTx3lPUrwA5fF0cGoFSQbdyX5dyIc00,3741
 pastel_gateway_sdk/models/user_id_or_email.py,sha256=sWXQc2jye9c7_tsSr7UlunD9PHzd7mWyLlmB8zBHHYc,5127
 pastel_gateway_sdk/models/user_update.py,sha256=tajhDKWEkaIsRSrlYAP2KjwBJkFo0q79aMuQoGwFw3M,3976
 pastel_gateway_sdk/models/validation_error.py,sha256=KpnJ7ww1HKmUEdemVr59qfUN2hs2H0RNssWKTyCT4OA,3202
-pastel_gateway_sdk-0.1.3.dist-info/METADATA,sha256=wwiCllx8D_hmungmCOXh7s46jIqwVyeSvT-u3W5rTzM,868
-pastel_gateway_sdk-0.1.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pastel_gateway_sdk-0.1.3.dist-info/top_level.txt,sha256=_b-A3GZ0_PNeEF2Eu6ThlH7rXufyf67xLE0M0uSb54c,19
-pastel_gateway_sdk-0.1.3.dist-info/RECORD,,
+pastel_gateway_sdk-0.1.4.dist-info/METADATA,sha256=DWW8B9SNZWCDw0wzg05TSVZ7fWmKprRNR9BgWYvfkog,24795
+pastel_gateway_sdk-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pastel_gateway_sdk-0.1.4.dist-info/top_level.txt,sha256=_b-A3GZ0_PNeEF2Eu6ThlH7rXufyf67xLE0M0uSb54c,19
+pastel_gateway_sdk-0.1.4.dist-info/RECORD,,
```

