# Comparing `tmp/mockee-0.3.2.tar.gz` & `tmp/mockee-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mockee-0.3.2.tar", last modified: Tue Dec  1 03:02:29 2020, max compression
+gzip compressed data, was "dist\mockee-0.4.0.tar", last modified: Thu Apr 11 03:20:26 2024, max compression
```

## Comparing `mockee-0.3.2.tar` & `mockee-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-12-01 03:02:29.000000 mockee-0.3.2/
--rw-rw-rw-   0        0        0       46 2020-11-27 03:21:07.000000 mockee-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8548 2020-12-01 03:02:29.000000 mockee-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6192 2020-11-27 07:19:42.000000 mockee-0.3.2/README.md
--rw-rw-rw-   0        0        0       27 2020-11-06 02:27:16.000000 mockee-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0      947 2020-12-01 03:02:29.000000 mockee-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      236 2020-11-26 01:49:35.000000 mockee-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-01 03:02:29.000000 mockee-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee/
--rw-rw-rw-   0        0        0       53 2020-12-01 03:02:26.000000 mockee-0.3.2/src/mockee/__init__.py
--rw-rw-rw-   0        0        0     1081 2020-12-01 03:00:15.000000 mockee-0.3.2/src/mockee/mockee.py
--rw-rw-rw-   0        0        0    10782 2020-12-01 03:00:04.000000 mockee-0.3.2/src/mockee/resolver.py
-drwxrwxrwx   0        0        0        0 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee.egg-info/
--rw-rw-rw-   0        0        0     8548 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-12-01 03:02:29.000000 mockee-0.3.2/src/mockee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:26.000000 mockee-0.4.0/
+-rw-rw-rw-   0        0        0       46 2024-04-11 03:10:40.000000 mockee-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8742 2024-04-11 03:20:26.000000 mockee-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6354 2024-04-11 03:10:40.000000 mockee-0.4.0/README.md
+-rw-rw-rw-   0        0        0       27 2024-04-11 03:20:04.000000 mockee-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0      947 2024-04-11 03:20:26.000000 mockee-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      232 2024-04-11 03:10:40.000000 mockee-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:26.000000 mockee-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee/
+-rw-rw-rw-   0        0        0      962 2024-04-11 03:10:40.000000 mockee-0.4.0/src/mockee/mockee.py
+-rw-rw-rw-   0        0        0    10950 2024-04-11 03:10:40.000000 mockee-0.4.0/src/mockee/resolver.py
+-rw-rw-rw-   0        0        0       28 2024-04-11 03:10:40.000000 mockee-0.4.0/src/mockee/__init__.py
+-rw-rw-rw-   0        0        0      107 2024-04-11 03:10:40.000000 mockee-0.4.0/src/mockee/__meta__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8742 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 03:20:26.000000 mockee-0.4.0/src/mockee.egg-info/top_level.txt
```

### Comparing `mockee-0.3.2/PKG-INFO` & `mockee-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockee
-Version: 0.3.2
+Version: 0.4.0
 Summary: Mock data(JSON) generator for Python3
 Home-page: https://gitee.com/hyjiacan/mockee
 Author: hyjiacan
 Author-email: hyjiacan@163.com
 Maintainer: hyjiacan
 Maintainer-email: hyjiacan@163.com
 License: MIT
@@ -60,15 +60,15 @@
             "len": 10
           }
         }
         ```
         
         - `GET:/api/test` 数据标识
         - `def` 描述返回的字段集合
-        - `len` 描述返回的数组长度，不指定或值为 `0` 时返回对象
+        - `len` 描述返回的数组长度，值为 `0` 时返回对象
         
         > 包含 `GET:/api/test` 的叫做 **入口定义文件**
         
         ### 表达式
         
         格式：`#>(i|f|b|s|j|d|t|dt|ref) exp`
         
@@ -140,18 +140,22 @@
         
         `enum-filename` 为枚举文件名，其中每行存放一个数据项，其中不允许出现空行。
         
         > 无论是范围还是枚举，值不允许出现空白字符
         
         #### JSON类型
         
