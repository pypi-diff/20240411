# Comparing `tmp/cryptojwt-1.8.4.tar.gz` & `tmp/cryptojwt-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptojwt-1.8.4.tar", max compression
+gzip compressed data, was "cryptojwt-1.9.0.tar", max compression
```

## Comparing `cryptojwt-1.8.4.tar` & `cryptojwt-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rwxr-xr-x   0        0        0    10759 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/LICENSE
--rw-r--r--   0        0        0      576 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/README.md
--rw-r--r--   0        0        0     1317 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      877 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/exception.py
--rw-r--r--   0        0        0     1119 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/__init__.py
--rw-r--r--   0        0        0     4388 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/aes.py
--rw-r--r--   0        0        0      606 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/exception.py
--rw-r--r--   0        0        0     2064 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/fernet.py
--rw-r--r--   0        0        0     7204 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwe.py
--rw-r--r--   0        0        0     7769 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_ec.py
--rw-r--r--   0        0        0     3050 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_hmac.py
--rw-r--r--   0        0        0     3638 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_rsa.py
--rw-r--r--   0        0        0     2749 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwekey.py
--rw-r--r--   0        0        0     1414 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/jwenc.py
--rw-r--r--   0        0        0     1775 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/rsa.py
--rw-r--r--   0        0        0     2910 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwe/utils.py
--rw-r--r--   0        0        0    10835 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/asym.py
--rw-r--r--   0        0        0    11294 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/ec.py
--rw-r--r--   0        0        0     4607 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/hmac.py
--rw-r--r--   0        0        0     8078 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/jwk.py
--rw-r--r--   0        0        0    11985 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/okp.py
--rw-r--r--   0        0        0    15334 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/rsa.py
--rw-r--r--   0        0        0      728 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/utils.py
--rw-r--r--   0        0        0      905 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/wrap.py
--rw-r--r--   0        0        0     4102 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwk/x509.py
--rw-r--r--   0        0        0      354 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/__init__.py
--rw-r--r--   0        0        0     3962 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/dsa.py
--rw-r--r--   0        0        0     2630 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/eddsa.py
--rw-r--r--   0        0        0      329 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/exception.py
--rw-r--r--   0        0        0     1535 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/hmac.py
--rw-r--r--   0        0        0    15416 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/jws.py
--rw-r--r--   0        0        0     2183 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/pss.py
--rw-r--r--   0        0        0     1580 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/rsa.py
--rw-r--r--   0        0        0     2831 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jws/utils.py
--rwxr-xr-x   0        0        0    14149 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwt.py
--rw-r--r--   0        0        0     8719 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/jwx.py
--rwxr-xr-x   0        0        0    40515 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/key_bundle.py
--rwxr-xr-x   0        0        0    21135 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/key_issuer.py
--rwxr-xr-x   0        0        0    29558 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/key_jar.py
--rw-r--r--   0        0        0        0 2024-04-10 07:41:00.007476 cryptojwt-1.8.4/src/cryptojwt/serialize/__init__.py
--rw-r--r--   0        0        0      472 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/serialize/item.py
--rw-r--r--   0        0        0     4504 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/simple_jwt.py
--rw-r--r--   0        0        0        0 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/tools/__init__.py
--rwxr-xr-x   0        0        0     4221 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/tools/jwtpeek.py
--rw-r--r--   0        0        0     7481 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/tools/keyconv.py
--rw-r--r--   0        0        0     2522 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/tools/keygen.py
--rw-r--r--   0        0        0     8709 2024-04-10 07:41:00.011476 cryptojwt-1.8.4/src/cryptojwt/utils.py
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 cryptojwt-1.8.4/PKG-INFO
+-rwxr-xr-x   0        0        0    10759 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/LICENSE
+-rw-r--r--   0        0        0      576 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/README.md
+-rw-r--r--   0        0        0     1317 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      877 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/exception.py
+-rw-r--r--   0        0        0     1119 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/__init__.py
+-rw-r--r--   0        0        0     4388 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/aes.py
+-rw-r--r--   0        0        0      606 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/exception.py
+-rw-r--r--   0        0        0     2064 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/fernet.py
+-rw-r--r--   0        0        0     7204 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe.py
+-rw-r--r--   0        0        0     7769 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_ec.py
+-rw-r--r--   0        0        0     3050 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_hmac.py
+-rw-r--r--   0        0        0     3638 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_rsa.py
+-rw-r--r--   0        0        0     2749 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwekey.py
+-rw-r--r--   0        0        0     1414 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/jwenc.py
+-rw-r--r--   0        0        0     1775 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/rsa.py
+-rw-r--r--   0        0        0     2910 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwe/utils.py
+-rw-r--r--   0        0        0    10835 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/asym.py
+-rw-r--r--   0        0        0    11294 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/ec.py
+-rw-r--r--   0        0        0     4607 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/hmac.py
+-rw-r--r--   0        0        0     8078 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/jwk.py
+-rw-r--r--   0        0        0    11985 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/okp.py
+-rw-r--r--   0        0        0    15334 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/rsa.py
+-rw-r--r--   0        0        0      728 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/utils.py
+-rw-r--r--   0        0        0      905 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/wrap.py
+-rw-r--r--   0        0        0     4102 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jwk/x509.py
+-rw-r--r--   0        0        0      354 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/__init__.py
+-rw-r--r--   0        0        0     3962 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/dsa.py
+-rw-r--r--   0        0        0     2630 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/eddsa.py
+-rw-r--r--   0        0        0      329 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/exception.py
+-rw-r--r--   0        0        0     1535 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/hmac.py
+-rw-r--r--   0        0        0    15416 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/jws.py
+-rw-r--r--   0        0        0     2183 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/pss.py
+-rw-r--r--   0        0        0     1580 2024-04-11 11:45:17.222844 cryptojwt-1.9.0/src/cryptojwt/jws/rsa.py
+-rw-r--r--   0        0        0     2831 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jws/utils.py
+-rwxr-xr-x   0        0        0    14149 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jwt.py
+-rw-r--r--   0        0        0     8719 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/jwx.py
+-rwxr-xr-x   0        0        0    40515 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_bundle.py
+-rwxr-xr-x   0        0        0    21135 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_issuer.py
+-rwxr-xr-x   0        0        0    29558 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/key_jar.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/serialize/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/serialize/item.py
+-rw-r--r--   0        0        0     4504 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/simple_jwt.py
+-rw-r--r--   0        0        0        0 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/__init__.py
+-rwxr-xr-x   0        0        0     4221 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/jwtpeek.py
+-rw-r--r--   0        0        0     7481 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/keyconv.py
+-rw-r--r--   0        0        0     2522 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/tools/keygen.py
+-rw-r--r--   0        0        0     8709 2024-04-11 11:45:17.226844 cryptojwt-1.9.0/src/cryptojwt/utils.py
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 cryptojwt-1.9.0/PKG-INFO
```

### Comparing `cryptojwt-1.8.4/LICENSE` & `cryptojwt-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/README.md` & `cryptojwt-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/pyproject.toml` & `cryptojwt-1.9.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
 ]
 
 [tool.poetry]
 name = "cryptojwt"
