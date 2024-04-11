# Comparing `tmp/aioxdl-0.0.5.tar.gz` & `tmp/aioxdl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.5.tar", last modified: Thu Apr 11 14:18:54 2024, max compression
+gzip compressed data, was "aioxdl-0.0.6.tar", last modified: Thu Apr 11 15:12:10 2024, max compression
```

## Comparing `aioxdl-0.0.5.tar` & `aioxdl-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:54.740553 aioxdl-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 14:18:48.000000 aioxdl-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 14:18:54.740553 aioxdl-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 14:18:48.000000 aioxdl-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:54.736553 aioxdl-0.0.5/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 14:18:48.000000 aioxdl-0.0.5/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-11 14:18:48.000000 aioxdl-0.0.5/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:54.740553 aioxdl-0.0.5/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 14:18:54.000000 aioxdl-0.0.5/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:18:54.740553 aioxdl-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 14:18:48.000000 aioxdl-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:12:10.955477 aioxdl-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:12:04.000000 aioxdl-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 15:12:10.955477 aioxdl-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 15:12:04.000000 aioxdl-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:12:10.951477 aioxdl-0.0.6/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 15:12:04.000000 aioxdl-0.0.6/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-11 15:12:04.000000 aioxdl-0.0.6/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:12:10.955477 aioxdl-0.0.6/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 15:12:10.000000 aioxdl-0.0.6/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:12:10.955477 aioxdl-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 15:12:04.000000 aioxdl-0.0.6/setup.py
```

### Comparing `aioxdl-0.0.5/LICENSE` & `aioxdl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.5/PKG-INFO` & `aioxdl-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.5
+Version: 0.0.6
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.5 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.6 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.5/README.md` & `aioxdl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.5/aioxdl/module.py` & `aioxdl-0.0.6/aioxdl/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,23 +37,25 @@
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsize += self.chunk
                         try: await self.display(progress)
                         except Exception: pass
 
-                return location
+                return location if location else None
 
 #=================================================================================================
 
     async def start(self, url, location, timeout=1000, progress=None):
         try:
             location = await self.download(url, location, timeout, progress)
         except aiohttp.ClientConnectorError as errors:
             self.error = errors
+        except aiohttp.ClientTimeoutError as errors:
+            self.error = errors
         except Exception as errors:
             self.error = errors
 
         return location
 
 #=================================================================================================
```

### Comparing `aioxdl-0.0.5/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.6/aioxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.5
+Version: 0.0.6
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.5 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.6 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.5/setup.py` & `aioxdl-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.5',
+    version='0.0.6',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     install_requires=['aiohttp'],
     long_description=long_description,
```