-        可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取数据项。
+        可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取所有数据。
         
         - `j` 表示此字段的值是一个JSON结构
         - `json.json` 是要读取的文件名。**注意：json文件的扩展名必须为 `.json`**
+        - `json.json` 文件的根可以是对象或者数组
+        
+        也可以使用 `#>j (#json.json#)` 这样的写法，指定从一个 JSON 文件(数组)中随机选择数据
+        
         - `json.json` 文件的根必须是数组
         
         > 此类型仅支持从文件读取。 
         
         #### 引用类型
         
         使用写法 `#>ref datetime.json` 以引入一个外部的数据结构定义。
```

### Comparing `mockee-0.3.2/README.md` & `mockee-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "len": 10
   }
 }
 ```
 
 - `GET:/api/test` 数据标识
 - `def` 描述返回的字段集合
-- `len` 描述返回的数组长度，不指定或值为 `0` 时返回对象
+- `len` 描述返回的数组长度，值为 `0` 时返回对象
 
 > 包含 `GET:/api/test` 的叫做 **入口定义文件**
 
 ### 表达式
 
 格式：`#>(i|f|b|s|j|d|t|dt|ref) exp`
 
@@ -127,18 +127,22 @@
 
 `enum-filename` 为枚举文件名，其中每行存放一个数据项，其中不允许出现空行。
 
 > 无论是范围还是枚举，值不允许出现空白字符
 
 #### JSON类型
 
-可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取数据项。
+可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取所有数据。
 
 - `j` 表示此字段的值是一个JSON结构
 - `json.json` 是要读取的文件名。**注意：json文件的扩展名必须为 `.json`**
+- `json.json` 文件的根可以是对象或者数组
+
+也可以使用 `#>j (#json.json#)` 这样的写法，指定从一个 JSON 文件(数组)中随机选择数据
+
 - `json.json` 文件的根必须是数组
 
 > 此类型仅支持从文件读取。 
 
 #### 引用类型
 
 使用写法 `#>ref datetime.json` 以引入一个外部的数据结构定义。
```

### Comparing `mockee-0.3.2/setup.cfg` & `mockee-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mockee-0.3.2/src/mockee/mockee.py` & `mockee-0.4.0/src/mockee/mockee.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,34 +4,32 @@
 
 from .resolver import Resolver
 
 
 class Mockee:
     CACHE = {}
 
-    def __init__(self, def_file: str, encoding='utf8', use_cache=True):
+    def __init__(self, def_file: str, encoding='utf8'):
         self.def_file = os.path.abspath(def_file)
         self.encoding = encoding
-        self.use_cache = use_cache
 
     def load(self):
         """
         从文件加载定义
         :return:
         """
         with open(self.def_file, encoding=self.encoding, mode='r') as fp:
             self.CACHE[self.def_file] = json.load(fp)
 
     @property
     def mock_data(self) -> dict:
-        if not self.use_cache or self.def_file not in self.CACHE:
+        if self.def_file not in self.CACHE:
             self.load()
 
         return self.CACHE[self.def_file]
 
     def make(self, data_id: str, options: dict) -> [Optional[dict], Optional[list]]:
         if data_id not in self.mock_data:
             return None
 
-        resolver = Resolver(self.mock_data[data_id], os.path.dirname(self.def_file), self.encoding,
-                            self.use_cache, options)
+        resolver = Resolver(self.mock_data[data_id], os.path.dirname(self.def_file), self.encoding, options)
         return resolver.resolve()
```

### Comparing `mockee-0.3.2/src/mockee/resolver.py` & `mockee-0.4.0/src/mockee/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 import time
 
 
 class Resolver:
     # 选择项文件缓存
     CHOICES_CACHE = {}
 
-    def __init__(self, defs: dict, def_dir: str, encoding: str, use_cache: bool, options: dict):
+    def __init__(self, defs: dict, def_dir: str, encoding: str, options: dict):
         self.defs = defs['def']
         self.def_dir = def_dir
         self.encoding = encoding
