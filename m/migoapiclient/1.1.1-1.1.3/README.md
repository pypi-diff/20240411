# Comparing `tmp/migoapiclient-1.1.1.tar.gz` & `tmp/migoapiclient-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.1.tar", last modified: Thu Apr 11 02:08:48 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.3.tar", last modified: Thu Apr 11 09:16:35 2024, max compression
```

## Comparing `migoapiclient-1.1.1.tar` & `migoapiclient-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 02:08:48.433237 migoapiclient-1.1.1/
--rw-rw-rw-   0        0        0     3900 2024-04-11 02:08:48.432237 migoapiclient-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 02:08:48.429241 migoapiclient-1.1.1/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.1/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    10948 2024-04-11 01:44:17.000000 migoapiclient-1.1.1/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.1/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:08:48.432237 migoapiclient-1.1.1/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-11 02:08:48.000000 migoapiclient-1.1.1/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-11 02:08:48.000000 migoapiclient-1.1.1/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 02:08:48.000000 migoapiclient-1.1.1/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 02:08:48.000000 migoapiclient-1.1.1/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 02:08:48.433237 migoapiclient-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-11 02:08:19.000000 migoapiclient-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:08:48.431238 migoapiclient-1.1.1/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/
+-rw-rw-rw-   0        0        0     3900 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.783522 migoapiclient-1.1.3/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.3/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    11016 2024-04-11 09:09:30.000000 migoapiclient-1.1.3/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.3/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.785522 migoapiclient-1.1.3/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 09:16:35.000000 migoapiclient-1.1.3/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:16:35.786522 migoapiclient-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-11 09:14:34.000000 migoapiclient-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:16:35.785522 migoapiclient-1.1.3/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.3/src/__init__.py
```

### Comparing `migoapiclient-1.1.1/PKG-INFO` & `migoapiclient-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.1
+Version: 1.1.3
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.1/README.md` & `migoapiclient-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.1/migoapiclient/api_client.py` & `migoapiclient-1.1.3/migoapiclient/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from datetime import datetime
 
 from dateutil.tz import tz
