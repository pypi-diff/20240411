# Comparing `tmp/pyco-types-1.1.6.tar.gz` & `tmp/pyco-types-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyco-types-1.1.6.tar", last modified: Thu Feb 29 09:56:02 2024, max compression
+gzip compressed data, was "dist/pyco-types-1.1.7.tar", last modified: Thu Apr 11 04:38:10 2024, max compression
```

## Comparing `pyco-types-1.1.6.tar` & `pyco-types-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-02-29 09:56:02.086116 pyco-types-1.1.6/
--rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.6/LICENSE.txt
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-02-29 09:56:02.085665 pyco-types-1.1.6/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)       42 2023-09-11 08:05:54.000000 pyco-types-1.1.6/README.md
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-02-29 09:56:02.082740 pyco-types-1.1.6/pyco_types/
--rw-r--r--   0 nico       (502) staff       (20)      327 2023-09-13 03:32:10.000000 pyco-types-1.1.6/pyco_types/__init__.py
--rw-r--r--   0 nico       (502) staff       (20)     3709 2024-01-05 13:47:40.000000 pyco-types-1.1.6/pyco_types/_common.py
--rw-r--r--   0 nico       (502) staff       (20)     2109 2024-01-05 13:12:01.000000 pyco-types-1.1.6/pyco_types/_convert_meta.py
--rw-r--r--   0 nico       (502) staff       (20)     3577 2024-01-05 10:16:54.000000 pyco-types-1.1.6/pyco_types/_factory.py
--rw-r--r--   0 nico       (502) staff       (20)      165 2024-02-29 09:55:13.000000 pyco-types-1.1.6/pyco_types/_version.py
--rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.6/pyco_types/co_datetime.py
--rw-r--r--   0 nico       (502) staff       (20)     2539 2024-01-05 13:11:22.000000 pyco-types-1.1.6/pyco_types/co_dict.py
--rw-r--r--   0 nico       (502) staff       (20)     3865 2024-01-01 06:15:00.000000 pyco-types-1.1.6/pyco_types/co_integer.py
--rw-r--r--   0 nico       (502) staff       (20)     3755 2024-01-05 13:43:50.000000 pyco-types-1.1.6/pyco_types/co_json.py
--rw-r--r--   0 nico       (502) staff       (20)     5156 2023-09-10 03:46:01.000000 pyco-types-1.1.6/pyco_types/co_regex.py
--rw-r--r--   0 nico       (502) staff       (20)     6473 2024-01-02 13:02:23.000000 pyco-types-1.1.6/pyco_types/const.py
-drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-02-29 09:56:02.085084 pyco-types-1.1.6/pyco_types.egg-info/
--rw-r--r--   0 nico       (502) staff       (20)      781 2024-02-29 09:56:01.000000 pyco-types-1.1.6/pyco_types.egg-info/PKG-INFO
--rw-r--r--   0 nico       (502) staff       (20)      456 2024-02-29 09:56:02.000000 pyco-types-1.1.6/pyco_types.egg-info/SOURCES.txt
--rw-r--r--   0 nico       (502) staff       (20)        1 2024-02-29 09:56:01.000000 pyco-types-1.1.6/pyco_types.egg-info/dependency_links.txt
--rw-r--r--   0 nico       (502) staff       (20)       23 2024-02-29 09:56:01.000000 pyco-types-1.1.6/pyco_types.egg-info/requires.txt
--rw-r--r--   0 nico       (502) staff       (20)       11 2024-02-29 09:56:01.000000 pyco-types-1.1.6/pyco_types.egg-info/top_level.txt
--rw-r--r--   0 nico       (502) staff       (20)       38 2024-02-29 09:56:02.086280 pyco-types-1.1.6/setup.cfg
--rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.6/setup.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.607056 pyco-types-1.1.7/
+-rw-r--r--   0 nico       (502) staff       (20)     7651 2023-09-12 06:46:27.000000 pyco-types-1.1.7/LICENSE.txt
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-11 04:38:10.606312 pyco-types-1.1.7/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)       42 2023-09-11 08:05:54.000000 pyco-types-1.1.7/README.md
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.603405 pyco-types-1.1.7/pyco_types/
+-rw-r--r--   0 nico       (502) staff       (20)      327 2023-09-13 03:32:10.000000 pyco-types-1.1.7/pyco_types/__init__.py
+-rw-r--r--   0 nico       (502) staff       (20)     3709 2024-01-05 13:47:40.000000 pyco-types-1.1.7/pyco_types/_common.py
+-rw-r--r--   0 nico       (502) staff       (20)     2109 2024-01-05 13:12:01.000000 pyco-types-1.1.7/pyco_types/_convert_meta.py
+-rw-r--r--   0 nico       (502) staff       (20)     3577 2024-01-05 10:16:54.000000 pyco-types-1.1.7/pyco_types/_factory.py
+-rw-r--r--   0 nico       (502) staff       (20)     6233 2024-04-11 04:36:21.000000 pyco-types-1.1.7/pyco_types/_int_exts.py
+-rw-r--r--   0 nico       (502) staff       (20)      185 2024-04-11 04:23:42.000000 pyco-types-1.1.7/pyco_types/_version.py
+-rw-r--r--   0 nico       (502) staff       (20)     5931 2024-02-29 09:31:06.000000 pyco-types-1.1.7/pyco_types/co_datetime.py
+-rw-r--r--   0 nico       (502) staff       (20)     2573 2024-04-11 02:14:39.000000 pyco-types-1.1.7/pyco_types/co_dict.py
+-rw-r--r--   0 nico       (502) staff       (20)     2651 2024-04-11 04:25:38.000000 pyco-types-1.1.7/pyco_types/co_integer.py
+-rw-r--r--   0 nico       (502) staff       (20)     3755 2024-01-05 13:43:50.000000 pyco-types-1.1.7/pyco_types/co_json.py
+-rw-r--r--   0 nico       (502) staff       (20)     5156 2023-09-10 03:46:01.000000 pyco-types-1.1.7/pyco_types/co_regex.py
+-rw-r--r--   0 nico       (502) staff       (20)     6473 2024-01-02 13:02:23.000000 pyco-types-1.1.7/pyco_types/const.py
+drwxr-xr-x   0 nico       (502) staff       (20)        0 2024-04-11 04:38:10.605749 pyco-types-1.1.7/pyco_types.egg-info/
+-rw-r--r--   0 nico       (502) staff       (20)      781 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (502) staff       (20)      480 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (502) staff       (20)        1 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (502) staff       (20)       23 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/requires.txt
+-rw-r--r--   0 nico       (502) staff       (20)       11 2024-04-11 04:38:10.000000 pyco-types-1.1.7/pyco_types.egg-info/top_level.txt
+-rw-r--r--   0 nico       (502) staff       (20)       38 2024-04-11 04:38:10.607276 pyco-types-1.1.7/setup.cfg
+-rw-r--r--   0 nico       (502) staff       (20)     1283 2024-01-01 11:35:19.000000 pyco-types-1.1.7/setup.py
```

### Comparing `pyco-types-1.1.6/LICENSE.txt` & `pyco-types-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/PKG-INFO` & `pyco-types-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.6
+Version: 1.1.7
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.6/pyco_types/_common.py` & `pyco-types-1.1.7/pyco_types/_common.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/_convert_meta.py` & `pyco-types-1.1.7/pyco_types/_convert_meta.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/_factory.py` & `pyco-types-1.1.7/pyco_types/_factory.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/co_datetime.py` & `pyco-types-1.1.7/pyco_types/co_datetime.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/co_dict.py` & `pyco-types-1.1.7/pyco_types/co_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyco_types._common import CommonException, G_Symbol_UNSET
 
 
-class MyDict(dict):
+class CoDict(dict):
     ##; attr 只能使用 getattr 的方法访问
     _prviate_attr_map = {}  # type: dict
     ##; data 是缺省字段表, 
     _default_data_map = {}  # type: dict
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -43,28 +43,29 @@
                 errno = 40040
             else:
                 v = self.x_data_map.get(key, G_Symbol_UNSET)
                 if v is G_Symbol_UNSET:
                     errno = 40041
             if errno:
                 raise CommonException(
-                    error_msg=f"<MyDict>.getitem({key}) failed! suggest to update with $.x_set_data_map()",
+                    error_msg=f"<CoDict>.getitem({key}) failed! "
+                              f"suggest to update with $.x_set_data_map()",
                     errno=errno,
                     origin_data=self,
                     default_map=self.x_data_map
                 )
         return v
 
     def __getattr__(self, item):
         ##; 先调用 __getattribute__，然后因为属性不存在调用 __getattr__
         try:
             return self[item]
         except Exception as e:
             raise CommonException(
-                f"<MyDict>.getattr({item}) failed! ({self})",
+                f"<CoDict>.getattr({item}) failed! ({self})",
                 errno=40042,
                 origin_data=self,
             )
 
     def __setattr__(self, key: str, value):
         ##; 所有的内部属性，必须使用 "_" 作为前缀
         if key.startswith("_"):
