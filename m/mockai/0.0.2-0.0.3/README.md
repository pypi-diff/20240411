# Comparing `tmp/mockai-0.0.2.tar.gz` & `tmp/mockai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockai-0.0.2.tar", last modified: Thu Apr  4 07:13:33 2024, max compression
+gzip compressed data, was "mockai-0.0.3.tar", last modified: Thu Apr 11 15:39:51 2024, max compression
```

## Comparing `mockai-0.0.2.tar` & `mockai-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 07:13:33.573130 mockai-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-03 12:51:36.000000 mockai-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1801 2024-04-04 07:13:33.570923 mockai-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 07:13:33.552701 mockai-0.0.2/mockai/
--rw-rw-rw-   0        0        0       45 2024-04-03 11:57:47.000000 mockai-0.0.2/mockai/__init__.py
--rw-rw-rw-   0        0        0      591 2024-04-03 15:25:37.000000 mockai-0.0.2/mockai/_default.py
--rw-rw-rw-   0        0        0     1253 2024-04-03 14:29:26.000000 mockai-0.0.2/mockai/main.py
--rw-rw-rw-   0        0        0     1861 2024-04-03 15:31:14.000000 mockai-0.0.2/mockai/mock_ai.py
-drwxrwxrwx   0        0        0        0 2024-04-04 07:13:33.562900 mockai-0.0.2/mockai.egg-info/
--rw-rw-rw-   0        0        0     1801 2024-04-04 07:13:33.000000 mockai-0.0.2/mockai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-04 07:13:33.000000 mockai-0.0.2/mockai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 07:13:33.000000 mockai-0.0.2/mockai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-04 07:13:33.000000 mockai-0.0.2/mockai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 07:13:33.000000 mockai-0.0.2/mockai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 07:13:33.573130 mockai-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      896 2024-04-04 07:05:37.000000 mockai-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 07:13:33.562900 mockai-0.0.2/tests/
--rw-rw-rw-   0        0        0     1136 2024-04-03 13:43:15.000000 mockai-0.0.2/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:39:51.711964 mockai-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 12:51:36.000000 mockai-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1801 2024-04-11 15:39:51.711964 mockai-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 15:39:51.696195 mockai-0.0.3/mockai/
+-rw-rw-rw-   0        0        0       45 2024-04-03 11:57:47.000000 mockai-0.0.3/mockai/__init__.py
+-rw-rw-rw-   0        0        0      591 2024-04-03 15:25:37.000000 mockai-0.0.3/mockai/_default.py
+-rw-rw-rw-   0        0        0     1253 2024-04-03 14:29:26.000000 mockai-0.0.3/mockai/main.py
+-rw-rw-rw-   0        0        0     1969 2024-04-11 15:37:30.000000 mockai-0.0.3/mockai/mock_ai.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:39:51.696195 mockai-0.0.3/mockai.egg-info/
+-rw-rw-rw-   0        0        0     1801 2024-04-11 15:39:51.000000 mockai-0.0.3/mockai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-11 15:39:51.000000 mockai-0.0.3/mockai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 15:39:51.000000 mockai-0.0.3/mockai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-11 15:39:51.000000 mockai-0.0.3/mockai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 15:39:51.000000 mockai-0.0.3/mockai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 15:39:51.711964 mockai-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      896 2024-04-11 15:39:48.000000 mockai-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:39:51.696195 mockai-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1136 2024-04-03 13:43:15.000000 mockai-0.0.3/tests/tests.py
```

### Comparing `mockai-0.0.2/LICENSE` & `mockai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mockai-0.0.2/PKG-INFO` & `mockai-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockai
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/chefkoch24/mockai
 Author: Felix Künnecke
 Author-email: kuenneckefelix@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `mockai-0.0.2/mockai/_default.py` & `mockai-0.0.3/mockai/_default.py`

 * *Files identical despite different names*

### Comparing `mockai-0.0.2/mockai/main.py` & `mockai-0.0.3/mockai/main.py`

 * *Files identical despite different names*

### Comparing `mockai-0.0.2/mockai/mock_ai.py` & `mockai-0.0.3/mockai/mock_ai.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         self.config = config_data
         self.commands = self._get_commands()
 
     def _get_commands(self):
         commands = {}
         for k,v in self.config.items():
             if k != '_default':
-                with open(v, 'r') as json_file:
+                path = os.path.join(os.getcwd(), v)
+                with open(path, 'r') as json_file:
                     try:
                         value = json.load(json_file)
                         commands[k] = value
                     except json.JSONDecodeError as e:
                         raise ValueError(f"Invalid JSON file: {e}")
         return commands
 
@@ -46,12 +47,13 @@
             # read default data structure to return
             result = self._get_default()
         return result
 
     def _get_default(self):
         default = self.config.get('_default')
         if default is not None:
-            with open(default, 'r') as json_file:
+            path = os.path.join(os.getcwd(), default)
+            with open(path, 'r') as json_file:
                 default_dict = json.load(json_file)
         else:
             default_dict = get_default()
         return default_dict
```

### Comparing `mockai-0.0.2/mockai.egg-info/PKG-INFO` & `mockai-0.0.3/mockai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockai
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/chefkoch24/mockai
 Author: Felix Künnecke
 Author-email: kuenneckefelix@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `mockai-0.0.2/setup.py` & `mockai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'MockAI is a library that allows you to mock AI responses using custom commands suitable for simulating responses during testing without AI inference cost.'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='mockai',
```

### Comparing `mockai-0.0.2/tests/tests.py` & `mockai-0.0.3/tests/tests.py`

 * *Files identical despite different names*

