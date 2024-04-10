# Comparing `tmp/jsonparse-0.9.0.tar.gz` & `tmp/jsonparse-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonparse-0.9.0.tar", last modified: Thu Sep 15 18:52:10 2022, max compression
+gzip compressed data, was "jsonparse-0.9.1.tar", last modified: Thu Sep 15 20:50:27 2022, max compression
```

## Comparing `jsonparse-0.9.0.tar` & `jsonparse-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:52:10.263264 jsonparse-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-15 18:52:01.000000 jsonparse-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-09-15 18:52:10.259264 jsonparse-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-09-15 18:52:01.000000 jsonparse-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:52:10.259264 jsonparse-0.9.0/jsonparse/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-15 18:52:01.000000 jsonparse-0.9.0/jsonparse/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12496 2022-09-15 18:52:01.000000 jsonparse-0.9.0/jsonparse/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:52:10.259264 jsonparse-0.9.0/jsonparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-09-15 18:52:10.000000 jsonparse-0.9.0/jsonparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-15 18:52:10.000000 jsonparse-0.9.0/jsonparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 18:52:10.000000 jsonparse-0.9.0/jsonparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-15 18:52:10.000000 jsonparse-0.9.0/jsonparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 18:52:10.263264 jsonparse-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-09-15 18:52:01.000000 jsonparse-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:50:27.760515 jsonparse-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-15 20:50:22.000000 jsonparse-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-09-15 20:50:27.760515 jsonparse-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-09-15 20:50:22.000000 jsonparse-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:50:27.760515 jsonparse-0.9.1/jsonparse/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-15 20:50:22.000000 jsonparse-0.9.1/jsonparse/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12538 2022-09-15 20:50:22.000000 jsonparse-0.9.1/jsonparse/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 20:50:27.760515 jsonparse-0.9.1/jsonparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-09-15 20:50:27.000000 jsonparse-0.9.1/jsonparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-09-15 20:50:27.000000 jsonparse-0.9.1/jsonparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 20:50:27.000000 jsonparse-0.9.1/jsonparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-15 20:50:27.000000 jsonparse-0.9.1/jsonparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 20:50:27.764515 jsonparse-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-09-15 20:50:22.000000 jsonparse-0.9.1/setup.py
```

### Comparing `jsonparse-0.9.0/LICENSE` & `jsonparse-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonparse-0.9.0/PKG-INFO` & `jsonparse-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonparse
-Version: 0.9.0
+Version: 0.9.1
 Summary: Search through JSON data key:values by key(s)
 Home-page: https://github.com/ctomkow/jsonparse
 Author: Craig Tomkow
 Author-email: ctomkow@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -93,12 +93,12 @@
 `find_key_chain(data: dict | list, keys: list) -> list`
 
 - Provide JSON data as a dictionary or a list, as well as a list of keys as strings.
 - Returns a list of values that match the corresponding key chain.
 
     > Wildcard **'*'** can be used as key(s) to match any.
 
-`find_key_value(data: dict | list, key: str, value: str | int | float | bool) -> list`
+`find_key_value(data: dict | list, key: str, value: str | int | float | bool | None) -> list`
 
 - Provide JSON data as a dictionary or a list, a key as a string,
-  and a value as a string, integer, float, or boolean.
+  and a value as a string, integer, float, boolean, or None.
 - Returns a list of set(s) that contain the key:value pair.
```

### Comparing `jsonparse-0.9.0/README.md` & `jsonparse-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,12 +77,12 @@
 `find_key_chain(data: dict | list, keys: list) -> list`
 
 - Provide JSON data as a dictionary or a list, as well as a list of keys as strings.
 - Returns a list of values that match the corresponding key chain.
 
     > Wildcard **'*'** can be used as key(s) to match any.
 
-`find_key_value(data: dict | list, key: str, value: str | int | float | bool) -> list`
+`find_key_value(data: dict | list, key: str, value: str | int | float | bool | None) -> list`
 
 - Provide JSON data as a dictionary or a list, a key as a string,
-  and a value as a string, integer, float, or boolean.
+  and a value as a string, integer, float, boolean, or None.
 - Returns a list of set(s) that contain the key:value pair.
```

### Comparing `jsonparse-0.9.0/jsonparse/parser.py` & `jsonparse-0.9.1/jsonparse/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 keys.pop(0)
 
         return self.queue_ref
 
     def find_key_value(self,
                        data: Union[dict, list],
                        key: str,
-                       value: Union[str, int, float, bool]) -> list:
+                       value: Union[str, int, float, bool, None]) -> list:
         """
         Search JSON data that consists of key:value pairs for all instances of
         provided key and value pair. The parent set that contains the key:value
         pair will be returned. The data can have complex nested
         dictionaries and lists. If duplicate key and value pairs exist in
         the data (at any layer) all matching key and value pair set(s)
         that contain the key:value pair will be returned. Data is parsed
@@ -250,22 +250,22 @@
                     self._stack_push(elem[e])
                     self._stack_trace()
         return value_list
 
     def _stack_all_key_and_value_in_dict(
             self,
             key: str,
-            value: Union[str, int, float, bool],
+            value: Union[str, int, float, bool, None],
             elem: dict) -> bool:
 
         if type(elem) is not dict:
             raise TypeError
         elif type(key) is not str:
             raise TypeError
-        elif not isinstance(value, (str, int, float, bool)):
+        elif not isinstance(value, (str, int, float, bool, type(None))):
             raise TypeError
 
         if len(elem) <= 0:  # don't want an empty dict on the stack
             pass
         else:
             for e in elem:
                 if e == key and elem[e] == value:
@@ -390,18 +390,18 @@
 
         return True
 
     def _valid_key_value_input(
             self,
             data: Union[dict, list],
             key: str,
-            value: Union[str, int, float, bool]) -> bool:
+            value: Union[str, int, float, bool, None]) -> bool:
 
         if not isinstance(data, (dict, list)):
             raise TypeError
         elif not isinstance(key, str):
             raise TypeError
         elif not key:  # if key is an empty string
             raise ValueError
-        elif not isinstance(value, (str, int, float, bool)):
+        elif not isinstance(value, (str, int, float, bool, type(None))):
             raise TypeError
         return True
```

### Comparing `jsonparse-0.9.0/jsonparse.egg-info/PKG-INFO` & `jsonparse-0.9.1/jsonparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonparse
-Version: 0.9.0
+Version: 0.9.1
 Summary: Search through JSON data key:values by key(s)
 Home-page: https://github.com/ctomkow/jsonparse
 Author: Craig Tomkow
 Author-email: ctomkow@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -93,12 +93,12 @@
 `find_key_chain(data: dict | list, keys: list) -> list`
 
 - Provide JSON data as a dictionary or a list, as well as a list of keys as strings.
 - Returns a list of values that match the corresponding key chain.
 
     > Wildcard **'*'** can be used as key(s) to match any.
 
-`find_key_value(data: dict | list, key: str, value: str | int | float | bool) -> list`
+`find_key_value(data: dict | list, key: str, value: str | int | float | bool | None) -> list`
 
 - Provide JSON data as a dictionary or a list, a key as a string,
-  and a value as a string, integer, float, or boolean.
+  and a value as a string, integer, float, boolean, or None.
 - Returns a list of set(s) that contain the key:value pair.
```

### Comparing `jsonparse-0.9.0/setup.py` & `jsonparse-0.9.1/setup.py`

 * *Files identical despite different names*