@@ -74,8 +75,8 @@
             # Set the normal dictionary key-value pair
             self[key] = value
 
     def __delattr__(self, item):
         try:
             del self[item]
         except KeyError:
-            raise AttributeError(f"<MyDict>:: delattr({self}), {item}")
+            raise AttributeError(f"<CoDict>:: delattr({self}), {item}")
```

### Comparing `pyco-types-1.1.6/pyco_types/co_json.py` & `pyco-types-1.1.7/pyco_types/co_json.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/co_regex.py` & `pyco-types-1.1.7/pyco_types/co_regex.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types/const.py` & `pyco-types-1.1.7/pyco_types/const.py`

 * *Files identical despite different names*

### Comparing `pyco-types-1.1.6/pyco_types.egg-info/PKG-INFO` & `pyco-types-1.1.7/pyco_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyco-types
-Version: 1.1.6
+Version: 1.1.7
 Summary: pyco types: Flexible Extensionable Python Types with Converter
 Home-page: https://github.com/vmicode/pyco-types
 Author: dodoru
 Author-email: dodoru@foxmail.com
 License: GNU LGPLv3
 Keywords: pyco-types,datetime,regex-patten,converter,type-formatter
 Platform: any
```

### Comparing `pyco-types-1.1.6/setup.py` & `pyco-types-1.1.7/setup.py`

 * *Files identical despite different names*

