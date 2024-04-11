# Comparing `tmp/peasant-0.6.1.tar.gz` & `tmp/peasant-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peasant-0.6.1.tar", last modified: Thu Mar 28 18:30:00 2024, max compression
+gzip compressed data, was "peasant-0.7.0.tar", last modified: Thu Apr 11 14:11:35 2024, max compression
```

## Comparing `peasant-0.6.1.tar` & `peasant-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.102327 peasant-0.6.1/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11348 2024-03-28 18:02:07.000000 peasant-0.6.1/LICENSE
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      127 2024-02-16 21:44:20.000000 peasant-0.6.1/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2640 2024-03-28 18:30:00.101327 peasant-0.6.1/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1307 2024-03-28 18:20:52.000000 peasant-0.6.1/README.md
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.096327 peasant-0.6.1/peasant/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      992 2024-03-28 18:22:01.000000 peasant-0.6.1/peasant/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6911 2024-03-28 17:57:42.000000 peasant-0.6.1/peasant/client.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.098327 peasant-0.6.1/peasant/security/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-01-23 18:19:05.000000 peasant-0.6.1/peasant/security/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1180 2024-03-28 18:00:16.000000 peasant-0.6.1/peasant/security/ec.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1289 2024-03-28 18:00:25.000000 peasant-0.6.1/peasant/security/jwk.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3491 2024-03-28 18:00:31.000000 peasant-0.6.1/peasant/security/keyring.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1371 2024-03-28 18:00:51.000000 peasant-0.6.1/peasant/security/rsa.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2184 2024-03-28 18:01:08.000000 peasant-0.6.1/peasant/server.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.100327 peasant-0.6.1/peasant.egg-info/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2640 2024-03-28 18:30:00.000000 peasant-0.6.1/peasant.egg-info/PKG-INFO
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      503 2024-03-28 18:30:00.000000 peasant-0.6.1/peasant.egg-info/SOURCES.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        1 2024-03-28 18:30:00.000000 peasant-0.6.1/peasant.egg-info/dependency_links.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      114 2024-03-28 18:30:00.000000 peasant-0.6.1/peasant.egg-info/requires.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       14 2024-03-28 18:30:00.000000 peasant-0.6.1/peasant.egg-info/top_level.txt
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.099327 peasant-0.6.1/requirements/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       28 2024-02-16 21:45:02.000000 peasant-0.6.1/requirements/all.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       35 2024-03-24 22:03:43.000000 peasant-0.6.1/requirements/basic.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2024-02-06 21:52:06.000000 peasant-0.6.1/requirements/tornado.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2024-03-28 18:30:00.102327 peasant-0.6.1/setup.cfg
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3087 2024-02-16 21:45:46.000000 peasant-0.6.1/setup.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 18:30:00.099327 peasant-0.6.1/tests/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2182 2024-02-18 04:48:13.000000 peasant-0.6.1/tests/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1020 2024-02-07 15:04:49.000000 peasant-0.6.1/tests/runtests.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1479 2024-03-25 06:13:44.000000 peasant-0.6.1/tests/tornado_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.755636 peasant-0.7.0/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    11348 2024-03-28 21:59:34.000000 peasant-0.7.0/LICENSE
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      161 2024-04-11 00:41:46.000000 peasant-0.7.0/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2766 2024-04-11 14:11:35.755636 peasant-0.7.0/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1307 2024-03-28 21:59:34.000000 peasant-0.7.0/README.md
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.748636 peasant-0.7.0/peasant/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      992 2024-04-11 00:22:35.000000 peasant-0.7.0/peasant/__init__.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.750636 peasant-0.7.0/peasant/client/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-29 18:53:17.000000 peasant-0.7.0/peasant/client/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1841 2024-03-29 19:02:02.000000 peasant-0.7.0/peasant/client/protocol.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3309 2024-04-08 05:28:16.000000 peasant-0.7.0/peasant/client/transport.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4466 2024-04-08 05:28:44.000000 peasant-0.7.0/peasant/client/transport_requests.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     9203 2024-04-08 06:27:29.000000 peasant-0.7.0/peasant/client/transport_tornado.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.751636 peasant-0.7.0/peasant/security/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/security/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1180 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/security/ec.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1289 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/security/jwk.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3491 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/security/keyring.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1371 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/security/rsa.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2184 2024-03-28 21:59:34.000000 peasant-0.7.0/peasant/server.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.754636 peasant-0.7.0/peasant.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2766 2024-04-11 14:11:35.000000 peasant-0.7.0/peasant.egg-info/PKG-INFO
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      733 2024-04-11 14:11:35.000000 peasant-0.7.0/peasant.egg-info/SOURCES.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        1 2024-04-11 14:11:35.000000 peasant-0.7.0/peasant.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      160 2024-04-11 14:11:35.000000 peasant-0.7.0/peasant.egg-info/requires.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       14 2024-04-11 14:11:35.000000 peasant-0.7.0/peasant.egg-info/top_level.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.752636 peasant-0.7.0/requirements/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       44 2024-04-07 18:40:45.000000 peasant-0.7.0/requirements/all.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       35 2024-03-29 19:53:34.000000 peasant-0.7.0/requirements/basic.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       17 2024-03-29 20:22:55.000000 peasant-0.7.0/requirements/requests.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       13 2024-04-11 14:10:04.000000 peasant-0.7.0/requirements/tornado.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       38 2024-04-11 14:11:35.756636 peasant-0.7.0/setup.cfg
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3031 2024-04-11 14:10:41.000000 peasant-0.7.0/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2024-04-11 14:11:35.753636 peasant-0.7.0/tests/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2182 2024-03-28 21:59:34.000000 peasant-0.7.0/tests/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1225 2024-04-08 04:27:35.000000 peasant-0.7.0/tests/runtests.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4536 2024-04-08 06:18:37.000000 peasant-0.7.0/tests/transport_requests_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2993 2024-04-07 21:36:28.000000 peasant-0.7.0/tests/transport_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3804 2024-04-08 06:26:06.000000 peasant-0.7.0/tests/transport_tornado_test.py
```

### Comparing `peasant-0.6.1/LICENSE` & `peasant-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/PKG-INFO` & `peasant-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peasant
-Version: 0.6.1
+Version: 0.7.0
 Summary: Peasant helps you to build APIs
 Home-page: https://github.com/candango/peasant
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 License: Apache License V2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,15 +24,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.18
 Requires-Dist: cryptography==42.0.5
 Provides-Extra: all
 Requires-Dist: cartola>=0.18; extra == "all"
 Requires-Dist: cryptography==42.0.5; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: tornado>=6.3; extra == "all"
