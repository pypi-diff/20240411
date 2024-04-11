# Comparing `tmp/stellrent-response-0.0.3.tar.gz` & `tmp/stellrent-response-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellrent-response-0.0.3.tar", last modified: Wed Mar 27 13:10:40 2024, max compression
+gzip compressed data, was "stellrent-response-0.0.4.tar", last modified: Thu Apr 11 18:17:45 2024, max compression
```

## Comparing `stellrent-response-0.0.3.tar` & `stellrent-response-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-03-27 13:10:40.048809 stellrent-response-0.0.3/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     1066 2024-03-20 21:00:04.000000 stellrent-response-0.0.3/LICENSE
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      156 2024-03-20 21:07:10.000000 stellrent-response-0.0.3/MANIFEST.in
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      875 2024-03-27 13:10:40.050807 stellrent-response-0.0.3/PKG-INFO
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       71 2024-03-20 21:22:01.000000 stellrent-response-0.0.3/README.md
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      934 2024-03-27 13:06:18.000000 stellrent-response-0.0.3/pyproject.toml
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       73 2024-03-27 13:10:40.057961 stellrent-response-0.0.3/setup.cfg
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     1802 2024-03-27 13:05:59.000000 stellrent-response-0.0.3/setup.py
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-03-27 13:10:39.869508 stellrent-response-0.0.3/stellrent_response/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-03-20 21:01:04.000000 stellrent-response-0.0.3/stellrent_response/__init__.py
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)     3685 2024-03-27 05:20:46.000000 stellrent-response-0.0.3/stellrent_response/json_response.py
-drwxrwxrwx   0 marcus    (1000) marcus    (1000)        0 2024-03-27 13:10:40.020223 stellrent-response-0.0.3/stellrent_response.egg-info/
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      875 2024-03-27 13:10:37.000000 stellrent-response-0.0.3/stellrent_response.egg-info/PKG-INFO
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)      339 2024-03-27 13:10:38.000000 stellrent-response-0.0.3/stellrent_response.egg-info/SOURCES.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)        1 2024-03-27 13:10:37.000000 stellrent-response-0.0.3/stellrent_response.egg-info/dependency_links.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       10 2024-03-27 13:10:37.000000 stellrent-response-0.0.3/stellrent_response.egg-info/requires.txt
--rwxrwxrwx   0 marcus    (1000) marcus    (1000)       19 2024-03-27 13:10:37.000000 stellrent-response-0.0.3/stellrent_response.egg-info/top_level.txt
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     1066 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/LICENSE
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      156 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/MANIFEST.in
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      875 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/PKG-INFO
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       71 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/README.md
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      878 2024-04-11 18:17:41.000000 stellrent-response-0.0.4/pyproject.toml
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       73 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/setup.cfg
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     1195 2024-04-11 18:17:21.000000 stellrent-response-0.0.4/setup.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/stellrent_response/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       21 2024-04-11 14:19:39.000000 stellrent-response-0.0.4/stellrent_response/__init__.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     3731 2024-04-11 18:16:11.000000 stellrent-response-0.0.4/stellrent_response/json_response.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/stellrent_response.egg-info/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      875 2024-04-11 18:17:45.000000 stellrent-response-0.0.4/stellrent_response.egg-info/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      475 2024-04-11 18:17:45.000000 stellrent-response-0.0.4/stellrent_response.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2024-04-11 18:17:45.000000 stellrent-response-0.0.4/stellrent_response.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       10 2024-04-11 18:17:45.000000 stellrent-response-0.0.4/stellrent_response.egg-info/requires.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       19 2024-04-11 18:17:45.000000 stellrent-response-0.0.4/stellrent_response.egg-info/top_level.txt
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:17:45.328285 stellrent-response-0.0.4/tests/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     2595 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/tests/test_json_bad_request_response.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      445 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/tests/test_json_response_success_nocontent_response.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      713 2024-04-11 13:49:45.000000 stellrent-response-0.0.4/tests/test_json_success_data_response.py
```

### Comparing `stellrent-response-0.0.3/LICENSE` & `stellrent-response-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stellrent-response-0.0.3/PKG-INFO` & `stellrent-response-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stellrent-response
-Version: 0.0.3
-Summary: Pattern responses for REST API Projects
+Version: 0.0.4
+Summary: Pattern responses for your API Projects
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-response
 Project-URL: Issues, https://github.com/stellrent/stellrent-response/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `stellrent-response-0.0.3/pyproject.toml` & `stellrent-response-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [project]
 name = "stellrent-response"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Marcus Rodrigues Magalhães", email="marcusrodrigues.magalhaes@stellantis.com" },
 ]
