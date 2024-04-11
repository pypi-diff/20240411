# Comparing `tmp/mokei-0.1.2.tar.gz` & `tmp/mokei-0.2.1.tar.gz`

## Comparing `mokei-0.1.2.tar` & `mokei-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 mokei-0.1.2/.github/workflows/test-ci-cd.yml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/__init__.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/client.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/config.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/datatypes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/exceptions.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/logging.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/middlewares.py
--rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/mokei.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/request.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/websocket.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/wsclient.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mokei-0.1.2/src/mokei/js/mokei.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mokei-0.1.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.1.2/LICENSE
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.1.2/README.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/__init__.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/client.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/config.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/datatypes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/exceptions.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/logging.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/middlewares.py
+-rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/mokei.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/request.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/websocket.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/wsclient.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mokei-0.2.1/src/mokei/js/mokei.js
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mokei-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.2.1/README.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.2.1/PKG-INFO
```

### Comparing `mokei-0.1.2/src/mokei/client.py` & `mokei-0.2.1/src/mokei/client.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/config.py` & `mokei-0.2.1/src/mokei/config.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/logging.py` & `mokei-0.2.1/src/mokei/logging.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/mokei.py` & `mokei-0.2.1/src/mokei/mokei.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/websocket.py` & `mokei-0.2.1/src/mokei/websocket.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/wsclient.py` & `mokei-0.2.1/src/mokei/wsclient.py`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/src/mokei/js/mokei.js` & `mokei-0.2.1/src/mokei/js/mokei.js`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/LICENSE` & `mokei-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/README.md` & `mokei-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mokei-0.1.2/pyproject.toml` & `mokei-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mokei"
-version = "0.1.2"
+version = "0.2.1"
 authors = [
   { name="deuxglaces", email="dev@deuxglaces.com" },
 ]
 description = "A simple asynchronous Python web framework built on aiohttp."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mokei-0.1.2/PKG-INFO` & `mokei-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mokei
-Version: 0.1.2
+Version: 0.2.1
 Summary: A simple asynchronous Python web framework built on aiohttp.
 Project-URL: Homepage, https://github.com/deuxglaces/mokei
 Project-URL: Issues, https://github.com/deuxglaces/mokei/issues
 Author-email: deuxglaces <dev@deuxglaces.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

