# Comparing `tmp/sparkproxy-0.3.0.tar.gz` & `tmp/sparkproxy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.3.0.tar", last modified: Wed Apr 10 01:59:03 2024, max compression
+gzip compressed data, was "sparkproxy-0.3.1.tar", last modified: Wed Apr 10 05:12:49 2024, max compression
```

## Comparing `sparkproxy-0.3.0.tar` & `sparkproxy-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.344485 sparkproxy-0.3.0/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.3.0/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 01:59:03.344362 sparkproxy-0.3.0/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     4266 2024-04-10 01:58:30.000000 sparkproxy-0.3.0/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-10 01:59:03.344526 sparkproxy-0.3.0/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.3.0/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.341087 sparkproxy-0.3.0/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-10 01:56:26.000000 sparkproxy-0.3.0/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     3048 2024-04-10 01:27:54.000000 sparkproxy-0.3.0/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.3.0/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.342528 sparkproxy-0.3.0/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-08 15:29:41.000000 sparkproxy-0.3.0/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.3.0/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.343500 sparkproxy-0.3.0/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.3.0/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.3.0/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2511 2024-04-10 01:48:16.000000 sparkproxy-0.3.0/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.343839 sparkproxy-0.3.0/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.344041 sparkproxy-0.3.0/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.0/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     7059 2024-04-10 01:53:25.000000 sparkproxy-0.3.0/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 01:59:03.341913 sparkproxy-0.3.0/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-10 01:59:03.000000 sparkproxy-0.3.0/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.631207 sparkproxy-0.3.1/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.3.1/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 05:12:49.631089 sparkproxy-0.3.1/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     4202 2024-04-10 05:11:45.000000 sparkproxy-0.3.1/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-10 05:12:49.631243 sparkproxy-0.3.1/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.3.1/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.629037 sparkproxy-0.3.1/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-10 05:10:34.000000 sparkproxy-0.3.1/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.3.1/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-08 16:29:22.000000 sparkproxy-0.3.1/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630113 sparkproxy-0.3.1/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.3.1/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.3.1/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630593 sparkproxy-0.3.1/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.3.1/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.3.1/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.3.1/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630735 sparkproxy-0.3.1/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.630915 sparkproxy-0.3.1/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.3.1/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     7059 2024-04-10 01:53:25.000000 sparkproxy-0.3.1/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-10 05:12:49.629775 sparkproxy-0.3.1/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-10 05:12:49.000000 sparkproxy-0.3.1/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.3.0/LICENSE` & `sparkproxy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/PKG-INFO` & `sparkproxy-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.3.0/README.md` & `sparkproxy-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 ```python
 from sparkproxy import Auth
 from sparkproxy import SparkProxyClient
 
 supplier_no = 'test0001'
 with open("key.pem", 'rb') as pem_file:
-    private_key = pem_file.read().decode("utf-8")
+    private_key = pem_file.read()
 with open("spark.pub", 'rb') as pem_file:
-    rsa_public_key = pem_file.read().decode("utf-8")
+    rsa_public_key = pem_file.read()
 client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key, public_key=rsa_public_key))
 
 # 获取订单&实例信息
 ret, info = client.check_available()
 print(ret)
 print(info)
 ```
@@ -47,15 +47,15 @@
 from sparkproxy import SparkProxyClient
 
 # 双方协商的商户号
 supplier_no = 'test0001'
 
 # 使用私钥对请求签名（认证）, 生成方式参考 [examples示例](https://github.com/yungoo/spark-sdk-python/tree/master/examples/genrsa.py)。
 with open("key.pem", 'rb') as pem_file:
-    private_key = pem_file.read().decode("utf-8")
+    private_key = pem_file.read()
 client = SparkProxyClient(Auth(supplier_no=supplier_no, private_key=private_key))
 
 ret, info = client.get_product_stock(proxy_type=103)
 if ret is not None:
     print('All is OK')
 else:
     print(info) # error message in info
