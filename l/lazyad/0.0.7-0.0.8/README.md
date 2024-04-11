# Comparing `tmp/lazyad-0.0.7.tar.gz` & `tmp/lazyad-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyad-0.0.7.tar", last modified: Thu Apr 11 06:58:11 2024, max compression
+gzip compressed data, was "lazyad-0.0.8.tar", last modified: Thu Apr 11 07:23:16 2024, max compression
```

## Comparing `lazyad-0.0.7.tar` & `lazyad-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.804797 lazyad-0.0.7/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 06:58:11.804597 lazyad-0.0.7/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.7/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.801956 lazyad-0.0.7/lazyad/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       41 2024-04-11 06:24:40.000000 lazyad-0.0.7/lazyad/__init__.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.803872 lazyad-0.0.7/lazyad/crawlers/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.7/lazyad/crawlers/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.7/lazyad/crawlers/chuangliang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.7/lazyad/crawlers/oceanengine.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.7/lazyad/crawlers/qq.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.804288 lazyad-0.0.7/lazyad/open/
--rw-r--r--   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:24:12.000000 lazyad-0.0.7/lazyad/open/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1780 2024-04-11 06:57:50.000000 lazyad-0.0.7/lazyad/open/qq.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.802854 lazyad-0.0.7/lazyad.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      340 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-11 06:58:11.804838 lazyad-0.0.7/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-04-11 06:57:50.000000 lazyad-0.0.7/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.775597 lazyad-0.0.8/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 07:23:16.775420 lazyad-0.0.8/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.8/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.773053 lazyad-0.0.8/lazyad/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       41 2024-04-11 06:24:40.000000 lazyad-0.0.8/lazyad/__init__.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.774733 lazyad-0.0.8/lazyad/crawlers/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.8/lazyad/crawlers/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.8/lazyad/crawlers/chuangliang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.8/lazyad/crawlers/oceanengine.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.8/lazyad/crawlers/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.775130 lazyad-0.0.8/lazyad/open/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:24:12.000000 lazyad-0.0.8/lazyad/open/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2886 2024-04-11 07:22:45.000000 lazyad-0.0.8/lazyad/open/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.773706 lazyad-0.0.8/lazyad.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      340 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-11 07:23:16.775637 lazyad-0.0.8/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-04-11 07:22:45.000000 lazyad-0.0.8/setup.py
```

### Comparing `lazyad-0.0.7/PKG-INFO` & `lazyad-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.7
+Version: 0.0.8
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.7/README.md` & `lazyad-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.7/lazyad/crawlers/chuangliang.py` & `lazyad-0.0.8/lazyad/crawlers/chuangliang.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.7/lazyad/crawlers/oceanengine.py` & `lazyad-0.0.8/lazyad/crawlers/oceanengine.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.7/lazyad/crawlers/qq.py` & `lazyad-0.0.8/lazyad/crawlers/qq.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.7/lazyad/open/qq.py` & `lazyad-0.0.8/lazyad/open/qq.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,38 +12,82 @@
     """
     参考示例代码的生成一个随机数
     :return:
     """
     return str(time.time()) + str(random.randint(0, 999999))
 
 
-def oauth_token(
+def oauth_token2(
+        app_id,
+        app_secret,
+        redirect_uri,
+        grant_type='authorization_code',
+        auth_code=None,
+        refresh_token=None,
+):
+    """
+    OAuth 2.0 授权
+    获取/刷新token
+    相关文档：https://developers.e.qq.com/docs/start/authorization
+    :param auth_code:
+    :param app_id:
+    :param app_secret:
+    :param grant_type: 请求的类型，可选值：authorization_code（授权码方式获取 token）、refresh_token（刷新 token）
+    :param refresh_token:
+    :param redirect_uri:
+    :return:
+    """
+    redirect_uri = f'{redirect_uri}?app_id={app_id}'
+
+    url = 'https://api.e.qq.com/oauth/token'
+    params = {
+        'client_id': app_id,
+        'client_secret': app_secret,
+        'grant_type': grant_type
+    }
+    if auth_code:
+        params['authorization_code'] = auth_code
+    if refresh_token:
+        params['refresh_token'] = refresh_token
+    if redirect_uri:
+        params['redirect_uri'] = redirect_uri
+
+    for k in params:
+        if type(params[k]) is not str:
+            params[k] = json.dumps(params[k])
+
+    return lazyrequests.lazy_requests(
+        method="GET",
+        url=url,
+        params=params
+    )
+
+
+def oauth_token3(
         access_token,
         app_id,
         app_secret,
+        redirect_uri,
         grant_type='authorization_code',
         auth_code=None,
         refresh_token=None,
-        redirect_uri=None
 ):
     """
     获取/刷新token
     相关文档：https://developers.e.qq.com/v3.0/docs/api/oauth/token
     :param access_token:
     :param auth_code:
     :param app_id:
     :param app_secret:
     :param grant_type: 请求的类型，可选值：authorization_code（授权码方式获取 token）、refresh_token（刷新 token）
     :param refresh_token:
-    :param redirect_uri:
+    :param redirect_uri: 回调地址
     :return:
     """
-    if grant_type and not redirect_uri:
-        redirect_uri = f'https://open.fanshang888.com/api/cache/receive/open_api/ad/ad_developer/qq/callback?app_id={app_id}'
-
+    redirect_uri = f'{redirect_uri}?app_id={app_id}'
     url = 'https://api.e.qq.com/v3.0/oauth/token'
     params = {
         'access_token': access_token,
         'timestamp': int(time.time()),
         'nonce': make_nonce,
 
         'client_id': app_id,
```

### Comparing `lazyad-0.0.7/lazyad.egg-info/PKG-INFO` & `lazyad-0.0.8/lazyad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.7
+Version: 0.0.8
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.7/setup.py` & `lazyad-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazyad",
-    version="0.0.7",
+    version="0.0.8",
     description="基于Python的懒人包-适用于广告投放模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazyad",
     packages=setuptools.find_packages(),
```

