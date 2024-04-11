# Comparing `tmp/migoapiclient-1.0.8.tar.gz` & `tmp/migoapiclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.0.8.tar", last modified: Wed Apr  3 09:52:30 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.0.tar", last modified: Wed Apr 10 09:46:43 2024, max compression
```

## Comparing `migoapiclient-1.0.8.tar` & `migoapiclient-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:52:30.144523 migoapiclient-1.0.8/
--rw-rw-rw-   0        0        0     3900 2024-04-03 09:52:30.144523 migoapiclient-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:52:30.141522 migoapiclient-1.0.8/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.0.8/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    10123 2024-04-03 09:52:01.000000 migoapiclient-1.0.8/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.0.8/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:52:30.144523 migoapiclient-1.0.8/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-03 09:52:30.000000 migoapiclient-1.0.8/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 09:52:30.000000 migoapiclient-1.0.8/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:52:30.000000 migoapiclient-1.0.8/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 09:52:30.000000 migoapiclient-1.0.8/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:52:30.145498 migoapiclient-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-03 09:52:27.000000 migoapiclient-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:52:30.143520 migoapiclient-1.0.8/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:46:43.514027 migoapiclient-1.1.0/
+-rw-rw-rw-   0        0        0     3900 2024-04-10 09:46:43.511028 migoapiclient-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 09:46:43.500249 migoapiclient-1.1.0/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.0/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    10393 2024-04-10 09:40:33.000000 migoapiclient-1.1.0/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.0/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:46:43.510050 migoapiclient-1.1.0/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-10 09:46:43.000000 migoapiclient-1.1.0/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-10 09:46:43.000000 migoapiclient-1.1.0/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 09:46:43.000000 migoapiclient-1.1.0/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-10 09:46:43.000000 migoapiclient-1.1.0/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 09:46:43.514027 migoapiclient-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-10 09:33:04.000000 migoapiclient-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:46:43.506063 migoapiclient-1.1.0/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.0/src/__init__.py
```

### Comparing `migoapiclient-1.0.8/PKG-INFO` & `migoapiclient-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.8
+Version: 1.1.0
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.8/README.md` & `migoapiclient-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.8/migoapiclient/api_client.py` & `migoapiclient-1.1.0/migoapiclient/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
                     url,
                     kwargs.get('headers', ''),
                     kwargs.get('params', ''),
                     kwargs.get('json', {}),
                     response_data.get('message', ''),
                 )
                 self.log_manager.write_request_error_log(msg)
+                raise Exception(msg)
             return response_data
         except Exception as e:
             msg = ERROR_MSG.format(
                 now_datetime,
                 url,
                 kwargs.get('headers', ''),
                 kwargs.get('params', ''),
@@ -147,25 +148,29 @@
         """
         获取店铺授权信息
         :param migo_shop_id 米果店铺ID
         """
         uri = f'/data-collection-service/node/auths/{migo_shop_id}'
         return self.try_get(self.host + uri)
 
-    def get_node_info_list(self, migo_shop_id: int):
+    def get_node_info_list(self, migo_shop_id: int = None):
         """
         获取节点信息列表
         :param migo_shop_id 米果店铺ID
         """
         post_data = {
-            "nodeConfigId": self.node_id,
-            "shopId": migo_shop_id
+            "nodeConfigId": self.node_id
         }
+        if migo_shop_id:
+            post_data['shopId'] = migo_shop_id
         uri = f'/data-collection-service/node/search'
-        return self.try_post(self.host + uri, json=post_data)
+        response_data = self.try_post(self.host + uri, json=post_data)
+        if migo_shop_id:
+            response_data['data'] = response_data['data'][0]  # 如果是查询单个店铺的话，数据解析成字典
+        return response_data
 
     def post_auth_data(self, migo_shop_id, **kwargs):
         """
         刷新认证数据
         :param migo_shop_id 米果店铺ID
         :param kwargs 所需的认证参数
         """
```

### Comparing `migoapiclient-1.0.8/migoapiclient/file_manager.py` & `migoapiclient-1.1.0/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.8/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.0/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.8
+Version: 1.1.0
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.8/setup.py` & `migoapiclient-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.0.8'
+VERSION = '1.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

