# Comparing `tmp/socktalk-0.1.5.tar.gz` & `tmp/socktalk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.5.tar", last modified: Thu Apr 11 11:56:02 2024, max compression
+gzip compressed data, was "socktalk-0.1.6.tar", last modified: Thu Apr 11 12:03:15 2024, max compression
```

## Comparing `socktalk-0.1.5.tar` & `socktalk-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.409703 socktalk-0.1.5/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.5/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     4129 2024-04-11 11:56:02.409703 socktalk-0.1.5/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3638 2024-04-11 11:54:10.000000 socktalk-0.1.5/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.405703 socktalk-0.1.5/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.5/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.5/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.5/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.5/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.5/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 11:56:02.409703 socktalk-0.1.5/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1005 2024-04-11 11:50:34.000000 socktalk-0.1.5/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 11:56:02.409703 socktalk-0.1.5/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     4129 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 11:56:02.000000 socktalk-0.1.5/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.628796 socktalk-0.1.6/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.6/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 12:03:15.628796 socktalk-0.1.6/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3648 2024-04-11 12:01:29.000000 socktalk-0.1.6/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.624796 socktalk-0.1.6/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.6/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.6/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.6/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.6/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.6/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 12:03:15.628796 socktalk-0.1.6/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1002 2024-04-11 12:03:03.000000 socktalk-0.1.6/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.628796 socktalk-0.1.6/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.5/LICENSE` & `socktalk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.5/PKG-INFO` & `socktalk-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Socket-based AI chat server and multi-user chat client
-Project-URL: Source, https://github.com/mdkmk/chat_server
+Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt5==5.15.10
@@ -24,34 +24,24 @@
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
 
-    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
-
-    SERVER_IP_ADDRESS=127.0.0.1
-
-    SERVER_PORT=1234
-
-    SEND_FULL_CHAT_HISTORY=True
-
-    AI_MODE1_ACTIVE=True
-
-    AI_MODE1_INTERVAL=1
-
-    AI_MODE1_MODEL=gpt-3.5-turbo
-
-    AI_MODE2_ACTIVE=True
-
-    AI_MODE2_INTERVAL=60
-
-    AI_MODE2_MODEL=gpt-3.5-turbo
-
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
     AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

### Comparing `socktalk-0.1.5/README.md` & `socktalk-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,24 @@
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
 
-    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
-
-    SERVER_IP_ADDRESS=127.0.0.1
-
-    SERVER_PORT=1234
-
-    SEND_FULL_CHAT_HISTORY=True
-
-    AI_MODE1_ACTIVE=True
-
-    AI_MODE1_INTERVAL=1
-
-    AI_MODE1_MODEL=gpt-3.5-turbo
-
-    AI_MODE2_ACTIVE=True
-
-    AI_MODE2_INTERVAL=60
-
-    AI_MODE2_MODEL=gpt-3.5-turbo
-
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
     AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

### Comparing `socktalk-0.1.5/server_client/ai_client.py` & `socktalk-0.1.6/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.5/server_client/client.py` & `socktalk-0.1.6/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.5/server_client/server.py` & `socktalk-0.1.6/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.5/server_client/start_server_with_ai_client.py` & `socktalk-0.1.6/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.5/setup.py` & `socktalk-0.1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     project_urls={
-        'Source': 'https://github.com/mdkmk/chat_server'
+        'Source': 'https://github.com/mdkmk/socktalk'
     },
     install_requires=[
         'PyQt5==5.15.10',
         'openai==1.14.2'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `socktalk-0.1.5/socktalk.egg-info/PKG-INFO` & `socktalk-0.1.6/socktalk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Socket-based AI chat server and multi-user chat client
-Project-URL: Source, https://github.com/mdkmk/chat_server
+Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt5==5.15.10
@@ -24,34 +24,24 @@
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. AI model can be adjusted. Mode2 content can be adjusted. See below for more details.
 
     ### ".env" file example
 
-    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>
-
-    SERVER_IP_ADDRESS=127.0.0.1
-
-    SERVER_PORT=1234
-
-    SEND_FULL_CHAT_HISTORY=True
-
-    AI_MODE1_ACTIVE=True
-
-    AI_MODE1_INTERVAL=1
-
-    AI_MODE1_MODEL=gpt-3.5-turbo
-
-    AI_MODE2_ACTIVE=True
-
-    AI_MODE2_INTERVAL=60
-
-    AI_MODE2_MODEL=gpt-3.5-turbo
-
+    OPENAI_API_KEY=<OPENAI_API_KEY_HERE>  
+    SERVER_IP_ADDRESS=127.0.0.1  
+    SERVER_PORT=1234  
+    SEND_FULL_CHAT_HISTORY=True  
+    AI_MODE1_ACTIVE=True  
+    AI_MODE1_INTERVAL=1  
+    AI_MODE1_MODEL=gpt-3.5-turbo  
+    AI_MODE2_ACTIVE=True  
+    AI_MODE2_INTERVAL=60  
+    AI_MODE2_MODEL=gpt-3.5-turbo  
     AI_MODE2_CONTENT="Say something interesting from a random Wikipedia page and start your response with 'Did you know', but don't mention the source."
 
 
 2) "chat_server": Runs a chat server without a connected AI client. No .env file necessary.
 
 
 3) "chat_client": Runs the user chat client.
```