@@ -76,15 +76,15 @@
 Dp62XP8SrvUPBqGlWGEKNh60n2njcUUIkMDitM2yb1vuRluu3Mzk/TvaE23JOMqA
 0HPsd7IG9rNCyn7vcRXvVj1jLTVw/J+f7FJB4OzZqmOEe8kq69WCP4JIkXPvAT53
 wvarJGl6cincWuZvIwIDAQAB
 -----END PUBLIC KEY-----
 '''
 
 with open("key.pem", 'rb') as pem_file:
-    private_key = pem_file.read().decode("utf-8")
+    private_key = pem_file.read()
 
 supplier_no = 'test0001'
 auth = Auth(supplier_no=supplier_no, private_key=private_key, public_key=rsa_public_key)
 
 
 def verify_request(req):
     if req.is_json:
```

### Comparing `sparkproxy-0.3.0/setup.py` & `sparkproxy-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/auth.py` & `sparkproxy-0.3.1/sparkproxy/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,22 +67,22 @@
             req_id:            回调请求的请求ID
             timestamp:         回调请求的时间戳
 
         Returns:
             返回ValueError异常表示验证失败
         """
         if not supplier_no:
-            raise ValueError(f"签名参数supplierNo未提供。reqId: {req_id}")
+            raise ValueError("签名参数supplierNo未提供。reqId: {}".format(req_id))
         if not sign:
-            raise ValueError(f"签名参数sign未提供。reqId: {req_id}")
+            raise ValueError("签名参数sign未提供。reqId: {}".format(req_id))
 
         if time.time() - timestamp > 600:
-            raise ValueError(f"签名已过期。reqId: {req_id}")
+            raise ValueError("签名已过期。reqId: {}".format(req_id))
 
-        str_to_sign = f"supplierNo={supplier_no}&timestamp={timestamp}"
+        str_to_sign = "supplierNo={}&timestamp={}".format(supplier_no, timestamp)
 
         try:
             rsa_verify(sign, str_to_sign, self.__public_key)
         except InvalidSignature:
-            raise ValueError(f"签名校验错误。reqId: {req_id}")
+            raise ValueError("签名校验错误。reqId: {}".format(req_id))
         except Exception as e:
-            raise ValueError(f"签名验证过程中出现问题: {e}")
+            raise ValueError("签名验证过程中出现问题: {}".format(e))
```

### Comparing `sparkproxy-0.3.0/sparkproxy/compat.py` & `sparkproxy-0.3.1/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/config.py` & `sparkproxy-0.3.1/sparkproxy/config.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/__init__.py` & `sparkproxy-0.3.1/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/client.py` & `sparkproxy-0.3.1/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/middleware/base.py` & `sparkproxy-0.3.1/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.3.1/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.3.1/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/http/response.py` & `sparkproxy-0.3.1/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy/rsa.py` & `sparkproxy-0.3.1/sparkproxy/rsa.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+# coding=utf-8
+from __future__ import absolute_import, division, print_function
 import binascii
 
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric import padding
+# 尝试导入Python 3中的库，如果失败，则回退到Python 2的等效库
+import sys
+
+try:
+    from cryptography.hazmat.backends import default_backend
+    from cryptography.hazmat.primitives import serialization, hashes
+    from cryptography.hazmat.primitives.asymmetric import padding
+except ImportError:
+    # Python 2的兼容代码，或其他回退代码
+    # 注意：cryptography库在Python 2和Python 3中的用法相同，所以这里主要是演示结构
+    pass
 
 
 # 兼容Python 2和3的编码函数
 def to_bytes(data, encoding='utf-8'):
-    if isinstance(data, str):
-        return data.encode(encoding)
-    return data
+    """确保s是字节类型"""
+    if sys.version_info[0] < 3:
+        # Python 2.x，s已经是字节串
+        return data
+    else:
+        # Python 3.x，确保是bytes
+        return data.encode(encoding) if isinstance(data, str) else data
 
 
 def to_string(data, encoding='utf-8'):
     """
     将数据转换为字符串。
 
     Args:
@@ -46,25 +59,25 @@
         return data.hex()  # Python 3
     except AttributeError:
         return binascii.hexlify(data)  # Python 2
 
 
 def rsa_load_pem_private_key(pri_key):
     private_key = serialization.load_pem_private_key(
-        to_bytes(pri_key),
+        pri_key,
         password=None,
         backend=default_backend()
     )
     return private_key
 
 
 def rsa_load_pem_public_key(pub_key):
     public_key = serialization.load_pem_public_key(
-        to_bytes(pub_key),
-        backend=default_backend()  # 显式指定后端
+        pub_key,
+        backend=default_backend()
     )
     return public_key
 
 
 def rsa_public_encrypt(msg, public_key):
     decoded_msg = to_bytes(msg)
```

### Comparing `sparkproxy-0.3.0/sparkproxy/services/openapi/client.py` & `sparkproxy-0.3.1/sparkproxy/services/openapi/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.3.0/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.3.1/sparkproxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.3.0/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.3.1/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