-description = "Pattern responses for REST API Projects"
 readme = "README.md"
 # license = 'MIT'
 requires-python = '>=3.7'
 classifiers = [
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.11',
```

### Comparing `stellrent-response-0.0.3/setup.py` & `stellrent-response-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 #!/usr/bin/env python3
+# step 1: python setup.py sdist bdist_wheel
+# step 2: twine upload dist/* --verbose
 # https://medium.com/the-research-nest/how-to-publish-your-python-code-as-a-pip-package-in-5-simple-steps-3b36286293ec
 """
 Parts of this file were taken from the pyzmq project
 (https://github.com/zeromq/pyzmq) which have been permitted for use under the
 BSD license. Parts are from lxml (https://github.com/lxml/lxml)
 """
 from setuptools import setup
 
-VERSION = '0.0.3'
-
 with open('requirements.txt') as requirements_file:
     REQUIRED_MODULES = [line.strip() for line in requirements_file]
 
 with open('requirements-dev.txt') as requirements_dev_file:
     REQUIRED_DEV_MODULES = [line.strip() for line in requirements_dev_file]
 
 def readme():
     with open('README.md') as readme_file:
         return readme_file.read()
     
 setup(
     name='stellrent-response',
-    version=VERSION,
     author='Marcus R. Magalhães',
     author_email='marcusrodrigues.magalhaes@stellantis.com',
     description='Pattern responses for your API Projects',
     packages=['stellrent_response'],
     include_package_data=True,
     long_description=readme(),
     long_description_content_type='text/markdown',
     install_requires=REQUIRED_MODULES
-)
-
-# if __name__ == "__main__":
-#     # Freeze to support parallel compilation when using spawn instead of fork
-#     multiprocessing.freeze_support()
-#     setup(
-#         name = 'stellrent-response',
-#         version=VERSION,
-#         description='Pattern responses for your API Projects',
-#         long_description=readme(),
-#         keywords='response json api pattern',
-#         author='Marcus R. Magalhães',
-#         author_email='marcusrodrigues.magalhaes@stellantis.com',
-#         packages=['src'],
-#         install_requires = REQUIRED_MODULES,
-#         ext_modules = REQUIRED_DEV_MODULES,
-#         include_package_data=True
-#     )
+)
```

### Comparing `stellrent-response-0.0.3/stellrent_response/json_response.py` & `stellrent-response-0.0.4/stellrent_response/json_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,37 @@
     403: "Forbidden",
     405: "Method not alowed",
     500: "Internal Server Error"
 }
 
 class DefaultResponse():
 
+    __logger = logging.getLogger()
+
     def __init__(self, logger=None):
         if logger is None:
-            self.logger = logging.getLogger()
+            self.__logger = logging.getLogger()
         else:
             if isinstance(logger, logging.getLogger()):
-                self.logger = logger
+                self.__logger = logger
             else:
-                self.logger = logging.getLogger()
-                self.logger.warn("Invalid logger: " + type(logger) + ". Expected logger type: " + type(self.logger))
+                self.__logger = logging.getLogger()
+                self.__logger.warn("Invalid logger: " + type(logger) + ". Expected logger type: " + type(self.logger))
         self.__content_type__ = "application/json"
         self.response_data = None
         self.response_status = 200
 
     def make_response(self, data=None, details=None):
         body_response = {}
         for i in inspect.getmembers(self):
             if i[0].startswith('response_') and not inspect.ismethod(i[0]):
                 if i[1] is not None:
                     body_response[i[0].replace('response_', "")] = i[1]
         
-        self.logger.debug("RAW Response data: %s", body_response)
+        self.__logger.debug("RAW Response data: %s", body_response)
         
         if "data" in body_response:
             return body_response['data'], body_response['status']
         return body_response, body_response['status']
     
 class DataResponse(DefaultResponse):
     def __init__(self, data):
```

### Comparing `stellrent-response-0.0.3/stellrent_response.egg-info/PKG-INFO` & `stellrent-response-0.0.4/stellrent_response.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stellrent-response
-Version: 0.0.3
-Summary: Pattern responses for REST API Projects
+Version: 0.0.4
+Summary: Pattern responses for your API Projects
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-response
 Project-URL: Issues, https://github.com/stellrent/stellrent-response/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

