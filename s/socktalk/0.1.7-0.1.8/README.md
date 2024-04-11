# Comparing `tmp/socktalk-0.1.7.tar.gz` & `tmp/socktalk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.7.tar", last modified: Thu Apr 11 14:44:26 2024, max compression
+gzip compressed data, was "socktalk-0.1.8.tar", last modified: Thu Apr 11 15:12:23 2024, max compression
```

## Comparing `socktalk-0.1.7.tar` & `socktalk-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.723447 socktalk-0.1.7/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.7/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 14:44:26.719447 socktalk-0.1.7/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3648 2024-04-11 12:01:29.000000 socktalk-0.1.7/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.719447 socktalk-0.1.7/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.7/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.7/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.7/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.7/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.7/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 14:44:26.723447 socktalk-0.1.7/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1002 2024-04-11 14:43:17.000000 socktalk-0.1.7/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.719447 socktalk-0.1.7/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:12:23.478523 socktalk-0.1.8/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.8/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4647 2024-04-11 15:12:23.478523 socktalk-0.1.8/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3648 2024-04-11 12:01:29.000000 socktalk-0.1.8/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:12:23.478523 socktalk-0.1.8/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.8/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.8/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.8/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.8/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.8/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 15:12:23.478523 socktalk-0.1.8/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1449 2024-04-11 15:11:02.000000 socktalk-0.1.8/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 15:12:23.478523 socktalk-0.1.8/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4647 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      301 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 15:12:23.000000 socktalk-0.1.8/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.7/LICENSE` & `socktalk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.7/PKG-INFO` & `socktalk-0.1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: socktalk
-Version: 0.1.7
-Summary: Socket-based AI chat server and multi-user chat client
-Project-URL: Source, https://github.com/mdkmk/socktalk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: openai==1.14.2
-
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
```

### Comparing `socktalk-0.1.7/README.md` & `socktalk-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: socktalk
+Version: 0.1.8
+Summary: Socket-based AI chat server and multi-user chat client
+Project-URL: Source, https://github.com/mdkmk/socktalk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: annotated-types==0.6.0
+Requires-Dist: anyio==4.3.0
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: distro==1.9.0
+Requires-Dist: exceptiongroup==1.2.0
+Requires-Dist: h11==0.14.0
+Requires-Dist: httpcore==1.0.5
+Requires-Dist: httpx==0.27.0
+Requires-Dist: idna==3.7
+Requires-Dist: openai==1.14.2
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic_core==2.16.3
+Requires-Dist: PyQt5==5.15.10
+Requires-Dist: PyQt5-Qt5==5.15.2
+Requires-Dist: PyQt5-sip==12.13.0
+Requires-Dist: sniffio==1.3.1
+Requires-Dist: tqdm==4.66.2
+Requires-Dist: typing_extensions==4.11.0
+
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
```

### Comparing `socktalk-0.1.7/server_client/ai_client.py` & `socktalk-0.1.8/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.7/server_client/client.py` & `socktalk-0.1.8/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.7/server_client/server.py` & `socktalk-0.1.8/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.7/server_client/start_server_with_ai_client.py` & `socktalk-0.1.8/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.7/socktalk.egg-info/PKG-INFO` & `socktalk-0.1.8/socktalk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyQt5==5.15.10
+Requires-Dist: annotated-types==0.6.0
+Requires-Dist: anyio==4.3.0
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: distro==1.9.0
+Requires-Dist: exceptiongroup==1.2.0
+Requires-Dist: h11==0.14.0
+Requires-Dist: httpcore==1.0.5
+Requires-Dist: httpx==0.27.0
+Requires-Dist: idna==3.7
 Requires-Dist: openai==1.14.2
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic_core==2.16.3
+Requires-Dist: PyQt5==5.15.10
+Requires-Dist: PyQt5-Qt5==5.15.2
+Requires-Dist: PyQt5-sip==12.13.0
+Requires-Dist: sniffio==1.3.1
+Requires-Dist: tqdm==4.66.2
+Requires-Dist: typing_extensions==4.11.0
 
 # "socktalk" Socket-based AI chat server and multi-user chat client
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
 If running the code using the python library "socktalk" (pip install socktalk):
```

