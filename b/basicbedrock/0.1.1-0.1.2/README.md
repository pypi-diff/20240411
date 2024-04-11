# Comparing `tmp/basicbedrock-0.1.1.tar.gz` & `tmp/basicbedrock-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.1.tar", last modified: Thu Apr 11 00:28:17 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.2.tar", last modified: Thu Apr 11 01:02:51 2024, max compression
```

## Comparing `basicbedrock-0.1.1.tar` & `basicbedrock-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.242970 basicbedrock-0.1.1/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.1/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 00:28:17.242720 basicbedrock-0.1.1/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-11 00:28:17.243025 basicbedrock-0.1.1/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.238760 basicbedrock-0.1.1/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.239658 basicbedrock-0.1.1/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    15825 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.241812 basicbedrock-0.1.1/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3008 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3659 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     6036 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     7095 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4710 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3221 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2864 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.242404 basicbedrock-0.1.1/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.241953 basicbedrock-0.1.1/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.443719 basicbedrock-0.1.2/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.2/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 01:02:51.443455 basicbedrock-0.1.2/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-11 00:58:01.000000 basicbedrock-0.1.2/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-11 01:02:51.443779 basicbedrock-0.1.2/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.438031 basicbedrock-0.1.2/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.439226 basicbedrock-0.1.2/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-11 00:58:01.000000 basicbedrock-0.1.2/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    15997 2024-04-11 00:57:42.000000 basicbedrock-0.1.2/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.442098 basicbedrock-0.1.2/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3008 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3659 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6036 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     7095 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4710 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3221 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2864 2024-04-11 00:27:04.000000 basicbedrock-0.1.2/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.443093 basicbedrock-0.1.2/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 01:02:51.000000 basicbedrock-0.1.2/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-11 01:02:51.000000 basicbedrock-0.1.2/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-11 01:02:51.000000 basicbedrock-0.1.2/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-11 01:02:51.000000 basicbedrock-0.1.2/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-11 01:02:51.000000 basicbedrock-0.1.2/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 01:02:51.442333 basicbedrock-0.1.2/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:02:05.000000 basicbedrock-0.1.2/test/tests.py
```

### Comparing `basicbedrock-0.1.1/LICENSE` & `basicbedrock-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/PKG-INFO` & `basicbedrock-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.1
+Version: 0.1.2
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.1/README.md` & `basicbedrock-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/pyproject.toml` & `basicbedrock-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.1/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.2/src/basicbedrock/basicbedrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         self._n = self._default_n
         self._s = self._default_stop
 
     @property
     def top_p(self) -> float:
         """
         returns the top_p parameter
-        :return:
+        :return: a float representing the top_p parameter
         """
         return self._p
 
     @top_p.setter
     def top_p(self, top_p: float):
         """
         sets the top_p parameter
@@ -310,15 +310,15 @@
         """
         self._p = self._default_p
 
     @property
     def top_k(self) -> int:
         """
         returns the top_k parameter
-        :return:
+        :return: a int representing the top_k parameter
         """
         return self._k
 
     @top_k.setter
     def top_k(self, k: int):
         """
         sets the top_k parameter
@@ -339,15 +339,15 @@
         """
         self._k = self._default_k
 
     @property
     def temp(self) -> float:
         """
         returns the temp parameter
-        :return:
+        :return: a float representing the temperature
         """
         return self._t
 
     @temp.setter
     def temp(self, temp: float):
         """
         sets the temp parameter
@@ -365,18 +365,18 @@
         """
         resets the temp parameter
         :return:
         """
         self._t = self._default_t
 
     @property
-    def max_tokens(self):
+    def max_tokens(self)->int:
         """
         returns the max_tokens parameter
-        :return:
+        :return: the int max_tokens parameter
         """
         return self._n
 
     @max_tokens.setter
     def max_tokens(self, n_tokens: int):
         """
         sets the max_tokens parameter
@@ -396,34 +396,34 @@
         :return:
         """
         self._n = self._default_n
 
     @property
     def stop_words(self) -> list:
         """
-        returns the max_tokens parameter
-        :return:
+        returns the stop_words parameter
+        :return: a list of stop words
         """
 
         return self._s
 
     @stop_words.setter
     def stop_words(self, stop_words: List[str]):
         """
-        sets the max_tokens parameter
+        sets the stop_words parameter
         :param n_tokens:
         :return:
         """
         if not isinstance(stop_words, list):
             raise ValueError(f"stop_tokens must be a list, not a {type(stop_words)}")
         for i, item in enumerate(stop_words):
             if not isinstance(item, str):
                 raise ValueError(f"stop_tokens must be a list of strings, but element {i} is a {type(item)}")
         self._s = stop_words
 
     @stop_words.deleter
     def stop_words(self):
         """
-        resets the max_tokens parameter
+        resets the stop_words parameter
         :return:
         """
         self._s = self._default_stop
```

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.2/src/basicbedrock/models/__init__.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/ai21.py` & `basicbedrock-0.1.2/src/basicbedrock/models/ai21.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.2/src/basicbedrock/models/amazon.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.1.2/src/basicbedrock/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.2/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/cohere.py` & `basicbedrock-0.1.2/src/basicbedrock/models/cohere.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.2/src/basicbedrock/models/meta.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.2/src/basicbedrock/models/mistral.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.1.2/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.1
+Version: 0.1.2
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.1.1/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.2/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.1/test/tests.py` & `basicbedrock-0.1.2/test/tests.py`

 * *Files identical despite different names*

