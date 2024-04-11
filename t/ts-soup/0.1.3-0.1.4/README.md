# Comparing `tmp/ts-soup-0.1.3.tar.gz` & `tmp/ts-soup-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-j1z64cs_\ts-soup-0.1.3.tar", last modified: Thu Apr 11 08:52:20 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-exlwxpyl\ts-soup-0.1.4.tar", last modified: Thu Apr 11 09:07:03 2024, max compression
```

## Comparing `ts-soup-0.1.3.tar` & `ts-soup-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 08:52:20.711168 ts-soup-0.1.3/
--rw-rw-rw-   0        0        0     1028 2024-04-11 08:52:20.710167 ts-soup-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 08:52:20.711168 ts-soup-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-11 08:51:38.000000 ts-soup-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:52:20.696927 ts-soup-0.1.3/ts_soup/
--rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts-soup-0.1.3/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.1.3/ts_soup/app.py
--rw-rw-rw-   0        0        0    15528 2024-04-09 06:42:47.000000 ts-soup-0.1.3/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:52:20.707625 ts-soup-0.1.3/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.1.3/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3692 2024-04-11 08:50:44.000000 ts-soup-0.1.3/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     4330 2024-04-11 08:50:44.000000 ts-soup-0.1.3/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:52:20.708627 ts-soup-0.1.3/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-11 08:52:20.000000 ts-soup-0.1.3/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-11 08:52:20.000000 ts-soup-0.1.3/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 08:52:20.000000 ts-soup-0.1.3/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 08:52:20.000000 ts-soup-0.1.3/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 09:07:03.658453 ts-soup-0.1.4/
+-rw-rw-rw-   0        0        0     1028 2024-04-11 09:07:03.657452 ts-soup-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:07:03.658453 ts-soup-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-11 09:06:42.000000 ts-soup-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:07:03.645352 ts-soup-0.1.4/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts-soup-0.1.4/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.1.4/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15530 2024-04-11 09:01:36.000000 ts-soup-0.1.4/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:07:03.653692 ts-soup-0.1.4/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.1.4/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-11 09:01:36.000000 ts-soup-0.1.4/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     4331 2024-04-11 09:01:36.000000 ts-soup-0.1.4/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:07:03.656016 ts-soup-0.1.4/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-11 09:07:03.000000 ts-soup-0.1.4/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-11 09:07:03.000000 ts-soup-0.1.4/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:07:03.000000 ts-soup-0.1.4/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 09:07:03.000000 ts-soup-0.1.4/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.1.3/PKG-INFO` & `ts-soup-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.3
+Version: 0.1.4
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.1.3/README.md` & `ts-soup-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.3/setup.py` & `ts-soup-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.3",
+  version="0.1.4",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.1.3/ts_soup/app.py` & `ts-soup-0.1.4/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.3/ts_soup/common.py` & `ts-soup-0.1.4/ts_soup/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     @abstractmethod
     def build_source(self, to_update_date):
         """
         :param to_update_date:
         :return: yyyy-mm-dd 格式日期列表
         """
-        ...
+        pass
 
 
 class BaseTarget(ABC):
     """
     定义需要使用在入口函数中注册的数据库连接的target的基类，即 如果需要使用数据库连接，则需要继承BaseTarget
     """
     def __init__(self,db: str = None):
@@ -188,15 +188,15 @@
 
     @abstractmethod
     def build_output(self, cur_result):
         """
         :param to_update_date:
         :return: yyyy-mm-dd 格式日期列表
         """
-        ...
+        pass
 
 
 class Executor:
     """
     数据处理原则：
         n2one: 数据源配置为is_data=True的对应日期查询结果只要存在一个全为空，则视当天的所有数据都为空，不更新数据表，也不更新操作记录表(updated_state)
         one2n:
```

### Comparing `ts-soup-0.1.3/ts_soup/workers/sources.py` & `ts-soup-0.1.4/ts_soup/workers/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ts_soup.common import query_in_sql,BaseSource
 
 
 class Source(BaseSource):
     def __init__(self,
                  tb: str,
                  db: str = None,
-                 empty_check=False,
+                 empty_check=True,
                  query_field: str = '*',
                  index_field='date',
                  other_condition: str = None):
         """
         单表查询数据源信息
         :param tb: 数据表名
         :param db: 数据库名
@@ -37,15 +37,15 @@
 class MultiSource(BaseSource):
     """
     多数据源联合查询时使用
     """
     def __init__(self,
                  relations: list,
                  db: str=None ,
-                 empty_check=False,
+                 empty_check=True,
                  index_field='date'):
         """
         :param relations:连接条件模板如下：
         {'left':'','right':'','l_on':'','r_on':'','how':'','lquery_field':'','rquery_field':' ','l_cons':'','r_cons':''},
         :param db:
         :param empty_check:
         :param index_field:
@@ -64,15 +64,15 @@
             join_stm+=f"{rel['how']} join {rel['right']} on {rel['left']}.{rel['l_on']}={rel['right']}.{rel['r_on']} "
             where_clause += (f" and {rel['left']+'.'+rel['l_cons']}" if rel['l_cons']!='' else '')+(f"and {rel['right']+'.'+rel['r_cons']}" if rel['r_cons']!='' else '')
         base_sql = f'select {",".join(query_params)} from {self.relations[0]["left"]} {join_stm} where 1=1 {where_clause} and {self.index_field} in ({query_in_sql(to_update_date)})'
         return pd.read_sql(base_sql,con=self.db)
 
 
 class RawSqlSource(BaseSource):
-    def __init__(self,  index_field,sql,db:str=None, empty_check=False):
+    def __init__(self,  index_field,sql,db:str=None, empty_check=True):
         """
         直接使用sql的源
         :param db:
         :param index_field:
         :param empty_check:
         :param sql:
         """
```

### Comparing `ts-soup-0.1.3/ts_soup/workers/targets.py` & `ts-soup-0.1.4/ts_soup/workers/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, tb,
                  db: str = None,
                  index_field: str = 'date',
                  drop_axis=0,
                  drop_na_subset=None,
                  drop_na_thresh=2,
                  has_unique_idx=False,
-                 drop_na_when_insert_date=True
+                 drop_na_when_insert_date=False
                  ):
         """
         目标表信息，如果该表需要分表，则tb传入没有分表年份的表名，年份在写入时会自动加入，同时is_seperated设置为True
         :param tb:表名，
         :param db:数据库
         :param index_field:作为索引的字段，一般为日期
         :param drop_axis:如果存在空数据，drop_na的轴
```

### Comparing `ts-soup-0.1.3/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.1.4/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.3
+Version: 0.1.4
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