-version = "1.8.4"
+version = "1.9.0"
 description = "Python implementation of JWT, JWE, JWS and JWK"
 authors = ["Roland Hedberg <roland@catalogix.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT"
 readme = "README.md"
 packages = [
     { include = "cryptojwt", from = "src" }
```

### Comparing `cryptojwt-1.8.4/src/cryptojwt/__init__.py` & `cryptojwt-1.9.0/src/cryptojwt/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/exception.py` & `cryptojwt-1.9.0/src/cryptojwt/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/__init__.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/aes.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/aes.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/exception.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/exception.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/fernet.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/fernet.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwe.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_ec.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_ec.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_hmac.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwe_rsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwe_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwekey.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwekey.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/jwenc.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/jwenc.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/rsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwe/utils.py` & `cryptojwt-1.9.0/src/cryptojwt/jwe/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/__init__.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/asym.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/asym.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/ec.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/ec.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/hmac.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/jwk.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/jwk.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/okp.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/okp.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/rsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/utils.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/wrap.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/wrap.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwk/x509.py` & `cryptojwt-1.9.0/src/cryptojwt/jwk/x509.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/dsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/eddsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/eddsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/hmac.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/hmac.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/jws.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/jws.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/pss.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/pss.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/rsa.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jws/utils.py` & `cryptojwt-1.9.0/src/cryptojwt/jws/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwt.py` & `cryptojwt-1.9.0/src/cryptojwt/jwt.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/jwx.py` & `cryptojwt-1.9.0/src/cryptojwt/jwx.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/key_bundle.py` & `cryptojwt-1.9.0/src/cryptojwt/key_bundle.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/key_issuer.py` & `cryptojwt-1.9.0/src/cryptojwt/key_issuer.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/key_jar.py` & `cryptojwt-1.9.0/src/cryptojwt/key_jar.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/simple_jwt.py` & `cryptojwt-1.9.0/src/cryptojwt/simple_jwt.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/tools/jwtpeek.py` & `cryptojwt-1.9.0/src/cryptojwt/tools/jwtpeek.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/tools/keyconv.py` & `cryptojwt-1.9.0/src/cryptojwt/tools/keyconv.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/tools/keygen.py` & `cryptojwt-1.9.0/src/cryptojwt/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/src/cryptojwt/utils.py` & `cryptojwt-1.9.0/src/cryptojwt/utils.py`

 * *Files identical despite different names*

### Comparing `cryptojwt-1.8.4/PKG-INFO` & `cryptojwt-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptojwt
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python implementation of JWT, JWE, JWS and JWK
 Home-page: https://github.com/IdentityPython/JWTConnect-Python-CryptoJWT
 License: Apache-2.0
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

