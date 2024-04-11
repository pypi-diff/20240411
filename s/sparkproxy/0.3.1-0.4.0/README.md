# Comparing `tmp/sparkproxy-0.3.1.tar.gz` & `tmp/sparkproxy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.3.1.tar", last modified: Wed Apr 10 05:12:49 2024, max compression
+gzip compressed data, was "sparkproxy-0.4.0.tar", last modified: Thu Apr 11 02:15:10 2024, max compression
```

## Comparing `sparkproxy-0.3.1.tar` & `sparkproxy-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.631207 sparkproxy-0.3.1/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.3.1/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 05:12:49.631089 sparkproxy-0.3.1/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     4202 2024-04-10 05:11:45.000000 sparkproxy-0.3.1/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-10 05:12:49.631243 sparkproxy-0.3.1/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.3.1/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.629037 sparkproxy-0.3.1/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-10 05:10:34.000000 sparkproxy-0.3.1/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.3.1/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.3.1/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630113 sparkproxy-0.3.1/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.3.1/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.3.1/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630593 sparkproxy-0.3.1/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.3.1/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.3.1/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630735 sparkproxy-0.3.1/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630915 sparkproxy-0.3.1/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     7059 2024-04-10 01:53:25.000000 sparkproxy-0.3.1/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.629775 sparkproxy-0.3.1/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.475259 sparkproxy-0.4.0/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.4.0/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-11 02:15:10.475100 sparkproxy-0.4.0/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     4823 2024-04-11 02:14:51.000000 sparkproxy-0.4.0/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-11 02:15:10.475311 sparkproxy-0.4.0/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.4.0/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.470801 sparkproxy-0.4.0/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-11 01:44:56.000000 sparkproxy-0.4.0/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.4.0/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.4.0/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.4.0/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.472697 sparkproxy-0.4.0/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.4.0/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.4.0/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.473699 sparkproxy-0.4.0/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.4.0/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.4.0/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.4.0/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.4.0/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.4.0/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.4.0/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.474374 sparkproxy-0.4.0/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.0/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.474616 sparkproxy-0.4.0/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.0/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     7059 2024-04-10 01:53:25.000000 sparkproxy-0.4.0/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 02:15:10.471688 sparkproxy-0.4.0/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-11 02:15:10.000000 sparkproxy-0.4.0/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.3.1/LICENSE` & `sparkproxy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/PKG-INFO` & `sparkproxy-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.3.1/README.md` & `sparkproxy-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -98,14 +98,35 @@
         return "Bad request", 400
 
     return None, 200
 
 
 app = Flask(__name__)
 
+@app.route("/checkAvailable", methods=["POST"])
+def receiveCheckAvailable():
+    # 验签
+    ret, code = verify_request(request)
+    if ret is not None:
+        return ret, code
+
+    # 取出参数字符串，把16进制字符串转为二进制
+    cyper_text = request.json["data"]
+
+    # 通过自己的私钥解密
+    plain_text = auth.decrypt_using_private_key(cyper_text)
+
+    # 把解密字符串用对方的公钥加密，并转为16进制字符串
+    new_cyper_text = auth.encrypt_using_remote_public_key(plain_text)
+
+    return {
+        "code": 200,
+        "msg": "ok",
+        "data": new_cyper_text
+    }
 
 @app.route("/product/sync", methods=["POST"])
 def receiveSyncProducts():
     ret, code = verify_request(request)
     if ret is not None:
         return ret, code
```

### Comparing `sparkproxy-0.3.1/setup.py` & `sparkproxy-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/auth.py` & `sparkproxy-0.4.0/sparkproxy/auth.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/compat.py` & `sparkproxy-0.4.0/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/config.py` & `sparkproxy-0.4.0/sparkproxy/config.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/__init__.py` & `sparkproxy-0.4.0/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/client.py` & `sparkproxy-0.4.0/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/middleware/base.py` & `sparkproxy-0.4.0/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.4.0/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.4.0/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/http/response.py` & `sparkproxy-0.4.0/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/rsa.py` & `sparkproxy-0.4.0/sparkproxy/rsa.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy/services/openapi/client.py` & `sparkproxy-0.4.0/sparkproxy/services/openapi/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.1/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.4.0/sparkproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.3.1/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.4.0/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