-        self.use_cache = use_cache
         self.options = options
         # 需要生成的数据长度
         # 0 表示返回单个对象
-        self.data_length = int(defs['len']) if 'len' in defs else 0
+        self.data_length = int(defs['len'])
         # 自增长整数基数
         self.i_base = options['i_base'] if 'i_base' in options else 0
         # 当需要返回多个数据时，当前数据的索引
         self.data_index = 0
         self.date_range = self.resolve_date_range()
         self.date_steps = {}
         self.resolve_date_step(self.data_length)
@@ -67,15 +66,15 @@
         if offset is None:
             offset = self.data_index
         return self.date_range[0] + self.date_steps[length] * offset
 
     def load_file(self, filename):
         abs_filename = os.path.abspath(os.path.join(self.def_dir, filename))
 
-        if self.use_cache and abs_filename in self.CHOICES_CACHE:
+        if abs_filename in self.CHOICES_CACHE:
             return self.CHOICES_CACHE[abs_filename]
 
         with open(abs_filename, encoding=self.encoding, mode='r') as fp:
             if filename.endswith('.json'):
                 import json
                 self.CHOICES_CACHE[abs_filename] = json.load(fp)
             else:
@@ -228,15 +227,21 @@
 
         # 引用定义文件
         if data_type == 'ref':
             return self.resolve_data(self.load_file(exp))
 
         # JSON值选择文件
         if data_type == 'j':
-            return self.get_json_value(self.load_file(exp))
+            if exp.startswith('(#') and exp.endswith('#)'):
+                # 从文件加载数据(选择其中一部分)
+                data = self.load_file(exp[2:-2])
+                return self.get_json_value(data)
+
+            # 从文件加载数据，使用整个数据
+            return self.load_file(exp)
 
         if data_type == 'i' and exp == 'auto':
             return self.next_int(offset)
 
         if exp is not None:
             if exp.startswith('(#') and exp.endswith('#)'):
                 # 从文件加载枚举
```

### Comparing `mockee-0.3.2/src/mockee.egg-info/PKG-INFO` & `mockee-0.4.0/src/mockee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockee
-Version: 0.3.2
+Version: 0.4.0
 Summary: Mock data(JSON) generator for Python3
 Home-page: https://gitee.com/hyjiacan/mockee
 Author: hyjiacan
 Author-email: hyjiacan@163.com
 Maintainer: hyjiacan
 Maintainer-email: hyjiacan@163.com
 License: MIT
@@ -60,15 +60,15 @@
             "len": 10
           }
         }
         ```
         
         - `GET:/api/test` 数据标识
         - `def` 描述返回的字段集合
-        - `len` 描述返回的数组长度，不指定或值为 `0` 时返回对象
+        - `len` 描述返回的数组长度，值为 `0` 时返回对象
         
         > 包含 `GET:/api/test` 的叫做 **入口定义文件**
         
         ### 表达式
         
         格式：`#>(i|f|b|s|j|d|t|dt|ref) exp`
         
@@ -140,18 +140,22 @@
         
         `enum-filename` 为枚举文件名，其中每行存放一个数据项，其中不允许出现空行。
         
         > 无论是范围还是枚举，值不允许出现空白字符
         
         #### JSON类型
         
-        可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取数据项。
+        可以使用 `#>j json.json` 这样的写法来指定从一个 JSON 文件中读取所有数据。
         
         - `j` 表示此字段的值是一个JSON结构
         - `json.json` 是要读取的文件名。**注意：json文件的扩展名必须为 `.json`**
+        - `json.json` 文件的根可以是对象或者数组
+        
+        也可以使用 `#>j (#json.json#)` 这样的写法，指定从一个 JSON 文件(数组)中随机选择数据
+        
         - `json.json` 文件的根必须是数组
         
         > 此类型仅支持从文件读取。 
         
         #### 引用类型
         
         使用写法 `#>ref datetime.json` 以引入一个外部的数据结构定义。
```