+Provides-Extra: requests
+Requires-Dist: requests==2.31.0; extra == "requests"
 Provides-Extra: tornado
 Requires-Dist: tornado>=6.3; extra == "tornado"
 
 # Candango Peasant
 
 Peasant is a protocol abstraction of how to control agents that need to
 communicate with a central entity or entities.
```

### Comparing `peasant-0.6.1/README.md` & `peasant-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant/__init__.py` & `peasant-0.7.0/peasant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __author__ = "Flavio Garcia <piraz@candango.org>"
-__version__ = (0, 6, 1)
+__version__ = (0, 7, 0)
 __licence__ = "Apache License V2.0"
 
 
 def get_version():
     if isinstance(__version__[-1], str):
         return '.'.join(map(str, __version__[:-1])) + __version__[-1]
     return ".".join(map(str, __version__))
```

### Comparing `peasant-0.6.1/peasant/security/ec.py` & `peasant-0.7.0/peasant/security/ec.py`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant/security/jwk.py` & `peasant-0.7.0/peasant/security/jwk.py`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant/security/keyring.py` & `peasant-0.7.0/peasant/security/keyring.py`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant/security/rsa.py` & `peasant-0.7.0/peasant/security/rsa.py`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant/server.py` & `peasant-0.7.0/peasant/server.py`

 * *Files identical despite different names*

### Comparing `peasant-0.6.1/peasant.egg-info/PKG-INFO` & `peasant-0.7.0/peasant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peasant
-Version: 0.6.1
+Version: 0.7.0
 Summary: Peasant helps you to build APIs
 Home-page: https://github.com/candango/peasant
 Author: Flavio Garcia
 Author-email: piraz@candango.org
 License: Apache License V2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,15 +24,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cartola>=0.18
 Requires-Dist: cryptography==42.0.5
 Provides-Extra: all
 Requires-Dist: cartola>=0.18; extra == "all"
 Requires-Dist: cryptography==42.0.5; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 Requires-Dist: tornado>=6.3; extra == "all"
+Provides-Extra: requests
+Requires-Dist: requests==2.31.0; extra == "requests"
 Provides-Extra: tornado
 Requires-Dist: tornado>=6.3; extra == "tornado"
 
 # Candango Peasant
 
 Peasant is a protocol abstraction of how to control agents that need to
 communicate with a central entity or entities.
```

### Comparing `peasant-0.6.1/tests/__init__.py` & `peasant-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