+from requests import Response
 
 from .file_manager import LogFileManager
 import time
 import requests
 
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
@@ -29,37 +30,49 @@
         """
         super(ApiClient, self).__init__()
         self.retry_count = retry_count
         self.node_id = node_id
         self.timeout = timeout
         self.host = host
 
+    def res_callback(self, res_data: Response):
+        """
+        响应回调
+        :param res_data 响应数据
+        """
+        return res_data
+
     def try_get(self, url, error_count: int = 0, **kwargs):
         """
         尝试重发get请求
         """
         while error_count <= self.retry_count:
             try:
                 kwargs['timeout'] = self.timeout
-                return self.get(url, **kwargs)
+                res_data = self.get(url, **kwargs)
+                return self.res_callback(res_data)
             except Exception as e:
                 print(e)
+                time.sleep(error_count)
                 error_count += 1
                 return self.try_get(url, error_count, **kwargs)
+        raise Exception('已经尝试请求：{}次，服务器依然没有响应'.format(self.retry_count))
 
     def try_post(self, url: str, error_count: int = 0, **kwargs):
         """
         尝试重发post请求
         """
         while error_count <= self.retry_count:
             try:
                 kwargs['timeout'] = self.timeout
-                return self.post(url, **kwargs)
+                res_data = self.post(url, **kwargs)
+                return self.res_callback(res_data)
             except Exception as e:
                 print(e)
+                time.sleep(error_count)
                 error_count += 1
                 time.sleep(error_count)
                 return self.try_post(url, error_count, **kwargs)
         raise Exception('已经尝试请求：{}次，服务器依然没有响应'.format(self.retry_count))
 
 
 class MigoApiClient(ApiClient):
@@ -78,96 +91,74 @@
         self.headers = {
             'AUTH-KEY': auth_key,
             'CURRENT-USER-NAME': 'system',
             'CURRENT-USER-ID': '100001'
         }
         self.log_manager = LogFileManager(log_path)
 
-    def try_post(self, url, error_count: int = 0, **kwargs):
-        now_datetime = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+    def res_callback(self, response_data: dict):
+        """
+        响应回调
+        """
+        if response_data['code'] != 200:
+            raise Exception(response_data['message'])
+        return response_data
+
+    def migo_try_get(self, url, migo_shop_id, data_type: str, error_count: int = 0, **kwargs):
+        """
+        自定义发get请求
+        :param url 链接
+        :param migo_shop_id 米果店铺ID
+        :param data_type 数据类型
+        :param error_count 重试次数
+        """
         try:
-            kwargs['headers'] = kwargs.get('headers', dict())
-            kwargs['headers'].update(self.headers)
-            response = super(MigoApiClient, self).try_post(url, error_count, **kwargs)
-            response_data = response.json()
-            if response_data and response_data['code'] != 200:
-                msg = ERROR_MSG.format(
-                    now_datetime,
-                    url,
-                    kwargs.get('headers', ''),
-                    kwargs.get('params', ''),
-                    kwargs.get('json', {}),
-                    response_data.get('message', ''),
-                )
-                self.log_manager.write_request_error_log(msg)
-                raise Exception(msg)
-            return response_data
+            return self.try_get(url, error_count, **kwargs)
         except Exception as e:
-            msg = ERROR_MSG.format(
-                now_datetime,
-                url,
-                kwargs.get('headers', ''),
-                kwargs.get('params', ''),
-                kwargs.get('json', ''),
-                str(e)
-            )
-            self.log_manager.write_system_error_log(msg)
+            log_params = kwargs.get('params', {})
+            log_data = kwargs['json'] if kwargs.get('json', {}) else kwargs.get('data', {})
+            self.post_error_log(str(e), data_type, migo_shop_id, log_data, log_params)
             raise e
 
-    def try_get(self, url, error_count: int = 0, **kwargs):
-        now_datetime = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+    def migo_try_post(self, url, migo_shop_id, data_type: str, error_count: int = 0, **kwargs):
+        """
+        自定义发post请求
+        :param url 链接
+        :param migo_shop_id 米果店铺ID
+        :param data_type 数据类型
+        :param error_count 重试次数
+        """
         try:
-            kwargs['headers'] = kwargs.get('headers', dict())
-            kwargs['headers'].update(self.headers)
-            response = super(MigoApiClient, self).try_get(url, error_count, **kwargs)
-            response_data = response.json()
-            if response_data and response_data['code'] != 200:
-                msg = ERROR_MSG.format(
-                    now_datetime,
-                    url,
-                    kwargs.get('headers', ''),
-                    kwargs.get('params', ''),
-                    kwargs.get('json', {}),
-                    response_data.get('message', ''),
-                )
-                self.log_manager.write_request_error_log(msg)
-                raise Exception(msg)
-            return response_data
+            return self.try_post(url, error_count, **kwargs)
         except Exception as e:
-            msg = ERROR_MSG.format(
-                now_datetime,
-                url,
-                kwargs.get('headers', ''),
-                kwargs.get('params', ''),
-                kwargs.get('json', ''),
-                str(e)
-            )
-            self.log_manager.write_system_error_log(msg)
-            raise Exception(msg)
+            log_params = kwargs.get('params', {})
+            log_data = kwargs['json'] if kwargs.get('json', {}) else kwargs.get('data', {})
+            self.post_error_log(str(e), data_type, migo_shop_id, log_data, log_params)
+            raise e
 
     def get_shop_auth(self, migo_shop_id: int):
         """
         获取店铺授权信息
         :param migo_shop_id 米果店铺ID
         """
         uri = f'/data-collection-service/node/auths/{migo_shop_id}'
-        return self.try_get(self.host + uri)
+        return self.migo_try_get(self.host + uri, migo_shop_id, '获取店铺授权信息')
 
     def get_node_info_list(self, migo_shop_id: int = None):
         """
         获取节点信息列表
         :param migo_shop_id 米果店铺ID
         """
         post_data = {
             "nodeConfigId": self.node_id
         }
         if migo_shop_id:
             post_data['shopId'] = migo_shop_id
         uri = f'/data-collection-service/node/search'
-        response_data = self.try_post(self.host + uri, json=post_data)
+        response_data = self.migo_try_post(self.host + uri, migo_shop_id, '获取节点信息列表', json=post_data)
         if migo_shop_id:
             response_data['data'] = response_data['data'][0]  # 如果是查询单个店铺的话，数据解析成字典
         return response_data
 
     def post_auth_data(self, migo_shop_id, **kwargs):
         """
         刷新认证数据
@@ -176,15 +167,15 @@
         """
         post_data = {
             "crawlData": json.dumps(kwargs),
             "nodeConfigId": self.node_id,
             "shopId": migo_shop_id
         }
         uri = '/data-collection-service/node/refresh'
-        return self.try_post(self.host + uri, json=post_data)
+        return self.migo_try_post(self.host + uri, migo_shop_id, '刷新认证数据', json=post_data)
 
     def post_crawl_data(self, crawl_data: dict, data_type: str, migo_shop_id: str):
         """
         推送采集数据
         :param crawl_data 采集数据
         :param data_type 业务类型，订单或物流或其他
         :param migo_shop_id 店铺ID
