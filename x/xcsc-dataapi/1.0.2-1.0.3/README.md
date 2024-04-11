# Comparing `tmp/xcsc_dataapi-1.0.2.tar.gz` & `tmp/xcsc_dataapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsc_dataapi-1.0.2.tar", last modified: Tue Apr  2 02:38:14 2024, max compression
+gzip compressed data, was "xcsc_dataapi-1.0.3.tar", last modified: Thu Apr 11 01:58:32 2024, max compression
```

## Comparing `xcsc_dataapi-1.0.2.tar` & `xcsc_dataapi-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.429722 xcsc_dataapi-1.0.2/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-04-02 02:38:14.429502 xcsc_dataapi-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.2/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2024-04-02 02:38:14.429764 xcsc_dataapi-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.426999 xcsc_dataapi-1.0.2/test/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/test/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      264 2024-04-02 02:28:41.000000 xcsc_dataapi-1.0.2/test/dataapi_test.py
--rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 09:05:28.000000 xcsc_dataapi-1.0.2/test/token_test.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.427381 xcsc_dataapi-1.0.2/xcsc_dataapi/
--rw-r--r--   0 root         (0) staff       (20)        5 2024-04-02 02:27:21.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/VERSION.txt
--rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.428558 xcsc_dataapi-1.0.2/xcsc_dataapi/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1952 2024-04-02 02:28:54.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/client.py
--rw-r--r--   0 root         (0) staff       (20)     2877 2024-04-02 02:29:11.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/data/token.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.428883 xcsc_dataapi-1.0.2/xcsc_dataapi/util/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/util/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.2/xcsc_dataapi/util/sm4_cbc_util.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-02 02:38:14.429257 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      453 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       42 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       18 2024-04-02 02:38:14.000000 xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.807881 xcsc_dataapi-1.0.3/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-11 01:58:32.807586 xcsc_dataapi-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.3/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-11 01:58:32.807981 xcsc_dataapi-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.800601 xcsc_dataapi-1.0.3/test/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/test/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      264 2024-04-02 02:28:41.000000 xcsc_dataapi-1.0.3/test/dataapi_test.py
+-rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 09:05:28.000000 xcsc_dataapi-1.0.3/test/token_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.802234 xcsc_dataapi-1.0.3/xcsc_dataapi/
+-rw-r--r--   0 root         (0) staff       (20)        5 2024-04-11 01:57:29.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/VERSION.txt
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.806480 xcsc_dataapi-1.0.3/xcsc_dataapi/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1952 2024-04-02 02:28:54.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/client.py
+-rw-r--r--   0 root         (0) staff       (20)     2889 2024-04-11 01:48:58.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/token.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.806867 xcsc_dataapi-1.0.3/xcsc_dataapi/util/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/util/sm4_cbc_util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.807283 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      453 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       42 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       18 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/top_level.txt
```

### Comparing `xcsc_dataapi-1.0.2/PKG-INFO` & `xcsc_dataapi-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xcsc_dataapi-1.0.2/README.md` & `xcsc_dataapi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.2/setup.py` & `xcsc_dataapi-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.2/xcsc_dataapi/data/client.py` & `xcsc_dataapi-1.0.3/xcsc_dataapi/data/client.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.2/xcsc_dataapi/data/token.py` & `xcsc_dataapi-1.0.3/xcsc_dataapi/data/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,18 @@
     if init_response.status_code == 200:
         init_result = init_response.json()
         code = init_result['code']
         if code == '0':
             # access_token会有失效时间，请在有效期内使用，不要每次请求api都重新生成新的access_token!!!
             access_token_in = init_result['data']['accessToken']  # access_token
         else:
-            Exception('获取令牌token失败：' + init_result['msg'])
+            raise Exception('获取令牌token失败：' + init_result['msg'])
 
     else:
-        Exception('初始化获取accessToken请求失败,'+init_response.text)
+        raise Exception('初始化获取accessToken请求失败,'+init_response.text)
 
     return access_token_in
 
 
 def pro_api(token=''):
     """
                 Parameters
```

### Comparing `xcsc_dataapi-1.0.2/xcsc_dataapi/util/sm4_cbc_util.py` & `xcsc_dataapi-1.0.3/xcsc_dataapi/util/sm4_cbc_util.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.2/xcsc_dataapi.egg-info/PKG-INFO` & `xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