@@ -192,64 +183,75 @@
         uri = '/data-collection-service/node/save'
         # 自动修正丢失的店铺ID
         if 'shopId' not in crawl_data:
             crawl_data['shopId'] = migo_shop_id
 
         if 'tableName' not in crawl_data:
             msg = '表名不能为空'
-            self.post_error_log(msg, data_type, self.node_id, migo_shop_id, crawl_data)
+            self.post_error_log(msg, data_type, migo_shop_id, crawl_data)
             raise Exception(msg)
-        return self.try_post(self.host + uri, json=crawl_data)
+        return self.migo_try_post(self.host + uri, migo_shop_id, data_type + '推送采集数据', 0, json=crawl_data)
 
     def get_heartbeat(self):
         """
         发送心跳
         """
         uri = f'/data-collection-service/node/heartbeat/{self.node_id}'
         return self.try_get(self.host + uri, error_count=0)
 
-    def post_error_log(self, error_msg: str, data_type: str, node_id: str, shop_id: str, log_data: dict = None,
+    def post_error_log(self, error_msg: str, data_type: str, shop_id: str, log_data: dict = None,
                        log_params: dict = None, log_stack: str = None):
         """
-        上传日志
+        上传日志，如果上传失败就写入到本地日志中
         :param error_msg 错误信息
         :param data_type 数据类型
-        :param node_id 节点ID
         :param shop_id 店铺ID
         :param log_data 请求的post参数
         :param log_params 请求的get参数
         :param log_stack 日志其他信息
         """
         uri = '/data-collection-service/node/logsave'
         post_data = {
             "data": [
                 {
                     "id": str(time.time()).replace('.', ''),
                     "shopId": shop_id,
-                    "nodeId": node_id,
+                    "nodeId": self.node_id,
                     "dataType": data_type,
                     "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
                     "logData": json.dumps(log_data),
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": error_msg
                 }
             ],
             "primaryKey": "id",
             "refreshNow": 0,
             "tableName": "log_node_spider_error"
         }
-        response_data = self.try_post(self.host + uri, 0, json=post_data)
-        return response_data
+        try:
+            res_data = self.try_post(self.host + uri, 0, json=post_data)
+            return res_data
+        except Exception as e:
+            msg = ERROR_MSG.format(
+                datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+                self.host + uri,
+                self.headers,
+                '',
+                post_data,
+                str(e),
+            )
+            self.log_manager.write_request_error_log(msg)
+            raise e
 
     def post_info_log(self, msg: str, data_type: str, node_id: str, shop_id: str, log_data: dict = None,
                       log_params: dict = None, log_stack: str = None):
         """
         上传日志
-        :param msg 错误信息
+        :param msg 信息
         :param data_type 数据类型
         :param node_id 节点ID
         :param shop_id 店铺ID
         :param log_data 请求的post参数
         :param log_params 请求的get参数
         :param log_stack 日志其他信息
         """
@@ -268,24 +270,23 @@
                     "logMsg": msg
                 }
             ],
             "primaryKey": "id",
             "refreshNow": 0,
             "tableName": "log_node_spider"
         }
-        response_data = self.try_post(self.host + uri, 0, json=post_data)
-        return response_data
+        return self.migo_try_post(self.host + uri, shop_id, '上传日志', 0, json=post_data)
 
     def post_node_es_query(self, column_list: list, table_name: str, es_query: dict):
         """
         根据es语法获取节点信息
         :param column_list 字段名
         :param table_name 表名
         :param es_query es查询语句
         """
         uri = '/data-collection-service/node/es/query'
         post_data = {
             'sourceStrings': column_list,
             'queryString': json.dumps(es_query),
             'indexName': table_name
         }
-        return self.try_post(self.host + uri, 0, json=post_data)
+        return self.migo_try_post(self.host + uri, 0, '获取节点信息', 0, json=post_data)
```

### Comparing `migoapiclient-1.1.1/migoapiclient/file_manager.py` & `migoapiclient-1.1.3/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.1/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.3/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.1
+Version: 1.1.3
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.1/setup.py` & `migoapiclient-1.1.3/setup.py`

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
-VERSION = '1.1.1'
+VERSION = '1.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

